# Comparing `tmp/ikctl-0.1.7.tar.gz` & `tmp/ikctl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikctl-0.1.7.tar", last modified: Sun Mar 24 12:41:27 2024, max compression
+gzip compressed data, was "ikctl-0.1.9.tar", last modified: Thu Apr 11 15:10:41 2024, max compression
```

## Comparing `ikctl-0.1.7.tar` & `ikctl-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 dml       (1000) dml       (1000)        0 2024-03-24 12:41:27.762476 ikctl-0.1.7/
--rw-rw-r--   0 dml       (1000) dml       (1000)    11357 2023-10-03 19:19:30.000000 ikctl-0.1.7/LICENSE
--rw-r--r--   0 dml       (1000) dml       (1000)     2414 2024-03-24 12:41:27.762476 ikctl-0.1.7/PKG-INFO
--rw-rw-r--   0 dml       (1000) dml       (1000)     2033 2024-03-24 12:40:50.000000 ikctl-0.1.7/README.md
-drwxrwxr-x   0 dml       (1000) dml       (1000)        0 2024-03-24 12:41:27.758476 ikctl-0.1.7/ikctl/
--rw-rw-r--   0 dml       (1000) dml       (1000)       30 2024-03-24 12:13:52.000000 ikctl-0.1.7/ikctl/__init__.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     1045 2024-01-06 12:03:18.000000 ikctl-0.1.7/ikctl/commands.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     4075 2024-03-23 18:29:12.000000 ikctl-0.1.7/ikctl/config.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     1583 2024-01-06 10:57:54.000000 ikctl-0.1.7/ikctl/connect.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     1282 2023-10-19 21:13:41.000000 ikctl-0.1.7/ikctl/context.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     1408 2024-03-24 10:59:09.000000 ikctl-0.1.7/ikctl/create_config_files.py
--rw-rw-r--   0 dml       (1000) dml       (1000)      971 2023-11-03 22:06:00.000000 ikctl-0.1.7/ikctl/execute.py
--rw-rw-r--   0 dml       (1000) dml       (1000)      327 2023-10-03 19:22:08.000000 ikctl-0.1.7/ikctl/logs.py
--rwxrwxr-x   0 dml       (1000) dml       (1000)      794 2024-03-24 12:21:33.000000 ikctl-0.1.7/ikctl/main.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     3023 2024-01-06 11:57:59.000000 ikctl-0.1.7/ikctl/pipeline.py
--rw-rw-r--   0 dml       (1000) dml       (1000)      927 2024-01-06 11:24:38.000000 ikctl-0.1.7/ikctl/sftp.py
--rw-rw-r--   0 dml       (1000) dml       (1000)     1044 2024-01-06 11:47:49.000000 ikctl-0.1.7/ikctl/view.py
-drwxrwxr-x   0 dml       (1000) dml       (1000)        0 2024-03-24 12:41:27.762476 ikctl-0.1.7/ikctl.egg-info/
--rw-r--r--   0 dml       (1000) dml       (1000)     2414 2024-03-24 12:41:27.000000 ikctl-0.1.7/ikctl.egg-info/PKG-INFO
--rw-rw-r--   0 dml       (1000) dml       (1000)      408 2024-03-24 12:41:27.000000 ikctl-0.1.7/ikctl.egg-info/SOURCES.txt
--rw-rw-r--   0 dml       (1000) dml       (1000)        1 2024-03-24 12:41:27.000000 ikctl-0.1.7/ikctl.egg-info/dependency_links.txt
--rw-rw-r--   0 dml       (1000) dml       (1000)       51 2024-03-24 12:41:27.000000 ikctl-0.1.7/ikctl.egg-info/entry_points.txt
--rw-rw-r--   0 dml       (1000) dml       (1000)       23 2024-03-24 12:41:27.000000 ikctl-0.1.7/ikctl.egg-info/requires.txt
--rw-rw-r--   0 dml       (1000) dml       (1000)        6 2024-03-24 12:41:27.000000 ikctl-0.1.7/ikctl.egg-info/top_level.txt
--rw-rw-r--   0 dml       (1000) dml       (1000)       38 2024-03-24 12:41:27.762476 ikctl-0.1.7/setup.cfg
--rw-rw-r--   0 dml       (1000) dml       (1000)      735 2024-03-24 12:41:09.000000 ikctl-0.1.7/setup.py
+drwxrwxr-x   0 dml       (1000) dml       (1000)        0 2024-04-11 15:10:41.798424 ikctl-0.1.9/
+-rw-rw-r--   0 dml       (1000) dml       (1000)    11357 2023-10-03 19:19:30.000000 ikctl-0.1.9/LICENSE
+-rw-r--r--   0 dml       (1000) dml       (1000)     2414 2024-04-11 15:10:41.798424 ikctl-0.1.9/PKG-INFO
+-rw-rw-r--   0 dml       (1000) dml       (1000)     2033 2024-03-24 12:40:50.000000 ikctl-0.1.9/README.md
+drwxrwxr-x   0 dml       (1000) dml       (1000)        0 2024-04-11 15:10:41.794424 ikctl-0.1.9/ikctl/
+-rw-rw-r--   0 dml       (1000) dml       (1000)       30 2024-03-24 12:13:52.000000 ikctl-0.1.9/ikctl/__init__.py
+-rw-rw-r--   0 dml       (1000) dml       (1000)     1049 2024-04-11 10:24:08.000000 ikctl-0.1.9/ikctl/commands.py
+-rw-rw-r--   0 dml       (1000) dml       (1000)     4078 2024-04-11 15:07:31.000000 ikctl-0.1.9/ikctl/config.py
+-rw-rw-r--   0 dml       (1000) dml       (1000)     1607 2024-04-11 12:11:52.000000 ikctl-0.1.9/ikctl/connect.py
+-rw-rw-r--   0 dml       (1000) dml       (1000)     1282 2023-10-19 21:13:41.000000 ikctl-0.1.9/ikctl/context.py
+-rw-rw-r--   0 dml       (1000) dml       (1000)     1408 2024-03-24 10:59:09.000000 ikctl-0.1.9/ikctl/create_config_files.py
+-rw-rw-r--   0 dml       (1000) dml       (1000)      970 2024-04-11 09:58:32.000000 ikctl-0.1.9/ikctl/execute.py
+-rw-rw-r--   0 dml       (1000) dml       (1000)      327 2023-10-03 19:22:08.000000 ikctl-0.1.9/ikctl/logs.py
+-rwxrwxr-x   0 dml       (1000) dml       (1000)      794 2024-04-11 09:56:10.000000 ikctl-0.1.9/ikctl/main.py
+-rw-rw-r--   0 dml       (1000) dml       (1000)     2943 2024-04-11 14:46:17.000000 ikctl-0.1.9/ikctl/pipeline.py
+-rw-rw-r--   0 dml       (1000) dml       (1000)      927 2024-01-06 11:24:38.000000 ikctl-0.1.9/ikctl/sftp.py
+-rw-rw-r--   0 dml       (1000) dml       (1000)     1044 2024-01-06 11:47:49.000000 ikctl-0.1.9/ikctl/view.py
+drwxrwxr-x   0 dml       (1000) dml       (1000)        0 2024-04-11 15:10:41.798424 ikctl-0.1.9/ikctl.egg-info/
+-rw-r--r--   0 dml       (1000) dml       (1000)     2414 2024-04-11 15:10:41.000000 ikctl-0.1.9/ikctl.egg-info/PKG-INFO
+-rw-rw-r--   0 dml       (1000) dml       (1000)      408 2024-04-11 15:10:41.000000 ikctl-0.1.9/ikctl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dml       (1000) dml       (1000)        1 2024-04-11 15:10:41.000000 ikctl-0.1.9/ikctl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dml       (1000) dml       (1000)       51 2024-04-11 15:10:41.000000 ikctl-0.1.9/ikctl.egg-info/entry_points.txt
+-rw-rw-r--   0 dml       (1000) dml       (1000)       23 2024-04-11 15:10:41.000000 ikctl-0.1.9/ikctl.egg-info/requires.txt
+-rw-rw-r--   0 dml       (1000) dml       (1000)        6 2024-04-11 15:10:41.000000 ikctl-0.1.9/ikctl.egg-info/top_level.txt
+-rw-rw-r--   0 dml       (1000) dml       (1000)       38 2024-04-11 15:10:41.798424 ikctl-0.1.9/setup.cfg
+-rw-rw-r--   0 dml       (1000) dml       (1000)      735 2024-04-11 15:07:46.000000 ikctl-0.1.9/setup.py
```

### Comparing `ikctl-0.1.7/LICENSE` & `ikctl-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.7/PKG-INFO` & `ikctl-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikctl
-Version: 0.1.7
+Version: 0.1.9
 Summary: App to installer packages on remote servers
 Home-page: https://github.com/3nueves/ikctl
 Author: David Moya López
 Author-email: 3nueves@gmail.com
 License: Apache v2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ikctl-0.1.7/README.md` & `ikctl-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.7/ikctl/commands.py` & `ikctl-0.1.9/ikctl/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """ execute script bash in remote server """
 
         try:
             self.logger.info(re.sub("echo (.*) \|","echo ************ |",f'EXEC: {self.command}\n'))
             stdin, stdout, stderr = self.client.exec_command(self.command)
             for l in stdout :
                 print(f"{l.strip()}")
