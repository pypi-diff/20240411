# Comparing `tmp/quotientai-0.0.1.tar.gz` & `tmp/quotientai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quotientai-0.0.1.tar", max compression
+gzip compressed data, was "quotientai-0.0.2.tar", max compression
```

## Comparing `quotientai-0.0.1.tar` & `quotientai-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11345 2024-04-09 13:37:32.091277 quotientai-0.0.1/LICENSE
--rw-r--r--   0        0        0      390 2024-04-09 13:37:32.091277 quotientai-0.0.1/README.md
--rw-r--r--   0        0        0     1011 2024-04-09 13:37:32.091277 quotientai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      288 2024-04-09 13:37:32.091277 quotientai-0.0.1/quotientai/__init__.py
--rw-r--r--   0        0        0       47 2024-04-09 13:37:32.091277 quotientai-0.0.1/quotientai/cli/__init__.py
--rw-r--r--   0        0        0    17533 2024-04-09 13:37:32.091277 quotientai-0.0.1/quotientai/cli/entrypoint.py
--rw-r--r--   0        0        0     9162 2024-04-09 13:37:32.091277 quotientai-0.0.1/quotientai/cli/format.py
--rw-r--r--   0        0        0    38427 2024-04-09 13:37:32.091277 quotientai-0.0.1/quotientai/client.py
--rw-r--r--   0        0        0      181 2024-04-09 13:37:32.091277 quotientai-0.0.1/quotientai/exceptions.py
--rw-r--r--   0        0        0     3118 2024-04-09 13:37:32.091277 quotientai-0.0.1/quotientai/utils.py
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 quotientai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-04-11 06:20:12.620846 quotientai-0.0.2/LICENSE
+-rw-r--r--   0        0        0      390 2024-04-11 06:20:12.620846 quotientai-0.0.2/README.md
+-rw-r--r--   0        0        0     1011 2024-04-11 06:20:12.620846 quotientai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/cli/__init__.py
+-rw-r--r--   0        0        0    19112 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/cli/entrypoint.py
+-rw-r--r--   0        0        0     9663 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/cli/format.py
+-rw-r--r--   0        0        0    41502 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/client.py
+-rw-r--r--   0        0        0      181 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/exceptions.py
+-rw-r--r--   0        0        0     3118 2024-04-11 06:20:12.620846 quotientai-0.0.2/quotientai/utils.py
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 quotientai-0.0.2/PKG-INFO
```

### Comparing `quotientai-0.0.1/LICENSE` & `quotientai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quotientai-0.0.1/pyproject.toml` & `quotientai-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quotientai"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     "Vic Weiss <vic@quotientai.co>",
     "Freddie Vargus <freddie@quotientai.co>",
     "Allison Kunz <allison@quotient.co>",
 ]
 description = "CLI for evaluating large language models with Quotient"
 readme = "README.md"
