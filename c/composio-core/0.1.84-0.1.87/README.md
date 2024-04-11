# Comparing `tmp/composio_core-0.1.84.tar.gz` & `tmp/composio_core-0.1.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.84.tar", last modified: Sun Apr  7 19:52:51 2024, max compression
+gzip compressed data, was "composio_core-0.1.87.tar", last modified: Thu Apr 11 12:40:19 2024, max compression
```

## Comparing `composio_core-0.1.84.tar` & `composio_core-0.1.87.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:52:51.413766 composio_core-0.1.84/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-02 18:29:17.000000 composio_core-0.1.84/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)      770 2024-04-07 19:52:51.413565 composio_core-0.1.84/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-02 18:29:17.000000 composio_core-0.1.84/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:52:51.409611 composio_core-0.1.84/composio/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      176 2024-04-02 18:29:17.000000 composio_core-0.1.84/composio/__init__.py
--rwxr-xr-x   0 karanvaidya   (501) staff       (20)    12769 2024-04-07 19:52:31.000000 composio_core-0.1.84/composio/composio_cli.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:52:51.411641 composio_core-0.1.84/composio/sdk/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-02 18:29:17.000000 composio_core-0.1.84/composio/sdk/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     5864 2024-04-07 18:28:35.000000 composio_core-0.1.84/composio/sdk/core.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    10555 2024-04-07 19:51:58.000000 composio_core-0.1.84/composio/sdk/enums.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    16559 2024-04-07 18:28:35.000000 composio_core-0.1.84/composio/sdk/sdk.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2107 2024-04-07 15:47:29.000000 composio_core-0.1.84/composio/sdk/storage.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2861 2024-04-06 13:52:08.000000 composio_core-0.1.84/composio/sdk/utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:52:51.413310 composio_core-0.1.84/composio_core.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      770 2024-04-07 19:52:51.000000 composio_core-0.1.84/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      466 2024-04-07 19:52:51.000000 composio_core-0.1.84/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 19:52:51.000000 composio_core-0.1.84/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-07 19:52:51.000000 composio_core-0.1.84/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       91 2024-04-07 19:52:51.000000 composio_core-0.1.84/composio_core.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-07 19:52:51.000000 composio_core-0.1.84/composio_core.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      509 2024-04-06 13:53:19.000000 composio_core-0.1.84/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       92 2024-04-06 13:54:53.000000 composio_core-0.1.84/requirements.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 19:52:51.413808 composio_core-0.1.84/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1134 2024-04-07 19:52:16.000000 composio_core-0.1.84/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:19.874112 composio_core-0.1.87/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-02 18:29:17.000000 composio_core-0.1.87/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      798 2024-04-11 12:40:19.873878 composio_core-0.1.87/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-02 18:29:17.000000 composio_core-0.1.87/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:19.870844 composio_core-0.1.87/composio/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      176 2024-04-02 18:29:17.000000 composio_core-0.1.87/composio/__init__.py
+-rwxr-xr-x   0 karanvaidya   (501) staff       (20)    18767 2024-04-11 12:39:00.000000 composio_core-0.1.87/composio/composio_cli.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:19.872444 composio_core-0.1.87/composio/sdk/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-02 18:29:17.000000 composio_core-0.1.87/composio/sdk/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     6564 2024-04-11 12:39:00.000000 composio_core-0.1.87/composio/sdk/core.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    10555 2024-04-11 12:39:00.000000 composio_core-0.1.87/composio/sdk/enums.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    17472 2024-04-11 12:39:00.000000 composio_core-0.1.87/composio/sdk/sdk.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2300 2024-04-11 12:39:00.000000 composio_core-0.1.87/composio/sdk/storage.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2997 2024-04-11 12:39:00.000000 composio_core-0.1.87/composio/sdk/utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:19.873585 composio_core-0.1.87/composio_core.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      798 2024-04-11 12:40:19.000000 composio_core-0.1.87/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      466 2024-04-11 12:40:19.000000 composio_core-0.1.87/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-11 12:40:19.000000 composio_core-0.1.87/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-11 12:40:19.000000 composio_core-0.1.87/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      104 2024-04-11 12:40:19.000000 composio_core-0.1.87/composio_core.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-11 12:40:19.000000 composio_core-0.1.87/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      529 2024-04-11 12:39:00.000000 composio_core-0.1.87/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      105 2024-04-11 12:39:00.000000 composio_core-0.1.87/requirements.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-11 12:40:19.874159 composio_core-0.1.87/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1128 2024-04-11 12:39:53.000000 composio_core-0.1.87/setup.py
```

### Comparing `composio_core-0.1.84/PKG-INFO` & `composio_core-0.1.87/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.84
+Version: 0.1.87
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,11 +13,12 @@
 Requires-Dist: requests
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: beaupy>=3.7.2
 Requires-Dist: termcolor>=2.4.0
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: openai>=1.14.1
+Requires-Dist: rich>=13.7.1
 
 # Composio Core Package
 
 Core package to act as a bridge between composio platform and other services.
