# Comparing `tmp/pystackql-3.5.3.tar.gz` & `tmp/pystackql-3.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystackql-3.5.3.tar", last modified: Sun Apr  7 23:10:28 2024, max compression
+gzip compressed data, was "pystackql-3.5.4.tar", last modified: Thu Apr 11 04:43:56 2024, max compression
```

## Comparing `pystackql-3.5.3.tar` & `pystackql-3.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-07 23:10:28.942846 pystackql-3.5.3/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 pystackql-3.5.3/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6948 2024-04-07 23:10:28.939320 pystackql-3.5.3/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5176 2024-04-07 23:00:24.000000 pystackql-3.5.3/README.rst
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-07 23:10:28.808299 pystackql-3.5.3/pystackql/
--rwxrwxrwx   0 javen     (1000) javen     (1000)      101 2024-03-15 01:52:38.000000 pystackql-3.5.3/pystackql/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5209 2024-03-15 01:52:38.000000 pystackql-3.5.3/pystackql/_util.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1751 2024-03-15 01:52:38.000000 pystackql-3.5.3/pystackql/base_stackql_magic.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1740 2024-03-15 01:52:38.000000 pystackql-3.5.3/pystackql/magic.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1743 2024-03-15 01:52:38.000000 pystackql-3.5.3/pystackql/magics.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)    24984 2024-04-07 21:53:32.000000 pystackql-3.5.3/pystackql/stackql.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-07 23:10:28.913750 pystackql-3.5.3/pystackql.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6948 2024-04-07 23:10:28.000000 pystackql-3.5.3/pystackql.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      324 2024-04-07 23:10:28.000000 pystackql-3.5.3/pystackql.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-07 23:10:28.000000 pystackql-3.5.3/pystackql.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       24 2024-04-07 23:10:28.000000 pystackql-3.5.3/pystackql.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       10 2024-04-07 23:10:28.000000 pystackql-3.5.3/pystackql.egg-info/top_level.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-07 23:10:28.945108 pystackql-3.5.3/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1254 2024-04-07 21:54:28.000000 pystackql-3.5.3/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-11 04:43:56.644050 pystackql-3.5.4/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 pystackql-3.5.4/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6948 2024-04-11 04:43:56.635576 pystackql-3.5.4/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5176 2024-04-11 04:43:41.000000 pystackql-3.5.4/README.rst
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-11 04:43:56.223930 pystackql-3.5.4/pystackql/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      101 2024-03-15 01:52:38.000000 pystackql-3.5.4/pystackql/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5209 2024-03-15 01:52:38.000000 pystackql-3.5.4/pystackql/_util.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1751 2024-03-15 01:52:38.000000 pystackql-3.5.4/pystackql/base_stackql_magic.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1740 2024-03-15 01:52:38.000000 pystackql-3.5.4/pystackql/magic.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1743 2024-03-15 01:52:38.000000 pystackql-3.5.4/pystackql/magics.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    25338 2024-04-11 04:38:32.000000 pystackql-3.5.4/pystackql/stackql.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-11 04:43:56.572406 pystackql-3.5.4/pystackql.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6948 2024-04-11 04:43:55.000000 pystackql-3.5.4/pystackql.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      324 2024-04-11 04:43:55.000000 pystackql-3.5.4/pystackql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-11 04:43:55.000000 pystackql-3.5.4/pystackql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       24 2024-04-11 04:43:55.000000 pystackql-3.5.4/pystackql.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       10 2024-04-11 04:43:55.000000 pystackql-3.5.4/pystackql.egg-info/top_level.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-11 04:43:56.647414 pystackql-3.5.4/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1254 2024-04-11 04:43:41.000000 pystackql-3.5.4/setup.py
```

### Comparing `pystackql-3.5.3/LICENSE` & `pystackql-3.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.3/PKG-INFO` & `pystackql-3.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystackql
-Version: 3.5.3
+Version: 3.5.4
 Summary: A Python interface for StackQL
 Home-page: https://github.com/stackql/pystackql
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT License
         
         Copyright (c) 2022 StackQL Studios
