# Comparing `tmp/auto-qchem-1.3.6.tar.gz` & `tmp/auto-qchem-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/auto-qchem-1.3.6.tar", last modified: Wed Apr 10 21:56:18 2024, max compression
+gzip compressed data, was "auto-qchem-1.3.7.tar", last modified: Wed Apr 10 22:09:41 2024, max compression
```

## Comparing `auto-qchem-1.3.6.tar` & `auto-qchem-1.3.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/
--rw-r--r--   0 mac        (501) staff       (20)    35149 2022-10-06 20:25:51.000000 auto-qchem-1.3.6/LICENSE.md
--rw-r--r--   0 mac        (501) staff       (20)      306 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1452 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/auto_qchem.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      306 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/auto_qchem.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      593 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/auto_qchem.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/auto_qchem.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      221 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/auto_qchem.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       10 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/auto_qchem.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/autoqchem/
--rw-r--r--   0 mac        (501) staff       (20)        0 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    24645 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/db_functions.py
--rw-r--r--   0 mac        (501) staff       (20)     2587 2022-10-06 20:25:51.000000 auto-qchem-1.3.6/autoqchem/descriptor_functions.py
--rw-r--r--   0 mac        (501) staff       (20)      981 2022-10-06 20:25:51.000000 auto-qchem-1.3.6/autoqchem/draw_utils.py
--rw-r--r--   0 mac        (501) staff       (20)     6445 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/gaussian_input_generator.py
--rw-r--r--   0 mac        (501) staff       (20)    19324 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/gaussian_log_extractor.py
--rw-r--r--   0 mac        (501) staff       (20)     5232 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/helper_classes.py
--rw-r--r--   0 mac        (501) staff       (20)     4234 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/helper_functions.py
--rw-r--r--   0 mac        (501) staff       (20)     2700 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/molecule.py
--rw-r--r--   0 mac        (501) staff       (20)     2274 2023-05-30 22:08:50.000000 auto-qchem-1.3.6/autoqchem/openbabel_utils.py
--rw-r--r--   0 mac        (501) staff       (20)    11508 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/rdkit_utils.py
--rw-r--r--   0 mac        (501) staff       (20)    28471 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/sge_manager.py
--rw-r--r--   0 mac        (501) staff       (20)    26054 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/autoqchem/slurm_manager.py
--rw-r--r--   0 mac        (501) staff       (20)     1374 2023-08-18 17:24:25.000000 auto-qchem-1.3.6/autoqchem/test.py
--rw-r--r--   0 mac        (501) staff       (20)      211 2024-04-10 21:52:33.000000 auto-qchem-1.3.6/config.yml
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-10 21:56:18.000000 auto-qchem-1.3.6/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1089 2024-04-10 21:56:10.000000 auto-qchem-1.3.6/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-10 22:09:41.963503 auto-qchem-1.3.7/
+-rw-r--r--   0 mac        (501) staff       (20)    35149 2022-10-06 20:25:51.000000 auto-qchem-1.3.7/LICENSE.md
+-rw-r--r--   0 mac        (501) staff       (20)      306 2024-04-10 22:09:41.963341 auto-qchem-1.3.7/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1452 2024-04-10 21:52:33.000000 auto-qchem-1.3.7/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-10 22:09:41.960708 auto-qchem-1.3.7/auto_qchem.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      306 2024-04-10 22:09:41.000000 auto-qchem-1.3.7/auto_qchem.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      593 2024-04-10 22:09:41.000000 auto-qchem-1.3.7/auto_qchem.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-10 22:09:41.000000 auto-qchem-1.3.7/auto_qchem.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      221 2024-04-10 22:09:41.000000 auto-qchem-1.3.7/auto_qchem.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       10 2024-04-10 22:09:41.000000 auto-qchem-1.3.7/auto_qchem.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-10 22:09:41.963023 auto-qchem-1.3.7/autoqchem/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2024-04-10 21:52:33.000000 auto-qchem-1.3.7/autoqchem/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    24645 2024-04-10 21:52:33.000000 auto-qchem-1.3.7/autoqchem/db_functions.py
+-rw-r--r--   0 mac        (501) staff       (20)     2587 2022-10-06 20:25:51.000000 auto-qchem-1.3.7/autoqchem/descriptor_functions.py
+-rw-r--r--   0 mac        (501) staff       (20)      981 2022-10-06 20:25:51.000000 auto-qchem-1.3.7/autoqchem/draw_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)     6445 2024-04-10 21:52:33.000000 auto-qchem-1.3.7/autoqchem/gaussian_input_generator.py
+-rw-r--r--   0 mac        (501) staff       (20)    19324 2024-04-10 21:52:33.000000 auto-qchem-1.3.7/autoqchem/gaussian_log_extractor.py
+-rw-r--r--   0 mac        (501) staff       (20)     5232 2024-04-10 21:52:33.000000 auto-qchem-1.3.7/autoqchem/helper_classes.py
+-rw-r--r--   0 mac        (501) staff       (20)     5129 2024-04-10 22:09:20.000000 auto-qchem-1.3.7/autoqchem/helper_functions.py
+-rw-r--r--   0 mac        (501) staff       (20)     2700 2024-04-10 21:52:33.000000 auto-qchem-1.3.7/autoqchem/molecule.py
+-rw-r--r--   0 mac        (501) staff       (20)     2274 2023-05-30 22:08:50.000000 auto-qchem-1.3.7/autoqchem/openbabel_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)    11508 2024-04-10 21:52:33.000000 auto-qchem-1.3.7/autoqchem/rdkit_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)    28641 2024-04-10 22:09:20.000000 auto-qchem-1.3.7/autoqchem/sge_manager.py
+-rw-r--r--   0 mac        (501) staff       (20)    26054 2024-04-10 21:52:33.000000 auto-qchem-1.3.7/autoqchem/slurm_manager.py
+-rw-r--r--   0 mac        (501) staff       (20)     1374 2023-08-18 17:24:25.000000 auto-qchem-1.3.7/autoqchem/test.py
+-rw-r--r--   0 mac        (501) staff       (20)      211 2024-04-10 21:52:33.000000 auto-qchem-1.3.7/config.yml
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-10 22:09:41.963576 auto-qchem-1.3.7/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1089 2024-04-10 22:09:37.000000 auto-qchem-1.3.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `auto-qchem-1.3.6/LICENSE.md` & `auto-qchem-1.3.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/README.md` & `auto-qchem-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/auto_qchem.egg-info/SOURCES.txt` & `auto-qchem-1.3.7/auto_qchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/autoqchem/db_functions.py` & `auto-qchem-1.3.7/autoqchem/db_functions.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/autoqchem/descriptor_functions.py` & `auto-qchem-1.3.7/autoqchem/descriptor_functions.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/autoqchem/draw_utils.py` & `auto-qchem-1.3.7/autoqchem/draw_utils.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/autoqchem/gaussian_input_generator.py` & `auto-qchem-1.3.7/autoqchem/gaussian_input_generator.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/autoqchem/gaussian_log_extractor.py` & `auto-qchem-1.3.7/autoqchem/gaussian_log_extractor.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/autoqchem/helper_classes.py` & `auto-qchem-1.3.7/autoqchem/helper_classes.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/autoqchem/helper_functions.py` & `auto-qchem-1.3.7/autoqchem/helper_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -60,14 +60,42 @@
     c = fabric.Connection(host)
     c.client = client
     c.transport = client.get_transport()
 
     return c
 
 
+def ssh_connect_pem(host, user, pem_path) -> fabric.Connection:
+    """Create ssh connection using fabric and paramiko, tries rsa key in .pem file, otherwise asks for password (without DUO authentication).
+
+    :param host: remote host
+    :param user: username to authenticate on remote host
+    :param pem_path: private rsa key - full path to .pem file (optional)
+    :return: fabric.Connection
+    """
+
+    client = paramiko.SSHClient()
+    client.load_system_host_keys()
+
+    try:
+        if pem_path:
+		client.connect(host,username=user,key_filename=pem_path)
+	else:
+		client.connect(host,username=user)
+    		client.get_transport().auth_password(username=user,password=getpass.getpass(f"{user}@{host}'s password:"))
+    except paramiko.ssh_exception.SSHException:
+        pass
+
+    c = fabric.Connection(host)
+    c.client = client
+    c.transport = client.get_transport()
+
+    return c
+
+
 def cleanup_directory_files(dir_path, types=()) -> None:
     """Remove files with specific extension(s) from a directory.
 
     :param dir_path: path of the directory to cleanup
     :param types: a tuple with file extenstions that will be removed
     """
```

