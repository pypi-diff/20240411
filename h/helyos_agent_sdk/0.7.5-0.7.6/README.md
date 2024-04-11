# Comparing `tmp/helyos_agent_sdk-0.7.5.tar.gz` & `tmp/helyos_agent_sdk-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helyos_agent_sdk-0.7.5.tar", max compression
+gzip compressed data, was "helyos_agent_sdk-0.7.6.tar", max compression
```

## Comparing `helyos_agent_sdk-0.7.5.tar` & `helyos_agent_sdk-0.7.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2024-02-25 08:47:54.315736 helyos_agent_sdk-0.7.5/LICENSE
--rw-r--r--   0        0        0     2735 2024-02-25 10:10:09.047168 helyos_agent_sdk-0.7.5/README.md
--rw-r--r--   0        0        0      238 2024-02-25 08:47:54.357133 helyos_agent_sdk-0.7.5/helyos_agent_sdk/__init__.py
--rw-r--r--   0        0        0    20264 2024-02-25 08:47:54.357339 helyos_agent_sdk-0.7.5/helyos_agent_sdk/client.py
--rw-r--r--   0        0        0    16343 2024-02-25 08:47:54.357636 helyos_agent_sdk-0.7.5/helyos_agent_sdk/connector.py
--rw-r--r--   0        0        0     6892 2024-02-25 08:47:54.357812 helyos_agent_sdk-0.7.5/helyos_agent_sdk/crypto.py
--rw-r--r--   0        0        0     4318 2024-02-25 08:47:54.357995 helyos_agent_sdk-0.7.5/helyos_agent_sdk/database_connector.py
--rw-r--r--   0        0        0      461 2024-02-25 08:47:54.358106 helyos_agent_sdk-0.7.5/helyos_agent_sdk/exceptions.py
--rw-r--r--   0        0        0     3719 2024-02-25 08:47:54.358212 helyos_agent_sdk-0.7.5/helyos_agent_sdk/models.py
--rw-r--r--   0        0        0    18950 2024-02-25 08:47:54.358327 helyos_agent_sdk-0.7.5/helyos_agent_sdk/mqtt_client.py
--rw-r--r--   0        0        0     3781 2024-02-25 08:47:54.358472 helyos_agent_sdk-0.7.5/helyos_agent_sdk/summary_request.py
--rw-r--r--   0        0        0      502 2024-02-25 08:47:54.358585 helyos_agent_sdk-0.7.5/helyos_agent_sdk/utils.py
--rw-r--r--   0        0        0     1307 2024-02-25 10:12:03.019266 helyos_agent_sdk-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     4009 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-02-25 08:47:54.315736 helyos_agent_sdk-0.7.6/LICENSE
+-rw-r--r--   0        0        0     2721 2024-03-12 11:26:02.106259 helyos_agent_sdk-0.7.6/README.md
+-rw-r--r--   0        0        0      238 2024-02-25 08:47:54.357133 helyos_agent_sdk-0.7.6/helyos_agent_sdk/__init__.py
+-rw-r--r--   0        0        0    20562 2024-04-11 12:58:29.767158 helyos_agent_sdk-0.7.6/helyos_agent_sdk/client.py
+-rw-r--r--   0        0        0    16343 2024-02-25 08:47:54.357636 helyos_agent_sdk-0.7.6/helyos_agent_sdk/connector.py
+-rw-r--r--   0        0        0     6892 2024-02-25 08:47:54.357812 helyos_agent_sdk-0.7.6/helyos_agent_sdk/crypto.py
+-rw-r--r--   0        0        0     4318 2024-02-25 08:47:54.357995 helyos_agent_sdk-0.7.6/helyos_agent_sdk/database_connector.py
+-rw-r--r--   0        0        0      461 2024-02-25 08:47:54.358106 helyos_agent_sdk-0.7.6/helyos_agent_sdk/exceptions.py
+-rw-r--r--   0        0        0     3719 2024-02-25 08:47:54.358212 helyos_agent_sdk-0.7.6/helyos_agent_sdk/models.py
+-rw-r--r--   0        0        0    19250 2024-04-11 12:58:29.767812 helyos_agent_sdk-0.7.6/helyos_agent_sdk/mqtt_client.py
+-rw-r--r--   0        0        0     3781 2024-02-25 08:47:54.358472 helyos_agent_sdk-0.7.6/helyos_agent_sdk/summary_request.py
+-rw-r--r--   0        0        0      502 2024-02-25 08:47:54.358585 helyos_agent_sdk-0.7.6/helyos_agent_sdk/utils.py
+-rw-r--r--   0        0        0     1273 2024-04-11 12:58:29.768406 helyos_agent_sdk-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     3953 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.7.6/PKG-INFO
```

### Comparing `helyos_agent_sdk-0.7.5/LICENSE` & `helyos_agent_sdk-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.7.5/README.md` & `helyos_agent_sdk-0.7.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
   <p align="center">
     Methods and data strrctures to connect autonomous vehicles to helyOS.
     <br />
     <a href="https://helyosframework.github.io/helyos_agent_sdk/"><strong>Explore the docs »</strong></a>
     <br />
     <br />
