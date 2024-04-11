# Comparing `tmp/qcloud_setup-1.0.8.tar.gz` & `tmp/qcloud_setup-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcloud_setup-1.0.8.tar", last modified: Sun Aug 27 23:51:29 2023, max compression
+gzip compressed data, was "qcloud_setup-1.0.9.tar", last modified: Tue Oct 24 12:38:18 2023, max compression
```

## Comparing `qcloud_setup-1.0.8.tar` & `qcloud_setup-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-08-27 23:51:29.147787 qcloud_setup-1.0.8/
--rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:32:28.000000 qcloud_setup-1.0.8/LICENSE.txt
--rw-r-----   0 agilbert   (501) staff       (20)    18169 2023-08-27 23:51:29.147350 qcloud_setup-1.0.8/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)    17142 2023-08-27 23:50:57.000000 qcloud_setup-1.0.8/README.md
--rw-r-----   0 agilbert   (501) staff       (20)      747 2023-08-27 23:51:19.000000 qcloud_setup-1.0.8/pyproject.toml
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-08-27 23:51:29.146549 qcloud_setup-1.0.8/qcloud_setup.egg-info/
--rw-r-----   0 agilbert   (501) staff       (20)    18169 2023-08-27 23:51:29.000000 qcloud_setup-1.0.8/qcloud_setup.egg-info/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)      422 2023-08-27 23:51:29.000000 qcloud_setup-1.0.8/qcloud_setup.egg-info/SOURCES.txt
--rw-r-----   0 agilbert   (501) staff       (20)        1 2023-08-27 23:51:29.000000 qcloud_setup-1.0.8/qcloud_setup.egg-info/dependency_links.txt
--rw-r-----   0 agilbert   (501) staff       (20)       51 2023-08-27 23:51:29.000000 qcloud_setup-1.0.8/qcloud_setup.egg-info/entry_points.txt
--rw-r-----   0 agilbert   (501) staff       (20)      151 2023-08-27 23:51:29.000000 qcloud_setup-1.0.8/qcloud_setup.egg-info/requires.txt
--rw-r-----   0 agilbert   (501) staff       (20)       13 2023-08-27 23:51:29.000000 qcloud_setup-1.0.8/qcloud_setup.egg-info/top_level.txt
--rw-r-----   0 agilbert   (501) staff       (20)       38 2023-08-27 23:51:29.147847 qcloud_setup-1.0.8/setup.cfg
--rw-r-----   0 agilbert   (501) staff       (20)      914 2023-08-27 23:51:12.000000 qcloud_setup-1.0.8/setup.py
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-08-27 23:51:29.145347 qcloud_setup-1.0.8/src/
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-08-27 23:51:29.147157 qcloud_setup-1.0.8/src/qcloud_setup/
--rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-25 11:45:44.000000 qcloud_setup-1.0.8/src/qcloud_setup/__init__.py
--rw-r-----   0 agilbert   (501) staff       (20)    21623 2023-06-25 23:43:46.000000 qcloud_setup-1.0.8/src/qcloud_setup/api-gateway.yaml
--rw-r-----   0 agilbert   (501) staff       (20)     6219 2023-06-25 23:43:46.000000 qcloud_setup-1.0.8/src/qcloud_setup/cognito.yaml
--rw-r-----   0 agilbert   (501) staff       (20)     5829 2023-07-25 11:18:10.000000 qcloud_setup-1.0.8/src/qcloud_setup/iam-policy.yaml
--rwxr-x---   0 agilbert   (501) staff       (20)    60837 2023-08-08 11:52:56.000000 qcloud_setup-1.0.8/src/qcloud_setup/qcloud_admin.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-10-24 12:38:18.130819 qcloud_setup-1.0.9/
+-rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:32:28.000000 qcloud_setup-1.0.9/LICENSE.txt
+-rw-r--r--   0 agilbert   (501) staff       (20)    18455 2023-10-24 12:38:18.130472 qcloud_setup-1.0.9/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)    17142 2023-08-27 23:50:57.000000 qcloud_setup-1.0.9/README.md
+-rw-r-----   0 agilbert   (501) staff       (20)      747 2023-10-24 12:37:43.000000 qcloud_setup-1.0.9/pyproject.toml
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-10-24 12:38:18.128282 qcloud_setup-1.0.9/qcloud_setup.egg-info/
+-rw-r--r--   0 agilbert   (501) staff       (20)    18455 2023-10-24 12:38:18.000000 qcloud_setup-1.0.9/qcloud_setup.egg-info/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)      422 2023-10-24 12:38:18.000000 qcloud_setup-1.0.9/qcloud_setup.egg-info/SOURCES.txt
+-rw-r-----   0 agilbert   (501) staff       (20)        1 2023-10-24 12:38:18.000000 qcloud_setup-1.0.9/qcloud_setup.egg-info/dependency_links.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       51 2023-10-24 12:38:18.000000 qcloud_setup-1.0.9/qcloud_setup.egg-info/entry_points.txt
+-rw-r-----   0 agilbert   (501) staff       (20)      151 2023-10-24 12:38:18.000000 qcloud_setup-1.0.9/qcloud_setup.egg-info/requires.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       13 2023-10-24 12:38:18.000000 qcloud_setup-1.0.9/qcloud_setup.egg-info/top_level.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       38 2023-10-24 12:38:18.130874 qcloud_setup-1.0.9/setup.cfg
+-rw-r-----   0 agilbert   (501) staff       (20)      914 2023-10-24 12:37:57.000000 qcloud_setup-1.0.9/setup.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-10-24 12:38:18.126863 qcloud_setup-1.0.9/src/
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-10-24 12:38:18.129469 qcloud_setup-1.0.9/src/qcloud_setup/
+-rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-25 11:45:44.000000 qcloud_setup-1.0.9/src/qcloud_setup/__init__.py
+-rw-r-----   0 agilbert   (501) staff       (20)    21623 2023-06-25 23:43:46.000000 qcloud_setup-1.0.9/src/qcloud_setup/api-gateway.yaml
+-rw-r-----   0 agilbert   (501) staff       (20)     6219 2023-06-25 23:43:46.000000 qcloud_setup-1.0.9/src/qcloud_setup/cognito.yaml
+-rw-r-----   0 agilbert   (501) staff       (20)     5829 2023-07-25 11:18:10.000000 qcloud_setup-1.0.9/src/qcloud_setup/iam-policy.yaml
+-rwxr-x---   0 agilbert   (501) staff       (20)    60451 2023-10-12 04:08:36.000000 qcloud_setup-1.0.9/src/qcloud_setup/qcloud_admin.py
```

### Comparing `qcloud_setup-1.0.8/LICENSE.txt` & `qcloud_setup-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.8/PKG-INFO` & `qcloud_setup-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: qcloud_setup
-Version: 1.0.8
-Summary: Q-Cloud setup utility for cluster administrators
-Home-page: https://q-chem.com
-Author: Andrew Gilbert
-Author-email: "Q-Chem Inc." <support@q-chem.com>
-License: Confidential property of Q-Chem, Inc.
-        Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
-        All rights reserved.
-        
-        The above copyright notice is intended as a precaution against
-        inadvertent publication and does not imply publication or any
-        waiver of confidentiality. The year included in the foregoing 
-        notice is the year of creation. This software product contains
-        proprietary, confidential information and trade secrets of
-        Q-Chem, Inc. and its licensors. No use may be made of this
-        software except according to written agreement with Q-Chem, Inc.
-        
-Project-URL: Homepage, https://q-chem.com
-Keywords: qcloud,qchem,q-cloud,q-chem
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 -----------------------------------------------------------------------
 
 <h1 align="center"> Q-Cloud Administrator Documentation </h1>
 
 -----------------------------------------------------------------------
