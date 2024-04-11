# Comparing `tmp/PlaywrightSafeThread-0.5.3.1.tar.gz` & `tmp/PlaywrightSafeThread-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlaywrightSafeThread-0.5.3.1.tar", last modified: Wed Apr  3 10:29:20 2024, max compression
+gzip compressed data, was "PlaywrightSafeThread-0.5.4.tar", last modified: Thu Apr 11 15:21:54 2024, max compression
```

## Comparing `PlaywrightSafeThread-0.5.3.1.tar` & `PlaywrightSafeThread-0.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:29:20.074632 PlaywrightSafeThread-0.5.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-03 10:29:20.074632 PlaywrightSafeThread-0.5.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:29:20.070632 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:29:20.070632 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/browser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/browser/plawright_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)    26504 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/browser/threadsafe_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:29:20.070632 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-03 10:29:20.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 10:29:20.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:29:20.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 10:29:20.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 10:29:20.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:29:20.074632 PlaywrightSafeThread-0.5.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:21:54.792239 PlaywrightSafeThread-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-11 15:21:51.000000 PlaywrightSafeThread-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-11 15:21:54.792239 PlaywrightSafeThread-0.5.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:21:54.792239 PlaywrightSafeThread-0.5.4/PlaywrightSafeThread/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-11 15:21:51.000000 PlaywrightSafeThread-0.5.4/PlaywrightSafeThread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:21:54.792239 PlaywrightSafeThread-0.5.4/PlaywrightSafeThread/browser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:21:51.000000 PlaywrightSafeThread-0.5.4/PlaywrightSafeThread/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-11 15:21:51.000000 PlaywrightSafeThread-0.5.4/PlaywrightSafeThread/browser/plawright_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26548 2024-04-11 15:21:51.000000 PlaywrightSafeThread-0.5.4/PlaywrightSafeThread/browser/threadsafe_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:21:54.792239 PlaywrightSafeThread-0.5.4/PlaywrightSafeThread.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-11 15:21:54.000000 PlaywrightSafeThread-0.5.4/PlaywrightSafeThread.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-11 15:21:54.000000 PlaywrightSafeThread-0.5.4/PlaywrightSafeThread.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:21:54.000000 PlaywrightSafeThread-0.5.4/PlaywrightSafeThread.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 15:21:54.000000 PlaywrightSafeThread-0.5.4/PlaywrightSafeThread.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 15:21:54.000000 PlaywrightSafeThread-0.5.4/PlaywrightSafeThread.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-11 15:21:51.000000 PlaywrightSafeThread-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:21:54.792239 PlaywrightSafeThread-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-11 15:21:51.000000 PlaywrightSafeThread-0.5.4/setup.py
```

### Comparing `PlaywrightSafeThread-0.5.3.1/LICENSE` & `PlaywrightSafeThread-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PlaywrightSafeThread-0.5.3.1/PKG-INFO` & `PlaywrightSafeThread-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightSafeThread
-Version: 0.5.3.1
+Version: 0.5.4
 Summary: PlaywrightSafeThread
 Home-page: https://github.com/3mora2/PlaywrightSafeThread
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/PlaywrightSafeThread/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/browser/plawright_shim.py` & `PlaywrightSafeThread-0.5.4/PlaywrightSafeThread/browser/plawright_shim.py`

 * *Files identical despite different names*

### Comparing `PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/browser/threadsafe_browser.py` & `PlaywrightSafeThread-0.5.4/PlaywrightSafeThread/browser/threadsafe_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,17 +408,17 @@
         return self
 
     def __exit__(self, *args):
         self.stop()
 
     def check_is_install(self, browser):
         env = self.get_driver_env()
-        driver_executable = compute_driver_executable()
+        driver_executable, driver_cli = compute_driver_executable()
 
-        completed_process = subprocess.check_output(f"{driver_executable} install {browser}  --dry-run", env=env,
+        completed_process = subprocess.check_output(f"{driver_executable} {driver_cli} install {browser}  --dry-run", env=env,
                                                     **creation_flags_dict())
 
         locale_ = ":".join(next(filter(lambda x: "Install location" in x,
                                        completed_process.decode().split("\n")), "").split(":")[1:]).strip()
 
         return locale_ and os.path.exists(locale_)
 
@@ -430,17 +430,17 @@
         # NOTE: we do this to deal with pyinstaller
         if getattr(sys, "frozen", False):
             env.setdefault("PLAYWRIGHT_BROWSERS_PATH", "0")
         return env
 
     def run_playwright(self, *args: str):
         env = self.get_driver_env()
-        driver_executable = compute_driver_executable()
+        driver_executable, driver_cli = compute_driver_executable()
 
-        with subprocess.Popen([str(driver_executable), *args], env=env, stdout=subprocess.PIPE,
+        with subprocess.Popen([driver_executable, driver_cli, *args], env=env, stdout=subprocess.PIPE,
                               stderr=subprocess.STDOUT, **creation_flags_dict()) as process:
             for line in process.stdout:
                 Logger.info(line.decode('utf-8'))
 
     ####################################################################################################################
     async def first_page(self) -> "Page":
         page = self.context.pages[0] if self.context.pages else await self.context.new_page()
```

### Comparing `PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/PKG-INFO` & `PlaywrightSafeThread-0.5.4/PlaywrightSafeThread.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightSafeThread
-Version: 0.5.3.1
+Version: 0.5.4
 Summary: PlaywrightSafeThread
 Home-page: https://github.com/3mora2/PlaywrightSafeThread
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/PlaywrightSafeThread/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PlaywrightSafeThread-0.5.3.1/README.md` & `PlaywrightSafeThread-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `PlaywrightSafeThread-0.5.3.1/setup.py` & `PlaywrightSafeThread-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 long_description = open("README.md", encoding="utf-8").read()
 description = "PlaywrightSafeThread"
 
-version = "0.5.3.1"
+version = "0.5.4"
 
 setup(
     name="PlaywrightSafeThread",
     version=version,
     license="MIT License",
     author="Ammar Alkotb",
     author_email="ammar.alkotb@gmail.com",
```