-    <a href="https://github.com/">View Demo</a>
+    <a href="https://github.com/helyOSFramework/helyos_agent_slim_simulator">Demo</a>
     ·
     <a href="https://github.com/helyOSFramework/helyos_agent_sdk/issues">Report Bug</a>
     ·
     <a href="https://github.com/helyOSFramework/helyos_agent_sdk/issues">Request Feature</a>
   </p>
 </div>
 
@@ -80,15 +80,11 @@
 ```
 
 
 ### Contributing
 
 Keep it simple. Keep it minimal.
 
-### Authors
-
-*   Carlos E. Viol Barbosa
-*   ...
 
 ### License
 
 This project is licensed under the MIT License
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 
                                  _[_L_o_g_o_]_[_L_o_g_o_]
                           ******** hheellyyOOSS AAggeenntt SSDDKK ********
     Methods and data strrctures to connect autonomous vehicles to helyOS.
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
-                  _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
+                     _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 ## About The Project The helyos-agent-sdk python package encloses methods and
 data structures definitions that facilitate the connection to helyOS core via
 RabbitMQ. ### List of features * RabbitMQ client for communication with helyOS
 core. * Support for both AMQP and MQTT protocols. * Definition of agent and
 assignment status. * Easy access to helyOS assignments and instant actions
 through callbacks. * SSL support and application-level security with RSA
 signature. * Automatic reconnection to handle connection disruptions. ###
@@ -24,9 +24,9 @@
 agent_connector = AgentConnector(helyOS_client) agent_connector.publish_sensors
 (x=-30167, y=3000, z=0, orientations=[1500, 0], sensor= {"my_custom_format":
 {}}) # ... # agent_connector.publish_state(status, resources,
 assignment_status) # ... # agent_connector.consume_instant_action_messages
 (my_reserve_callback, my_release_callback, my_cancel_assignm_callback,
 any_other_callback) agent_connector.consume_assignment_messages
 (my_assignment_callback) agent_connector.start_listening() ``` ### Contributing
-Keep it simple. Keep it minimal. ### Authors * Carlos E. Viol Barbosa * ... ###
-License This project is licensed under the MIT License
+Keep it simple. Keep it minimal. ### License This project is licensed under the
+MIT License
```

### Comparing `helyos_agent_sdk-0.7.5/helyos_agent_sdk/client.py` & `helyos_agent_sdk-0.7.6/helyos_agent_sdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import time
+import time, warnings
 from functools import wraps
 import pika
 import os
 import json
 import ssl
 from .exceptions import *
 from helyos_agent_sdk.models import AGENT_STATE, CheckinResponseMessage
@@ -17,14 +17,18 @@
 REGISTRATION_TOKEN = os.environ.get(
     'REGISTRATION_TOKEN', '0000-0000-0000-0000-0000')
 
 
 def connect_rabbitmq(rabbitmq_host, rabbitmq_port, username, passwd, enable_ssl=False, ca_certificate=None, temporary=False):
     credentials = pika.PlainCredentials(username, passwd)
     if enable_ssl:
+        if rabbitmq_port == 5672:
+            warnings.warn('Warning: SSL is enabled, but the port is set to 5672, which is the default for non-encrypted AMQP connection.' +
+                          ' Consider using port 5671.', UserWarning)
+
         context = ssl.create_default_context(cadata=ca_certificate)
         if ca_certificate is not None:
             context.check_hostname = True
             context.verify_mode = ssl.CERT_REQUIRED
         else:
             context.check_hostname = False
             context.verify_mode = ssl.CERT_NONE
@@ -361,15 +365,16 @@
             raise HelyOSCheckinError('Check in refused: received invalid message format')
 
         if not self.checkin_guard_interceptor(ch, sender, checkin_data, received_message_str, signature):
             raise HelyOSCheckinError('Check in refused: checkin_guard_interceptor returned False')
 
 
         password = body.pop('rbmq_password', None)
