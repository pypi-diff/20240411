# Comparing `tmp/alita_tools-0.0.5.tar.gz` & `tmp/alita_tools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alita_tools-0.0.5.tar", last modified: Thu Apr  4 06:35:27 2024, max compression
+gzip compressed data, was "alita_tools-0.0.6.tar", last modified: Thu Apr 11 12:50:02 2024, max compression
```

## Comparing `alita_tools-0.0.5.tar` & `alita_tools-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/
--rwx------   0 arozumenko   (501) staff       (20)    11357 2024-03-30 06:45:53.000000 alita_tools-0.0.5/LICENSE
--rwx------   0 arozumenko   (501) staff       (20)      993 2024-04-04 06:35:27.780000 alita_tools-0.0.5/PKG-INFO
--rwx------   0 arozumenko   (501) staff       (20)      102 2024-03-30 06:45:53.000000 alita_tools-0.0.5/README.md
--rwx------   0 arozumenko   (501) staff       (20)      809 2024-04-03 08:00:02.000000 alita_tools-0.0.5/pyproject.toml
--rwx------   0 arozumenko   (501) staff       (20)      148 2024-04-03 06:36:12.000000 alita_tools-0.0.5/requirements.txt
--rwx------   0 arozumenko   (501) staff       (20)       38 2024-04-04 06:35:27.790000 alita_tools-0.0.5/setup.cfg
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 17:59:06.000000 alita_tools-0.0.5/src/__init__.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/alita_tools/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 06:51:51.000000 alita_tools-0.0.5/src/alita_tools/__init__.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/alita_tools/base/
--rwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 14:42:43.000000 alita_tools-0.0.5/src/alita_tools/base/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)      719 2024-04-02 15:17:01.000000 alita_tools-0.0.5/src/alita_tools/base/tool.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/alita_tools/confluence/
--rwx------   0 arozumenko   (501) staff       (20)     1077 2024-04-02 14:44:26.000000 alita_tools-0.0.5/src/alita_tools/confluence/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)    10955 2024-04-02 06:41:36.000000 alita_tools-0.0.5/src/alita_tools/confluence/api_wrapper.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/alita_tools/datasources/
--rwx------   0 arozumenko   (501) staff       (20)     1773 2024-04-03 08:43:31.000000 alita_tools-0.0.5/src/alita_tools/datasources/__init__.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/alita_tools/github/
--rwx------   0 arozumenko   (501) staff       (20)      979 2024-04-02 06:55:08.000000 alita_tools-0.0.5/src/alita_tools/github/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)    15406 2024-04-04 06:35:17.000000 alita_tools-0.0.5/src/alita_tools/github/api_wrapper.py
--rwx------   0 arozumenko   (501) staff       (20)      907 2024-04-02 11:15:34.000000 alita_tools-0.0.5/src/alita_tools/github/tool.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.740000 alita_tools-0.0.5/src/alita_tools/jira/
--rwx------   0 arozumenko   (501) staff       (20)     1059 2024-04-02 14:44:32.000000 alita_tools-0.0.5/src/alita_tools/jira/__init__.py
--rwx------   0 arozumenko   (501) staff       (20)    11399 2024-04-02 16:05:32.000000 alita_tools-0.0.5/src/alita_tools/jira/api_wrapper.py
-drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-04 06:35:27.730000 alita_tools-0.0.5/src/alita_tools.egg-info/
--rwx------   0 arozumenko   (501) staff       (20)      993 2024-04-04 06:35:27.000000 alita_tools-0.0.5/src/alita_tools.egg-info/PKG-INFO
--rwx------   0 arozumenko   (501) staff       (20)      643 2024-04-04 06:35:27.000000 alita_tools-0.0.5/src/alita_tools.egg-info/SOURCES.txt
--rwx------   0 arozumenko   (501) staff       (20)        1 2024-04-04 06:35:27.000000 alita_tools-0.0.5/src/alita_tools.egg-info/dependency_links.txt
--rwx------   0 arozumenko   (501) staff       (20)      149 2024-04-04 06:35:27.000000 alita_tools-0.0.5/src/alita_tools.egg-info/requires.txt
--rwx------   0 arozumenko   (501) staff       (20)       21 2024-04-04 06:35:27.000000 alita_tools-0.0.5/src/alita_tools.egg-info/top_level.txt
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-11 12:50:02.470000 alita_tools-0.0.6/
+-rwx------   0 arozumenko   (501) staff       (20)    11357 2024-03-30 06:45:53.000000 alita_tools-0.0.6/LICENSE
+-rwx------   0 arozumenko   (501) staff       (20)     1040 2024-04-11 12:50:02.760000 alita_tools-0.0.6/PKG-INFO
+-rwx------   0 arozumenko   (501) staff       (20)      102 2024-03-30 06:45:53.000000 alita_tools-0.0.6/README.md
+-rwx------   0 arozumenko   (501) staff       (20)      809 2024-04-11 12:47:56.000000 alita_tools-0.0.6/pyproject.toml
+-rwx------   0 arozumenko   (501) staff       (20)      180 2024-04-11 12:47:43.000000 alita_tools-0.0.6/requirements.txt
+-rwx------   0 arozumenko   (501) staff       (20)       38 2024-04-11 12:50:02.760000 alita_tools-0.0.6/setup.cfg
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-11 12:50:02.490000 alita_tools-0.0.6/src/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 17:59:06.000000 alita_tools-0.0.6/src/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-11 12:50:02.510000 alita_tools-0.0.6/src/alita_tools/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-03-30 06:51:51.000000 alita_tools-0.0.6/src/alita_tools/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-11 12:50:02.550000 alita_tools-0.0.6/src/alita_tools/base/
+-rwx------   0 arozumenko   (501) staff       (20)        0 2024-04-02 14:42:43.000000 alita_tools-0.0.6/src/alita_tools/base/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)      719 2024-04-02 15:17:01.000000 alita_tools-0.0.6/src/alita_tools/base/tool.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-11 12:50:02.570000 alita_tools-0.0.6/src/alita_tools/confluence/
+-rwx------   0 arozumenko   (501) staff       (20)     1077 2024-04-02 14:44:26.000000 alita_tools-0.0.6/src/alita_tools/confluence/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    10955 2024-04-02 06:41:36.000000 alita_tools-0.0.6/src/alita_tools/confluence/api_wrapper.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-11 12:50:02.600000 alita_tools-0.0.6/src/alita_tools/datasources/
+-rwx------   0 arozumenko   (501) staff       (20)     1996 2024-04-11 07:37:21.000000 alita_tools-0.0.6/src/alita_tools/datasources/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-11 12:50:02.620000 alita_tools-0.0.6/src/alita_tools/github/
+-rwx------   0 arozumenko   (501) staff       (20)      979 2024-04-02 06:55:08.000000 alita_tools-0.0.6/src/alita_tools/github/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    15406 2024-04-04 06:35:17.000000 alita_tools-0.0.6/src/alita_tools/github/api_wrapper.py
+-rwx------   0 arozumenko   (501) staff       (20)      907 2024-04-02 11:15:34.000000 alita_tools-0.0.6/src/alita_tools/github/tool.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-11 12:50:02.640000 alita_tools-0.0.6/src/alita_tools/jira/
+-rwx------   0 arozumenko   (501) staff       (20)     1059 2024-04-02 14:44:32.000000 alita_tools-0.0.6/src/alita_tools/jira/__init__.py
+-rwx------   0 arozumenko   (501) staff       (20)    11532 2024-04-09 08:08:34.000000 alita_tools-0.0.6/src/alita_tools/jira/api_wrapper.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-11 12:50:02.670000 alita_tools-0.0.6/src/alita_tools/openapi/
+-rwx------   0 arozumenko   (501) staff       (20)     2394 2024-04-11 12:28:08.000000 alita_tools-0.0.6/src/alita_tools/openapi/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-11 12:50:02.690000 alita_tools-0.0.6/src/alita_tools/prompts/
+-rwx------   0 arozumenko   (501) staff       (20)      742 2024-04-11 07:37:27.000000 alita_tools-0.0.6/src/alita_tools/prompts/__init__.py
+drwx------   0 arozumenko   (501) staff       (20)        0 2024-04-11 12:50:02.530000 alita_tools-0.0.6/src/alita_tools.egg-info/
+-rwx------   0 arozumenko   (501) staff       (20)     1040 2024-04-11 12:50:02.000000 alita_tools-0.0.6/src/alita_tools.egg-info/PKG-INFO
+-rwx------   0 arozumenko   (501) staff       (20)      715 2024-04-11 12:50:02.000000 alita_tools-0.0.6/src/alita_tools.egg-info/SOURCES.txt
+-rwx------   0 arozumenko   (501) staff       (20)        1 2024-04-11 12:50:02.000000 alita_tools-0.0.6/src/alita_tools.egg-info/dependency_links.txt
+-rwx------   0 arozumenko   (501) staff       (20)      181 2024-04-11 12:50:02.000000 alita_tools-0.0.6/src/alita_tools.egg-info/requires.txt
+-rwx------   0 arozumenko   (501) staff       (20)       21 2024-04-11 12:50:02.000000 alita_tools-0.0.6/src/alita_tools.egg-info/top_level.txt
```

### Comparing `alita_tools-0.0.5/LICENSE` & `alita_tools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.5/PKG-INFO` & `alita_tools-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Default set of tools and toolkits available within ProjectAlita and CodeMie applications.
 Author-email: Artem Rozumenko <support@projectalita.ai>, Vadym Vlasenko <vadym_vlasenko@epam.com>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/application-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,11 +14,12 @@
 Requires-Dist: pydantic==1.10.9
 Requires-Dist: langchain_core==0.1.30
 Requires-Dist: langchain==0.1.11
 Requires-Dist: pygithub==2.3.0
 Requires-Dist: atlassian_python_api==3.41.11
 Requires-Dist: markdownify==0.12.1
 Requires-Dist: pillow==10.2.0