```

### Comparing `quotientai-0.0.1/quotientai/cli/entrypoint.py` & `quotientai-0.0.2/quotientai/cli/entrypoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import click
 
 from quotientai.cli.format import (
     format_api_keys_table,
     format_datasets_table,
     format_jobs_table,
+    format_metrics_table,
     format_models_table,
     format_prompt_template_table,
     format_recipes_table,
     format_results_summary_table,
     format_results_table,
     format_system_prompt_table,
     format_tasks_table,
@@ -569,21 +570,34 @@
 @click.option(
     "--seed",
     default=42,
     show_default=True,
     type=int,
     help="Seed for the job (optional).",
 )
+@click.option(
+    "--metric-id",
+    type=str,
+    required=False,
+    multiple=True,
+)
 @click.option("--show-progress", is_flag=True, help="Show the job's progress.")
-def create_job(task_id, recipe_id, num_fewshot_examples, limit, seed, show_progress):
+def create_job(
+    task_id, recipe_id, num_fewshot_examples, limit, seed, metric_id, show_progress
+):
     """Command to create a new job."""
     try:
         client = QuotientClient()
         new_job = client.create_job(
-            task_id, recipe_id, num_fewshot_examples, limit, seed
+            task_id=task_id,
+            recipe_id=recipe_id,
+            num_fewshot_examples=num_fewshot_examples,
+            limit=limit,
+            seed=seed,
+            metric_ids=metric_id,
         )
         print(format_jobs_table([new_job]))
 
         if show_progress:
             show_job_progress(client, new_job["id"])
 
     except QuotientAIException as e:
@@ -603,9 +617,57 @@
         client = QuotientClient()
         show_job_progress(client, job_id)
 
     except QuotientAIException as e:
         click.echo(str(e))
 
 
+###########################
+#          Metrics        #
+###########################
+
+
+@list.command(name="metrics")
+def list_metrics():
+    """Command to list all available metrics"""
+    try:
+        client = QuotientClient()
+        metrics = client.list_metrics()
+        print(format_metrics_table(metrics))
+
+    except QuotientAIException as e:
+        click.echo(str(e))
+
+
+@create.command(name="rubric-based-metric")
+@click.option("--name", required=True, type=str, help="Name of the rubric metric.")
+@click.option(
+    "--description", required=True, type=str, help="Description of the rubric metric."
+)
+@click.option(
+    "--model-id", required=True, type=int, help="Model ID for the rubric metric."
+)
+@click.option(
+    "--rubric-template",
+    required=True,
+    type=str,
+    help="Rubric template for the rubric metric.",
+)
+def create_rubric_metric(name, description, model_id, rubric_template):
+    """Command to create a new rubric metric."""
+    try:
+        client = QuotientClient()
+        metrics = client.create_rubric_based_metric(
+            name=name,
+            description=description,
+            model_id=model_id,
+            rubric_template=rubric_template,
+        )
+
+        print(format_metrics_table([metrics]))
+
+    except QuotientAIException as e:
+        click.echo(str(e))
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `quotientai-0.0.1/quotientai/cli/format.py` & `quotientai-0.0.2/quotientai/cli/format.py`

 * *Files 5% similar despite different names*

```diff
@@ -181,15 +181,14 @@
     table = PrettyTable()
     table.field_names = ["ID", "Name", "File", "File Format", "Owner"]
 
     # Add rows to the table
     for item in data:
         id = item["id"]
         name = item["name"]
-        dataset_type = item["dataset_type"]
         url = (
             truncate_string(select_file_name_from_url(item["url"]))
             if item["url"] is not None
             else "N/A"
         )
         file_format = item["file_format"] if item["file_format"] is not None else "N/A"
         owner = (
@@ -283,14 +282,39 @@
         table.add_row([question, completion, expected_answer])
 
     has_more_results = len(data["results"]) > table_length
 
     return table, has_more_results
 
 
+def format_metrics_table(data):
+    table = PrettyTable()
+    table.field_names = [
+        "ID",
+        "Name",
+        "Owner",
+    ]
+
+    # Add row to the general table
+    for metric_data in data:
+        owner_id = (
+            metric_data["owner_profile_id"]
+            if metric_data["owner_profile_id"] is not None
+            else "Open to all"
+        )
+        table.add_row(
+            [
+                metric_data["id"],
+                metric_data["name"],
+                owner_id,
+            ]
+        )
+    return table
+
+
 def save_results_to_file(data):
     data_to_frame = []
     for item in data["results"]:
         content = item["content"]
         row = {
             "id": content["id"],
             "input_text": content["input_text"],
```

### Comparing `quotientai-0.0.1/quotientai/client.py` & `quotientai-0.0.2/quotientai/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -889,15 +889,21 @@
                 f"Failed to list jobs: {api_err.message} ({api_err.code})"
             ) from api_err
         except Exception as e:
             raise QuotientAIException(f"Failed to list jobs: {str(e)}") from e
 
     @require_api_key
     def create_job(
-        self, task_id, recipe_id, num_fewshot_examples=0, limit=100, seed=42
+        self,
+        task_id,
+        recipe_id,
+        num_fewshot_examples=0,
+        limit=100,
+        seed=42,
+        metric_ids=None,
     ):
         """
         Create a new job with a given task, recipe, and optional parameters.
 
         Parameters:
         ----------
         task_id : int
@@ -906,34 +912,40 @@
             The ID of the recipe to use for evaluation
         num_fewshot_examples : int, optional
             The number of few-shot examples to use for evaluation. Default is 0.
         limit : int, optional
             The number of examples to evaluate. Default is 100.
         seed : int, optional
             The random seed to use for evaluation. Default is 42.
+        metric_ids : list[int], optional
+            A list of metrics to use for evaluation. Default is None.
 
         Returns:
         --------
         dict
             The job record from the API.
         """
         job_data = {
             "task_id": task_id,
             "recipe_id": recipe_id,
             "num_fewshot_examples": num_fewshot_examples,
             "limit": limit,
             "seed": seed,
         }