-        self.ca_certificate = body.get('ca_certificate', self.ca_certificate)
+        if self.ca_certificate is None:
+            self.ca_certificate = body.get('ca_certificate', self.ca_certificate)
         if self.helyos_public_key is None:
             self.helyos_public_key = body.get('helyos_public_key', self.helyos_public_key)
 
         if password:
             self.connection = connect_rabbitmq(
                 self.rabbitmq_host, self.rabbitmq_port, body['rbmq_username'], password, self.enable_ssl, self.ca_certificate)
             self.channel = self.connection.channel()
```

### Comparing `helyos_agent_sdk-0.7.5/helyos_agent_sdk/connector.py` & `helyos_agent_sdk-0.7.6/helyos_agent_sdk/connector.py`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.7.5/helyos_agent_sdk/crypto.py` & `helyos_agent_sdk-0.7.6/helyos_agent_sdk/crypto.py`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.7.5/helyos_agent_sdk/database_connector.py` & `helyos_agent_sdk-0.7.6/helyos_agent_sdk/database_connector.py`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.7.5/helyos_agent_sdk/models.py` & `helyos_agent_sdk-0.7.6/helyos_agent_sdk/models.py`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.7.5/helyos_agent_sdk/mqtt_client.py` & `helyos_agent_sdk-0.7.6/helyos_agent_sdk/mqtt_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import json
 import ssl
 
 from helyos_agent_sdk.models import CheckinResponseMessage
 from .exceptions import *
 import paho.mqtt.client as mqtt