-Requires-Dist: alita_sdk
+Requires-Dist: requests_openapi==1.0.5
+Requires-Dist: alita_sdk==0.0.16
 
 # application-tools
 Default set of tools available in ProjectAlita and CodeMie application interfaces
```

### Comparing `alita_tools-0.0.5/pyproject.toml` & `alita_tools-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alita_tools"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Artem Rozumenko", email="support@projectalita.ai" },
   { name="Vadym Vlasenko", email="vadym_vlasenko@epam.com"}
 ]
 description = "Default set of tools and toolkits available within ProjectAlita and CodeMie applications."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `alita_tools-0.0.5/src/alita_tools/base/tool.py` & `alita_tools-0.0.6/src/alita_tools/base/tool.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.5/src/alita_tools/confluence/__init__.py` & `alita_tools-0.0.6/src/alita_tools/confluence/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.5/src/alita_tools/confluence/api_wrapper.py` & `alita_tools-0.0.6/src/alita_tools/confluence/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.5/src/alita_tools/github/__init__.py` & `alita_tools-0.0.6/src/alita_tools/github/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.5/src/alita_tools/github/api_wrapper.py` & `alita_tools-0.0.6/src/alita_tools/github/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.5/src/alita_tools/github/tool.py` & `alita_tools-0.0.6/src/alita_tools/github/tool.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.5/src/alita_tools/jira/__init__.py` & `alita_tools-0.0.6/src/alita_tools/jira/__init__.py`

 * *Files identical despite different names*