```

### Comparing `qcloud_setup-1.0.8/README.md` & `qcloud_setup-1.0.9/qcloud_setup.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1
+Name: qcloud-setup
+Version: 1.0.9
+Summary: Q-Cloud setup utility for cluster administrators
+Home-page: https://q-chem.com
+Author: Andrew Gilbert
+Author-email: "Q-Chem Inc." <support@q-chem.com>
+License: Confidential property of Q-Chem, Inc.
+        Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
+        All rights reserved.
+        
+        The above copyright notice is intended as a precaution against
+        inadvertent publication and does not imply publication or any
+        waiver of confidentiality. The year included in the foregoing 
+        notice is the year of creation. This software product contains
+        proprietary, confidential information and trade secrets of
+        Q-Chem, Inc. and its licensors. No use may be made of this
+        software except according to written agreement with Q-Chem, Inc.
+        
+Project-URL: Homepage, https://q-chem.com
+Keywords: qcloud,qchem,q-cloud,q-chem
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: boto3==1.21.33
+Requires-Dist: botocore==1.24.33
+Requires-Dist: demjson3>=3.0.6
+Requires-Dist: paramiko>=3.1.0
+Requires-Dist: pick>=2.2.0
+Requires-Dist: PyYAML>=5.3
+Requires-Dist: pyopenssl>=22.1.0
+Requires-Dist: Requests>=2.27.1
+Requires-Dist: aws-parallelcluster==3.1.5
+
 -----------------------------------------------------------------------
 
 <h1 align="center"> Q-Cloud Administrator Documentation </h1>
 
 -----------------------------------------------------------------------
