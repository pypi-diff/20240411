# Comparing `tmp/xnode-1.0.0.tar.gz` & `tmp/xnode-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnode-1.0.0.tar", last modified: Wed Apr  3 04:31:36 2024, max compression
+gzip compressed data, was "xnode-1.0.0.1.tar", last modified: Thu Apr 11 05:21:11 2024, max compression
```

## Comparing `xnode-1.0.0.tar` & `xnode-1.0.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 04:31:36.025776 xnode-1.0.0/
--rw-rw-rw-   0        0        0     1088 2024-01-30 04:45:17.000000 xnode-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       19 2024-04-02 15:59:42.000000 xnode-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2120 2024-04-03 04:31:36.023776 xnode-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1548 2024-04-02 15:44:09.000000 xnode-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 04:31:36.025776 xnode-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1016 2024-04-02 15:41:43.000000 xnode-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 04:31:36.004108 xnode-1.0.0/xnode/
--rw-rw-rw-   0        0        0       21 2024-04-02 15:38:17.000000 xnode-1.0.0/xnode/__init__.py
--rw-rw-rw-   0        0        0     5475 2024-04-03 04:29:07.000000 xnode-1.0.0/xnode/cli.py
--rw-rw-rw-   0        0        0     8156 2024-04-02 21:00:42.000000 xnode-1.0.0/xnode/files.py
-drwxrwxrwx   0        0        0        0 2024-04-03 04:31:36.021807 xnode-1.0.0/xnode/pop/
--rw-rw-rw-   0        0        0     6846 2024-01-17 23:46:57.000000 xnode-1.0.0/xnode/pop/autoctrl.py
--rw-rw-rw-   0        0        0     5172 2024-02-07 04:10:07.000000 xnode-1.0.0/xnode/pop/core.py
--rw-rw-rw-   0        0        0     4579 2024-01-30 00:49:42.000000 xnode-1.0.0/xnode/pop/ext.py
--rw-rw-rw-   0        0        0     7396 2024-02-19 04:38:47.000000 xnode-1.0.0/xnode/pop/tphg.py
--rw-rw-rw-   0        0        0     6497 2023-10-05 06:33:32.000000 xnode-1.0.0/xnode/pyboard.py
--rw-rw-rw-   0        0        0      793 2024-01-25 00:42:40.000000 xnode-1.0.0/xnode/xnode.py
-drwxrwxrwx   0        0        0        0 2024-04-03 04:31:36.022780 xnode-1.0.0/xnode.egg-info/
--rw-rw-rw-   0        0        0     2120 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       29 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 05:21:11.835149 xnode-1.0.0.1/
+-rw-rw-rw-   0        0        0     1088 2024-01-30 04:45:17.000000 xnode-1.0.0.1/LICENSE
+-rw-rw-rw-   0        0        0       19 2024-04-08 06:03:18.000000 xnode-1.0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2299 2024-04-11 05:21:11.834143 xnode-1.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1727 2024-04-08 06:00:19.000000 xnode-1.0.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 05:21:11.835149 xnode-1.0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1018 2024-04-08 05:23:52.000000 xnode-1.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:21:11.785470 xnode-1.0.0.1/xnode/
+-rw-rw-rw-   0        0        0       23 2024-04-08 05:23:46.000000 xnode-1.0.0.1/xnode/__init__.py
+-rw-rw-rw-   0        0        0     8587 2024-04-08 08:02:01.000000 xnode-1.0.0.1/xnode/cli.py
+-rw-rw-rw-   0        0        0     6621 2024-04-08 04:23:48.000000 xnode-1.0.0.1/xnode/files.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:21:11.831732 xnode-1.0.0.1/xnode/pop/
+-rw-rw-rw-   0        0        0     6846 2024-01-17 23:46:57.000000 xnode-1.0.0.1/xnode/pop/autoctrl.py
+-rw-rw-rw-   0        0        0     5172 2024-02-07 04:10:07.000000 xnode-1.0.0.1/xnode/pop/core.py
+-rw-rw-rw-   0        0        0     4579 2024-01-30 00:49:42.000000 xnode-1.0.0.1/xnode/pop/ext.py
+-rw-rw-rw-   0        0        0     7396 2024-02-19 04:38:47.000000 xnode-1.0.0.1/xnode/pop/tphg.py
+-rw-rw-rw-   0        0        0     6497 2023-10-05 06:33:32.000000 xnode-1.0.0.1/xnode/pyboard.py
+-rw-rw-rw-   0        0        0      793 2024-01-25 00:42:40.000000 xnode-1.0.0.1/xnode/xnode.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:21:11.832741 xnode-1.0.0.1/xnode.egg-info/
+-rw-rw-rw-   0        0        0     2299 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       29 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-11 05:21:11.000000 xnode-1.0.0.1/xnode.egg-info/top_level.txt
```

### Comparing `xnode-1.0.0/LICENSE` & `xnode-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0/README.md` & `xnode-1.0.0.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,71 @@
 This is a CLI management tool for MicroPython-based XNode.
 