### Comparing `alita_tools-0.0.5/src/alita_tools/jira/api_wrapper.py` & `alita_tools-0.0.6/src/alita_tools/jira/api_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     issue_key: str = Field(
         description="""The issue key of the Jira issue to which the comment is to be added, e.g. "TEST-123"."""
     )
     comment: str = Field(description="""The comment to be added to the Jira issue, e.g. "This is a test comment.""")
 
 
 
-
 class JiraApiWrapper(BaseModel):
     base_url: str
     api_key: Optional[str] = None,
     username: Optional[str] = None
     token: Optional[str] = None
     cloud: Optional[bool] = True
     limit: Optional[int] = 5
@@ -127,27 +126,27 @@
             parsed.append(
                 {"id": id, "key": key, "name": name, "type": type, "style": style}
             )
         return parsed
 
     
     def create_issue_validate(self, params: Dict[str, Any]):
-        if "fields" not in params:
+        if params.get("fields") is None:
             raise ToolException("""
             Jira fields are provided in a wrong way.
             For example, to create a low priority task called "test issue" with description "test description", you would pass in the following STRING dictionary:
             {{"fields: {{{{"project": {{"key": "project_key"}}, "summary": "test issue", "description": "test description", "issuetype": {{"name": "Task"}}, "priority": {{"name": "Major"}}}}}}
             """)