```

### Comparing `qcloud_setup-1.0.8/pyproject.toml` & `qcloud_setup-1.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qcloud_setup"
-version = "1.0.8"
+version = "1.0.9"
 description = "Q-Cloud setup utility for cluster administrators" 
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["qcloud", "qchem", "q-cloud", "q-chem"] 
 authors = [
   {name = "Q-Chem Inc.", email = "support@q-chem.com" }
```

### Comparing `qcloud_setup-1.0.8/qcloud_setup.egg-info/PKG-INFO` & `qcloud_setup-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qcloud-setup
-Version: 1.0.8
+Name: qcloud_setup
+Version: 1.0.9
 Summary: Q-Cloud setup utility for cluster administrators
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -18,14 +18,23 @@
         software except according to written agreement with Q-Chem, Inc.
         
 Project-URL: Homepage, https://q-chem.com
 Keywords: qcloud,qchem,q-cloud,q-chem
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: boto3==1.21.33
+Requires-Dist: botocore==1.24.33
+Requires-Dist: demjson3>=3.0.6
+Requires-Dist: paramiko>=3.1.0
+Requires-Dist: pick>=2.2.0
+Requires-Dist: PyYAML>=5.3
+Requires-Dist: pyopenssl>=22.1.0
+Requires-Dist: Requests>=2.27.1
+Requires-Dist: aws-parallelcluster==3.1.5
 
 -----------------------------------------------------------------------
 
 <h1 align="center"> Q-Cloud Administrator Documentation </h1>
 
 -----------------------------------------------------------------------
```

### Comparing `qcloud_setup-1.0.8/setup.py` & `qcloud_setup-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="qcloud_setup",
     python_requires='>=3.7',
-    version="1.0.8",
+    version="1.0.9",
     url="https://q-chem.com",
     author="Andrew Gilbert",
     author_email="support@q-chem.com",
     description="Utility for setting up Q-Cloud administrators",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(where="src"),
```

### Comparing `qcloud_setup-1.0.8/src/qcloud_setup/api-gateway.yaml` & `qcloud_setup-1.0.9/src/qcloud_setup/api-gateway.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.8/src/qcloud_setup/cognito.yaml` & `qcloud_setup-1.0.9/src/qcloud_setup/cognito.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.8/src/qcloud_setup/iam-policy.yaml` & `qcloud_setup-1.0.9/src/qcloud_setup/iam-policy.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.8/src/qcloud_setup/qcloud_admin.py` & `qcloud_setup-1.0.9/src/qcloud_setup/qcloud_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,32 +100,14 @@
     response = client.delete_snapshot(
        SnapshotId=snapshot_id
     )   
     checklist("Cleaning up temporary installation files","COMPLETE",True)
 
 
 
-def get_snapshot_id(region):
-    snapshots = { 
-       "us-east-1" : "snap-07e1149ce851713a8",
-    }
-
-    if "QCLOUD_SNAPSHOT_ID" in os.environ:
-       id = os.getenv('QCLOUD_SNAPSHOT_ID')
-
-    elif region in snapshots:
-       id = snapshots[region] 
-
-    else:
-       raise QCloudError("Failed to determine snapshot id for region {}".format(region))
-
-    return id
-
-
-
 class MyParser(argparse.ArgumentParser):
     def error(self, message):
         sys.stderr.write('error: %s\n' % message)
         self.print_help()
         sys.exit(2)
 
 
@@ -267,16 +249,16 @@
 
        session = boto3.Session(
           aws_access_key_id = access_key, 
           aws_secret_access_key = secret_key,
           region_name = region )
 
        os.environ["AWS_DEFAULT_REGION"] = region
-       #os.environ["AWS_ACCESS_KEY_ID"] = access_key
-       #os.environ["AWS_SECRET_ACCESS_KEY"] = secret_key
+       os.environ["AWS_ACCESS_KEY_ID"] = access_key
+       os.environ["AWS_SECRET_ACCESS_KEY"] = secret_key
 
     except (botocore.exceptions.ClientError,
             botocore.exceptions.NoCredentialsError):
        raise QCloudError(mesg)
 
     return session
     
@@ -735,15 +717,14 @@
              }
     scheduling = {'Scheduler': 'slurm' }
     scheduling['SlurmSettings'] = { 'ScaledownIdletime': 5 }
     scheduling['SlurmQueues'] = [ queue ]
     config.set('Scheduling', scheduling)
 
     # SharedStorage
-    #snapshot_id = get_snapshot_id(session.region_name)
     qcloud = {'EbsSettings': { 'Size': 5, 'SnapshotId': 'SNAPSHOT_ID', 
               'Encrypted': False,
               'VolumeType': 'gp2'}, 
               'MountDir': '/mnt/qcloud',
               'Name': 'qcloud-ebs',
               'StorageType': 'Ebs' }
 
@@ -1511,15 +1492,15 @@
        raise QCloudError("Could not obtain ssh key")
     if (not public_ip):
        raise QCloudError("Could not obtain public IP address of head node")
 
     if not os.path.exists(key_name):
        path = Path(Path.home(), '.ssh', key_name)
        if not path.exists():
-          raise QCloudError("Could not obtain key file")
+          raise QCloudError("Could not find key file {}".key_name)
        key_name = path
 
     key = paramiko.RSAKey.from_private_key_file(key_name)
     ssh_client = paramiko.SSHClient()
     ssh_client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
     ssh_client.connect(hostname=public_ip, username='ec2-user', pkey=key)
     checklist("Connection established", "", True)
@@ -1866,18 +1847,20 @@
 
         elif args.list:
             list_stacks(session)
 
         elif args.debug:
             debug_api(session, name)
 
+        elif args.config:
+            pass
+
         else:
            print("ERROR: Invalid option specified")
            parser.print_help(sys.stderr)
-            
 
 
     except KeyboardInterrupt:
         print("\n")
         pass
 
     except QCloudError as e:
```