+### Help
+```sh
+xnode
+```
+or
+```sh
+xnode --help
+```
+
 ### Find serial port
 ```sh
 xnode scan
 ```
 
-### Initialize XNode (with zigbee) file system
+### Option Rules
+- Options and values can have spaces or omit spaces.
+- Options and values can be inserted with the = character.
+
 ```sh
-xnode --sport<com_port_name> format b
+<option><value>  
+<option> <value>
+<option>=<value> 
 ```
-> com3 is the port number found by scan
 
-### Install Pop library on XNode
-- Copy all modules included in the sub-pop folder to the pop sub-folder under XNode's lib.
+### Initialize XNode file system (Only xnode type b)
+```sh
+xnode -s<com_port_name> init
+```
+or
 ```sh
-xnode --sport<com_port_name> put pop /flash/lib/pop
-xnode --sport<com_port_name> ls /flash/lib/pop
+xnode --sport<com_port_name> init
 ```
-> The Pop library (core.py, etc.) must be included in the lib folder of the current path.
+> \<com_port_name\> is the port number found by scan. 
 
-### Executes the PC's MicroPython script by sequentially passing it to the XNode
+### Check list of XNode file systems
 ```sh
-xnode --sport<com_port_name> run app.py
+xnode -s<com_port_name> ls
+xnode -s<com_port_name> ls /flash/lib/xnode/pop
 ```
-> Wait for serial output until the script finishes
 
-**Additional Options**
-   - -n: Does not wait for serial output, so it appears as if the program has terminated on the PC side.
-     - Script continues to run on XNode
-     - Used to check data output serially from XNode with other tools (PuTTY, smon, etc.)
-   - -ni (or -in): Does not display the pressed key in the terminal window (Echo off)
+### Put PC file into XNode
+```sh
+xnode -s<com_port_name> put my.py /flash/main.py
+```
+> my.py is the name of the script written on the PC, main.py is the name to be installed on XNode  
+>> Automatically runs /flash/main.py if it exists when XNode starts
 
-### Install and run the MicroPython script on XNode
+### Get XNode file to PC
 ```sh
-xnode --sport<com_port_name> put app.py main.py
-xnode --sport<com_port_name> ls
+xnode -s<com_port_name> get /flash/main.py main.py
 ```
-> app.py is the name of the script written on the PC, main.py is the name to be installed on XNode
-> Automatically runs /flash/main.py if it exists when XNode starts
 
 ### Delete XNode file
 ```sh
-xnode --sport<com_port_name> rm main.py
-xnode --sport<com_port_name> ls
-```
+xnode -s<com_port_name> rm /flash/main.py
+```
+
+### Executes the PC's MicroPython script by sequentially passing it to the XNode
+```sh
+xnode -s<com_port_name> run app.py
+```
+> Wait for serial output until the script finishes  
+>> To force quit in running state, press Ctrl+c
+
+**Additional Options**
+   - -n: Does not wait for serial output, so it appears as if the program has terminated on the PC side.
+     - Script continues to run on XNode
+     - Used to check data output serially from XNode with other tools (PuTTY, smon, etc.)
+   - -ni (or -in): Does not display the pressed key in the terminal window (Echo off)
```