-        if "project" not in params["fields"]:
+        if params["fields"].get("project") is None:
             raise ToolException("Jira project key is required to create an issue. Ask user to provide it.")
     
     def update_issue_validate(self, params: Dict[str, Any]):
-        if "key" not in params:
+        if params.get("key") is None:
             raise ToolException("Jira issue key is required to update an issue. Ask user to provide it.")
-        if "fields" not in params:
+        if params.get("fields") is None:
             raise ToolException("""
         Jira fields are provided in a wrong way.
         For example, to update a task with key XXX-123 with new summary, description and custom field, you would pass in the following STRING dictionary: 
         {{"key": "issue key", "fields": {{"summary": "updated issue", "description": "updated description", "customfield_xxx": "updated custom field"}}}}
         """)
 
 
@@ -163,14 +162,16 @@
         try:
             params = json.loads(issue_json)
             self.create_issue_validate(params)
             issue = self.client.issue_create(fields=dict(params["fields"]))
             issue_url = f"{self.client.url}browse/{issue['key']}"
             logger.info(f"issue is created: {issue}")
             return f"Done. Issue {issue['key']} is created successfully. You can view it at {issue_url}. Details: {str(issue)}"
+        except ToolException as e:
+            raise e
         except Exception as e:
             stacktrace = format_exc()
             logger.error(f"Error creating Jira issue: {stacktrace}")
             raise ToolException(f"Error creating Jira issue: {stacktrace}")
     
     def update_issue(self, issue_json: str):
         """ Update an issue in Jira."""
@@ -180,14 +181,16 @@
             key = params["key"]
             fields = {"fields": dict(params["fields"])}
             issue = self.client.update_issue(issue_key=key, update=dict(fields))
             issue_url = f"{self.client.url}browse/{key}"
             output = f"Done. Issue {key} has been updated successfully. You can view it at {issue_url}. Details: {str(issue)}"
             logger.info(output)
             return output
+        except ToolException as e:
+            raise e
         except Exception as e:
             stacktrace = format_exc()
             logger.error(f"Error updating Jira issue: {stacktrace}")
             return f"Error updating Jira issue: {stacktrace}"
 
     def add_comments(self, issue_key: str, comment: str):
         """ Add a comment to a Jira issue."""
```

### Comparing `alita_tools-0.0.5/src/alita_tools.egg-info/PKG-INFO` & `alita_tools-0.0.6/src/alita_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Default set of tools and toolkits available within ProjectAlita and CodeMie applications.
 Author-email: Artem Rozumenko <support@projectalita.ai>, Vadym Vlasenko <vadym_vlasenko@epam.com>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/application-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,11 +14,12 @@
 Requires-Dist: pydantic==1.10.9
 Requires-Dist: langchain_core==0.1.30
 Requires-Dist: langchain==0.1.11
 Requires-Dist: pygithub==2.3.0
 Requires-Dist: atlassian_python_api==3.41.11
 Requires-Dist: markdownify==0.12.1
 Requires-Dist: pillow==10.2.0
-Requires-Dist: alita_sdk
+Requires-Dist: requests_openapi==1.0.5
+Requires-Dist: alita_sdk==0.0.16
 
 # application-tools
 Default set of tools available in ProjectAlita and CodeMie application interfaces
```

### Comparing `alita_tools-0.0.5/src/alita_tools.egg-info/SOURCES.txt` & `alita_tools-0.0.6/src/alita_tools.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 src/alita_tools/confluence/__init__.py
 src/alita_tools/confluence/api_wrapper.py
 src/alita_tools/datasources/__init__.py
 src/alita_tools/github/__init__.py
 src/alita_tools/github/api_wrapper.py
 src/alita_tools/github/tool.py
 src/alita_tools/jira/__init__.py
-src/alita_tools/jira/api_wrapper.py
+src/alita_tools/jira/api_wrapper.py
+src/alita_tools/openapi/__init__.py
+src/alita_tools/prompts/__init__.py
```