```

### Comparing `composio_core-0.1.84/composio/sdk/core.py` & `composio_core-0.1.87/composio/sdk/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 class FrameworkEnum(Enum):
     AUTOGEN = "autogen"
     LANGCHAIN = "langchain"
 
 __IS_FIRST_TIME__ = True
 
+class UnauthorizedAccessException(Exception):
+    pass
+
 class ComposioCore:
     sdk: Composio = None
     framework: FrameworkEnum = None
 
     def __init__(self, base_url = get_base_url(), manage_auth = True, framework: FrameworkEnum = None):
         global __IS_FIRST_TIME__
 
@@ -46,14 +49,20 @@
                                 "name": git_info.name,
                                 "email": git_info.email
                             } if git_info.name and git_info.email else None
                         });
                         __IS_FIRST_TIME__ = False
                     except:
                         pass
+    
+    def get_authenticated_user(self):
+        api_key = get_api_key()
+        return {
+            "api_key": api_key,
+        }
 
     def is_authenticated(self):
         if self.sdk is None:
             return False
         return True
 
     def set_base_url(self, base_url: str):
@@ -66,30 +75,31 @@
     def logout(self):
         self.http_client.headers.pop('x-api-key')
         user_data = load_user_data()
         user_data.pop('api_key')
         delete_user_connections()
         save_user_data(user_data)
 
-    def authenticate(self, hash: str):
-        resp = self.http_client.post(f"{self.base_url}/v1/client/auth/identify", json={
-            "hash": hash,
-        });
-        if resp.status_code == 202:
-            api_key = resp.json().get('apiKey')
-            self.http_client.headers.update({
-                'Content-Type': 'application/json',
-                'x-api-key': api_key
-            })
-            self.sdk = Composio(api_key, self.base_url)
-            if self.manage_auth:
-                save_api_key(api_key)
-            return api_key
+    def generate_cli_auth_session(self):
+        resp = self.http_client.get(f"{self.base_url}/v1/cli/generate-cli-session");
+        if resp.status_code == 200:
+            resp = resp.json()
+            if resp.get('key'):
+                return resp['key']
 