+
+        if metric_ids is not None:
+            job_data.update({"metric_ids": metric_ids})
+
         try:
             url = f"{self.eval_scheduler_url}/create-eval-job"
             headers = {
                 "Authorization": f"Bearer {self.api_key}",
                 "Accept": "application/json",
             }
-            response = requests.post(url, headers=headers, params=job_data)
+            response = requests.post(url, headers=headers, json=job_data)
             result = response.json()
             if response.status_code != 200:
                 if "detail" in result:
                     raise FastAPIError(response.status_code, result["detail"])
                 else:
                     response.raise_for_status()
             job_id = result["id"]
@@ -1025,9 +1037,88 @@
             return data.data
         except APIError as api_err:
             raise QuotientAIException(
                 f"Failed to retrieve job progress: {api_err.message} ({api_err.code})"
             ) from api_err
         except Exception as e:
             raise QuotientAIException(
+                f"Failed to retrieve job progress: {str(e)}"
+            ) from e
+
+    ###########################
+    #          Metrics        #
+    ###########################
+
+    @require_api_key
+    def create_rubric_based_metric(
+        self, name: str, description: str, model_id: int, rubric_template: str
+    ) -> dict:
+        """
+        Create a new metric with a given name and description.
+
+        Parameters:
+        -----------
+        name : str
+            The name of the metric
+        description : str
+            The description of the metric
+        model_id : int
+            The ID of the model to use for the metric
+        rubric_template : str
+            The rubric template to use for the metric. Must include `{input_text}` with in the template.
+
+        Returns:
+        --------
+        dict
+            The metric record from the API.
+        """
+        try:
+            # check for valid template
+            if "{input_text}" not in rubric_template:
+                raise QuotientAIInvalidInputException(
+                    "Rubric template must include `{input_text}`"
+                )
+
+            byo_metric_data = {
+                "name": name,
+                "rubric_template": rubric_template,
+                "model_id": model_id,
+                "created_at": datetime.utcnow().isoformat(),
+            }
+            response = (
+                self.supaclient.from_("byo_rubric_metric")
+                .insert(byo_metric_data)
+                .execute()
+            )
+            byo_rubric_metric_id = response.data[0]["id"]
+
+            metric_data = {
+                "name": name,
+                "title": name,
+                "description": description,
+                "byo_rubric_metric_id": byo_rubric_metric_id,
+                "created_at": datetime.utcnow().isoformat(),
+            }
+            response = self.supaclient.from_("metrics").insert(metric_data).execute()
+            if not response.data:
+                raise ValueError("Metric creation failed, no data returned.")
+            return response.data[0]
+        except APIError as api_err:
+            raise QuotientAIException(
+                f"Failed to create metric: {api_err.message} ({api_err.code})"
+            ) from api_err
+        except Exception as e:
+            raise QuotientAIException(f"Failed to create metric: {str(e)}") from e
+
+    @require_api_key
+    def list_metrics(self):
+        try:
+            data = self.supaclient.from_("metrics").select("*").execute()
+            return data.data
+        except APIError as api_err:
+            raise QuotientAIException(
+                f"Failed to retrieve job progress: {api_err.message} ({api_err.code})"
+            ) from api_err
+        except Exception as e:
+            raise QuotientAIException(
                 f"Failed to retrieve job progress: {str(e)}"
             ) from e
```

### Comparing `quotientai-0.0.1/quotientai/utils.py` & `quotientai-0.0.2/quotientai/utils.py`

 * *Files identical despite different names*

### Comparing `quotientai-0.0.1/PKG-INFO` & `quotientai-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quotientai
-Version: 0.0.1
+Version: 0.0.2
 Summary: CLI for evaluating large language models with Quotient
 License: Apache-2.0
 Keywords: quotient,evaluation,llms,machine learning,ai
 Author: Vic Weiss
 Author-email: vic@quotientai.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

