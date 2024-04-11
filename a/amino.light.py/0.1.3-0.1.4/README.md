# Comparing `tmp/amino.light.py-0.1.3.tar.gz` & `tmp/amino.light.py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.light.py-0.1.3.tar", last modified: Wed Apr 10 20:50:28 2024, max compression
+gzip compressed data, was "amino.light.py-0.1.4.tar", last modified: Wed Apr 10 21:46:44 2024, max compression
```

## Comparing `amino.light.py-0.1.3.tar` & `amino.light.py-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 20:50:28.835242 amino.light.py-0.1.3/
-drwxrwxrwx   0        0        0        0 2024-04-10 20:50:28.712244 amino.light.py-0.1.3/AminoLightPy/
--rw-rw-rw-   0        0        0      296 2024-04-10 20:45:21.000000 amino.light.py-0.1.3/AminoLightPy/__init__.py
--rw-rw-rw-   0        0        0    17388 2024-04-10 00:15:18.000000 amino.light.py-0.1.3/AminoLightPy/acm.py
--rw-rw-rw-   0        0        0    72454 2024-04-10 13:49:30.000000 amino.light.py-0.1.3/AminoLightPy/client.py
--rw-rw-rw-   0        0        0     2643 2024-04-08 13:03:57.000000 amino.light.py-0.1.3/AminoLightPy/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-10 20:50:28.714244 amino.light.py-0.1.3/AminoLightPy/lib/
--rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.1.3/AminoLightPy/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 20:50:28.745244 amino.light.py-0.1.3/AminoLightPy/lib/util/
--rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.1.3/AminoLightPy/lib/util/__init__.py
--rw-rw-rw-   0        0        0    32075 2024-04-09 21:58:19.000000 amino.light.py-0.1.3/AminoLightPy/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     1354 2024-04-09 22:00:38.000000 amino.light.py-0.1.3/AminoLightPy/lib/util/helpers.py
--rw-rw-rw-   0        0        0    95642 2024-04-10 20:48:55.000000 amino.light.py-0.1.3/AminoLightPy/lib/util/objects.py
--rw-rw-rw-   0        0        0    17113 2024-04-10 13:21:35.000000 amino.light.py-0.1.3/AminoLightPy/socket.py
--rw-rw-rw-   0        0        0    75163 2024-04-10 13:49:22.000000 amino.light.py-0.1.3/AminoLightPy/sub_client.py
--rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3567 2024-04-10 20:50:28.834245 amino.light.py-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2771 2024-04-10 20:49:56.000000 amino.light.py-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 20:50:28.832241 amino.light.py-0.1.3/amino.light.py.egg-info/
--rw-rw-rw-   0        0        0     3567 2024-04-10 20:50:26.000000 amino.light.py-0.1.3/amino.light.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2024-04-10 20:50:27.000000 amino.light.py-0.1.3/amino.light.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 20:50:26.000000 amino.light.py-0.1.3/amino.light.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-10 20:50:26.000000 amino.light.py-0.1.3/amino.light.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-10 20:50:26.000000 amino.light.py-0.1.3/amino.light.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 20:50:28.849240 amino.light.py-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1298 2024-04-10 20:46:02.000000 amino.light.py-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 21:46:43.974547 amino.light.py-0.1.4/
+drwxrwxrwx   0        0        0        0 2024-04-10 21:46:43.833546 amino.light.py-0.1.4/AminoLightPy/
+-rw-rw-rw-   0        0        0      296 2024-04-10 21:46:16.000000 amino.light.py-0.1.4/AminoLightPy/__init__.py
+-rw-rw-rw-   0        0        0    17388 2024-04-10 00:15:18.000000 amino.light.py-0.1.4/AminoLightPy/acm.py
+-rw-rw-rw-   0        0        0    72454 2024-04-10 21:35:41.000000 amino.light.py-0.1.4/AminoLightPy/client.py
+-rw-rw-rw-   0        0        0     2643 2024-04-08 13:03:57.000000 amino.light.py-0.1.4/AminoLightPy/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-10 21:46:43.836545 amino.light.py-0.1.4/AminoLightPy/lib/
+-rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.1.4/AminoLightPy/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 21:46:43.846547 amino.light.py-0.1.4/AminoLightPy/lib/util/
+-rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.1.4/AminoLightPy/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    32075 2024-04-09 21:58:19.000000 amino.light.py-0.1.4/AminoLightPy/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     1354 2024-04-09 22:00:38.000000 amino.light.py-0.1.4/AminoLightPy/lib/util/helpers.py
+-rw-rw-rw-   0        0        0    95642 2024-04-10 21:45:50.000000 amino.light.py-0.1.4/AminoLightPy/lib/util/objects.py
+-rw-rw-rw-   0        0        0    17113 2024-04-10 21:45:48.000000 amino.light.py-0.1.4/AminoLightPy/socket.py
+-rw-rw-rw-   0        0        0    75163 2024-04-10 21:35:47.000000 amino.light.py-0.1.4/AminoLightPy/sub_client.py
+-rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2804 2024-04-10 21:46:43.973547 amino.light.py-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2010 2024-04-10 21:00:12.000000 amino.light.py-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 21:46:43.970545 amino.light.py-0.1.4/amino.light.py.egg-info/
+-rw-rw-rw-   0        0        0     2804 2024-04-10 21:46:42.000000 amino.light.py-0.1.4/amino.light.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2024-04-10 21:46:42.000000 amino.light.py-0.1.4/amino.light.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 21:46:42.000000 amino.light.py-0.1.4/amino.light.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-10 21:46:42.000000 amino.light.py-0.1.4/amino.light.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-10 21:46:42.000000 amino.light.py-0.1.4/amino.light.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 21:46:43.990544 amino.light.py-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2024-04-10 21:46:11.000000 amino.light.py-0.1.4/setup.py
```

### Comparing `amino.light.py-0.1.3/AminoLightPy/acm.py` & `amino.light.py-0.1.4/AminoLightPy/acm.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.3/AminoLightPy/client.py` & `amino.light.py-0.1.4/AminoLightPy/client.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.3/AminoLightPy/constants.py` & `amino.light.py-0.1.4/AminoLightPy/constants.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.3/AminoLightPy/lib/util/exceptions.py` & `amino.light.py-0.1.4/AminoLightPy/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.3/AminoLightPy/lib/util/helpers.py` & `amino.light.py-0.1.4/AminoLightPy/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.3/AminoLightPy/lib/util/objects.py` & `amino.light.py-0.1.4/AminoLightPy/lib/util/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,25 +607,26 @@
 class FromCode:
     def __init__(self, data):
         self.json = data
 
         extensions = data.get("extensions") or {}
         linkInfo = extensions.get("linkInfo") or {}
 
