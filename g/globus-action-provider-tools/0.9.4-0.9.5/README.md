# Comparing `tmp/globus-action-provider-tools-0.9.4.tar.gz` & `tmp/globus-action-provider-tools-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-action-provider-tools-0.9.4.tar", last modified: Tue Jun  9 19:54:35 2020, max compression
+gzip compressed data, was "globus-action-provider-tools-0.9.5.tar", last modified: Wed Jul 22 19:24:20 2020, max compression
```

## Comparing `globus-action-provider-tools-0.9.4.tar` & `globus-action-provider-tools-0.9.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0    11357 2020-06-03 22:48:49.846490 globus-action-provider-tools-0.9.4/LICENSE
--rw-r--r--   0        0        0    49790 2020-06-05 20:59:04.340793 globus-action-provider-tools-0.9.4/README.rst
--rw-r--r--   0        0        0       22 2020-06-09 19:53:03.903273 globus-action-provider-tools-0.9.4/globus_action_provider_tools/__init__.py
--rw-r--r--   0        0        0     3008 2020-06-03 22:48:49.921820 globus-action-provider-tools-0.9.4/globus_action_provider_tools/action_request.yaml
--rw-r--r--   0        0        0     3982 2020-06-03 22:48:49.931164 globus-action-provider-tools-0.9.4/globus_action_provider_tools/action_status.yaml
--rw-r--r--   0        0        0    19906 2020-04-17 20:55:56.683239 globus-action-provider-tools-0.9.4/globus_action_provider_tools/actions_spec.openapi.yaml
--rw-r--r--   0        0        0     8527 2020-06-03 22:48:49.870161 globus-action-provider-tools-0.9.4/globus_action_provider_tools/authentication.py
--rw-r--r--   0        0        0     1491 2020-06-05 20:59:04.349196 globus-action-provider-tools-0.9.4/globus_action_provider_tools/authorization.py
--rw-r--r--   0        0        0     1358 2020-05-05 21:57:00.264584 globus-action-provider-tools-0.9.4/globus_action_provider_tools/caching.py
--rw-r--r--   0        0        0     2775 2020-06-05 20:59:04.350351 globus-action-provider-tools-0.9.4/globus_action_provider_tools/data_types.py
--rw-r--r--   0        0        0      640 2020-04-17 20:55:56.684263 globus-action-provider-tools-0.9.4/globus_action_provider_tools/errors.py
--rw-r--r--   0        0        0      286 2020-06-03 22:48:49.786981 globus-action-provider-tools-0.9.4/globus_action_provider_tools/flask/__init__.py
--rw-r--r--   0        0        0    12594 2020-06-03 22:49:29.884700 globus-action-provider-tools-0.9.4/globus_action_provider_tools/flask/api_helpers.py
--rw-r--r--   0        0        0     1124 2020-06-03 22:48:49.839577 globus-action-provider-tools-0.9.4/globus_action_provider_tools/groups_client.py
--rw-r--r--   0        0        0     1551 2020-06-08 20:01:53.881220 globus-action-provider-tools-0.9.4/globus_action_provider_tools/mocks.py
--rw-r--r--   0        0        0        0 2020-06-09 19:44:34.485315 globus-action-provider-tools-0.9.4/globus_action_provider_tools/testing/__init__.py
--rw-r--r--   0        0        0     1551 2020-06-09 19:44:34.486516 globus-action-provider-tools-0.9.4/globus_action_provider_tools/testing/mocks.py
--rw-r--r--   0        0        0      266 2020-06-09 19:44:34.487310 globus-action-provider-tools-0.9.4/globus_action_provider_tools/testing/patches.py
--rw-r--r--   0        0        0     2064 2020-06-03 22:48:49.923304 globus-action-provider-tools-0.9.4/globus_action_provider_tools/validation.py
--rw-r--r--   0        0        0     1598 2020-06-09 19:53:03.904431 globus-action-provider-tools-0.9.4/pyproject.toml
--rw-r--r--   0        0        0    51775 2020-06-09 19:54:35.925089 globus-action-provider-tools-0.9.4/setup.py
--rw-r--r--   0        0        0    50995 2020-06-09 19:54:35.928568 globus-action-provider-tools-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2020-06-03 22:48:49.846490 globus-action-provider-tools-0.9.5/LICENSE
+-rw-r--r--   0        0        0    49790 2020-06-05 20:59:04.340793 globus-action-provider-tools-0.9.5/README.rst
+-rw-r--r--   0        0        0       22 2020-07-22 19:23:46.388913 globus-action-provider-tools-0.9.5/globus_action_provider_tools/__init__.py
+-rw-r--r--   0        0        0     3008 2020-06-03 22:48:49.921820 globus-action-provider-tools-0.9.5/globus_action_provider_tools/action_request.yaml
+-rw-r--r--   0        0        0     3982 2020-06-03 22:48:49.931164 globus-action-provider-tools-0.9.5/globus_action_provider_tools/action_status.yaml
+-rw-r--r--   0        0        0    19910 2020-07-22 19:23:46.389989 globus-action-provider-tools-0.9.5/globus_action_provider_tools/actions_spec.openapi.yaml
+-rw-r--r--   0        0        0     8548 2020-07-22 19:23:46.390404 globus-action-provider-tools-0.9.5/globus_action_provider_tools/authentication.py
+-rw-r--r--   0        0        0     1491 2020-06-05 20:59:04.349196 globus-action-provider-tools-0.9.5/globus_action_provider_tools/authorization.py
+-rw-r--r--   0        0        0     1358 2020-05-05 21:57:00.264584 globus-action-provider-tools-0.9.5/globus_action_provider_tools/caching.py
+-rw-r--r--   0        0        0     2775 2020-07-22 18:18:21.305170 globus-action-provider-tools-0.9.5/globus_action_provider_tools/data_types.py
+-rw-r--r--   0        0        0      640 2020-04-17 20:55:56.684263 globus-action-provider-tools-0.9.5/globus_action_provider_tools/errors.py
+-rw-r--r--   0        0        0      286 2020-07-20 19:58:42.374852 globus-action-provider-tools-0.9.5/globus_action_provider_tools/flask/__init__.py
+-rw-r--r--   0        0        0    12987 2020-07-22 19:23:46.390783 globus-action-provider-tools-0.9.5/globus_action_provider_tools/flask/api_helpers.py
+-rw-r--r--   0        0        0     1124 2020-06-03 22:48:49.839577 globus-action-provider-tools-0.9.5/globus_action_provider_tools/groups_client.py
+-rw-r--r--   0        0        0     1551 2020-06-08 20:01:53.881220 globus-action-provider-tools-0.9.5/globus_action_provider_tools/mocks.py
+-rw-r--r--   0        0        0     1083 2020-07-21 00:32:01.733767 globus-action-provider-tools-0.9.5/globus_action_provider_tools/test.http
+-rw-r--r--   0        0        0        0 2020-06-09 19:44:34.485315 globus-action-provider-tools-0.9.5/globus_action_provider_tools/testing/__init__.py
+-rw-r--r--   0        0        0     1551 2020-07-10 20:41:05.840692 globus-action-provider-tools-0.9.5/globus_action_provider_tools/testing/mocks.py
+-rw-r--r--   0        0        0      266 2020-06-10 17:30:51.723493 globus-action-provider-tools-0.9.5/globus_action_provider_tools/testing/patches.py
+-rw-r--r--   0        0        0     2064 2020-06-03 22:48:49.923304 globus-action-provider-tools-0.9.5/globus_action_provider_tools/validation.py
+-rw-r--r--   0        0        0     1596 2020-07-22 19:23:46.391602 globus-action-provider-tools-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    51775 2020-07-22 19:24:20.751306 globus-action-provider-tools-0.9.5/setup.py
+-rw-r--r--   0        0        0    50995 2020-07-22 19:24:20.754272 globus-action-provider-tools-0.9.5/PKG-INFO
```

### Comparing `globus-action-provider-tools-0.9.4/LICENSE` & `globus-action-provider-tools-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-action-provider-tools-0.9.4/README.rst` & `globus-action-provider-tools-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/action_request.yaml` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/action_request.yaml`

 * *Files identical despite different names*

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/action_status.yaml` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/action_status.yaml`

 * *Files identical despite different names*

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/actions_spec.openapi.yaml` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/actions_spec.openapi.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,423 +1,424 @@
 openapi: 3.0.0
 info:
   title: Globus Actions API
-  description: ''
+  description: ""
   version: 2018-12-05.1
   contact:
     name: Globus Support
-    url: 'https://support.globus.org/hc/en-us/requests/new'
-    email: 'support@globus.org'
-  termsOfService: 'https://www.globus.org/legal/terms'
+    url: "https://support.globus.org/hc/en-us/requests/new"
+    email: "support@globus.org"
+  termsOfService: "https://www.globus.org/legal/terms"
 
 # Commented this out so users can run their service wherever they care to.
 # Should we make this a runtime param to request_validator somehow?
 #servers:
 #  - url: 'https://actions.automate.globus.org/<action>'
 #    description: production
 
 paths:
   /:
     get:
-      summary: 'Introspect the Action Provider for invocation, authorization and administrative and other information'
+      summary: "Introspect the Action Provider for invocation, authorization and administrative and other information"
       tags:
         - /
       security:
-        - bearer_token: ['https://auth.globus.org/scopes/{provider_scope_name}']
+        - bearer_token: ["https://auth.globus.org/scopes/{provider_scope_name}"]
       responses:
-        '200':
+        "200":
           description: Successful response containing details about this action provider.
           content:
             application/json:
               schema:
                 type: object
                 properties:
                   data:
-                    $ref: '#/components/schemas/ProviderDescription'
+                    $ref: "#/components/schemas/ProviderDescription"
                 example:
-                  types: ['Action']
-                  api_version: '1.0'
-                  globus_auth_scope: 'https://auth.globus.org/scopes/helloworld.actions.automate.globus.org/run_status_release'
-                  title: 'Hello World'
-                  subtitle: 'An Action responding Hello to the input name string'
-                  admin_contact: 'support@globus.org'
+                  types: ["Action"]
+                  api_version: "1.0"
+                  globus_auth_scope: "https://auth.globus.org/scopes/helloworld.actions.automate.globus.org/run_status_release"
+                  title: "Hello World"
+                  subtitle: "An Action responding Hello to the input name string"
+                  admin_contact: "support@globus.org"
                   visible_to:
-                    - 'public'
+                    - "public"
                   runnable_by:
-                    - 'all_authenticated_users'
+                    - "all_authenticated_users"
                   synchronous: false
-        '404':
-          description: 'No provider description is present or visible on the requested URL. Visibility may be limited by the visible_to property of the Provider Description'
-        '401':
-          description: 'Authorization header missing or invalid.'
-        '403':
-          description: 'Insufficient permissions for this resource.'
+        "404":
+          description: "No provider description is present or visible on the requested URL. Visibility may be limited by the visible_to property of the Provider Description"
+        "401":
+          description: "Authorization header missing or invalid."
+        "403":
+          description: "Insufficient permissions for this resource."
   /run:
     post:
       summary: Start an action executing (running)
       tags:
         - /run
       security:
-        - bearer_token: ['https://auth.globus.org/scopes/{provider_scope_name}']
+        - bearer_token: ["https://auth.globus.org/scopes/{provider_scope_name}"]
       requestBody:
         required: true
         content:
           application/json:
             schema:
               type: object
               properties:
                 data:
-                  $ref: '#/components/schemas/ActionRequest'
+                  $ref: "#/components/schemas/ActionRequest"
               example:
                 request_id: abc123
-                label: 'Saying hello to John Doe'
+                label: "Saying hello to John Doe"
                 body:
-                  hello_name: 'John Doe'
+                  hello_name: "John Doe"
       responses:
-        '202':
+        "202":
           description: Action Started
           content:
             application/json:
               schema:
-                $ref: '#/components/schemas/ActionStatus'
-        '200':
-          description: 'OK: A previous request with the same request_id and body has previously been received and processed'
+                $ref: "#/components/schemas/ActionStatus"
+        "200":
+          description: "OK: A previous request with the same request_id and body has previously been received and processed"
           content:
             application/json:
               schema:
-                $ref: '#/components/schemas/ActionStatus'
-        '400':
-          description: 'Invalid request including request body not compliant with the input schema of the provider'
-        '401':
-          description: 'Authorization header missing or invalid.'
-        '403':
-          description: 'Not authorized. The requesting user is not in the runnable_by list of the provider'
+                $ref: "#/components/schemas/ActionStatus"
+        "400":
+          description: "Invalid request including request body not compliant with the input schema of the provider"
+        "401":
+          description: "Authorization header missing or invalid."
+        "403":
+          description: "Not authorized. The requesting user is not in the runnable_by list of the provider"
 
   /{action_id}/status:
     parameters:
-        - name: action_id
-          required: true
-          in: path
-          description: ID of an action to check the status.
-          schema:
-            type: string
+      - name: action_id
+        required: true
+        in: path
+        description: ID of an action to check the status.
+        schema:
+          type: string
     get:
       summary: Get the status of a previously run action
       tags:
         - /status
       security:
-        - bearer_token: ['https://auth.globus.org/scopes/{provider_scope_name}']
+        - bearer_token: ["https://auth.globus.org/scopes/{provider_scope_name}"]
       responses:
-        '200':
+        "200":
           description: Status of the Action
           content:
             application/json:
               schema:
-                $ref: '#/components/schemas/ActionStatus'
-        '404':
-          description: 'No action with the provided action_id is known. It may never have been executed, or it may have been previously released via the /release operation or after the release timeout occurred'
-        '401':
-          description: 'Authorization header missing or invalid.'
-        '403':
-          description: 'Not authorized. The requesting user is not in the monitor_by list of the provider'
+                $ref: "#/components/schemas/ActionStatus"
+        "404":
+          description: "No action with the provided action_id is known. It may never have been executed, or it may have been previously released via the /release operation or after the release timeout occurred"
+        "401":
+          description: "Authorization header missing or invalid."
+        "403":
+          description: "Not authorized. The requesting user is not in the monitor_by list of the provider"
 
   /{action_id}/cancel:
     parameters:
       - name: action_id
         required: true
         in: path
         description: ID of an action to cancel.
         schema:
           type: string
     post:
-      summary: 'Cancel a running Action'
+      summary: "Cancel a running Action"
       tags:
         - /cancel
       security:
-        - bearer_token: ['https://auth.globus.org/scopes/{provider_scope_name}']
+        - bearer_token: ["https://auth.globus.org/scopes/{provider_scope_name}"]
       responses:
-        '200':
-          description: 'Cancellation successful. Final status returned in the body.'
+        "200":
+          description: "Cancellation successful. Final status returned in the body."
           content:
             application/json:
               schema:
-                $ref: '#/components/schemas/ActionStatus'
-        '400':
-          description: 'Invalid request. The provider does not support cancellation for this action.'
-        '404':
-          description: 'No action with the provided action_id is known. It may never have been executed, or it may have been previously released via the /release operation or after the release timeout occurred'
-        '409':
-          description: 'The Action is in a state, including completed or already processing a previous cancellation request, that does not support a cancel operation.'
-        '401':
-          description: 'Authorization header missing or invalid.'
-        '403':
-          description: 'Not authorized. The requesting user is not in the manage_by list of the provider'
+                $ref: "#/components/schemas/ActionStatus"
+        "400":
+          description: "Invalid request. The provider does not support cancellation for this action."
+        "404":
+          description: "No action with the provided action_id is known. It may never have been executed, or it may have been previously released via the /release operation or after the release timeout occurred"
+        "409":
+          description: "The Action is in a state, including completed or already processing a previous cancellation request, that does not support a cancel operation."
+        "401":
+          description: "Authorization header missing or invalid."
+        "403":
+          description: "Not authorized. The requesting user is not in the manage_by list of the provider"
 
   /{action_id}/release:
     parameters:
       - name: action_id
         required: true
         in: path
         description: ID of an action to release.
         schema:
           type: string
     post:
-      summary: 'Release the provider from storing the state of a completed Action'
+      summary: "Release the provider from storing the state of a completed Action"
       tags:
         - /release
       security:
-        - bearer_token: ['https://auth.globus.org/scopes/{provider_scope_name}']
+        - bearer_token: ["https://auth.globus.org/scopes/{provider_scope_name}"]
       responses:
-        '200':
-          description: 'Release successful. Final status returned in the body.'
+        "200":
+          description: "Release successful. Final status returned in the body."
           content:
             application/json:
               schema:
-                $ref: '#/components/schemas/ActionStatus'
-        '404':
-          description: 'No action with the provided action_id is known. It may never have been executed, or it may have been previously released via the /release operation or after the release timeout occurred'
-        '409':
-          description: 'The Action is in a state, such as still actively executing, that does not support a release operation.'
-        '401':
-          description: 'Authorization header missing or invalid.'
-        '403':
-          description: 'Not authorized. The requesting user is not in the manage_by list of the provider'
+                $ref: "#/components/schemas/ActionStatus"
+        "404":
+          description: "No action with the provided action_id is known. It may never have been executed, or it may have been previously released via the /release operation or after the release timeout occurred"
+        "409":
+          description: "The Action is in a state, such as still actively executing, that does not support a release operation."
+        "401":
+          description: "Authorization header missing or invalid."
+        "403":
+          description: "Not authorized. The requesting user is not in the manage_by list of the provider"
 
 security:
   - bearer_token: []
 
 components:
   securitySchemes:
     bearer_token:
       type: oauth2
       flows:
         clientCredentials:
-          tokenUrl: 'https://auth.globus.org/v2/oauth2/token'
+          tokenUrl: "https://auth.globus.org/v2/oauth2/token"
           scopes:
             https://auth.globus.org/scopes/{provider_scope_name}: Authorization to perform operations at the action provider
         authorizationCode:
-          authorizationUrl: 'https://auth.globus.org/v2/oauth2/authorize'
-          tokenUrl: 'https://auth.globus.org/v2/oauth2/token'
-          refreshUrl: 'https://auth.globus.org/v2/oauth2/token'
+          authorizationUrl: "https://auth.globus.org/v2/oauth2/authorize"
+          tokenUrl: "https://auth.globus.org/v2/oauth2/token"
+          refreshUrl: "https://auth.globus.org/v2/oauth2/token"
           scopes:
             https://auth.globus.org/scopes/{provider_scope_name}: Authorization to perform operations at the action provider
 
   schemas:
     ProviderDescription:
       type: object
-      required: [types, api_version, title, synchronous, log_supported, runnable_by]
+      required:
+        [types, api_version, title, synchronous, log_supported, runnable_by]
       properties:
         types:
           type: array
           items:
             type: string
             enum:
               - Action
               - Event
-            description: 'The type of provider being described. In the initial release, only Action providers are supported'
+            description: "The type of provider being described. In the initial release, only Action providers are supported"
         api_version:
           type: string
           enum:
-            - '1.0'
+            - "1.0"
         globus_auth_scope:
           type: string
           format: uri
-          description: 'The scope of any bearer token to be used on authenticated accesses to the provider.'
+          description: "The scope of any bearer token to be used on authenticated accesses to the provider."
         title:
           type: string
-          description: 'A non-unique, human-friendly name used for displaying the provider to end users.'
+          description: "A non-unique, human-friendly name used for displaying the provider to end users."
           minLength: 1
           maxLength: 128
         subtitle:
           type: string
-          description: 'A concise summary of the provider’s purpose.'
+          description: "A concise summary of the provider’s purpose."
           minLength: 1
           maxLength: 128
         description:
           type: string
-          description: 'A detailed description of the provider for end user display.'
+          description: "A detailed description of the provider for end user display."
           minLength: 1
           maxLength: 4096
         keywords:
-          description: 'A set of terms used to categorize the provider which may be used in query and discovery operations. Maximum total length of all keywords is 1024 characters.'
+          description: "A set of terms used to categorize the provider which may be used in query and discovery operations. Maximum total length of all keywords is 1024 characters."
           type: array
           items:
             type: string
         visible_to:
           type: array
           description: 'A set of Principal URN values, or the value "public" indicating the identity of users who can view the provider description via introspection or when indexed in any provider catalog service'
           items:
-            $ref: '#/components/schemas/PrincipalURN_or_public'
+            $ref: "#/components/schemas/PrincipalURN_or_public"
           uniqueItems: true
         runnable_by:
           type: array
           description: 'A set of Principal URN values, or the value "public" indicating the identity of users who can use the /run operation to initiate an action with the provider'
           items:
-            $ref: '#/components/schemas/PrincipalURN_or_all_authenticated_users'
+            $ref: "#/components/schemas/PrincipalURN_or_all_authenticated_users"
           uniqueItems: true
         administered_by:
           type: array
-          description: 'The set of Principal URN values of users who may perform administrative operations, including updating the description itself, on the provider'
+          description: "The set of Principal URN values of users who may perform administrative operations, including updating the description itself, on the provider"
           items:
-            $ref: '#/components/schemas/PrincipalURN'
+            $ref: "#/components/schemas/PrincipalURN"
           uniqueItems: true
         admin_contact:
           type: string
-          description: 'A method of contacting an administrator of the provider, typically an e-mail address, in case of concerns with the operation of the provider'
+          description: "A method of contacting an administrator of the provider, typically an e-mail address, in case of concerns with the operation of the provider"
         synchronous:
           type: boolean
-          description: 'True if *all* /run operations on the provider return a completed (SUCCEEDED or FAILED) status in the result of the run operation. False if at least some invocations may return an in progress (ACTIVE or INACTIVE) status value requiring use of the /status operation to determine further state of the action.'
+          description: "True if *all* /run operations on the provider return a completed (SUCCEEDED or FAILED) status in the result of the run operation. False if at least some invocations may return an in progress (ACTIVE or INACTIVE) status value requiring use of the /status operation to determine further state of the action."
         log_supported:
           type: boolean
-          description: 'True if the provider supports the /log operation providing detailed information on the intermediate states of a request.'
+          description: "True if the provider supports the /log operation providing detailed information on the intermediate states of a request."
         maximum_deadline:
           type: string
-          description: 'An ISO 8601 time duration value. On providers which support asynchronous operations, the maximum allowed value for deadline of an action.'
+          description: "An ISO 8601 time duration value. On providers which support asynchronous operations, the maximum allowed value for deadline of an action."
         input_schema:
           type: object
-          description: 'A JSON Schema compliant definition of the format of the `body` field of the action request document when requesting a /run operation.'
+          description: "A JSON Schema compliant definition of the format of the `body` field of the action request document when requesting a /run operation."
         event_types:
           type: array
-          description: 'For Action Providers which also support Event operations, as indicated by values in the types field, the set of Action status operations which may be subscribed to as events'
+          description: "For Action Providers which also support Event operations, as indicated by values in the types field, the set of Action status operations which may be subscribed to as events"
           items:
             type: string
             enum:
-              - 'STARTED'
-              - 'STATUS_UPDATE'
-              - 'LOG_UPDATE'
-              - 'COMPLETED'
-              - 'FAILED'
+              - "STARTED"
+              - "STATUS_UPDATE"
+              - "LOG_UPDATE"
+              - "COMPLETED"
+              - "FAILED"
 
     ActionRequest:
       type: object
       required: [request_id, body]
       additionalProperties: false
       properties:
         request_id:
           type: string
-          description: 'A unique identifier representing the *request* to start an action. Multiple uses of the same request_id must have the same content or they will be rejected. Only one instance of the operation will be executed, so requests with the same request_id may be repeated to attempt to guarantee execution of an action'
+          description: "A unique identifier representing the *request* to start an action. Multiple uses of the same request_id must have the same content or they will be rejected. Only one instance of the operation will be executed, so requests with the same request_id may be repeated to attempt to guarantee execution of an action"
         body:
           type: object
-          description: 'The action-provider specific content describing the action to run. Format for the body may be provided in the input_schema field of the Action Provider Description'
+          description: "The action-provider specific content describing the action to run. Format for the body may be provided in the input_schema field of the Action Provider Description"
         label:
           type: string
-          description: 'A short human presentable description of the Action requested'
+          description: "A short human presentable description of the Action requested"
           minLength: 1
           maxLength: 64
         monitor_by:
           type: array
           items:
-            $ref: '#/components/schemas/PrincipalURN'
-          description: 'A list of principal URNs containing identities which are allowed to monitor the progress of the action using the /status and /log operations. When not provided, defaults to the user that initiated the action.'
+            $ref: "#/components/schemas/PrincipalURN"
+          description: "A list of principal URNs containing identities which are allowed to monitor the progress of the action using the /status and /log operations. When not provided, defaults to the user that initiated the action."
           uniqueItems: true
         manage_by:
           type: array
           items:
-            $ref: '#/components/schemas/PrincipalURN'
-          description: 'A list of principal URN containing identities which are allowed to manage the progress of the action using the /cancel and /release operations. When not provided, defaults to the user that initiated the action.'
+            $ref: "#/components/schemas/PrincipalURN"
+          description: "A list of principal URN containing identities which are allowed to manage the progress of the action using the /cancel and /release operations. When not provided, defaults to the user that initiated the action."
           uniqueItems: true
         allowed_clients:
           type: array
           items:
-            $ref: '#/components/schemas/AllowedClients'
+            $ref: "#/components/schemas/AllowedClients"
         deadline:
           type: string
           format: date-time
-          description: 'A timestamp indicating by which time the action must complete. The request may be rejected if the Action Provider does not expect to be able to complete the action before the deadline or if it represents a time greater than the maximum_deadline specified in the Provider Description.'
+          description: "A timestamp indicating by which time the action must complete. The request may be rejected if the Action Provider does not expect to be able to complete the action before the deadline or if it represents a time greater than the maximum_deadline specified in the Provider Description."
         release_after:
-          $ref: '#/components/schemas/ISO8601_duration'
-          description: 'An ISO8601 time duration value indicating how long retention of the status of the action be retained after it reaches a completed state. Action Providers may limit the maximum value. It is recommended that Providers provide a default release_after value of approximately 30 days.'
+          $ref: "#/components/schemas/ISO8601_duration"
+          description: "An ISO8601 time duration value indicating how long retention of the status of the action be retained after it reaches a completed state. Action Providers may limit the maximum value. It is recommended that Providers provide a default release_after value of approximately 30 days."
 
     ActionStatus:
       type: object
       required: [action_id, status, details, creator_id]
-      description: 'The status of an Action which has already been initiated with the /run operation.'
+      description: "The status of an Action which has already been initiated with the /run operation."
       properties:
         action_id:
           type: string
-          description: 'The id of the Action itself.'
+          description: "The id of the Action itself."
         status:
           type: string
-          description: 'The current state of the Action'
+          description: "The current state of the Action"
           enum:
             - SUCCEEDED
             - FAILED
             - ACTIVE
             - INACTIVE
         creator_id:
-          $ref: '#/components/schemas/PrincipalURN'
+          $ref: "#/components/schemas/PrincipalURN"
         label:
           type: string
-          description: 'A short human presentable description of the Action'
+          description: "A short human presentable description of the Action"
           minLength: 1
           maxLength: 64
         monitor_by:
           type: array
           items:
-            $ref: '#/components/schemas/PrincipalURN'
-          description: 'A list of principal URNs containing identities which are allowed to monitor the progress of the action using the /status and /log operations. When not provided, defaults to the user that initiated the action.'
+            $ref: "#/components/schemas/PrincipalURN"
+          description: "A list of principal URNs containing identities which are allowed to monitor the progress of the action using the /status and /log operations. When not provided, defaults to the user that initiated the action."
           uniqueItems: true
         manage_by:
           type: array
           items:
-            $ref: '#/components/schemas/PrincipalURN'
-          description: 'A list of principal URN containing identities which are allowed to manage the progress of the action using the /cancel and /release operations. When not provided, defaults to the user that initiated the action.'
+            $ref: "#/components/schemas/PrincipalURN"
+          description: "A list of principal URN containing identities which are allowed to manage the progress of the action using the /cancel and /release operations. When not provided, defaults to the user that initiated the action."
           uniqueItems: true
         start_time:
           type: string
           format: date-time
-          description: 'The time in ISO8601 format when the Action started executing (not necessarily the exact same time when the action /run operation was invoked).'
+          description: "The time in ISO8601 format when the Action started executing (not necessarily the exact same time when the action /run operation was invoked)."
         completion_time:
           type: string
           format: date-time
-          description: 'The time in ISO8601 format when the Action reached a terminal (SUCCEEDED or FAILED) status'
+          description: "The time in ISO8601 format when the Action reached a terminal (SUCCEEDED or FAILED) status"
         release_after:
-          $ref: '#/components/schemas/ISO8601_duration'
-          description: 'An ISO8601 time duration value indicating how long retention of the status of the action be retained after it reaches a completed state.'
+          $ref: "#/components/schemas/ISO8601_duration"
+          description: "An ISO8601 time duration value indicating how long retention of the status of the action be retained after it reaches a completed state."
         display_status:
           type: string
-          description: 'A short, human consumable string describing the current status of this action. This can be used to provide more detailed, presentable summary of the Action status. For example, a batch system may use “Queued” or “Running” as display_status when the Action has status “ACTIVE”. Similarly, a reason the action is blocked, such as requiring additional authentication may be used when the status is “INACTIVE.”'
+          description: "A short, human consumable string describing the current status of this action. This can be used to provide more detailed, presentable summary of the Action status. For example, a batch system may use “Queued” or “Running” as display_status when the Action has status “ACTIVE”. Similarly, a reason the action is blocked, such as requiring additional authentication may be used when the status is “INACTIVE.”"
           minLength: 1
           maxLength: 64
         details:
           type: object
-          description: 'A provider-specific object representing the full state of the Action. When the Action is in a SUCCEEDED state, this may be considered the result or return value from the Action. When the Action is in a FAILED state, this represents the cause or reason for failure. While running, the details MAY provide information about the Action in progress such as a measure of its progress to completion.'
+          description: "A provider-specific object representing the full state of the Action. When the Action is in a SUCCEEDED state, this may be considered the result or return value from the Action. When the Action is in a FAILED state, this represents the cause or reason for failure. While running, the details MAY provide information about the Action in progress such as a measure of its progress to completion."
       example:
-        action_id: '6529'
+        action_id: "6529"
         status: ACTIVE
         creator_id: urn:globus:auth:identity:ae2a1750-d274-11e5-b867-e74762c29f57
         details:
-          estimated_complete: '2019-06-21T17:15:04.805868+00:00'
+          estimated_complete: "2019-06-21T17:15:04.805868+00:00"
         manage_by:
-        - urn:globus:auth:identity:ca73e829-715f-4522-9dec-a507fe57a661
-        - urn:globus:auth:identity:ae2a1750-d274-11e5-b867-e74762c29f57
+          - urn:globus:auth:identity:ca73e829-715f-4522-9dec-a507fe57a661
+          - urn:globus:auth:identity:ae2a1750-d274-11e5-b867-e74762c29f57
         monitor_by:
-        - urn:globus:auth:identity:ca73e829-715f-4522-9dec-a507fe57a661
-        - urn:globus:auth:identity:ae2a1750-d274-11e5-b867-e74762c29f57
+          - urn:globus:auth:identity:ca73e829-715f-4522-9dec-a507fe57a661
+          - urn:globus:auth:identity:ae2a1750-d274-11e5-b867-e74762c29f57
         release_after: P30D
-        start_time: '2019-06-21T17:01:55.806781+00:00'
+        start_time: "2019-06-21T17:01:55.806781+00:00"
 
     PrincipalURN:
       type: string
-      pattern: '^urn:globus:(auth:identity|groups:id):([a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12})$'
-      description: 'A URN representation of an Identity in Globus either of a user from Globus Auth or a group from Globus Groups.'
+      pattern: "^urn:globus:(auth:identity|groups:id):([a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12})$"
+      description: "A URN representation of an Identity in Globus either of a user from Globus Auth or a group from Globus Groups."
 
     PrincipalURN_or_public:
       type: string
-      pattern: '^(urn:globus:(auth:identity|groups:id):([a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}))|public$'
+      pattern: "^(urn:globus:(auth:identity|groups:id):([a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}))|public$"
       description: 'A URN representation of an Identity in Globus either of a user from Globus Auth or a group from Globus Groups or the special value "public"'
 
     PrincipalURN_or_all_authenticated_users:
       type: string
-      pattern: '^(urn:globus:(auth:identity|groups:id):([a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}))|all_authenticated_users$'
+      pattern: "^(urn:globus:(auth:identity|groups:id):([a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}))|all_authenticated_users$"
       description: 'A URN representation of an Identity in Globus either of a user from Globus Auth or a group from Globus Groups or the special value "all_authenticated_users" indicating any user who presents valid credentials (bearer token)'
 
     ISO8601_duration:
       type: string
       pattern: '^P(?!$)(\d+(?:\.\d+)?Y)?(\d+(?:\.\d+)?M)?(\d+(?:\.\d+)?W)?(\d+(?:\.\d+)?D)?(T(?=\d)(\d+(?:\.\d+)?H)?(\d+(?:\.\d+)?M)?(\d+(?:\.\d+)?S)?)?$'
       description: ISO8601 duration format. Regex sourced from https://stackoverflow.com/a/32045167/845210
 
     # TO DO: This is not complete in terms of specifying individual users in the list
     AllowedClients:
       type: string
-      description: ''
-      pattern: '^(public|globus|creator|.$)$'
+      description: ""
+      pattern: "^(public|globus|creator|.$)$"
```

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/authentication.py` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,17 @@
         try:
             assert resp.get("active", False) is True, "Invalid token."
             assert resp.get("nbf", now + 4) < (
                 time() + 3
             ), "Token not yet valid -- check system clock?"
             assert resp.get("exp", 0) > (time() - 3), "Token expired."
             scopes = frozenset(resp.get("scope", "").split())
-            assert (
-                scopes == self.expected_scopes
-            ), f"Token invalid scopes. Expected: {self.expected_scopes}, got: {scopes}"
+            assert scopes.intersection(
+                set(self.expected_scopes)
+            ), f"Token invalid scopes. Expected one of: {self.expected_scopes}, got: {scopes}"
             aud = resp.get("aud", [])
             assert (
                 self.expected_audience in aud
             ), f"Token not intended for us: audience={aud}"
             assert "identity_set" in resp, "Missing identity_set"
         except AssertionError as err:
             our_err = TokenValidationError(err)
```

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/authorization.py` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/authorization.py`

 * *Files identical despite different names*

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/caching.py` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/caching.py`

 * *Files identical despite different names*

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/data_types.py` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/data_types.py`

 * *Files identical despite different names*

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/errors.py` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/errors.py`

 * *Files identical despite different names*

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/flask/api_helpers.py` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/flask/api_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
+import logging
 from dataclasses import asdict
-from typing import Any, Callable, Dict, Optional, Tuple, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 from urllib.parse import urlsplit, urlunsplit
 
 import flask
 from flask import Request, Response, jsonify, request
 from jsonschema.validators import Draft7Validator
 from werkzeug.exceptions import BadRequest, HTTPException, NotFound, Unauthorized
 
@@ -46,14 +47,16 @@
 _response_schema_types = {
     "run": "ActionStatus",
     "status": "ActionStatus",
     "cancel": "ActionStatus",
     "release": "ActionStatus",
 }
 
+log = logging.getLogger(__name__)
+
 
 def _api_operation_for_request(request: flask.Request) -> str:
     method = request.path.rsplit("/", 1)
     op_name = method[-1]
     return op_name
 
 
@@ -148,14 +151,15 @@
     client_name: Optional[str],
     provider_description: ActionProviderDescription,
     action_run_callback: ActionRunType,
     action_status_callback: ActionStatusType,
     action_cancel_callback: ActionCancelType,
     action_release_callback: ActionReleaseType,
     action_log_callback: Optional[ActionLogType] = None,
+    additional_scopes: Optional[List[str]] = None,
 ) -> None:
     """Add routes to a Flask Blueprint to implement the required operations of the Action
     Provider Interface: Introspect, Run, Status, Cancel and Release. The route handlers
     added to the blueprint perform basic functionality such as input validation and
     authorization checks where appropriate, and use the provided callbacks to implement
     the action provider specific functionality. See description of each callback below
     for a description of functionality performed prior to invoking the callback.
@@ -211,18 +215,25 @@
     integer can be added to the return (making the return a (ActionStatus, int) tuple)
     which defines the HTTP status code to be returned. This is useful in the case where
     an existing request with the same id and body are seen which should return a 200 HTTP
     status rather than the normal 201 HTTP status (which is the default when the status
     code is not returned).
 
     """
+    if additional_scopes:
+        all_accepted_scopes = additional_scopes + [
+            provider_description.globus_auth_scope
+        ]
+    else:
+        all_accepted_scopes = [provider_description.globus_auth_scope]
+
     checker = TokenChecker(
         client_id=client_id,
         client_secret=client_secret,
-        expected_scopes=[provider_description.globus_auth_scope],
+        expected_scopes=all_accepted_scopes,
         expected_audience=client_name,
     )
 
     blueprint.json_encoder = ActionProviderJsonEncoder
 
     if isinstance(provider_description.input_schema, str):
         input_schema = json.loads(provider_description.input_schema)
@@ -248,14 +259,15 @@
 
     @blueprint.route("/run", methods=["POST"])
     def action_run() -> ViewReturn:
         auth_state = _check_token(request, checker)
         if not auth_state.check_authorization(
             provider_description.runnable_by, allow_all_authenticated_users=True
         ):
+            log.info(f"Unauthorized call to action run, errors: {auth_state.errors}")
             raise Unauthorized()
         if blueprint.url_prefix:
             request.path = request.path.lstrip(blueprint.url_prefix)
             if request.url_rule is not None:
                 request.url_rule.rule = request.url_rule.rule.lstrip(
                     blueprint.url_prefix
                 )
```

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/groups_client.py` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/groups_client.py`

 * *Files identical despite different names*

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/mocks.py` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/mocks.py`

 * *Files identical despite different names*

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/testing/mocks.py` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/testing/mocks.py`

 * *Files identical despite different names*

