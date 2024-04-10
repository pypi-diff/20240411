# Comparing `tmp/neon-iris-0.1.1a4.tar.gz` & `tmp/neon-iris-0.1.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-iris-0.1.1a4.tar", last modified: Mon Jan 29 19:55:31 2024, max compression
+gzip compressed data, was "neon-iris-0.1.1a5.tar", last modified: Wed Apr 10 22:23:25 2024, max compression
```

## Comparing `neon-iris-0.1.1a4.tar` & `neon-iris-0.1.1a5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 19:55:31.535099 neon-iris-0.1.1a4/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-01-29 19:55:31.535099 neon-iris-0.1.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 19:55:31.535099 neon-iris-0.1.1a4/neon_iris/
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    20917 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 19:55:31.535099 neon-iris-0.1.1a4/neon_iris/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/models/web_sat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 19:55:31.535099 neon-iris-0.1.1a4/neon_iris/res/
--rw-r--r--   0 runner    (1001) docker     (127)    67090 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/res/start_listening.wav
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 19:55:31.535099 neon-iris-0.1.1a4/neon_iris/static/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/static/sprite.css
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/static/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 19:55:31.535099 neon-iris-0.1.1a4/neon_iris/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/voice_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17146 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/web_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/neon_iris/web_sat_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 19:55:31.535099 neon-iris-0.1.1a4/neon_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-01-29 19:55:31.000000 neon-iris-0.1.1a4/neon_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-01-29 19:55:31.000000 neon-iris-0.1.1a4/neon_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 19:55:31.000000 neon-iris-0.1.1a4/neon_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-29 19:55:31.000000 neon-iris-0.1.1a4/neon_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-29 19:55:31.000000 neon-iris-0.1.1a4/neon_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-29 19:55:31.000000 neon-iris-0.1.1a4/neon_iris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 19:55:31.535099 neon-iris-0.1.1a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-01-29 19:55:24.000000 neon-iris-0.1.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/neon_iris/
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21291 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/neon_iris/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/models/web_sat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/neon_iris/res/
+-rw-r--r--   0 runner    (1001) docker     (127)    67090 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/res/start_listening.wav
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/neon_iris/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/static/sprite.css
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/static/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/neon_iris/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/voice_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/web_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/web_sat_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/neon_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-10 22:23:25.000000 neon-iris-0.1.1a5/neon_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-10 22:23:25.000000 neon-iris-0.1.1a5/neon_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:23:25.000000 neon-iris-0.1.1a5/neon_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 22:23:25.000000 neon-iris-0.1.1a5/neon_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-10 22:23:25.000000 neon-iris-0.1.1a5/neon_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 22:23:25.000000 neon-iris-0.1.1a5/neon_iris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/setup.py
```

### Comparing `neon-iris-0.1.1a4/LICENSE.md` & `neon-iris-0.1.1a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/PKG-INFO` & `neon-iris-0.1.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-iris
-Version: 0.1.1a4
+Version: 0.1.1a5
 Summary: Interactive Relay for Intelligence Systems
 Home-page: https://github.com/neongeckocom/neon-iris
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-iris-0.1.1a4/README.md` & `neon-iris-0.1.1a5/README.md`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris/__init__.py` & `neon-iris-0.1.1a5/neon_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris/cli.py` & `neon-iris-0.1.1a5/neon_iris/cli.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris/client.py` & `neon-iris-0.1.1a5/neon_iris/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,16 @@
             self._handle_profile_update(message)
         elif message.msg_type == "neon.clear_data":
             self._handle_clear_data(message)
         elif message.msg_type == "klat.error":
             self.handle_error_response(message)
         elif message.msg_type == "neon.languages.get.response":
             self._handle_supported_languages(message)
+        elif message.msg_type == "neon.alert_expired":
+            self.handle_alert(message)
         elif message.msg_type.endswith(".response"):
             self.handle_api_response(message)
         else:
             LOG.warning(f"Message not handled: {message.msg_type}")
 
     def handle_neon_error(self, channel, method, _, body):
         """
@@ -227,14 +229,20 @@
 
     @abstractmethod
     def clear_media(self, message: Message):
         """
         Override this method to handle requests to clear media (photos, etc)
         """
 
+    @abstractmethod
+    def handle_alert(self, message: Message):
+        """
+        Override this method to handle alerts (timers, alarms, reminders)
+        """
+
     def _handle_profile_update(self, message: Message):
         updated_profile = message.data["profile"]
         if updated_profile['user']['username'] == \
                 self.user_config['user']['username']:
             self._user_config.from_dict(updated_profile)
             LOG.info("Updated user profile")
         else:
@@ -465,14 +473,17 @@
 
     def handle_api_response(self, message: Message):
         pass
 
     def clear_caches(self, message: Message):
         print("Cached Responses Cleared")
 
+    def handle_alert(self, message: Message):
+        print(f"\nAlert Expired: {message.data.get('alert_name')}")
+
     def clear_media(self, message: Message):
         pass
 
     def send_utterance(self, utterance: str, lang: str = "en-us",
                        _=None, __=None):
         """
         Queue a string request for skills processing
```