-            for l in stderr:
-                print(f"stderr: {l.strip()}")
+            # for l in stderr:
+            #     print(f"stderr: {l.strip()}")
             self.check = stdout.channel.recv_exit_status()
 
             return self.check, None, None
 
         except paramiko.SSHException as e:
             self.logger.error(e)
```

### Comparing `ikctl-0.1.7/ikctl/config.py` & `ikctl-0.1.9/ikctl/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         """ Extract values from config file """
         hosts = []
 
         for m in config["servers"]:
             if group == m["name"]:
                 user     = m.get("user", "kub")
                 port     = m.get("port", 22)
-                password = m.get("password", "test")
+                password = m.get("password", "no_pass")
                 pkey     = m.get("pkey", None)
                 if m.get("hosts", None):
                     hosts = [host for host in m['hosts']]
             elif group is None:
                 user     = m.get("user", "kub")
                 port     = m.get("port", 22)
                 password = m.get("password", "test")
```

### Comparing `ikctl-0.1.7/ikctl/connect.py` & `ikctl-0.1.9/ikctl/connect.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,24 +29,24 @@
 
         # if not self.pkey:
         #     password = getpass("input your password: ")
 
         try:
             client = paramiko.SSHClient()
 
+            client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+
             if self.pkey:
                 private_key = paramiko.RSAKey.from_private_key_file(self.pkey)