-        self.community: Community = Community(extensions.get("community")).Community
+        community = Community(extensions.get("community")).Community
+        self.community: Community = community
         self.path = data.get("path")
         self.objectType = linkInfo.get("objectType")
         self.shortCode = linkInfo.get("shortCode")
         self.fullPath = linkInfo.get("fullPath")
         self.targetCode = linkInfo.get("targetCode")
         self.objectId = linkInfo.get("objectId")
         self.shortUrl = linkInfo.get("shareURLShortCode")
         self.fullUrl = linkInfo.get("shareURLFullPath")
         self.comIdPost = linkInfo.get("ndcId")
-        self.comId = self.comIdPost or extensions.get("community") or {}.get("ndcId")
+        self.comId = self.comIdPost or community.comId
 
     @property
     def FromCode(self):
         return self
 
 class UserProfileCountList:
     __slots__ = (
```

### Comparing `amino.light.py-0.1.3/AminoLightPy/socket.py` & `amino.light.py-0.1.4/AminoLightPy/socket.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.3/AminoLightPy/sub_client.py` & `amino.light.py-0.1.4/AminoLightPy/sub_client.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.3/LICENSE` & `amino.light.py-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.3/README.md` & `amino.light.py-0.1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -26,41 +26,18 @@
 
 *  ⚡ **Optimization** : Most of the code has been rewritten.
 * ⚙ **Backward compatibility** : Write code with correct syntax.
 * 🎮 **Commands support** : Go even further with new requests.
 
 <h2 align="center">Usage</h2>
 
-Install the package :
+Install the dependencies and start the coding.
 
-`pip install amino.light.py`
-
----
-
-Import the `Client` and `SubClient` objects into your bot's code, and create your own help manual :
-
-```py
-from AminoLightPy import Client, SubClient
-# Your help message
-help_message = """
-Welcome!
-This is help page.
-"""
-# Create Client object
-client = Client()
-# Login into account
-client.login("example_mail@gmail.com", "example_password")
-# And display the help !
-@client.event("on_text_message")
-def on_message(data):
-	if data.message.author.userId != client.profile.userId:  # Do not answer to myself
-		# Create SubClient object
-		sub_client = SubClient(comId=data.comId, profile=client.profile)
-		if data.message.content.startswith('/help'):
-			sub_client.send_message(chatId=data.message.chatId, message=help_message)
+```sh
+pip install amino.light.py
 ```
 
 <h2 align="center">Example</h2>
 
 Simply copy code above, and type `/help` in the chat.
 
 Also, take a look at the code for this interactive help !
@@ -70,8 +47,8 @@
 If you can't find what you're looking for or need help with this library, you can [telegram me](https://t.me/augustlight) or an Discord - *engineer48*. We will be glad to help !
 
 
 <h2 align="center">Notes</h2>
 
 * *This is not my project. Amino libraries already existed before me. I just wanted to create a simple and effective way to support bots*
 
-* *This is working only with the Python.*
+MIT
```

#### html2text {}

```diff
@@ -6,27 +6,17 @@
                    _F_e_a_t_u_r_e_s â¢ _U_s_a_g_e â¢ _E_x_a_m_p_l_e â¢ _N_o_t_e_s
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
                              ********** FFeeaattuurreess **********
 * â¡ **Optimization** : Most of the code has been rewritten. * â **Backward
 compatibility** : Write code with correct syntax. * ð® **Commands support** :
 Go even further with new requests.
                                ********** UUssaaggee **********
-Install the package : `pip install amino.light.py` --- Import the `Client` and
-`SubClient` objects into your bot's code, and create your own help manual :
-```py from AminoLightPy import Client, SubClient # Your help message
-help_message = """ Welcome! This is help page. """ # Create Client object
-client = Client() # Login into account client.login("example_mail@gmail.com",
-"example_password") # And display the help ! @client.event("on_text_message")
-def on_message(data): if data.message.author.userId != client.profile.userId: #
-Do not answer to myself # Create SubClient object sub_client = SubClient
-(comId=data.comId, profile=client.profile) if data.message.content.startswith
-('/help'): sub_client.send_message(chatId=data.message.chatId,
-message=help_message) ```
+Install the dependencies and start the coding. ```sh pip install amino.light.py
+```
                               ********** EExxaammppllee **********
 Simply copy code above, and type `/help` in the chat. Also, take a look at the
 code for this interactive help ! --- If you can't find what you're looking for
 or need help with this library, you can [telegram me](https://t.me/augustlight)
 or an Discord - *engineer48*. We will be glad to help !
                                ********** NNootteess **********
 * *This is not my project. Amino libraries already existed before me. I just
-wanted to create a simple and effective way to support bots* * *This is working
-only with the Python.*
+wanted to create a simple and effective way to support bots* MIT
```

### Comparing `amino.light.py-0.1.3/amino.light.py.egg-info/SOURCES.txt` & `amino.light.py-0.1.4/amino.light.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.1.3/setup.py` & `amino.light.py-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "augustlight",
     "aminolightpy",
     "amino.py"
 ]
 
 setup(
     name="amino.light.py",
-    version="0.1.3",
+    version="0.1.4",
     url="https://github.com/AugustLigh/AminoLightPy",
     license="MIT",
     description="Best Amino.py alternative",
     author="AugustLight",
     packages=find_packages(),
     install_requires=["requests", "websocket-client"],
     long_description=long_description,
```