### Comparing `neon-iris-0.1.1a4/neon_iris/llm.py` & `neon-iris-0.1.1a5/neon_iris/llm.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris/models/__init__.py` & `neon-iris-0.1.1a5/neon_iris/models/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris/models/web_sat.py` & `neon-iris-0.1.1a5/neon_iris/models/web_sat.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris/res/start_listening.wav` & `neon-iris-0.1.1a5/neon_iris/res/start_listening.wav`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris/static/sprite.css` & `neon-iris-0.1.1a5/neon_iris/static/sprite.css`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris/static/styles.css` & `neon-iris-0.1.1a5/neon_iris/static/styles.css`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris/templates/index.html` & `neon-iris-0.1.1a5/neon_iris/templates/index.html`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris/util.py` & `neon-iris-0.1.1a5/neon_iris/util.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris/version.py` & `neon-iris-0.1.1a5/neon_iris/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.1a4"
+__version__ = "0.1.1a5"
```

### Comparing `neon-iris-0.1.1a4/neon_iris/voice_client.py` & `neon-iris-0.1.1a5/neon_iris/voice_client.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris/web_client.py` & `neon-iris-0.1.1a5/neon_iris/web_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 class GradIOClient(NeonAIClient):
     def __init__(self, lang: str = None):
         config = Configuration()
         self.config = config.get('iris') or dict()
         NeonAIClient.__init__(self, config.get("MQ"))
         self._await_response = Event()
+        self._alerts = dict()
         self._response = None
         self._transcribed = None
         self._current_tts = dict()
         self._profiles: Dict[str, dict] = dict()
         self._audio_path = join(xdg_data_home(), "iris", "stt")
         if not isdir(self._audio_path):
             makedirs(self._audio_path)
@@ -76,14 +77,22 @@
     def _start_session(self):
         sid = uuid4().hex
         self._current_tts[sid] = None
         self._profiles[sid] = self.user_config
         self._profiles[sid]['user']['username'] = sid
         return sid
 
+    def check_alerts(self, session_id: str):
+        if not self._alerts.get(session_id):
+            gradio.Info("No Alerts")
+            return session_id
+        while self._alerts.get(session_id):
+            gradio.Info(self._alerts[session_id].pop())
+        return session_id
+
     def update_profile(self, stt_lang: str, tts_lang: str, tts_lang_2: str,
                        time: int, date: str, uom: str, city: str, state: str,
                        country: str, first: str, middle: str, last: str,
                        pref_name: str, email: str, session_id: str):
         """
         Callback to handle user settings changes from the web UI
         """
@@ -211,14 +220,17 @@
             # with gradio.Row():
             #     tts_button = gradio.Button("Play TTS")
             #     tts_button.click(self.play_tts,
             #                      inputs=[client_session],
             #                      outputs=[tts_audio, client_session])
             # Define settings UI
             with gradio.Row():
+                submit = gradio.Button("Update User Settings")
+                check_alerts = gradio.Button("Check for Alerts")
+            with gradio.Row():
                 with gradio.Column():
                     lang = self.get_lang(client_session.value).split('-')[0]
                     stt_lang = gradio.Radio(label="Input Language",
                                             choices=self._languages.get("stt")
                                             or self.supported_languages,
                                             value=lang)
                     tts_lang = gradio.Radio(label="Response Language",
@@ -249,22 +261,23 @@
                 with gradio.Column():
                     first_name = gradio.Textbox(label="First Name")
                     middle_name = gradio.Textbox(label="Middle Name")
                     last_name = gradio.Textbox(label="Last Name")
                     pref_name = gradio.Textbox(label="Preferred Name")
                     email_addr = gradio.Textbox(label="Email Address")
                     # TODO: DoB, pic, about, phone?
-            submit = gradio.Button("Update User Settings")
             submit.click(self.update_profile,
                          inputs=[stt_lang, tts_lang, tts_lang_2, time_format,
                                  date_format, unit_of_measure, city, state,
                                  country, first_name, middle_name, last_name,
                                  pref_name, email_addr, client_session],
                          outputs=[client_session])
-            blocks.launch(server_name=address, server_port=port)
+            check_alerts.click(self.check_alerts, inputs=[client_session],
+                               outputs=[client_session])
+            blocks.queue().launch(server_name=address, server_port=port)
 
     def handle_klat_response(self, message: Message):
         """
         Handle a valid response from Neon. This includes text and base64-encoded
         audio in all requested languages.
         @param message: Neon response message
         """
@@ -303,14 +316,25 @@
         are not explicitly handled (i.e. get_stt, get_tts)
         @param message: Response message to something emitted by this client
         """
         LOG.debug(f"Got {message.msg_type}: {message.data}")
         if message.msg_type == "neon.audio_input.response":
             self._transcribed = message.data.get("transcripts", [""])[0]
 
+    def handle_alert(self, message: Message):
+        """
+        Handle an expired alert that was previously set by this session.
+        @param message: neon.alert_expired Message
+        """
+        user = message.context['username']
+        LOG.info(f"Alert expired for user: {user}")
+        alert = f"Alert Expired: {message.data.get('alert_name')}"
+        self._alerts.setdefault(user, list())
+        self._alerts[user].append(alert)
+
     def _handle_profile_update(self, message: Message):
         updated_profile = message.data["profile"]
         session_id = updated_profile['user']['username']
         if session_id in self._profiles:
             LOG.info(f"Got profile update for {session_id}")
             self._profiles[session_id] = updated_profile
         else:
```

### Comparing `neon-iris-0.1.1a4/neon_iris/web_sat_client.py` & `neon-iris-0.1.1a5/neon_iris/web_sat_client.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/neon_iris.egg-info/PKG-INFO` & `neon-iris-0.1.1a5/neon_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-iris
-Version: 0.1.1a4
+Version: 0.1.1a5
 Summary: Interactive Relay for Intelligence Systems
 Home-page: https://github.com/neongeckocom/neon-iris
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-iris-0.1.1a4/neon_iris.egg-info/SOURCES.txt` & `neon-iris-0.1.1a5/neon_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a4/setup.py` & `neon-iris-0.1.1a5/setup.py`

 * *Files identical despite different names*