-
-            client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-            
-            if not self.pkey:
-                client.connect(self.host, port=self.port, username=self.user, password=self.password, timeout=500)
-            else:
                 client.connect(self.host, port=self.port, username=self.user, pkey=private_key, timeout=500)
 
+            if self.password != "no_pass":
+                client.connect(self.host, port=self.port, username=self.user, password=self.password, allow_agent=False, look_for_keys=False, timeout=500)
+
+
             self.connection = client
             self.connection_sftp = client.open_sftp()
 
 
         except (paramiko.SSHException, FileNotFoundError) as e:
         # except FileNotFoundError as e:
             print()
```

### Comparing `ikctl-0.1.7/ikctl/context.py` & `ikctl-0.1.9/ikctl/context.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.7/ikctl/create_config_files.py` & `ikctl-0.1.9/ikctl/create_config_files.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.7/ikctl/execute.py` & `ikctl-0.1.9/ikctl/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from .commands import Commands
 
 class Exec:
     def __init__(self) -> None:
         pass
 
     def run(self, conn, options, commands, mode, password):
-
         if mode == "command":
             command = Commands(commands, conn.connection)
 
         elif options.sudo and options.parameter:
             command = Commands("echo "+password+" | sudo -S bash " + commands + " " + ' '.join(options.parameter), conn.connection)
             
         elif options.sudo and not options.parameter:
```

### Comparing `ikctl-0.1.7/ikctl/main.py` & `ikctl-0.1.9/ikctl/main.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.7/ikctl/pipeline.py` & `ikctl-0.1.9/ikctl/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,32 +55,32 @@
 
             # Load kit
             kits = self.data.extrac_config_kits(self.config_kits, options.install)
             if kits is None:
                 print("Kit not found")
                 sys.exit()
 
-            for host in hosts:
-                conn = Connection(user, port, host, pkey, password)
-                folder = self.sftp.list_dir(conn.connection_sftp, conn.user)
-                if ".ikctl" not in folder:
-                    self.logger.info("Create folder ikctl")
-                    self.sftp.create_folder(conn.connection_sftp)
-
-                print("###  Starting ikctl ###\n")
-
-                self.logger.info('HOST: %s\n', conn.host)
-
-                for local_kit in kits:
-                    # Destination route where we will upload the kits to the remote server
-                    remote_kit = ".ikctl/" + path.basename(local_kit)
-                    self.logger.info('UPLOAD: %s\n', remote_kit)
-                    self.sftp.upload_file(conn.connection_sftp, local_kit, remote_kit)
-                    self.kit_not_match = False
-                        
-                if ".sh" in remote_kit:
-                    check, log, err = self.exe.run(conn, options, remote_kit, "script", password)
-                    self.log.stdout(self.logger, log, err, check, level="DEBUG")
+        for host in hosts:
+            conn = Connection(user, port, host, pkey, password)
+            folder = self.sftp.list_dir(conn.connection_sftp, conn.user)
+            if ".ikctl" not in folder:
+                self.logger.info("Create folder ikctl")
+                self.sftp.create_folder(conn.connection_sftp)
+
+            print("###  Starting ikctl ###\n")
+
+            self.logger.info('HOST: %s\n', conn.host)
+
+            for local_kit in kits:
+                # Destination route where we will upload the kits to the remote server
+                remote_kit = ".ikctl/" + path.basename(local_kit)
+                self.logger.info('UPLOAD: %s\n', remote_kit)
+                self.sftp.upload_file(conn.connection_sftp, local_kit, remote_kit)
+                self.kit_not_match = False
+                    
+            if ".sh" in remote_kit:
+                check, log, err = self.exe.run(conn, options, remote_kit, "script", password)
+                self.log.stdout(self.logger, log, err, check, level="DEBUG")
 
-                self.logger.info(":END\n")
+            self.logger.info(":END\n")
 
-                conn.close_conn_sftp()
+            conn.close_conn_sftp()
```

### Comparing `ikctl-0.1.7/ikctl/sftp.py` & `ikctl-0.1.9/ikctl/sftp.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.7/ikctl/view.py` & `ikctl-0.1.9/ikctl/view.py`

 * *Files identical despite different names*

### Comparing `ikctl-0.1.7/ikctl.egg-info/PKG-INFO` & `ikctl-0.1.9/ikctl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ikctl
-Version: 0.1.7
+Version: 0.1.9
 Summary: App to installer packages on remote servers
 Home-page: https://github.com/3nueves/ikctl
 Author: David Moya López
 Author-email: 3nueves@gmail.com
 License: Apache v2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ikctl-0.1.7/setup.py` & `ikctl-0.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='ikctl',
-    version='0.1.7',
+    version='0.1.9',
     description="App to installer packages on remote servers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/3nueves/ikctl",
     author="David Moya López",
     author_email="3nueves@gmail.com",
     license="Apache v2.0",
```