### Comparing `auto-qchem-1.3.6/autoqchem/molecule.py` & `auto-qchem-1.3.7/autoqchem/molecule.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/autoqchem/openbabel_utils.py` & `auto-qchem-1.3.7/autoqchem/openbabel_utils.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/autoqchem/rdkit_utils.py` & `auto-qchem-1.3.7/autoqchem/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/autoqchem/sge_manager.py` & `auto-qchem-1.3.7/autoqchem/sge_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 
 logger = logging.getLogger(__name__)
 
 
 class sge_manager(object):
     """SGE manager class."""
 
-    def __init__(self, user, host):
+    def __init__(self, user, host, pem_path=None):
         """Initialize sge manager and load the cache file.
 
         :param user: username at remote host
         :type user: str
         :param host: remote host name
         :type host: str
+        :param pem_path: private rsa key - full path to .pem file (optional)
+        :type host: str
         """
 
         # set workdir and cache file
         self.workdir = appdirs.user_data_dir(appauthor="autoqchem", appname=host.split('.')[0]) # filepath may include spaces on Mac so enclose in quotes when used
         self.cache_file = os.path.join(f"{self.workdir}", "sge_manager.pkl")
         os.makedirs(f"{self.workdir}", exist_ok=True)
 
@@ -35,14 +37,15 @@
         # load jobs under management from cache_file (suppress exceptions, no file, empty file, etc.)
         with suppress(Exception):  # TODO this isn't very safe because may ignore important exceptions
             with open(self.cache_file, 'rb') as cf:
                 self.jobs = pickle.load(cf)
 
         self.host = host
         self.user = user