@@ -231,10 +231,10 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload dist/pystackql-3.5.3.tar.gz
+    twine upload dist/pystackql-3.5.4.tar.gz
```

### Comparing `pystackql-3.5.3/README.rst` & `pystackql-3.5.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -190,8 +190,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload dist/pystackql-3.5.3.tar.gz
+    twine upload dist/pystackql-3.5.4.tar.gz
```

### Comparing `pystackql-3.5.3/pystackql/_util.py` & `pystackql-3.5.4/pystackql/_util.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.3/pystackql/base_stackql_magic.py` & `pystackql-3.5.4/pystackql/base_stackql_magic.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.3/pystackql/magic.py` & `pystackql-3.5.4/pystackql/magic.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.3/pystackql/magics.py` & `pystackql-3.5.4/pystackql/magics.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.3/pystackql/stackql.py` & `pystackql-3.5.4/pystackql/stackql.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,39 +183,47 @@
 		- Generic error messages for other exceptions encountered during the query execution.
 
 		:raises FileNotFoundError: If the StackQL binary isn't found.
 		:raises Exception: For any other exceptions during the execution, providing a generic error message.
 		"""
 		local_params = self.params.copy()
 		local_params.insert(1, query)
+		output = {}
+
 		try:
 			with subprocess.Popen([self.bin_path] + local_params,
-								stdout=subprocess.PIPE, stderr=subprocess.PIPE) as iqlPopen:  # Capturing stderr separately
+					stdout=subprocess.PIPE, stderr=subprocess.PIPE) as iqlPopen:
 				stdout, stderr = iqlPopen.communicate()
+
 				if self.debug:
 					self._debug_log(f"Query: {query}")
 					self._debug_log(f"stdout: {stdout}")
 					self._debug_log(f"stderr: {stderr}")
+
+				# Check if stderr exists
 				if stderr:
-					# Prioritizing stderr since that’s where the expected messages seem to be
-					return stderr.decode('utf-8') if isinstance(stderr, bytes) else str(stderr)
-				else:
-					# Here, we may consider concatenating stdout and stderr, or handling them separately based on the use case
-					return stdout.decode('utf-8') if isinstance(stdout, bytes) else str(stdout)
+					output["error"] = stderr.decode('utf-8') if isinstance(stderr, bytes) else str(stderr)
+                
+				# Check if theres data
+				if stdout:
+					output["data"] = stdout.decode('utf-8') if isinstance(stdout, bytes) else str(stdout)
+
 		except FileNotFoundError:
-			return "ERROR %s not found" % self.bin_path
+			output["exception"] = f"ERROR: {self.bin_path} not found"
 		except Exception as e:
-			if 'stdout' in locals() and 'stderr' in locals():
-				return f"ERROR: {str(e)} {e.__doc__}, PARAMS: {local_params}, STDOUT: {stdout}, STDERR: {stderr}"
-			if 'stdout' in locals() and 'stderr' not in locals():
-				return f"ERROR: {str(e)} {e.__doc__}, PARAMS: {local_params},STDOUT: {stdout}"
-			elif 'stderr' in locals():
-				return f"ERROR: {str(e)} {e.__doc__}, PARAMS: {local_params},STDERR: {stderr}"
-			else:
-				return f"ERROR: {str(e)} {e.__doc__}, PARAMS: {local_params}"
+			error_details = {
+				"exception": str(e),
+				"doc": e.__doc__,
+				"params": local_params,
+				"stdout": stdout.decode('utf-8') if 'stdout' in locals() and isinstance(stdout, bytes) else "",
+				"stderr": stderr.decode('utf-8') if 'stderr' in locals() and isinstance(stderr, bytes) else ""
+			}
+			output["exception"] = f"ERROR: {json.dumps(error_details)}"
+
+		return output
 
 	def __init__(self, 
 				 server_mode=False, 
 				 server_address='127.0.0.1', 
 				 server_port=5466,
 				 backend_storage_mode='memory',
 				 backend_file_storage_location='stackql.db', 
@@ -470,78 +478,90 @@
 				return pd.DataFrame(result)
 			elif self.output == 'csv':
 				# return the string representation of the result
 				return result[0]['message']
 			else:
 				return result
 		else:
-			result_msg = self._run_query(query)
+			result = self._run_query(query)
+			if "exception" in result:
+				return {"error": result["exception"]}
+
+			# message on stderr
+			message = result["error"]
+
 			if self.output == 'pandas':
-				return pd.DataFrame({'message': [result_msg]})
+				return pd.DataFrame({'message': [message]}) if message else pd.DataFrame({'message': []})
 			elif self.output == 'csv':
-				return result_msg
+				return message
 			else:
-				return [{'message': result_msg}]			
+				return [{'message': message}]			
 	
-	def execute(self, query):
-		"""Executes a query using the StackQL instance and returns the output 
-		in the format specified by the `output` attribute.
-
-		Depending on the `server_mode` and `output` attribute of the instance, 
-		this method either runs the query against the StackQL server or executes 
-		it locally using a subprocess, returning the data in a dictionary, Pandas 
-		DataFrame, or CSV format.
+	def execute(self, query, suppress_errors=True):
+		"""
+		Executes a StackQL query and returns the output based on the specified output format.
 
-		:param query: The StackQL query string to be executed.
-		:type query: str
+		This method supports execution both in server mode and locally using subprocess. In server mode,
+		the query is sent to a StackQL server, while in local mode, it runs the query using a local binary.
 
-		:return: The output result of the query. Depending on the `output` attribute, 
-				the result can be a dictionary, a Pandas DataFrame, or a raw CSV string.
-				CSV output is currently not supported in `server_mode`.
-		:rtype: dict, pd.DataFrame, or str
+		Args:
+			query (str): The StackQL query string to be executed.
+			suppress_errors (bool, optional): If set to True, the method will return an empty list if an error occurs.
 
-		Example:
-			>>> from pystackql import StackQL
+		Returns:
+			dict, pd.DataFrame, or str: The output of the query, which can be a dictionary, a Pandas DataFrame,
+			or a raw CSV string, depending on the configured output format.
+
+		Raises:
+			ValueError: If an unsupported output format is specified.
+
+		Examples:
 			>>> stackql = StackQL()
-			>>> stackql_query = \"\"\"SELECT SPLIT_PART(machineType, '/', -1) as machine_type, 
-			... status, COUNT(*) as num_instances
-			... FROM google.compute.instances 
-			... WHERE project = 'stackql-demo' 
-			... AND zone = 'australia-southeast1-a'
-			... GROUP BY machine_type, status
-			... HAVING COUNT(*) > 2\"\"\"
-			>>> result = stackql.execute(stackql_query)
+			>>> query = '''
+				SELECT SPLIT_PART(machineType, '/', -1) as machine_type, status, COUNT(*) as num_instances
+				FROM google.compute.instances
+				WHERE project = 'stackql-demo' AND zone = 'australia-southeast1-a'
+				GROUP BY machine_type, status HAVING COUNT(*) > 2
+				'''
+			>>> result = stackql.execute(query)
 		"""
 		if self.server_mode:
-			# Use server mode
 			result = self._run_server_query(query)
-			
 			if self.output == 'pandas':
 				json_str = json.dumps(result)
 				return pd.read_json(StringIO(json_str))
 			elif self.output == 'csv':
 				raise ValueError("CSV output is not supported in server_mode.")
 			else:  # Assume 'dict' output
 				return result
-			
 		else:
-			# Local mode handling (existing logic)
 			output = self._run_query(query)
-			if self.output == 'csv':
-				return output
-			elif self.output == 'pandas':
-				try:
-					return pd.read_json(StringIO(output))
-				except ValueError:
-					return pd.DataFrame([{"error": "Invalid JSON output: {}".format(output.strip())}])
-			else:  # Assume 'dict' output
-				try:
-					return json.loads(output)
-				except ValueError:
-					return [{"error": "Invalid JSON output: {}".format(output.strip())}]
+			if "exception" in output:
+				return {"error": output["exception"]}
+
+			if "data" in output:
+				# theres data, return it
+				if self.output == 'csv':
+					return output["data"]
+				elif self.output == 'pandas':
+					try:
+						return pd.read_json(StringIO(output["data"]))
+					except ValueError:
+						return pd.DataFrame([{"error": "Invalid JSON output"}])
+				else:  # Assume 'dict' output
+					try:
+						return json.loads(output["data"])
+					except ValueError:
+						return {"error": "Invalid JSON output"}            
+			else:
+				if "error" in output:
+					if suppress_errors:
+						return []
+					else:
+						return {"error": output["error"]}
 
 	#
 	# asnyc query support
 	#
 
 	def _run_server_query_with_new_connection(self, query):
 		"""Run a query against a StackQL postgres wire protocol server with a new connection.
@@ -582,15 +602,21 @@
 			# Directly get the list of dicts; no JSON string conversion needed.
 			result = self._run_server_query_with_new_connection(query)
 		elif self.server_mode:
 			# Also directly get the list of dicts here.
 			result = self._run_server_query(query)  # Assuming this is a method that exists
 		else:
 			# Convert the JSON string to a Python object (list of dicts).
-			result = json.loads(self._run_query(query))
+			query_results = self._run_query(query)
+			if "exception" in query_results:
+				result = [{"error": query_results["exception"]}]
+			if "error" in query_results:
+				result = [{"error": query_results["error"]}]
+			if "data" in query_results:
+				result = json.loads(query_results["data"]) 
 		# Convert the result to a DataFrame if necessary.
 		if self.output == 'pandas':
 			return pd.DataFrame(result)
 		else:
 			return result
 
 	async def executeQueriesAsync(self, queries):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pystackql-3.5.3/pystackql.egg-info/PKG-INFO` & `pystackql-3.5.4/pystackql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystackql
-Version: 3.5.3
+Version: 3.5.4
 Summary: A Python interface for StackQL
 Home-page: https://github.com/stackql/pystackql
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT License
         
         Copyright (c) 2022 StackQL Studios
@@ -231,10 +231,10 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload dist/pystackql-3.5.3.tar.gz
+    twine upload dist/pystackql-3.5.4.tar.gz
```

### Comparing `pystackql-3.5.3/setup.py` & `pystackql-3.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 with open('LICENSE') as f:
     license = f.read()
 
 setup(
     name='pystackql',
-    version='3.5.3',
+    version='3.5.4',
     description='A Python interface for StackQL',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/pystackql',
     license=license,
     packages=['pystackql'],
```