### Comparing `xnode-1.0.0/setup.py` & `xnode-1.0.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name='xnode',
-    version='1.0.0',
+    version='1.0.0.1',
     description='This is a CLI management tool for MicroPython-based XNode.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='chanmin.park',
     author_email='devcamp@gmail.com',
     url='https://github.com/planxstudio/xkit',
     install_requires=['click', 'python-dotenv', 'pyserial'],
```

### Comparing `xnode-1.0.0/xnode/files.py` & `xnode-1.0.0.1/xnode/files.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,71 +33,35 @@
             if ex.args[2].decode("utf-8").find("OSError: [Errno 2] ENOENT") != -1:
                 raise RuntimeError("No such file: {0}".format(filename))
             else:
                 raise ex
         self._pyboard.exit_raw_repl()
         return binascii.unhexlify(out)
 
-    def ls(self, directory="/", long_format=True, recursive=False):
+    def ls(self, directory="/"):
         if not directory.startswith("/"):
             directory = "/" + directory
 
         command = """
-                import os\r\n
+            import os\r\n
         """
 
-        if recursive:
-            command += """
-                def listdir(directory):
-                    result = set()
-                    
-                    def _listdir(dir_or_file):
-                        try:
-                            children = os.listdir(dir_or_file)
-                        except OSError:                        
-                            os.stat(dir_or_file)
-                            result.add(dir_or_file) 
-                        else:
-                            if children:
-                                for child in children:
-                                    if dir_or_file == '/':
-                                        next = dir_or_file + child
-                                    else:
-                                        next = dir_or_file + '/' + child
-                                    
-                                    _listdir(next)
-                            else:
-                                result.add(dir_or_file)                     
+        command += """
+            def listdir(directory):
+                if directory == '/':                
+                    return sorted([directory + f for f in os.listdir(directory)])
+                else:
+                    return sorted([directory + '/' + f for f in os.listdir(directory)])\n"""
 
-                    _listdir(directory)
-                    return sorted(result)\n"""
-        else:
-            command += """
-                def listdir(directory):
-                    if directory == '/':                
-                        return sorted([directory + f for f in os.listdir(directory)])
-                    else:
-                        return sorted([directory + '/' + f for f in os.listdir(directory)])\n"""
-
-        if long_format:
-            command += """
-                r = []
-                for f in listdir('{0}'):
-                    size = os.stat(f)[6]                    
-                    r.append('{{0}} - {{1}} bytes'.format(f, size))
-                print(r)
-            """.format(
-                directory
-            )
-        else:
-            command += """
-                print(listdir('{0}'))
-            """.format(
-                directory
-            )
+        command += """
+            print(listdir('{0}'))
+        """.format(
+            directory
+        )
+            
         self._pyboard.enter_raw_repl()
         try:
             out = self._pyboard.exec_(textwrap.dedent(command))
         except PyboardError as ex:
             if ex.args[2].decode("utf-8").find("OSError: [Errno 2] ENOENT") != -1:
                 raise RuntimeError("No such directory: {0}".format(directory))
             else:
```

### Comparing `xnode-1.0.0/xnode/pop/autoctrl.py` & `xnode-1.0.0.1/xnode/pop/autoctrl.py`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0/xnode/pop/core.py` & `xnode-1.0.0.1/xnode/pop/core.py`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0/xnode/pop/ext.py` & `xnode-1.0.0.1/xnode/pop/ext.py`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0/xnode/pop/tphg.py` & `xnode-1.0.0.1/xnode/pop/tphg.py`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0/xnode/pyboard.py` & `xnode-1.0.0.1/xnode/pyboard.py`

 * *Files identical despite different names*

### Comparing `xnode-1.0.0/xnode/xnode.py` & `xnode-1.0.0.1/xnode/xnode.py`

 * *Files identical despite different names*

