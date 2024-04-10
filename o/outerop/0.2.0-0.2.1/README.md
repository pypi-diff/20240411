# Comparing `tmp/outerop-0.2.0.tar.gz` & `tmp/outerop-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outerop-0.2.0.tar", max compression
+gzip compressed data, was "outerop-0.2.1.tar", max compression
```

## Comparing `outerop-0.2.0.tar` & `outerop-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3314 2024-04-10 07:01:40.307706 outerop-0.2.0/README.md
--rw-r--r--   0        0        0    12518 2024-04-09 04:28:50.077741 outerop-0.2.0/outerop/__init__.py
--rw-r--r--   0        0        0      475 2024-04-10 07:09:01.769281 outerop-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3885 1970-01-01 00:00:00.000000 outerop-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3314 2024-04-10 07:01:40.307706 outerop-0.2.1/README.md
+-rw-r--r--   0        0        0    12723 2024-04-10 23:29:15.354365 outerop-0.2.1/outerop/__init__.py
+-rw-r--r--   0        0        0      475 2024-04-10 22:57:15.108527 outerop-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3885 1970-01-01 00:00:00.000000 outerop-0.2.1/PKG-INFO
```

### Comparing `outerop-0.2.0/README.md` & `outerop-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `outerop-0.2.0/outerop/__init__.py` & `outerop-0.2.1/outerop/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,80 +48,71 @@
         try:
             response = requests.post(
                 f"{self.config['baseURL']}/api/v1/log",
                 headers=headers,
                 data=json.dumps(self.buffer),
             )
             response.raise_for_status()
-        except requests.exceptions.RequestException:
+        except Exception as e:
             pass
         finally:
             self.pending_flush = False
             self.buffer = []
 
     def _prepare_event(self, event: Dict):
         return {**event}
 
 
 class Outerop:
     def __init__(self, outerop_api_key: str, options: Dict = None):
         self.outerop_api_key = outerop_api_key
-        self.options = {**{"baseURL": "https://app.outerop.com", "loggingEnabled": True}, **(options or {})}
-
-
-        self.log_collector = LogCollector(
-            {
-                "isEnabled": True,
-                "baseURL": self.options.get("baseURL", "https://app.outerop.com"),
-                "outeropApiKey": self.outerop_api_key,
-                "bypassHeader": self.options.get("bypassHeader"),
-            }
-        )
+        self.options = {
+            "baseURL": "https://app.outerop.com",
+            "loggingEnabled": True,
+            "cache": True,
+            **(options or {})
+        }
+        self.log_collector = LogCollector({
+            "isEnabled": True,
+            "baseURL": self.options.get("baseURL", "https://app.outerop.com"),
+            "outeropApiKey": self.outerop_api_key,
+            "bypassHeader": self.options.get("bypassHeader")
+        })
+        self.cache = self.options.get("cache", True)
 
         headers = {
             "Authorization": self.outerop_api_key,
             "Content-Type": "application/json",
+            **({"x-vercel-protection-bypass": self.options["bypassHeader"]} if self.options.get("bypassHeader") else {})
         }
-        if self.options.get("bypassHeader"):
-            headers["x-vercel-protection-bypass"] = self.options["bypassHeader"]
-
 
         self.client = requests.Session()
         self.client.headers.update(headers)
         self.client.base_url = self.options["baseURL"]
 
-        self.openai = None
-        if self.options.get("openaiApiKey"):
-            self.openai = OpenAI(api_key=self.options["openaiApiKey"])
-
-        self.anthropic = None
-        if self.options.get("anthropicApiKey"):
-            self.anthropic = Anthropic(api_key=self.options["anthropicApiKey"])
-
-        self.mistral = None
-        if self.options.get("mistralApiKey"):
-            self.mistral = MistralClient(api_key=self.options["mistralApiKey"])
+        self.openai = OpenAI(api_key=self.options["openaiApiKey"]) if self.options.get("openaiApiKey") else None
+        self.anthropic = Anthropic(api_key=self.options["anthropicApiKey"]) if self.options.get("anthropicApiKey") else None
+        self.mistral = MistralClient(api_key=self.options["mistralApiKey"]) if self.options.get("mistralApiKey") else None
 
         self.prompt_cache: Dict[str, Dict] = {}
         self.prompt_cache_ttl = options.get("promptCacheTTL", DEFAULT_TTL)  # Default TTL of 15 minutes
-        
-        
 
     def get_prompt(self, team_prompt_name: str, version_name_or_environment: str):
         cache_key = f"{team_prompt_name}-{version_name_or_environment}"
         current_time = time.time()
-        if cache_key in self.prompt_cache:
+        if self.cache and cache_key in self.prompt_cache:
             cached_prompt, timestamp = self.prompt_cache[cache_key]
             if current_time - timestamp < self.prompt_cache_ttl:
                 return cached_prompt
 
         try:
-            url = f"{self.options['baseURL']}/api/v1/prompt-by-version-name/{team_prompt_name}/{version_name_or_environment}"
-            if version_name_or_environment in list(Environment):
+            if version_name_or_environment in [env.value for env in Environment]:
                 url = f"{self.options['baseURL']}/api/v1/prompt-by-environment/{team_prompt_name}/{version_name_or_environment}"
+            else:
+                url = f"{self.options['baseURL']}/api/v1/prompt-by-version-name/{team_prompt_name}/{version_name_or_environment}"
 
             response = self.client.get(url)
             response.raise_for_status()
             prompt_data = response.json()["prompt"]
             self.prompt_cache[cache_key] = (prompt_data, current_time)  # Update cache with timestamp
             return prompt_data
         except requests.exceptions.RequestException as e:
@@ -166,16 +157,17 @@
                     tool_choice=prompt.get("tool_choice", "auto"),
                 )
                 end_time = time.perf_counter()
                 latency_ms = round((end_time - start_time) * 1000)
 
                 self.log_collector.record(
                     {
-                        "version": prompt["version"],
                         "team_prompt_id": prompt["team_prompt_id"],
+                        "team_prompt_name": team_prompt_name,
+                        "version_name": prompt['version_name'],
                         "environment": prompt["environment"],
                         "prompt_environment_id": prompt["id"],
                         "input": messages_without_id,
                         "output": result.choices[0].message.content,
                         "latency_ms": latency_ms,
                         "output_tokens": result.usage.completion_tokens,
                         "input_tokens": result.usage.prompt_tokens,
@@ -200,16 +192,17 @@
                 end_time = time.perf_counter()
                 latency_ms = round((end_time - start_time) * 1000)
 
                 print(f"result: {result}")
 
                 self.log_collector.record(
                     {
-                        "version": prompt["version"],
                         "team_prompt_id": prompt["team_prompt_id"],
+                        "team_prompt_name": team_prompt_name,
+                        "version_name": prompt['version_name'],
                         "environment": prompt["environment"],
                         "prompt_environment_id": prompt["id"],
                         "input": messages_without_id,
                         "output": result.choices[0].message.content,
                         "latency_ms": latency_ms,
                         "output_tokens": result.usage.completion_tokens,
                         "input_tokens": result.usage.prompt_tokens,
@@ -252,16 +245,17 @@
                 end_time = time.perf_counter()
                 latency_ms = round((end_time - start_time) * 1000)
 
                 openai_result = convert_anthropic_output_to_openai(result)
 
                 self.log_collector.record(
                     {
-                        "version": prompt["version"],
                         "team_prompt_id": prompt["team_prompt_id"],
+                        "team_prompt_name": team_prompt_name,
+                        "version_name": prompt['version_name'],
                         "prompt_environment_id": prompt["id"],
                         "environment": prompt["environment"],
                         "input": messages_without_id,
                         "output": openai_result["choices"][0]["message"]["content"],
                         "latency_ms": latency_ms,
                         "output_tokens": result.usage.output_tokens,
                         "input_tokens": result.usage.input_tokens,
```

### Comparing `outerop-0.2.0/PKG-INFO` & `outerop-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outerop
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Stephen Byrne
 Author-email: 39441007+stephenbyrne99@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