### Comparing `globus-action-provider-tools-0.9.4/globus_action_provider_tools/validation.py` & `globus-action-provider-tools-0.9.5/globus_action_provider_tools/validation.py`

 * *Files identical despite different names*

### Comparing `globus-action-provider-tools-0.9.4/pyproject.toml` & `globus-action-provider-tools-0.9.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "globus-action-provider-tools"
-version = "0.9.4"
+version = "0.9.5"
 description = "Tools to help developers build services that implement the Action Provider specification."
 authors = [
     "Jim Pruyne <pruyne@globus.org>",
     "Uriel Mandujano <uriel@globus.org>",
 ]
 keywords = [
   "globus",
@@ -60,9 +60,7 @@
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 line_length = 88
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
-
-
```

### Comparing `globus-action-provider-tools-0.9.4/setup.py` & `globus-action-provider-tools-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['whattimeisit-provider = '
                      'examples.flask.whattimeisitrightnow.app.app:main']}
 
 setup_kwargs = {
     'name': 'globus-action-provider-tools',
-    'version': '0.9.4',
+    'version': '0.9.5',
     'description': 'Tools to help developers build services that implement the Action Provider specification.',
     'long_description': 'Action Provider Tools Introduction\n==================================\n\nThis is an experimental and unsupported toolkit to help developers build Action Providers for use in Globus Automate including for invocation via Globus Flows.\n\nAs this is experimental, no support is implied or provided for any sort of use of this package. It is published for ease of distribution among those planning to use it for its intended, experimental, purpose.\n\nThis README is intended to introduce the concepts, requirements and overview of this toolkit to be used when implementing an Action for use with Globus Automate. The three main sections are 1) an introduction to the interface required of all Actions, 2) A description of how to prepare your service to use Globus Auth, and 3) A description of the content of this toolkit and how it can be used in a Python implementation. This overview does not provide any guidance on how to host or operate the Action so that it is accessible via the internet.\n\n\nActions Overview\n================\nThe fundamental purpose of the Globus Automate platform is to tie together multiple operations or units of work into a coordinated orchestration. We refer to each of these operations as an *Action*. In particular, the *Flows* service provides a means of coordinating multiple actions across potentially long periods of time to perform some aggregate function larger than any single Action provides. The *Triggers* service ties *Events*, or occurrences within a managed environment, to Actions such that each occurrence of the Event automatically invokes the Action associated with it.\n\nIn both the Flows and the Triggers cases, the Actions require a uniform interface for invocation, monitoring and possibly termination so that new Actions may be introduced without requiring customization or re-implementation of the invoking services. We refer to the service endpoints which can be invoked in this manner as *Action Providers* and the uniform interface for interacting with the Action Providers as the *Action Provider Interface*. We provide here an overview of the *Action Provider Interface* as a guide for use when implementing an *Action Provider*. \n\nThe Action Provider Interface\n-----------------------------\n\nThe Action Provider Interface is a RESTful model for starting, monitoring, canceling and removing state associated with the invocation of an Action. Following the REST resource life-cycle pattern, each Action invocation returns an identifier representing the invocation (an *Action Instance*). This identifier is used to monitor the progress of the Action Instance via further REST calls until its completion, or it may be used to request cancellation of the instance.\n\nBecause the interface is intended to support arbitrary Action types, we recognize that some Action instances may be long-running (asynchronous) such as the execution of a computational job. Other Actions may be short-running (synchronous), able to return their final result directly in response to their invocation request as is the case in typical RESTful models. The Action Life-cycle described below specifically supports these execution modes as well as handling failures and Actions which may be, temporarily, unable to make progress.\n\nAction Life-cycle\n^^^^^^^^^^^^^^^^^\n\nThe Life-cycle of an Action defines the set of states that the Action may be in, and how it can transition among the states. The states are defined as follows:\n\n*  ``ACTIVE``: The Action is executing and is making progress toward completion\n\n*  ``INACTIVE``: The Action is paused in its execution and is not making progress toward completion. Out-of-band (i.e. not via the Action Provider Interface) measures may be required to allow the Action to proceed.\n\n*  ``SUCCEEDED``: The Action reached a completion state which was considered "normal" or not due to failure or other unrecoverable error. \n\n*  ``FAILED``: The Action is in a completion state which is "not normal" such as due to an error condition which is not considered recoverable in any manner. \n\n*  *"Released"*: The Action Provider has removed the record of the existence of the Action. Further attempts to interact with the Action will be errors as if the Action had never existed. All resources associated with the Action may have been deleted or removed. This is not a true state in the sense that the state can be observed, but ultimately all Actions will be released and unavailable for further operations. Any subsequent references to the Action, e.g. via the API methods described below, will behave as if the Action never existed.\n\nUpon initial creation of an Action (see operations below), the Action may be in any of the first four states. If it is in an ``ACTIVE`` or ``INACTIVE`` state, the Action is considered "asynchronous" and further queries to get the state of the Action may return updated information. If the Action is in a the ``SUCCEEDED`` or ``FAILED`` states, the Action is synchronous, all information about the Action is returned on the creation operation and no changes to the state are possible.\n\nAn asynchronous Action may change state between ``ACTIVE`` and ``INACTIVE`` during its life time, and may update further details about its progress while in either of these states. When a completed state of ``SUCCEEDED`` or ``FAILED`` is reached, the Action state cannot be updated further. The Action Provider is, however, required to maintain this final state for some period of time so that the client of the Action may retrieve the completion state. Upon completion, the client may request that the Action be "released" or the Action Provider may do so on its own after the required time-out occurs. To save server resources, it is preferred that the client release the Action when it has reliably retrieved and processed the final state.\n\nAction Provider Interface and Document Types\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nThe primary purpose of the Action Provider Interface is to securely support and report Actions progressing through the life-cycle described above. The document types supporting this are the initial Action invocation *Action Request* document, and the *Action Status* document which contains the life-cycle status described above along with additional detailed status information specific to the type of Action being executed.\n\n.. note:: Below, we describe URL paths where operations can be performed. We assume that all of these share a common "Base URL" which we don\'t name in this document. The Base URL may be at any place in the URL path namespace desired by the Action Provider, and so may be used in conjunction with any other service URLs it may support.\n\n.. note:: For brevity and clear presentation, in the descriptions of document types in the following sections, we present the key concepts, but do not enumerate every option or field on the documents. Refer to the toolkit components, including the OpenAPI format specification (as described in the toolkit section), for a complete definition.\n\nStarting an Action: The Action Request Document and the ``POST /run`` Method\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nStarting an Action is performed by making a REST ``POST`` request to the path ``/run`` containing an Action Request document. The request document contains the following fields:\n\n*  ``request_id``: A client-generated Identifier for this request. A user may re-invoke the ``/run`` method with the same ``request_id`` any number of times, but the Action must only be initiated once. In this way, the user may re-issue the request in case it cannot be determined if a request was successfully initiated for example due to network failure.\n\n*  ``body``: An Action Provider-specific object which provides the input for the Action to be performed. The ``body`` must conform to the input specification for the Action Provider being invoked, and thus the client must understand the requirements of the Action Provider when providing the value of the ``body``. Thus, the Action Provider must provide documentation on the format for the ``body`` property.\n\n*  ``manage_by`` and ``monitor_by``: Each of these is a list of principal values in `URN format <https://docs.globus.org/api/search/#principal_Urns>`_, and they allow the user invoking the Action to delegate some capability over the Action to other principals. ``manage_by`` defines the principals who are allowed to attempt to change the execution of the Action (see operations ``/cancel`` and ``/release`` below) while it is running. ``monitor_by`` defines principals which are allowed to see the state of the Action before its state has been destroyed in a release operation. In both cases, the Globus Auth identity associated with the ``/run`` operation is implicitly part of both the ``manage_by`` and ``monitor_by`` sets. That is, the invoking user need not include their own identity into these lists.\n\nAny request to the ``/run`` method which contains an Action Request which adheres to the input schema will return an Action Status document as described in the next section. \n\nMonitoring and Completing an Action: The Action Status Document and Management Methods\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nAll information about an Action is contained in the Action Status document which is returned on almost all operations related to an Action (the exception is the log operation which is optional and is described briefly below). Notable fields of the Action Status document include:\n\n*  ``action_id``: The unique identifier for this particular action. The ``action_id`` may be any string, and it should be treated as an opaque value (that is, having no semantic or implied meaning) by the client. The client will first learn of an Action\'s ``action_id`` in the Action Status returned by the ``/run`` method.\n\n*  ``status`` and ``display_status``: These provide the description of the state of the Action. ``status`` is the specific life-cycle value as described above. ``display_status`` is an optional field the Action Provider may supply which gives a short text description of the status using language which is specific to the Action.\n\n*  ``details``: The Action Provider-specific state, particularly the completion state, of the Action are returned in the ``details`` field. In the completion states, the ``details`` can be considered the "result" or the "return value" of the Action. It is the successful return value for a ``SUCCEEDED`` status,  and it is the error result for the ``FAILED`` status. The exact content in ``details`` is always specific to the Action Provider, so must be documented by the Action Provider to describe its interpretation to clients.\n\n*  ``monitor_by`` and ``manage_by``: Same as in the Action Request.\n\n*  ``start_time`` and ``completion_time``: Represent the time the Action was first received by the ``/run`` operation and the time the Action Provider determined that the Action reached a completed state (``SUCCEEDED`` or ``FAILED``) respectively. Action Providers are not required to continuously monitor the progress of Actions, so the ``completion_time`` noted may be different than the executed Action\'s actual completion time.  These values **may** be the same in the case of a synchronous operation, but ``completion_time`` must never be before ``start_time``.\n\n*  ``release_after``: As stated above, Action state is automatically removed from the Action Provider after some time interval once it reaches a completion state. The ``release_after`` is a time duration, in seconds, which states how long after completion the Action will automatically be released. A typical value would be 30-days, but Action Providers may define their own policy which is to be exposed in the Action Status.\n\nIn addition to the ``/run`` method described above, the Action Status is the "universal" return value from operations on an Action. We describe the operations on Actions next. Each uses the ``action_id`` as part of the URL path much like other RESTful resources do with their ids, and none of them require any input body. \n\n*  ``GET /<action_id>/status``: This is a read-only operation for retrieving the most recent state of the Action. It is commonly used to poll an Action\'s state while awaiting it entering a completion state. Use of this API call requires that the user authenticate with a principal value which is in the ``monitor_by`` list established when the Action was started.\n\n*  ``POST /<action_id>/cancel``: Cancellation provides an advisory or hint to the Action Provider that the user does not want the Action to continue execution. The Action Provider is not required to ensure immediate completion or that the cancel operation truly causes the Action to terminate in any manner other than it would have without the cancel request. Thus, the Action Status returned from the cancel operation may contain a non-completion state. If the Action is already in a completed state, the Action Provider may treat the request much as a ``/status`` request to simply return the current status. Use of this API call requires that the user authenticates with a principal value which is in the ``manage_by`` list established when the Action was started. \n\n*  ``POST /<action_id>/release``: As described in the section on life-cycle, the very last step of the life-cycle is for the Action state to be removed from the Action Provider. A user can specify that it has retrieved the final state or is no longer interested in the state using the ``/release`` operation which returns the final state. If the Action is not already in a completion state, ``/release`` will return an error as this operation does not attempt to stop execution (that is what ``/cancel`` does). The Action Status document returned from ``/release`` will be the last record of the Action present at the Action Provider. After the call to ``/release`` the ``action_id`` is no longer valid, and use in any other calls will return an error, most likely an HTTP status 404 indicating the Action was not found.\n\nDetailed Execution History: logging\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nSome Actions, particularly those that are long running, may have associated with them a list or log of activities or sub-events which occurred during the Action\'s life. This detailed log is typically larger, more complex, or more fine-grain than the snapshot of the status returned by the ``/status`` method. Not all Action Providers or Actions are suitable for logging, so support is considered optional and will be advertised by the Action Provider in its description (see below). The request to retrieve the log takes the form ``GET /<action_id>/log?<filters,pagination>``. The filters and pagination query parameters are used to limit (e.g. based on start time) which log records to retrieve and the pagination parameter is used to scroll through a long set of log records across multiple requests. Each record in the log contains the following properties:\n\n*  ``time``: A timestamp representing the time this log record occurred.\n\n*  ``code``: A short Action Provider-specific description of the type of the log record.\n\n*  ``description``: A textual description of the purpose, cause, or information on the log record.\n\n*  ``details`` (optional): An object providing additional and structured Action Provider-specific representation of the log record.\n\n\nAction Provider Introspection (``GET /``)\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nThe Automate platform is intended to help users both find and make use of the variety of Action Providers which may be available on the network. The primary means of accomplishing this assistance is by making Action Providers, the services which implement the Action Provider Interface, self-describing via an *Introspection* interface. Accessing the introspection method is performed simply via a ``GET /``. That is, the HTTP ``GET`` method on the Base URL. The returned JSON document contains the following fields:\n\n*  ``api_version``: A version string defining the version of the Action Provider Interface supported by the Action Provider. The version described in this document and currently the only version available will have value ``"1.0"``.\n\n*  ``title``, ``subtitle``, ``description``, ``keywords``: Each of these provide human-readable text which helps a user discover the purpose of the Action Provider.\n\n*  ``visible_to`` and ``runnable_by``: Access to the action provider is limited by and published through these properties. Each contains a list of principal values in URN format. ``visible_to`` controls who can retrieve the information via introspection (this operation) and may contain the string ``"public"`` indicating that all users, even those who present no credentials, may access the information. The ``runnable_by`` property enumerates who can use the ``/run`` method to start an Action at this provider. It allows the string ``"all_authenticated_users"`` indicating that any user who presents valid credentials via a Bearer token may start an Action at the provider.\n\n*  ``synchronous`` and ``log_supported``: These are boolean values which simply describe capabilities and modes for the Action Provider. If ``synchronous`` is true, a user calling ``/run`` can assume that the returned status will always be in a completed (``SUCCEEDED`` or ``FAILED``) state and there will never be a need to poll using the ``/status`` method (use of ``/release`` is still permitted and encouraged to remove the status from the Action Provider). As indicated in the discussion of the ``/log`` method, support for it is optional, and the ``log_supported`` flag provides an indication to users whether they can make use of ``/log`` for fine grained monitoring of an Action.\n\n*  ``input_schema``: The ``input_schema`` value provides a complete schema description for the ``body`` property of the Action Request understood by this Action Provider. The schema is provided in `JSON Schema <https://json-schema.org/>`_ format.\n\n\nSetting Up an Action Provider in Globus Auth\n============================================\n\nThe Action Provider Interface makes use of and is bound closely with authentication via the `Globus Auth <https://globus.org/>`_ system. To authenticate RESTful requests using Globus Auth, a service must register as a "resource server". This is a multi-step process involving use of both the Globus Auth developer portal, and the Globus Auth API for configuring various access control states. To help with this process, we provide a step-by-step guide to using Globus Auth for this purpose:\n\n1. Register a new App on `<https://developers.globus.org>`_ using a browser. After insuring that you are logged in to the developer portal in a browser at this URL, perform the following steps:\n\n   - Click Add another project\n\n     - Provide a name, contact email and select which of your own Globus Auth linked identities are permitted to administer the project. You will be required to login with this identity in future interactions with the Globus Developer Portal to manipulate the resource server.\n\n   - Find your new, empty project, and select Add drop down and "new app"\n\n     - Provide a name for the specific app within the project. This will be a common name displayed to users when they make use of the Action Provider.\n\n     - When creating a resource server, the other fields on the app creation page are not used.\n\n       - "Redirects" is not used, but a value must be provided. You can use a URL associated with your service or a placeholder value like "https://localhost".\n\n       - "Scopes" are not relevant and make no difference, so this field should be left blank. The "Privacy Policy" and "Terms and Conditions" may be displayed to users making use of your action provider, but they are not required.\n\n   - Make note of the "Client Id" in the expanded description of your app. This value will be used elsewhere in the creation of the service and is often referenced as ``client_id``.\n\n   - In the section "Client Secrets" click "Create a new secret"\n\n     - Provide a name which is meaningful to you. It will not be displayed to other users.\n\n     - Make note of the generated secret. Like the ``client_id`` this will be used later in development. Be sure **not to lose it** as it can only be displayed once. However, new client secrets can be created and old ones deleted at any time should the need for a replacement secret arise.\n\n     - Set the client_id and client_secret on your command line to follow along with the rest of this guide.\n\n        .. code-block:: BASH    \n\n            export CLIENT_ID=<client_id>\n            export CLIENT_SECRET=<client_secret>\n\n2. Use the Globus Auth REST API to introspect your Action Provider Resource Server and create required Scopes.\n\n     .. note:: In the examples below, we will use the command line tool ``curl`` to perform the HTTP operations as it is very widely available. We also use the command line tool ``jq`` to format the ``curl`` command\'s json responses. However, other tools and clients exist for interacting with REST and HTTP services, so you may need to translate the ``curl`` and ``jq`` commands to your preferred tools.\n\n   - Introspect the Globus Auth client to see the same settings you setup in the developer portal. Notice we exported the ``<client_id>`` and ``<client_secret>`` values generated during your registration on the Globus Developer Portal into environment variables. \n    \n    .. code-block:: BASH\n\n        curl -s --user $CLIENT_ID:$CLIENT_SECRET https://auth.globus.org/v2/api/clients/$CLIENT_ID | jq\n        \n   - A successful return from this command is a JSON representation of the Globus Auth client similar to:\n\n        .. code-block:: JSON\n\n            {\n            "client": {\n                "scopes": [],\n                "redirect_uris": [\n                "https://localhost"\n                ],\n                "name": "My Action Provider",\n                "links": {\n                "privacy_policy": null,\n                "terms_and_conditions": null\n                },\n                "grant_types": [\n                "authorization_code",\n                "client_credentials",\n                "refresh_token",\n                "urn:globus:auth:grant_type:dependent_token"\n                ],\n                "fqdns": [],\n                "visibility": "private",\n                "project": "a47b9014-9250-4e21-9de5-b4aac81d464b",\n                "required_idp": null,\n                "preselect_idp": null,\n                "id": "8e98ba5a-21a9-4bef-ab6a-0fcdbed36405",\n                "public_client": false,\n                "parent_client": null\n              }\n            }\n\n\n   - Of note is the field ``scopes``. ``scopes`` are created to identify operations on the Action Provider. Typically, an Action Provide defines just one scope and it is provided to users in the Action Provider\'s introspection (``GET /``) information in the field ``globus_auth_scope``.\n\n     - Creating a Scope:  \n        - Creation of a scope is required as the scope will be used in authenticating REST calls on the Action Provider.\n        \n        - Start by creating a "scope definition" JSON document in the following format replacing the ``name``, ``description`` and optionally the ``scope_suffix``\n\n            .. code-block:: JSON\n\n                {\n                    "scope": {\n                        "name": "Action Provider Operations",\n                        "description": "All Operations on My Action Provider",\n                        "scope_suffix": "action_all",\n                        "dependent_scopes": [{\n                            "optional": false,\n                            "requires_refresh_token": true,\n                            "scope": "73320ffe-4cb4-4b25-a0a3-83d53d59ce4f"\n                         }],             \n                        "advertised": true,\n                        "allow_refresh_tokens": true\n                    }\n                }\n\n\n        - The ``name`` and ``description`` fields are purely informative and will be presented to other users who use the Globus Auth API to lookup the scope. The ``scope_suffix`` will be placed at the end of the generated "scope string" which is a URL identifier for the scope. It provides the context for the operations this scope covers among all operations your service provides. For Action Providers, we commonly use ``action_all`` to indicate all operations defined by the Action Provider API, but any string is acceptable.\n\n        - ``dependent_scopes`` define scopes of other Globus Auth resource servers that your Action Provider will invoke to perform its work. For example, if your Action Provider uses Globus Transfer to first move some data to compute upon, the scope for the Globus Transfer service would be placed in the ``dependent_scopes`` list. In the most common case, as shown in the example, the scope for the `Globus Groups API <https://docs.globus.org/api/groups/>`_ (with UUID ``73320ffe-4cb4-4b25-a0a3-83d53d59ce4f``) should be listed. This allows your Action Provider to determine what groups a user calling the provider belongs to and can therefore enforce policies, such as ``runnable_by`` or ``monitor_by`` based on group membership. If this scope is not listed as a dependent scope, the Action Provider Tools library will not be able to, and will therefore not attempt to, retrieve a user\'s groups and so no policies based on Groups may be used. We encourage you to consult the `Globus Auth Documentation <https://docs.globus.org/api/auth/>`_ for more information on creation and management of Scopes for more advanced scenarios such as other dependent Globus Auth based services such as Globus Transfer.\n            \n            Note: Scopes supplied in the dependent_scopes array must be identified by their UUID. The snippet below demonstrates how to lookup a scope\'s UUID based on its uniquely idenfitfying FQDN\n\n                .. code-block:: BASH\n                \n                    # Target FQDN is https://auth.globus.org/scopes/actions.globus.org/transfer/transfer\n                    export SCOPE_STRING=https://auth.globus.org/scopes/actions.globus.org/transfer/transfer\n                    curl -s -u "$CLIENT_ID:$CLIENT_SECRET" "https://auth.globus.org/v2/api/scopes?scope_strings=$SCOPE_STRING" | jq ".scopes[0].id"\n\n        \n        - The ``advertised`` property indicates whether the scope will be visible to all users who do scope look ups on Globus Auth. You may select either ``true`` or ``false`` for this depending on your own policy. ``allow_refresh_tokens`` should generally be set to ``true``, indicating that a client of the Action Provider who has authenticated the user via Globus Auth is allowed to refresh that authentication without further interactions from the user. Especially in the case where an Action may be long running and is monitored by an automated system like Globus Flows, it is important that token refresh is permitted.\n\n        - With the scope creation JSON document complete, use the following REST interaction to create the scope in Globus Auth via the ``curl`` command\n\n            .. code-block:: BASH\n\n                curl -s --user "$CLIENT_ID:$CLIENT_SECRET" -H \'Content-Type: application/json\' -XPOST https://auth.globus.org/v2/api/clients/$CLIENT_ID/scopes -d \'<Insert Scope creation document from above>\' | jq\n\n        - This should return the definition of the new scope matching the values provided in your scope creation document. As an example:\n\n            .. code-block:: JSON\n\n                {\n                    "scopes": [\n                        {\n                            "dependent_scopes": [{\n                                "optional": false,\n                                "requires_refresh_token": true,\n                                "scope": "73320ffe-4cb4-4b25-a0a3-83d53d59ce4f"\n                             }],\n                            "description": "<your description>",\n                            "allows_refresh_token": true,\n                            "client": "<client_id>",\n                            "advertised": true,\n                            "scope_string": "https://auth.globus.org/scopes/<client_id>/action_all",\n                            "id": "<A UUID for this scope>",\n                            "name": "<your scope name>"\n                        }\n                    ]\n                }\n\n        - The returned ``scope_string``, which always takes the form of a URL, will be the value exposed to users who wish to authenticate with Globus Auth to use your Action Provider. It will be part of the Action Provider description document, returned on the Action Provider Introspection operation (``GET /``) with the key ``globus_auth_scope``.\n\n        - Note that the returned value is an *array* of scopes. That is, more than one scope definition may be generated from the single scope creation request. This happens in the uncommon case where an FQDN has been registered for your ``client_id`` (refer to the `Globus Auth Documentation <https://docs.globus.org/api/auth/>`_ for information on FQDN registration if you desire it, though it is not recommended). In this case, a similar scope definition will also be generated, but the ``scope_string`` will contain the FQDN value(s). The ``scope_string`` values may be used interchangeably both by users requesting authentication to the Action Provider and in the ``globus_auth_scope`` value of the Action Provider Description. \n\n        - Check that the created scope(s) are correctly associated with the Action Provider:\n\n            .. code-block:: BASH\n\n                curl -s --user $CLIENT_ID:$CLIENT_SECRET https://auth.globus.org/v2/api/clients/$CLIENT_ID | jq\n\n3. Once your app and its scope(s) have been created and verified, remove your credentials from your command line environment.  Be sure to take note of the client ID and its associated client secret for use other places in the toolkit.\n\n            .. code-block:: BASH\n\n                unset CLIENT_ID CLIENT_SECRET\n                \nUsing the Toolkit\n==================\n\nThis toolkit provides the following components:\n\n1. Authentication helpers that make it easier to validate Globus Auth tokens and determine if a given request should be authorized\n\n2. An `OpenAPI v3 specification <http://spec.openapis.org/oas/v3.0.2>`_ and associated helpers that can be used to validate incoming requests and verify the responses your Action Provider generates. This document also defines the interface which must be supported by your REST API to have it function as an Action Provider.\n\n3. Simple bindings for the document types "Action Request" and "Action Status" to Python NamedTuple representations and helper functions for serializing and deserializing these structures to/from JSON.\n\n4. Helper methods for binding the REST API calls defined by the Action Interface to a Flask application. These helpers will perform the Authentication and Validation steps (as provided by components 1 and 2) and communicate with an Action Provider implementation using the structures defined in 3. For those users building an Action Provider using Flask, this provides a simplified method of getting the REST API implemented and removing common requirements so the focus can be on the logic of the Action provided.\n\n\nInstallation\n------------\n\nInstallation is via PyPi using, for example:\n\n.. code-block:: BASH\n\n    pip install globus-action-provider-tools\n\n\nAuthentication\n---------------\n\nThe authentication helpers can be used in your action provider as follows:\n\n.. code-block:: python\n\n    from globus_action_provider_tools.authentication import TokenChecker\n    # You will need to register a client and scope(s) in Globus Auth\n    # Then initialize a TokenChecker instance for your provider:\n    checker = TokenChecker(\n        client_id=\'YOUR_CLIENT_ID\',\n        client_secret=\'YOUR_CLIENT_SECRET\',\n        expected_scopes=[\'https://auth.globus.org/scopes/YOUR_SCOPES_HERE\'],\n    )\n\n\nWhen a request comes in, use your TokenChecker to validate the access token from the HTTP Authorization header.\n\n.. code-block:: python\n\n    access_token = request.headers[\'Authorization\'].replace(\'Bearer \', \'\')\n    auth_state = checker.check_token(access_token)\n\n\nThe AuthState has several properties and methods that will make it easier for you to decide whether or not to allow a request to proceed:\n\n.. code-block:: python\n\n    # This user\'s Globus identities:\n    auth_state.identities\n    # frozenset({\'urn:globus:auth:identity:9d437146-f150-42c2-be88-9d625d9e7cf9\',\n    #           \'urn:globus:auth:identity:c38f015b-8ad9-4004-9160-754b309b5b33\',\n    #           \'urn:globus:auth:identity:ffb5652b-d418-4849-9b57-556656706970\'})\n    # Groups this user is a member of:\n    auth_state.groups\n    # frozenset({\'urn:globus:groups:id:606dbaa9-3d57-44b8-a33e-422a9de0c712\',\n    #           \'urn:globus:groups:id:d2ff42bc-c708-460f-9e9b-b535c3776bdd\'})\n\n\nYou\'ll notice that both groups and identities are represented as strings that unambiguously signal what type of entity they represent. This makes it easy to merge the two sets without conflict, for situations where you\'d like to work with a single set containing all authentications:\n\n.. note:: The ``groups`` property will only have values if the Groups API scope is defined as a dependent scope as described in the previous section.\n\n.. code-block:: python\n\n    all_principals = auth_state.identities.union(auth_state.groups)\n\n\nThe AuthState object also offers a helper method, ``check_authorization()`` that is designed to help you test whether a request should be authorized:\n\n.. code-block:: python\n\n    resource_allows = [\'urn:globus:auth:identity:c38f015b-8ad9-4004-9160-754b309b5b33\']\n    auth_state.check_authorization(resource_allows)\n    # True\n\n\nThis method also accepts two special string values, ``\'public\'`` and ``\'all_authenticated_users\'``, together with keyword arguments that enable their use:\n\n.. code-block:: python\n\n    resource_allows = [\'public\']\n    auth_state.check_authorization(resource_allows, allow_public=True)\n    # True\n    resource_allows = [\'all_authenticated_users\']\n    auth_state.check_authorization(resource_allows, allow_all_authenticated_users=True)\n    # True\n\n\nCaching\n^^^^^^^\n\nTo avoid excessively taxing Globus Auth, the ``AuthState`` will, by default, cache identities and group memberships for 30 seconds.\n\nThe cache is initialized when you first instantiate your ``TokenChecker()``.  You should only need to create one TokenChecker instance for your application, and then you can re-use it to check each new token. In the event that you do need more than one TokenChecker, be aware that all TokenChecker instances in an app share the same underlying cache. \n\nIt is possible to customize a TokenChecker by supplying a custom configuration which gets passed on to the dogpile cache backend.  Note that each new instance of a TokenChecker with a custom configuration will drop the cache and recreate it with the desired settings.  Since all TokenCheckers share the same underlying cache, subsequent attempts to configure the cache will overwrite the previous cache\'s settings and therefore only the last applied configuration will persist.\n\n.. code-block:: python\n\n    # Create TokenChecker with default settings\n    my_token_checker = TokenChecker(\n        client_id=CLIENT_ID,\n        client_secret=CLIENT_SECRET,\n        expected_scopes=EXPECTED_SCOPES,\n    )\n\n    # Creating a TokenChecker with a custom config will drop the previous cache and\n    # create it with the new settings. Both TokenCheckers will use this new cache\n    new_token_checker = TokenChecker(\n            client_id=config["client_id"],\n            client_secret=config["client_secret"],\n            expected_scopes=config["expected_scopes"],\n            cache_config={\n                "backend": "dogpile.cache.pylibmc",\n                "timeout": "60",\n                "url": ["127.0.0.1"],\n            },\n        )\n\nValidation\n----------\n\nThere is an OpenAPI v3 specification for the Action Provider API available as described above. From this specification, we derive schemas that can be used to test incoming and outgoing messages. These schemas may be used to validate input documents and output documents within the service as follows.\n\n.. code-block:: python\n\n    from globus_action_provider_tools.validation import request_validator, response_validator, ValidationRequest\n    # Validating a request\n    request = ValidationRequest(provider_doc_type=\'ActionRequest\', request_data=<input data>)\n    result = request_validator.validate(request)\n    # Or a response:\n    response = ValidationRequest(provider_doc_type=\'ActionStatus\', request_data=<output data>)\n    result = response_validator.validate(response)\n    # get list of errors\n    errors = result.errors\n    # or get a single string summarizing all errors\n    err = result.error_msg\n\n\nThe request and response validation functions both take a ``ValidationRequest`` structure which has the name of the document type to be validated against and the data to be validated. At present, the document types supported are ``ActionRequest`` and ``ActionStatus`` documents as defined above.\n\n.. note:: There are additional validation helpers available for applications written using the Flask framework. Those are described below in the section describing the entire set of Flask helpers.\n\nData Types\n----------\n\nThe toolkit provides some simple bindings for the document types defined by the Action Provider Interface to type-annotated Python3 `NamedTuples <https://docs.python.org/3/library/typing.html#typing.NamedTuple>`_. This can provide a convenient way to manipulate these document types within an Action Provider implementation. There is also a Python JSON Encoder provided which can be used with the built-in Python json package to properly encode these data types into JSON.\n\n.. code-block:: python\n\n    from globus_action_provider_tools.data_types import (\n        ActionProviderDescription,\n        ActionProviderJsonEncoder,\n        ActionRequest,\n        ActionStatus,\n        ActionStatusValue,\n    )\n    status = ActionStatus(\n        status=ActionStatusValue.SUCCEEDED,\n        creator_id=caller_id,\n        monitor_by=request.monitor_by,\n        manage_by=request.manage_by,\n        start_time=str(datetime.datetime.now().isoformat()),\n        completion_time=str(datetime.datetime.now().isoformat()),\n        release_after=60 * 60 * 24 * 30,  # 30-days in seconds\n        display_status=ActionStatusValue.SUCCEEDED.name,\n        details=result_details,\n    )\n    json_string = json.dumps(action_status, cls=ActionProviderJsonEncoder)\n\n\nFlask Helper\n------------\n\nAs Action Providers are HTTP-servers, a common approach to building them is the use of the `Flask <https://palletsprojects.com/p/flask/>`_ framework. To aid in developing Flask-based Action Providers, helper methods are provided which encapsulate much of the other functionality in the framework: authentication, validation and serialization for easy use in a Flask-based application. Rather than defining each of the Action Provider Interface routes in the Flask application, helpers are provided which declare the necessary routes to Flask, perform the serialization, validation and authentication on the request, and pass only those requests which have satisfied these conditions on to a user-defined implementation of the routes.\n\nTo use the helpers, you must define functions corresponding to the various methods of the Action Provider interface (``run``, ``status``, ``release``, ``cancel``), and must provide the Action Provider introspection information in an instance of the ``ActionProviderDescription`` ``NamedTuple`` class defined in the tookit\'s ``data_types`` package. The application must also provide a Flask ``blueprint`` object to which the toolkit can attach the new routes. It is recommended that the ``blueprint`` be created with a ``url_prefix`` so that the Action Provider Interface routes are rooted at a distinct root path in the application\'s URL namespace.\n\nA brief example of setting up the flask helper is provided immediately below. A more complete example showing implementation of all the required functions is provided in the Appendix. It is appropriate to use the skeleton in the Appendix as a starting point for any new Action Providers which are developed.\n\n.. code-block:: python\n                \n    from globus_action_provider_tools.data_types import (\n        ActionProviderDescription,\n        ActionRequest,\n        ActionStatus,\n        ActionStatusValue,\n    )\n    from globus_action_provider_tools.flask import (\n        ActionStatusReturn,\n        add_action_routes_to_blueprint,\n    )\n    action_blueprint = Blueprint("action", __name__, url_prefix="/action")\n    provider_description = ActionProviderDescription(\n        globus_auth_scope="<scope created in Globus Auth>",\n        title="My Action Provider",\n        admin_contact="support@example.com",\n        synchronous=True,\n        input_schema={}, # JSON Schema representation of the input on the request\n        log_supported=False\n    )\n    add_action_routes_to_blueprint(\n        action_blueprint,\n        CLIENT_ID,\n        CLIENT_SECRET,\n        CLIENT_NAME,\n        provider_description,\n        action_run,\n        action_status,\n        action_cancel,\n        action_release,\n    )\n\n\nIn this example, the values ``CLIENT_ID``, ``CLIENT_SECRET`` and ``CLIENT_NAME`` are as defined in Globus Auth as described above (where ``CLIENT_NAME`` is almost always passed as ``None`` except in the uncommon, legacy case where a particular name has been associated with a Globus Auth client). The values ``action_run``, ``action_status``, ``action_cancel`` and ``action_release`` are all **functions** which will be called by the framework when the corresponding HTTP requests are called. Where appropriate, these functions are implemented in terms of the toolkit\'s data types so the need for JSON serialization and deserialization is greatly reduced from the application code. The framework will also provide validation of input ``ActionRequest`` data to the ``/run`` method prior to invoking the ``action_run`` function. As long as the return value from the various functions is of type ``ActionStatus``, the framework will also insure that the returned JSON data conforms to the Action Provider Interface. The example in the Appendix demonstrates how these functions can be implemented.\n\n\nAppendix: Example Action Provider\n=================================\n\n\n.. code-block:: python\n\n    import datetime\n    import uuid\n    from typing import Dict, Optional, Tuple\n\n    from flask import Blueprint, Flask\n    from werkzeug.exceptions import Conflict, NotFound\n\n    from globus_action_provider_tools.authorization import authorize_action_access_or_404\n    from globus_action_provider_tools.data_types import (\n        ActionProviderDescription,\n        ActionRequest,\n        ActionStatus,\n        ActionStatusValue,\n        AuthState,\n    )\n    from globus_action_provider_tools.flask import (\n        ActionStatusReturn,\n        add_action_routes_to_blueprint,\n    )\n\n    skeleton_blueprint = Blueprint("skeleton", __name__, url_prefix="/skeleton")\n\n    input_schema = {\n        "$id": "https://automate.globus.org/skeleton_action_provider.input.schema.json",\n        "$schema": "http://json-schema.org/draft-07/schema#",\n        "title": "Skeleton Action Provider Input Schema",\n        "type": "object",\n        "properties": {"input_string": {"type": "string"}},\n        "additionalProperties": False,\n        "required": ["input_string"],\n    }\n\n    provider_description = ActionProviderDescription(\n        globus_auth_scope="https://auth.globus.org/scopes/16e16447-209a-4825-ae19-25e279d91642/action_all_with_groups",\n        title="skeleton_action_provider",\n        admin_contact="support@globus.org",\n        synchronous=True,\n        input_schema=input_schema,\n        log_supported=False,  # This provider doesn\'t implement the log callback\n    )\n\n    # A simulated database mapping input user action requests identifiers to a previously\n    # seen request id and the corresponding action id\n    _fake_request_db: Dict[str, Tuple[ActionRequest, str]] = {}\n\n    _fake_action_db: Dict[str, ActionStatus] = {}\n\n\n    def _retrieve_action_status(action_id: str) -> ActionStatus:\n        status = _fake_action_db.get(action_id)\n        if status is None:\n            raise NotFound(f"No Action with id {action_id}")\n        return status\n\n\n    def action_run(request: ActionRequest, auth: AuthState) -> ActionStatusReturn:\n        """\n        Asynchronous actions most likely need to implement retry logic here to \n        prevent duplicate requests with matching request_ids from launching \n        another job. In the event that a request with an existing request_id \n        and creator_id arrives, this function should simply return the action\'s \n        status via the action_status function.\n\n        Synchronous actions or actions where it makes sense to execute repeated \n        runs with the same parameters need not implement retry logic.\n        """\n\n        caller_id = auth.effective_identity\n        request_id = request.request_id\n        full_request_id = f"{caller_id}:{request_id}"\n        prev_request = _fake_request_db.get(full_request_id)\n        if prev_request is not None:\n            if prev_request[0] == request:\n                return action_status(prev_request[1], auth)\n            else:\n                raise Conflict(\n                    f"Request with id {request_id} already present with different parameters "\n                )\n        # Local processing would happen here\n        result_details = {\n            # This is safe because the input has been validated against the input schema\n            "you_said": request.body["input_string"]\n        }\n        status = ActionStatus(\n            status=ActionStatusValue.SUCCEEDED,\n            creator_id=caller_id,\n            monitor_by=request.monitor_by,\n            manage_by=request.manage_by,\n            start_time=str(datetime.datetime.now().isoformat()),\n            completion_time=str(datetime.datetime.now().isoformat()),\n            release_after=request.release_after or "P30D",\n            display_status=ActionStatusValue.SUCCEEDED.name,\n            details=result_details,\n        )\n        _fake_request_db[full_request_id] = (request, status.action_id)\n        _fake_action_db[status.action_id] = status\n        return status\n\n\n    def action_status(action_id: str, auth: AuthState) -> ActionStatusReturn:\n        """\n        action_status retrieves the most recent state of the action. This endpoint \n        requires the user authenticate with a principal value which is in the \n        monitor_by list established when the Action was started.\n        """\n        status = _retrieve_action_status(action_id)\n        authorize_action_access_or_404(status, auth)\n        return status, 200\n\n\n    def action_cancel(action_id: str, auth: AuthState) -> ActionStatusReturn:\n        """ \n        Asynchronous actions need not ensure a running action is immediately \n        completed or terminated. In this scenario, action_cancel should return \n        an action in a non-completion state. If it has completed, return the action\'s\n        status.\n\n        Synchronous actions need not implement any logic in action_cancel. All \n        processing happens in the action_run callback so that action_cancel \n        simply returns the action_id\'s status.\n        """\n        status = _retrieve_action_status(action_id)\n        authorize_action_access_or_404(status, auth)\n        if status.status in (ActionStatusValue.SUCCEEDED, ActionStatusValue.FAILED):\n            return status\n        # Process Action cancellation\n        status.status = ActionStatusValue.FAILED\n        status.display_status = "Canceled by user request"\n        return status\n\n\n    def action_release(action_id: str, auth: AuthState) -> ActionStatusReturn:\n        """ \n        If the Action is not already in a completion state, action_release should \n        return an error as this operation does not attempt to stop execution.\n        Synchronous actions need not determine if the action_id is still in a \n        processing state. All processing starts and completes in the action_run \n        callback so that action_release simply removes the action_id and request_id \n        from history and returns the action_id\'s completion status.\n        """\n        status = _retrieve_action_status(action_id)\n        authorize_action_access_or_404(status, auth)\n        if status.status not in (ActionStatusValue.SUCCEEDED, ActionStatusValue.FAILED):\n            raise Conflict("Action is not complete")\n        _fake_action_db.pop(action_id)\n        # Both fake and badly inefficient\n        remove_req_id: Optional[str] = None\n        for req_id, req_and_action_id in _fake_request_db.items():\n            if req_and_action_id[1] == action_id:\n                remove_req_id = req_id\n                break\n        if remove_req_id is not None:\n            _fake_request_db.pop(remove_req_id)\n        return status, 200\n\n\n    def main():\n        app = Flask(__name__)\n        app.url_map.strict_slashes = False\n        add_action_routes_to_blueprint(\n            skeleton_blueprint,\n            CLIENT_ID,\n            CLIENT_SECRET,\n            None,\n            provider_description,\n            action_run,\n            action_status,\n            action_cancel,\n            action_release,\n        )\n        app.register_blueprint(skeleton_blueprint)\n        app.run(debug=True)\n\n\n    if __name__ == "__main__":\n        main()\n\n\n',
     'author': 'Jim Pruyne',
     'author_email': 'pruyne@globus.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `globus-action-provider-tools-0.9.4/PKG-INFO` & `globus-action-provider-tools-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-action-provider-tools
-Version: 0.9.4
+Version: 0.9.5
 Summary: Tools to help developers build services that implement the Action Provider specification.
 Keywords: globus,automation,workflow,action_provider
 Author: Jim Pruyne
 Author-email: pruyne@globus.org
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