-        raise Exception("Failed to authenticate")
+        raise Exception("Bad request to cli/generate-cli-session")
+    
+    def verify_cli_auth_session(self, key: str, code: str):
+        resp = self.http_client.get(f"{self.base_url}/v1/cli/verify-cli-code?key={key}&code={code}");
+        if resp.status_code == 200:
+            return resp.json()
+        elif resp.status_code == 401:
+            raise UnauthorizedAccessException("UnauthorizedError: Unauthorized access to cli/verify-cli-session")
+        
+        raise Exception("Bad request to cli/verify-cli-session")
     
     def initiate_connection(self, integrationId: Union[str, TestIntegration]) -> ConnectionRequest:
         if isinstance(integrationId, TestIntegration):
             integrationId = integrationId.value
 
         resp = self.http_client.post(f"{self.base_url}/v1/connectedAccounts", json={
             "integrationId": integrationId,
@@ -101,14 +111,24 @@
     
     def set_global_trigger(self, callback_url: str):
         try:
             self.sdk.set_global_trigger(callback_url)
         except Exception as e:
             raise Exception(f"Failed to set global trigger: {e}")
 
+    def disable_trigger(self, trigger_id: str):
+        return self.sdk.disable_trigger(trigger_id)
+ 
+    def list_active_triggers(self, trigger_ids: list[str] = None):
+        try:
+            resp = self.sdk.list_active_triggers(trigger_ids)
+            return resp
+        except Exception as e:
+            raise e
+
     def list_triggers(self, app_name: str):
         try:
             return self.sdk.list_triggers([app_name])
         except Exception as e:
             raise Exception(f"Failed to list triggers: {e}")
         
     def get_trigger_requirements(self, trigger_ids: list[str] = None):
@@ -133,15 +153,15 @@
         if not connectionId:
             raise Exception(f"User not authenticated or connection not found. Please authenticate using: composio-cli add {tool_name}")
 
         account = self.sdk.get_connected_account(connectionId)
         resp = account.execute_action(action, params)
         return resp
 
-    def get_list_of_connections(self, app_name: list[App | str] = None) -> list[ConnectedAccount]:
+    def get_list_of_connections(self, app_name: list[Union[App, str]] = None) -> list[ConnectedAccount]:
         for i, item in enumerate(app_name):
             if isinstance(item, App):
                 app_name[i] = item.value
 
         if app_name is not None:
             resp = [item for item in resp if item.appUniqueId in app_name]
```

### Comparing `composio_core-0.1.84/composio/sdk/enums.py` & `composio_core-0.1.87/composio/sdk/enums.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,206 +1,220 @@
 from enum import Enum
 
 class App(Enum):
-    ACCELO = "accelo"
-    SLACK = "slack"
+    GMAIL = "gmail"
+    ATTIO = "attio"
     ZENDESK = "zendesk"
-    ZOHO = "zoho"
-    APIFY = "apify"
-    GOOGLE_DRIVE = "google-drive"
-    EVENTBRITE = "eventbrite"
-    CALENDLY = "calendly"
+    TODOIST = "todoist"
+    KLAVIYO = "klaviyo"
+    BITBUCKET = "bitbucket"
+    MONDAY = "monday"
+    SLACK = "slack"
+    CLICKUP = "clickup"
+    DISCORD = "discord"
+    STRAVA = "strava"
     DROPBOX = "dropbox"
-    MIRO = "miro"
-    ZOHO_DESK = "zoho_desk"
-    HACKERRANK_WORK = "hackerrank-work"
-    ZOHO_INVENTORY = "zoho_inventory"
+    INTERCOM = "intercom"
+    SHOPIFY = "shopify"
     GOOGLE_SHEETS = "google-sheets"
-    ZOHO_INVOICE = "zoho_invoice"
+    ASANA = "asana"
+    EVENTBRITE = "eventbrite"
+    LINEAR = "linear"
     HUBSPOT = "hubspot"
-    ZOOM = "zoom"
-    GOOGLE_DOCS = "google-docs"
-    GURU = "guru"
-    GITHUB_OPEN_API_SPEC = "github_open_api_spec"
     JIRA = "jira"
-    GMAIL = "gmail"
-    FRESHDESK = "freshdesk"
-    FRONT = "front"
-    GORGIAS = "gorgias"
+    NOTION = "notion"
+    TASKADE = "taskade"
+    GOOGLE_DRIVE = "google-drive"
     GITLAB = "gitlab"
-    GOOGLE_CALENDAR = "google_calendar"
-    DISCORD = "discord"
-    ATLASSIAN = "atlassian"
-    ASANA = "asana"
-    CLICKUP = "clickup"
-    AMAZON = "amazon"
-    PIPEDRIVE = "pipedrive"
-    FRESHBOOKS = "freshbooks"
-    BITBUCKET = "bitbucket"
-    BAMBOOHR = "bamboohr"
-    BOLDSIGN = "boldsign"
-    MAILCHIMP = "mailchimp"
-    MONDAY = "monday"
-    LINEAR = "linear"
+    MIXPANEL = "mixpanel"
+    GOOGLE_DOCS = "google-docs"
     GUMROAD = "gumroad"
-    FIGMA = "figma"
-    PAGERDUTY = "pagerduty"
-    DEEL = "deel"
-    SMUGMUG = "smugmug"
-    GITHUB = "github"
-    TRELLO = "trello"
-    ATTIO = "attio"
-    STRAVA = "strava"
+    MAILCHIMP = "mailchimp"
     BOX = "box"
-    TASKADE = "taskade"
+    MIRO = "miro"
     KEAP = "keap"
+    SPLITWISE = "splitwise"
+    PAGERDUTY = "pagerduty"
+    ZOOM = "zoom"
+    TIMELY = "timely"
+    ZOHO = "zoho"
+    FRESHDESK = "freshdesk"
+    FIGMA = "figma"
+    PIPEDRIVE = "pipedrive"
+    APIFY = "apify"
     TWITCH = "twitch"
-    HARVEST = "harvest"
-    INTERCOM = "intercom"
-    KLAVIYO = "klaviyo"
-    NOTION = "notion"
-    SERVICEM8 = "servicem8"
-    SHORTCUT = "shortcut"
-    SHOPIFY = "shopify"
-    MIXPANEL = "mixpanel"
-    SALESFORCE = "salesforce"
+    STACK_EXCHANGE = "stack-exchange"
+    GITHUB_OPEN_API_SPEC = "github_open_api_spec"
+    ACCELO = "accelo"
     REDDIT = "reddit"
-    TODOIST = "todoist"
     SURVEY_MONKEY = "survey-monkey"
-    STACK_EXCHANGE = "stack-exchange"
-    TIMELY = "timely"
-    SPLITWISE = "splitwise"
-    XERO = "xero"
-    WAKATIME = "wakatime"
-    TYPEFORM = "typeform"
     TWITTER = "twitter"
+    XERO = "xero"
+    ZOHO_INVENTORY = "zoho_inventory"
+    ZOHO_MAIL = "zoho_mail"
+    AMAZON = "amazon"
+    SERVICEM8 = "servicem8"
+    SHORTCUT = "shortcut"
     ZOHO_BOOKS = "zoho_books"
+    ZOHO_INVOICE = "zoho_invoice"
+    GORGIAS = "gorgias"
+    SALESFORCE = "salesforce"
+    SMUGMUG = "smugmug"
+    WAKATIME = "wakatime"
     ZOHO_BIGIN = "zoho_bigin"
-    ZOHO_MAIL = "zoho_mail"
+    ZOHO_DESK = "zoho_desk"
+    HACKERRANK_WORK = "hackerrank-work"
+    BOLDSIGN = "boldsign"
+    GURU = "guru"
+    BAMBOOHR = "bamboohr"
+    HARVEST = "harvest"
+    ATLASSIAN = "atlassian"
+    DEEL = "deel"
+    FRONT = "front"
+    GITHUB = "github"
+    FRESHBOOKS = "freshbooks"
+    CALENDLY = "calendly"
+    TRELLO = "trello"
+    TYPEFORM = "typeform"
+    GOOGLE_CALENDAR = "google_calendar"
 
 class TestIntegration(Enum):
-    ACCELO = "test-accelo-connector"
-    SLACK = "test-slack-connector"
+    GMAIL = "test-gmail-connector"
+    ATTIO = "test-attio-connector"
     ZENDESK = "test-zendesk-connector"
-    ZOHO = "test-zoho-connector"
-    APIFY = "test-apify-connector"
-    GOOGLE_DRIVE = "test-google-drive-connector"
-    EVENTBRITE = "test-eventbrite-connector"
-    CALENDLY = "test-calendly-connector"
+    TODOIST = "test-todoist-connector"
+    KLAVIYO = "test-klaviyo-connector"
+    BITBUCKET = "test-bitbucket-connector"
+    MONDAY = "test-monday-connector"
+    SLACK = "test-slack-connector"
+    CLICKUP = "test-clickup-connector"
+    DISCORD = "test-discord-connector"
+    STRAVA = "test-strava-connector"
     DROPBOX = "test-dropbox-connector"
-    MIRO = "test-miro-connector"
-    ZOHO_DESK = "test-zoho_desk-connector"
-    HACKERRANK_WORK = "test-hackerrank-work-connector"
-    ZOHO_INVENTORY = "test-zoho_inventory-connector"
+    INTERCOM = "test-intercom-connector"
+    SHOPIFY = "test-shopify-connector"
     GOOGLE_SHEETS = "test-google-sheets-connector"
-    ZOHO_INVOICE = "test-zoho_invoice-connector"
+    ASANA = "test-asana-connector"
+    EVENTBRITE = "test-eventbrite-connector"
+    LINEAR = "test-linear-connector"
     HUBSPOT = "test-hubspot-connector"
-    ZOOM = "test-zoom-connector"
-    GOOGLE_DOCS = "test-google-docs-connector"
-    GURU = "test-guru-connector"
-    GITHUB_OPEN_API_SPEC = "test-github_open_api_spec-connector"
     JIRA = "test-jira-connector"
-    GMAIL = "test-gmail-connector"
-    FRESHDESK = "test-freshdesk-connector"
-    FRONT = "test-front-connector"
-    GORGIAS = "test-gorgias-connector"
+    NOTION = "test-notion-connector"
+    TASKADE = "test-taskade-connector"
+    GOOGLE_DRIVE = "test-google-drive-connector"
     GITLAB = "test-gitlab-connector"
-    GOOGLE_CALENDAR = "test-google_calendar-connector"
-    DISCORD = "test-discord-connector"
-    ATLASSIAN = "test-atlassian-connector"
-    ASANA = "test-asana-connector"
-    CLICKUP = "test-clickup-connector"
-    AMAZON = "test-amazon-connector"
-    PIPEDRIVE = "test-pipedrive-connector"
-    FRESHBOOKS = "test-freshbooks-connector"
-    BITBUCKET = "test-bitbucket-connector"
-    BAMBOOHR = "test-bamboohr-connector"
-    BOLDSIGN = "test-boldsign-connector"
-    MAILCHIMP = "test-mailchimp-connector"
-    MONDAY = "test-monday-connector"
-    LINEAR = "test-linear-connector"
+    MIXPANEL = "test-mixpanel-connector"
+    GOOGLE_DOCS = "test-google-docs-connector"
     GUMROAD = "test-gumroad-connector"
-    FIGMA = "test-figma-connector"
-    PAGERDUTY = "test-pagerduty-connector"
-    DEEL = "test-deel-connector"
-    SMUGMUG = "test-smugmug-connector"
-    GITHUB = "test-github-connector"
-    TRELLO = "test-trello-connector"
-    ATTIO = "test-attio-connector"
-    STRAVA = "test-strava-connector"
+    MAILCHIMP = "test-mailchimp-connector"
     BOX = "test-box-connector"
-    TASKADE = "test-taskade-connector"
+    MIRO = "test-miro-connector"
     KEAP = "test-keap-connector"
+    SPLITWISE = "test-splitwise-connector"
+    PAGERDUTY = "test-pagerduty-connector"
+    ZOOM = "test-zoom-connector"
+    TIMELY = "test-timely-connector"
+    ZOHO = "test-zoho-connector"
+    FRESHDESK = "test-freshdesk-connector"
+    FIGMA = "test-figma-connector"
+    PIPEDRIVE = "test-pipedrive-connector"
+    APIFY = "test-apify-connector"
     TWITCH = "test-twitch-connector"
-    HARVEST = "test-harvest-connector"
-    INTERCOM = "test-intercom-connector"
-    KLAVIYO = "test-klaviyo-connector"
-    NOTION = "test-notion-connector"
-    SERVICEM8 = "test-servicem8-connector"
-    SHORTCUT = "test-shortcut-connector"
-    SHOPIFY = "test-shopify-connector"
-    MIXPANEL = "test-mixpanel-connector"
-    SALESFORCE = "test-salesforce-connector"
+    STACK_EXCHANGE = "test-stack-exchange-connector"
+    GITHUB_OPEN_API_SPEC = "test-github_open_api_spec-connector"
+    ACCELO = "test-accelo-connector"
     REDDIT = "test-reddit-connector"
-    TODOIST = "test-todoist-connector"
     SURVEY_MONKEY = "test-survey-monkey-connector"
-    STACK_EXCHANGE = "test-stack-exchange-connector"
-    TIMELY = "test-timely-connector"
-    SPLITWISE = "test-splitwise-connector"
-    XERO = "test-xero-connector"
-    WAKATIME = "test-wakatime-connector"
-    TYPEFORM = "test-typeform-connector"
     TWITTER = "test-twitter-connector"
+    XERO = "test-xero-connector"
+    ZOHO_INVENTORY = "test-zoho_inventory-connector"
+    ZOHO_MAIL = "test-zoho_mail-connector"
+    AMAZON = "test-amazon-connector"
+    SERVICEM8 = "test-servicem8-connector"
+    SHORTCUT = "test-shortcut-connector"
     ZOHO_BOOKS = "test-zoho_books-connector"
+    ZOHO_INVOICE = "test-zoho_invoice-connector"
+    GORGIAS = "test-gorgias-connector"
+    SALESFORCE = "test-salesforce-connector"
+    SMUGMUG = "test-smugmug-connector"
+    WAKATIME = "test-wakatime-connector"
     ZOHO_BIGIN = "test-zoho_bigin-connector"
-    ZOHO_MAIL = "test-zoho_mail-connector"
+    ZOHO_DESK = "test-zoho_desk-connector"
+    HACKERRANK_WORK = "test-hackerrank-work-connector"
+    BOLDSIGN = "test-boldsign-connector"
+    GURU = "test-guru-connector"
+    BAMBOOHR = "test-bamboohr-connector"
+    HARVEST = "test-harvest-connector"
+    ATLASSIAN = "test-atlassian-connector"
+    DEEL = "test-deel-connector"
+    FRONT = "test-front-connector"
+    GITHUB = "test-github-connector"
+    FRESHBOOKS = "test-freshbooks-connector"
+    CALENDLY = "test-calendly-connector"
+    TRELLO = "test-trello-connector"
+    TYPEFORM = "test-typeform-connector"
+    GOOGLE_CALENDAR = "test-google_calendar-connector"
 
 class Action(Enum):
     def __init__(self, service, action):
         self.service = service
         self.action = action
 
-    SLACK_SEND_SLACK_MESSAGE = ("slack", "slack_send_slack_message")
-    SLACK_LIST_CHANNELS = ("slack", "slack_list_slack_channels")
-    SLACK_LIST_MEMBERS = ("slack", "slack_list_slack_members")
-    SLACK_LIST_MESSAGES = ("slack", "slack_list_slack_messages")
+    GMAIL_SEND_EMAIL = ("gmail", "gmail_send_email")
+    GMAIL_CREATE_EMAIL_DRAFT = ("gmail", "gmail_create_email_draft")
+    GMAIL_FIND_EMAIL_ID_IN_GMAIL = ("gmail", "gmail_find_email_id")
+    GMAIL_ADD_LABEL_TO_EMAIL = ("gmail", "gmail_add_label_to_email")
     ZENDESK_CREATE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_create_zendesk_organization")
     ZENDESK_DELETE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_delete_zendesk_organization")
     ZENDESK_COUNT_ZENDESK_ORGANIZATIONS = ("zendesk", "zendesk_count_zendesk_organizations")
     ZENDESK_GET_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_get_zendesk_organization")
     ZENDESK_GET_ZENDESK_ORGANIZATIONS = ("zendesk", "zendesk_get_all_zendesk_organizations")
     ZENDESK_UPDATE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_update_zendesk_organization")
     ZENDESK_CREATE_ZENDESK_TICKET = ("zendesk", "zendesk_create_zendesk_ticket")
     ZENDESK_DELETE_ZENDESK_TICKET = ("zendesk", "zendesk_delete_zendesk_ticket")
     ZENDESK_GET_ZENDESK_ABOUT_ME = ("zendesk", "zendesk_get_about_me")
-    APIFY_GET_APIFY_ACTORS = ("apify", "apify_list_apify_actors")
-    APIFY_CREATE_APIFY_ACTOR = ("apify", "apify_create_apify_actor")
-    APIFY_GET_ACTOR_ID = ("apify", "apify_get_actor_id")
-    APIFY_SEARCH_APIFY_STORE = ("apify", "apify_search_store")
-    APIFY_GET_LAST_RUN_DATA = ("apify", "apify_get_last_run_data")
-    APIFY_GET_APIFY_TASKS = ("apify", "apify_list_apify_tasks")
-    DROPBOX_GET_ABOUT_ME = ("dropbox", "dropbox_get_about_me")
-    GMAIL_SEND_EMAIL = ("gmail", "gmail_send_email")
-    GMAIL_CREATE_EMAIL_DRAFT = ("gmail", "gmail_create_email_draft")
-    GMAIL_FIND_EMAIL_ID_IN_GMAIL = ("gmail", "gmail_find_email_id")
-    GMAIL_ADD_LABEL_TO_EMAIL = ("gmail", "gmail_add_label_to_email")
-    ASANA_CREATE_SUBTASK = ("asana", "asana_create_subtask")
-    ASANA_GET_SUBTASKS = ("asana", "asana_get_subtasks")
+    SLACK_SEND_SLACK_MESSAGE = ("slack", "slack_send_slack_message")
+    SLACK_LIST_CHANNELS = ("slack", "slack_list_slack_channels")
+    SLACK_LIST_MEMBERS = ("slack", "slack_list_slack_members")
+    SLACK_LIST_MESSAGES = ("slack", "slack_list_slack_messages")
     CLICKUP_CREATE_TASK = ("clickup", "clickup_create_task")
     CLICKUP_GET_TASKS = ("clickup", "clickup_get_tasks")
     CLICKUP_GET_TASK = ("clickup", "clickup_get_task")
     CLICKUP_CREATE_LIST = ("clickup", "clickup_create_list")
     CLICKUP_GET_LISTS = ("clickup", "clickup_get_lists")
     CLICKUP_GET_SPACES = ("clickup", "clickup_get_spaces")
     CLICKUP_CREATE_SPACE = ("clickup", "clickup_create_space")
     CLICKUP_CREATE_FOLDER = ("clickup", "clickup_create_folder")
     CLICKUP_GET_FOLDERS = ("clickup", "clickup_get_folders")
+    DROPBOX_GET_ABOUT_ME = ("dropbox", "dropbox_get_about_me")
+    ASANA_CREATE_SUBTASK = ("asana", "asana_create_subtask")
+    ASANA_GET_SUBTASKS = ("asana", "asana_get_subtasks")
     LINEAR_CREATE_ISSUE = ("linear", "linear_create_linear_issue")
     LINEAR_GET_PROJECTS = ("linear", "linear_list_linear_projects")
     LINEAR_GET_TEAMS_BY_PROJECT = ("linear", "linear_list_linear_teams")
+    NOTION_GET_ABOUT_ME = ("notion", "notion_get_about_me")
+    NOTION_ADD_CONTENT_NOTION_PAGE = ("notion", "notion_add_notion_page_children")
+    NOTION_ARCHIVE_NOTION_PAGE = ("notion", "notion_archive_notion_page")
+    NOTION_CREATE_NOTION_DATABASE = ("notion", "notion_create_notion_database")
+    NOTION_CREATE_PAGE_COMMENT = ("notion", "notion_create_page_comment")
+    NOTION_CREATE_NOTION_PAGE = ("notion", "notion_create_notion_page")
+    NOTION_DELETE_BLOCKS = ("notion", "notion_delete_notion_page_children")
+    NOTION_FETCH_ALL_UNRESOLVED_COMMENTS = ("notion", "notion_fetch_notion_comment")
+    NOTION_FETCH_NOTION_DATABASE = ("notion", "notion_fetch_notion_database")
+    NOTION_FETCH_NOTION_PAGE = ("notion", "notion_fetch_notion_page")
+    NOTION_SEARCH_LIST_NOTION_PAGE = ("notion", "notion_search_notion_page")
+    NOTION_UPDATE_NOTION_DATABASE = ("notion", "notion_update_notion_database")
+    NOTION_FETCH_NOTION_BLOCKS = ("notion", "notion_fetch_notion_block")
+    NOTION_FETCH_NOTION_BLOCK_CHILDREN = ("notion", "notion_fetch_notion_child_block")
+    APIFY_GET_APIFY_ACTORS = ("apify", "apify_list_apify_actors")
+    APIFY_CREATE_APIFY_ACTOR = ("apify", "apify_create_apify_actor")
+    APIFY_GET_ACTOR_ID = ("apify", "apify_get_actor_id")
+    APIFY_SEARCH_APIFY_STORE = ("apify", "apify_search_store")
+    APIFY_GET_LAST_RUN_DATA = ("apify", "apify_get_last_run_data")
+    APIFY_GET_APIFY_TASKS = ("apify", "apify_list_apify_tasks")
     GITHUB_CREATE_ISSUE = ("github", "github_create_issue")
     GITHUB_GET_REPOSITORY = ("github", "github_list_github_repos")
     GITHUB_STAR_REPO = ("github", "github_star_repo")
     GITHUB_GET_ABOUT_ME = ("github", "github_get_about_me")
     GITHUB_FETCH_README = ("github", "github_fetch_readme")
     GITHUB_GET_COMMITS = ("github", "github_get_commits")
     GITHUB_GET_COMMITS_WITH_PATCH_FILE_FOR_THAT_COMMIT = ("github", "github_get_commits_with_code")
@@ -212,28 +226,14 @@
     TRELLO_ADD_TRELLO_CARD_COMMENT = ("trello", "trello_add_trello_card_comment")
     TRELLO_CREATE_TRELLO_LABEL = ("trello", "trello_create_trello_label")
     TRELLO_UPDATE_TRELLO_BOARD = ("trello", "trello_update_trello_board")
     TRELLO_GET_ABOUT_ME = ("trello", "trello_get_about_me")
     TRELLO_SEARCH_TRELLO = ("trello", "trello_search_trello")
     TRELLO_SEARCH_TRELLO_MEMBERS = ("trello", "trello_search_trello_member")
     TRELLO_UPDATE_TRELLO_CARD = ("trello", "trello_update_trello_card")
-    NOTION_GET_ABOUT_ME = ("notion", "notion_get_about_me")
-    NOTION_ADD_CONTENT_NOTION_PAGE = ("notion", "notion_add_notion_page_children")
-    NOTION_ARCHIVE_NOTION_PAGE = ("notion", "notion_archive_notion_page")
-    NOTION_CREATE_NOTION_DATABASE = ("notion", "notion_create_notion_database")
-    NOTION_CREATE_PAGE_COMMENT = ("notion", "notion_create_page_comment")
-    NOTION_CREATE_NOTION_PAGE = ("notion", "notion_create_notion_page")
-    NOTION_DELETE_BLOCKS = ("notion", "notion_delete_notion_page_children")
-    NOTION_FETCH_ALL_UNRESOLVED_COMMENTS = ("notion", "notion_fetch_notion_comment")
-    NOTION_FETCH_NOTION_DATABASE = ("notion", "notion_fetch_notion_database")
-    NOTION_FETCH_NOTION_PAGE = ("notion", "notion_fetch_notion_page")
-    NOTION_SEARCH_LIST_NOTION_PAGE = ("notion", "notion_search_notion_page")
-    NOTION_UPDATE_NOTION_DATABASE = ("notion", "notion_update_notion_database")
-    NOTION_FETCH_NOTION_BLOCKS = ("notion", "notion_fetch_notion_block")
-    NOTION_FETCH_NOTION_BLOCK_CHILDREN = ("notion", "notion_fetch_notion_child_block")
     TYPEFORM_GET_ABOUT_ME = ("typeform", "typeform_get_about_me")
 
 class Trigger(Enum):
     def __init__(self, service, trigger):
         self.service = service
         self.trigger = trigger
```

### Comparing `composio_core-0.1.84/composio/sdk/sdk.py` & `composio_core-0.1.87/composio/sdk/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,22 @@
     access_token: Optional[str] = None
     client_secret: Optional[str] = None
     consumer_id: Optional[str] = None
     consumer_secret: Optional[str] = None
     headers: Optional[dict] = None
     queryParams: Optional[dict] = None
 
+class ActiveTrigger(BaseModel):
+    id: str
+    connectionId: str
+    triggerName: str
+    triggerConfig: dict
+
+    def __init__(self, sdk_instance: "Composio", **data):
+        super().__init__(**data)
 
 class ConnectedAccount(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     integrationId: str
     connectionParams: AuthConnectionParams
     appUniqueId: str
     id: str
@@ -187,14 +195,31 @@
 
     def list_triggers(self, app_names: list[str] = None):
         resp = self.http_client.get(f"{self.base_url}/v1/triggers", params={
             "appNames": ",".join(app_names) if app_names else None
         })
         return resp.json()
     
+    def list_active_triggers(self, trigger_ids: list[str] = None) -> list[ActiveTrigger]:
+        url = f"{self.base_url}/v1/triggers/active_triggers"
+        if trigger_ids:
+            url = f"{url}?triggerIds={','.join(trigger_ids)}"
+        resp = self.http_client.get(url)
+        if resp.status_code == 200:
+            return [ActiveTrigger(self, **item) for item in resp.json()["triggers"]]
+        
+        raise Exception("Bad request")
+    
+    def disable_trigger(self, trigger_id: str):
+        resp = self.http_client.post(f"{self.base_url}/v1/triggers/disable/{trigger_id}")
+        if resp.status_code == 200:
+            return resp.json()
+        
+        raise Exception("Bad request")
+    
     def get_trigger_requirements(self, trigger_ids: list[str] = None):
         resp = self.http_client.get(f"{self.base_url}/v1/triggers", params={
             "triggerIds": ",".join(trigger_ids) if trigger_ids else None
         })
       
         return resp.json()
```

### Comparing `composio_core-0.1.84/composio/sdk/utils.py` & `composio_core-0.1.87/composio/sdk/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from .storage import get_base_account_api_key
 from .sdk import Composio
 import os
 from pydantic import BaseModel
 import subprocess
 
+from typing import Union
+
 def _get_enum_key(name):
-    return name.upper().replace(' ', '_').replace('-', '_')
+    characters_to_replace = [' ', '-', '/', '(', ')', '\\', ':', '"', '\'', '.']
+    for char in characters_to_replace:
+        name = name.replace(char, '_')
+    return name.upper()
 
 def generate_enums():
     sdk_client = Composio(get_base_account_api_key())
     apps = sdk_client.get_list_of_apps()
     actions = sdk_client.get_list_of_actions()
     triggers = sdk_client.get_list_of_triggers()
 
@@ -30,15 +35,15 @@
     enum_content += '    def __init__(self, service, action):\n'
     enum_content += '        self.service = service\n'
     enum_content += '        self.action = action\n\n'
     for app in apps["items"]:
         app_key = app['key']
         app_actions = [action for action in actions if action["appKey"] == app_key]
         for action in app_actions:
-            enum_name = f'{app_key.upper()}_{_get_enum_key(action["display_name"])}'
+            enum_name = f'{_get_enum_key(action["name"])}'
             enum_value = f'("{app_key}", "{action["name"]}")'
             enum_content += f'    {enum_name} = {enum_value}\n'
 
     enum_content += '\n'
     enum_content += 'class Trigger(Enum):\n'
     enum_content += '    def __init__(self, service, trigger):\n'
     enum_content += '        self.service = service\n'
@@ -51,17 +56,17 @@
             enum_value = f'("{app_key}", "{trigger["name"]}")'
             enum_content += f'    {enum_name} = {enum_value}\n'
         # enum_content += f'Actions.{app_name} = {app_name}\n\n'
     with open(os.path.join(os.path.dirname(__file__), 'enums.py'), 'w') as f:
         f.write(enum_content)
 
 class GitUserInfo(BaseModel):
-    name: str | None
-    email: str | None
+    name: Union[None, str] 
+    email: Union[None, str] 
 
 def get_git_user_info() -> GitUserInfo:
     try:
         name = subprocess.check_output(['git', 'config', 'user.name']).strip().decode('utf-8')
         email = subprocess.check_output(['git', 'config', 'user.email']).strip().decode('utf-8')
         return GitUserInfo(name=name, email=email)
     except subprocess.CalledProcessError:
-        return GitUserInfo(name=None, email=None)
+        return GitUserInfo(name=None, email=None)
```

### Comparing `composio_core-0.1.84/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.87/composio_core.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.84
+Version: 0.1.87
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,11 +13,12 @@
 Requires-Dist: requests
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: beaupy>=3.7.2
 Requires-Dist: termcolor>=2.4.0
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: openai>=1.14.1
+Requires-Dist: rich>=13.7.1
 
 # Composio Core Package
 
 Core package to act as a bridge between composio platform and other services.
```

### Comparing `composio_core-0.1.84/setup.py` & `composio_core-0.1.87/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 from setuptools import setup
 import os
-
 from setuptools import setup
 from setuptools.command.install import install
 
-
 def get_current_dir():
     return os.path.dirname(os.path.realpath(__file__))
 
-
 def resolve_paths(*paths):
     return os.path.join(*paths)
 
-
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
-
 class InstallCommandMiddleware(install):
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
-
 setup(
     name="composio_core",
-    version="0.1.84",
+    version="0.1.87",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