+        self.pem_path = pem_path
         self.remote_dir = f"/u/scratch/{self.user[0]}/{self.user}/gaussian"
         self.connection = None
 
     def connect(self) -> None:
         """Connect to remote host."""
 
         create_new_connection = False
@@ -54,15 +57,15 @@
                 self.connection.close()
                 self.connection = None
                 create_new_connection = True
         else:
             logger.info(f"Creating connection to {self.host} as {self.user}")
             create_new_connection = True
         if create_new_connection:
-            self.connection = ssh_connect_password(self.host, self.user)    # hoffman2 requires connecting with password (no DUO)
+            self.connection = ssh_connect_pem(self.host, self.user, self.pem_path)    # hoffman2 requires connecting with password or rsa key (no DUO)
             self.connection.run(f"mkdir -p {self.remote_dir}")
             logger.info(f"Connected to {self.host} as {self.user}.")
 
     def create_jobs_for_molecule(self,
                                  molecule,
                                  workflow_type="equilibrium",
                                  theory="APFD",
```

### Comparing `auto-qchem-1.3.6/autoqchem/slurm_manager.py` & `auto-qchem-1.3.7/autoqchem/slurm_manager.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/autoqchem/test.py` & `auto-qchem-1.3.7/autoqchem/test.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.3.6/setup.py` & `auto-qchem-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='auto-qchem',
-    version='1.3.6',
+    version='1.3.7',
     packages=['autoqchem'],
     data_files=['config.yml'],
     url='https://github.com/doyle-lab-ucla/auto-qchem',
     license='GPL',
     author='Andrzej Zuranski, Benjamin Shields, Jason Wang, Winston Gee',
     description='auto-qchem',
     long_description='automated dft calculation management software',
```