-import time
+import time, warnings
 from .crypto import Signing, generate_private_public_keys
 
 AGENTS_UL_EXCHANGE = os.environ.get(
     'AGENTS_UL_EXCHANGE', 'xchange_helyos.agents.ul')
 AGENTS_DL_EXCHANGE = os.environ.get(
     'AGENTS_DL_EXCHANGE', 'xchange_helyos.agents.dl')
 AGENT_ANONYMOUS_EXCHANGE = os.environ.get(
@@ -37,14 +37,18 @@
     def on_connect(client, userdata, flags, rc):
         global mqtt_msg
         mqtt_msg = LOGMSG[rc]
 
     mqtt_client.on_connect = on_connect
 
     if enable_ssl:
+        if rabbitmq_port == 1883:
+            warnings.warn('Warning: SSL is enabled, but the port is set to 1883, which is the default for non-encrypted MQTT connection.' + 
+                          'Consider using port 8883.', UserWarning)
+  
         context = ssl.create_default_context(cadata=ca_certificate)
         if ca_certificate is not None:
             context.check_hostname = True
             context.verify_mode = ssl.CERT_REQUIRED
         else:
             context.check_hostname = False
             context.verify_mode = ssl.CERT_NONE
@@ -360,15 +364,16 @@
 
         if not self.checkin_guard_interceptor(client, sender, checkin_data, received_message_str, signature):
             client.loop_stop()
             raise HelyOSCheckinError('Check in refused: checkin_guard_interceptor returned False')
 
 
         password = body.pop('rbmq_password', None)
-        self.ca_certificate = body.get('ca_certificate', self.ca_certificate)
+        if self.ca_certificate is None:
+            self.ca_certificate = body.get('ca_certificate', self.ca_certificate)
         if self.helyos_public_key is None:
             self.helyos_public_key = body.get('helyos_public_key', self.helyos_public_key)
 
         if password:
             self.connection = connect_mqtt(self.rabbitmq_host, self.rabbitmq_port,
                                            body['rbmq_username'], password, self.enable_ssl, self.ca_certificate)
             self.channel = self.connection
```

### Comparing `helyos_agent_sdk-0.7.5/helyos_agent_sdk/summary_request.py` & `helyos_agent_sdk-0.7.6/helyos_agent_sdk/summary_request.py`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.7.5/pyproject.toml` & `helyos_agent_sdk-0.7.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "helyos_agent_sdk"
-version = "0.7.5"
+version = "0.7.6"
 description = "Package encloses methods and data definitions that facilitate the connection of agents in the helyOS framework."
-authors = ["Carlos Viol Barbosa <you@example.com>, Julius Kolb <you@example.com>"]
+authors = ["Carlos Viol Barbosa , Julius Kolb "]
 readme = "README.md"
 packages = [{include = "helyos_agent_sdk"}]
 keywords = ["autonomous driving", "helyos", "agent", "robot"]
 
 homepage = "https://helyosframework.org"
 repository = "https://github.com/helyOSFramework/helyos_agent_sdk"
 documentation = "https://helyosframework.github.io/helyos_agent_sdk/"
```

### Comparing `helyos_agent_sdk-0.7.5/PKG-INFO` & `helyos_agent_sdk-0.7.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: helyos_agent_sdk
-Version: 0.7.5
+Version: 0.7.6
 Summary: Package encloses methods and data definitions that facilitate the connection of agents in the helyOS framework.
 Home-page: https://helyosframework.org
 Keywords: autonomous driving,helyos,agent,robot
-Author: Carlos Viol Barbosa
-Author-email: you@example.com>, Julius Kolb <you@example.com
+Author: Carlos Viol Barbosa , Julius Kolb 
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -41,15 +40,15 @@
 
   <p align="center">
     Methods and data strrctures to connect autonomous vehicles to helyOS.
     <br />
     <a href="https://helyosframework.github.io/helyos_agent_sdk/"><strong>Explore the docs »</strong></a>
     <br />
     <br />
-    <a href="https://github.com/">View Demo</a>
+    <a href="https://github.com/helyOSFramework/helyos_agent_slim_simulator">Demo</a>
     ·
     <a href="https://github.com/helyOSFramework/helyos_agent_sdk/issues">Report Bug</a>
     ·
     <a href="https://github.com/helyOSFramework/helyos_agent_sdk/issues">Request Feature</a>
   </p>
 </div>
 
@@ -109,16 +108,12 @@
 ```
 
 
 ### Contributing
 
 Keep it simple. Keep it minimal.
 
-### Authors
-
-*   Carlos E. Viol Barbosa
-*   ...
 
 ### License
 
 This project is licensed under the MIT License
```

#### html2text {}

```diff
@@ -1,33 +1,32 @@
-Metadata-Version: 2.1 Name: helyos_agent_sdk Version: 0.7.5 Summary: Package
+Metadata-Version: 2.1 Name: helyos_agent_sdk Version: 0.7.6 Summary: Package
 encloses methods and data definitions that facilitate the connection of agents
 in the helyOS framework. Home-page: https://helyosframework.org Keywords:
-autonomous driving,helyos,agent,robot Author: Carlos Viol Barbosa Author-email:
-you@example.com>, Julius Kolb
-example.com Requires-Python: >=3.7,<4.0 Classifier: Environment :: Console
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cryptography (>=41.0.3,<42.0.0) Requires-Dist: dataclasses-json
-(>=0.5.7,<0.6.0) Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0) Requires-Dist: pika
-(>=1.3.1,<2.0.0) Requires-Dist: pycryptodome (>=3.15.0,<4.0.0) Project-URL:
-Documentation, https://helyosframework.github.io/helyos_agent_sdk/ Project-URL:
-Repository, https://github.com/helyOSFramework/helyos_agent_sdk Description-
-Content-Type: text/markdown
+autonomous driving,helyos,agent,robot Author: Carlos Viol Barbosa , Julius Kolb
+Requires-Python: >=3.7,<4.0 Classifier: Environment :: Console Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Build Tools Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Requires-Dist: cryptography
+(>=41.0.3,<42.0.0) Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0) Requires-
+Dist: paho-mqtt (>=1.6.1,<2.0.0) Requires-Dist: pika (>=1.3.1,<2.0.0) Requires-
+Dist: pycryptodome (>=3.15.0,<4.0.0) Project-URL: Documentation, https://
+helyosframework.github.io/helyos_agent_sdk/ Project-URL: Repository, https://
+github.com/helyOSFramework/helyos_agent_sdk Description-Content-Type: text/
+markdown
 
                                  _[_L_o_g_o_]_[_L_o_g_o_]
                           ******** hheellyyOOSS AAggeenntt SSDDKK ********
     Methods and data strrctures to connect autonomous vehicles to helyOS.
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
-                  _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
+                     _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 ## About The Project The helyos-agent-sdk python package encloses methods and
 data structures definitions that facilitate the connection to helyOS core via
 RabbitMQ. ### List of features * RabbitMQ client for communication with helyOS
 core. * Support for both AMQP and MQTT protocols. * Definition of agent and
 assignment status. * Easy access to helyOS assignments and instant actions
 through callbacks. * SSL support and application-level security with RSA
 signature. * Automatic reconnection to handle connection disruptions. ###
@@ -43,9 +42,9 @@
 agent_connector = AgentConnector(helyOS_client) agent_connector.publish_sensors
 (x=-30167, y=3000, z=0, orientations=[1500, 0], sensor= {"my_custom_format":
 {}}) # ... # agent_connector.publish_state(status, resources,
 assignment_status) # ... # agent_connector.consume_instant_action_messages
 (my_reserve_callback, my_release_callback, my_cancel_assignm_callback,
 any_other_callback) agent_connector.consume_assignment_messages
 (my_assignment_callback) agent_connector.start_listening() ``` ### Contributing
-Keep it simple. Keep it minimal. ### Authors * Carlos E. Viol Barbosa * ... ###
-License This project is licensed under the MIT License
+Keep it simple. Keep it minimal. ### License This project is licensed under the
+MIT License
```

