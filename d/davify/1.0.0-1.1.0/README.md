# Comparing `tmp/davify-1.0.0.tar.gz` & `tmp/davify-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davify-1.0.0.tar", max compression
+gzip compressed data, was "davify-1.1.0.tar", max compression
```

## Comparing `davify-1.0.0.tar` & `davify-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    35122 2021-02-19 06:41:32.248090 davify-1.0.0/LICENSE
--rw-r--r--   0        0        0      852 2024-04-05 08:32:13.639368 davify-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-02-19 06:41:32.248090 davify-1.0.0/src/davify/__init__.py
--rw-r--r--   0        0        0     1922 2024-04-05 08:32:24.091359 davify-1.0.0/src/davify/clean_directory.py
--rwxr-xr-x   0        0        0     9226 2024-04-05 08:39:50.554710 davify-1.0.0/src/davify/cli.py
--rw-r--r--   0        0        0      838 2024-04-05 08:32:24.051359 davify-1.0.0/src/davify/config.py
--rw-r--r--   0        0        0     1673 2024-04-05 08:32:24.083359 davify-1.0.0/src/davify/keyring.py
--rw-r--r--   0        0        0     2954 2024-04-05 08:32:24.135358 davify-1.0.0/src/davify/transform.py
--rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 davify-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35122 2021-02-19 06:41:32.248090 davify-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2748 2024-04-11 05:32:53.538977 davify-1.1.0/README.md
+-rw-r--r--   0        0        0      896 2024-04-11 06:31:01.806561 davify-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-02-19 06:41:32.248090 davify-1.1.0/src/davify/__init__.py
+-rwxr-xr-x   0        0        0     9355 2024-04-11 06:35:33.101893 davify-1.1.0/src/davify/cli.py
+-rw-r--r--   0        0        0      838 2024-04-11 05:32:53.542978 davify-1.1.0/src/davify/config.py
+-rw-r--r--   0        0        0     1885 2024-04-11 06:32:39.654287 davify-1.1.0/src/davify/housekeeping.py
+-rw-r--r--   0        0        0     1671 2024-04-11 06:22:48.338681 davify-1.1.0/src/davify/keyring.py
+-rw-r--r--   0        0        0     2953 2024-04-11 06:21:17.358621 davify-1.1.0/src/davify/transform.py
+-rw-r--r--   0        0        0      552 2024-04-11 05:51:39.133037 davify-1.1.0/src/davify/upload.py
+-rw-r--r--   0        0        0     3508 1970-01-01 00:00:00.000000 davify-1.1.0/PKG-INFO
```

### Comparing `davify-1.0.0/LICENSE` & `davify-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `davify-1.0.0/pyproject.toml` & `davify-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "davify"
-version = "1.0.0"
+version = "1.1.0"
 description = "Davify uploads files to webdav servers and provides a download link for accessing them."
 keywords = ["webdav"]
 authors = ["Albert Weichselbraun <albert@weichselbraun.net>"]
 license = "GPL3"
 homepage = "https://github.com/AlbertWeichselbraun/davify"
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8 || ^3.9 || ^3.10 || ^3.11 || ^3.12"
-easywebdav = "^1.2.0"
 secretstorage = "^3.3.3"
 pyperclip = "^1.8.2"
 
+
 [tool.poetry.scripts]
-davify = "davify.cli.davify:cli"
+davify = "davify.cli:cli"
+clean-davify-directory = "davify.housekeeping:cli"
 
 [tool.poetry.extras]
 # add extra dependencies here if needed
 # code formatting with black
 
 [tool.black]
 line-length = 88
```

### Comparing `davify-1.0.0/src/davify/clean_directory.py` & `davify-1.1.0/src/davify/housekeeping.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python
 """
 removes outdated files from the given directory
 """
 
 from argparse import ArgumentParser
+from datetime import timedelta
+from glob import glob
 from os import remove
 from os.path import getmtime, basename
-from time import time
-from glob import glob
 from re import compile
-from datetime import timedelta
+from time import time
 
-from davify.transform import CHR_TO_TIME
 from davify.config import EXTRACT_LIFETIME_STR
+from davify.transform import CHR_TO_TIME
 
 
 def clean_directory(location):
     """
-    ::param location:
-        location to clean
+    :param location: location to clean
     """
     for fname in glob("{0}/*".format(location)):
         file_age_in_hours = timedelta(seconds=time() - getmtime(fname))
         file_max_age = get_max_file_age(fname)
 
         # only remove the file, if file_max_age > file_age and
         # file_max_age != 0 or None
@@ -40,32 +39,32 @@
         lifetime_str = m.group(1)
         assert len(lifetime_str) == 1
         return CHR_TO_TIME[lifetime_str]
 
     return None
 
 
+def cli():
+    """Cleans the given directory."""
+    parser = ArgumentParser()
+    parser.add_argument("directory", help="The directory to clean.")
+    args = parser.parse_args()
+    clean_directory(args.directory)
+
+
 # -----------------------------------------------------------
 # - Unit tests
 # -----------------------------------------------------------
 
 
 def test_max_file_age():
     from datetime import timedelta
 
     fname = "EIcLm-buchungen-fernw%C3%A4rme-23dez-0657.pdf"
     assert get_max_file_age(fname) == timedelta(weeks=1)
 
 
-def parse_arguments():
-    """prepares the argument parser"""
-    parser = ArgumentParser()
-    parser.add_argument("fname", help="The directory to clean.")
-    return parser.parse_args()
-
-
 # -----------------------------------------------------------------------------
-# The main program
+# Main program
 # -----------------------------------------------------------------------------
 if __name__ == "__main__":
-    args = parse_arguments()
-    clean_directory(args.fname)
+    cli()
```

### Comparing `davify-1.0.0/src/davify/cli.py` & `davify-1.1.0/src/davify/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,54 +3,57 @@
 """
 davify - uploads files to a webdav server for retrieval via https
 
    .. moduleauthor:: Albert Weichselbraun albert.weichselbraun@fhgr.ch
 
 """
 
+import sys
+import tarfile
 from argparse import ArgumentParser
-from time import strftime
-from os.path import splitext, basename, join as os_join, isdir
-from os import getenv
-from tempfile import TemporaryDirectory
 from glob import glob
-from typing import List
-from urllib.parse import quote
+from hashlib import sha3_224, sha1
+from os import getenv
+from os.path import splitext, basename, join as os_join, isdir
 from random import choice
-from string import ascii_lowercase, ascii_uppercase, digits
 from shutil import which
+from string import ascii_lowercase, ascii_uppercase, digits
+from tempfile import TemporaryDirectory
+from time import strftime
+from typing import List, Dict
+from urllib.parse import quote, urljoin
 from warnings import warn
-from hashlib import sha3_224, sha1
 
-import sys
-import tarfile
-import easywebdav
 import pyperclip
 
+from davify.config import FILENAME_PATTERN, FILE_URL_PATTERN, HASH_PATTERN, MESSAGE
 from davify.keyring import get_passwords, store_password
 from davify.transform import TIME_TO_CHR, VALID_LIFE_TIMES
-from davify.config import FILENAME_PATTERN, FILE_URL_PATTERN, HASH_PATTERN, MESSAGE
+from davify.upload import upload_to_webdav
 
 APPLICATION_NAME = "davify"
 TAR_FILE_MODE = "w:xz"
 TAR_FILE_EXT = ".txz"
 INT_TO_CHR = ascii_lowercase + ascii_uppercase + digits + "_-"
 
 
-def get_version_suffix():
-    """Returns a version suffix based on the current time and date."""
+def get_version_suffix() -> str:
+    """
+    :returns: A version suffix based on the current time and date."""
     return strftime("-%d%b-%I%M%p").lower()
 
 
-def get_file_name_dict(fname, file_lifetime, version_suffix=""):
+def get_file_name_dict(
+    fname: str, file_lifetime: str, version_suffix: str = ""
+) -> Dict:
     """
     :param fname: name of the file to davify
     :param file_lifetime: suggested file lifetime in accordance to \
                the available VALID_LIFE_TIMES.
-    :param fname_suffix: optional version_suffix
+    :param version_suffix: a suffix that indicates the file version.
 
     :returns: a filename which follows the following pattern \
           rrrrt-fname-suffix.ext
 
         rrrr   ... random prefix
         t      ... lifetime
         fname  ... filename (without extension)
@@ -66,38 +69,40 @@
         "fname": fname,
         "fname_quoted": quote(fname),
         "version_suffix": version_suffix,
         "ext": ext,
     }
 
 
-def upload(local_fname, lifetime, webdav_file_pattern, file_url_pattern):
+def upload(
+    local_path: str, lifetime: str, webdav_file_pattern: str, file_url_pattern: str
+) -> Dict:
     """Uploads the given file to the webdav server :)
 
-    :param local_fname: file name of the local file
+    :param local_path: file name of the local file
     :param lifetime: suggested lifetime of the uploaded file
     """
     file_storage = get_passwords()[0]
-    webdav = easywebdav.connect(
-        file_storage.server,
-        username=file_storage.username,
-        password=file_storage.password,
-        protocol=file_storage.protocol,
-    )
-    file_url_dict = get_file_name_dict(local_fname, lifetime, get_version_suffix())
+    file_url_dict = get_file_name_dict(local_path, lifetime, get_version_suffix())
     file_url_dict["protocol"] = file_storage.protocol
     file_url_dict["file_server"] = file_storage.server
     file_url_dict["file_path"] = file_storage.path
     file_url_dict["lifetime"] = lifetime
     file_url_dict["url"] = file_url_pattern.format(**file_url_dict)
 
-    remote_fname = os_join(
-        file_storage.path, quote(webdav_file_pattern.format(**file_url_dict))
+    url = urljoin(
+        f"{file_storage.protocol}://{file_storage.server}",
+        file_storage.path.rstrip("/")
+        + "/"
+        + quote(webdav_file_pattern.format(**file_url_dict)),
     )
-    webdav.upload(local_fname, remote_fname)
+    with open(local_path, "rb") as f:
+        data = f.read()
+        upload_to_webdav(data, url, file_storage.username, file_storage.password)
+
     return file_url_dict
 
 
 def print_notification_message(notification_message, file_url_dict):
     """
     Prints the notification message based on the file_url_dict and
     copies the url to the clipboard.
@@ -109,19 +114,19 @@
     print(msg)
 
     # and send it to the clipboard :)
     pyperclip.copy(msg)
 
 
 def setup_webdav_server(
-    default_protocol:str ="https",
-    default_server:str ="localhost",
-    default_port:int =443,
-    default_path: str="/",
-    default_username: str=getenv("USER"),
+    default_protocol: str = "https",
+    default_server: str = "localhost",
+    default_port: int = 443,
+    default_path: str = "/",
+    default_username: str = getenv("USER"),
 ) -> None:
     """
     Setup the webdav server authentification data.
     """
     from getpass import getpass
 
     print("Setup WebDAV server connection.")
@@ -133,15 +138,15 @@
     username = (
         input(f"WebDAV server username ({default_username}): ") or default_username
     )
     password = getpass("WebDAV server password: ")
     store_password(username, password, protocol, server, port, path)
 
 
-def archive_files(archive_name:str , file_pattern_list: List[str]):
+def archive_files(archive_name: str, file_pattern_list: List[str]):
     """
     Stores all files listed in file_pattern_list in the archive with
     name archive_name.
 
     :param archive_name: the name of the archive to create
     :param file_pattern_list: a list of file pattern to archive
     """
@@ -152,26 +157,25 @@
                 tar.add(fname, recursive=True)
 
 
 def get_archive_name(filename: str) -> str:
     """
     Computes the archive name based on the given filename.
 
-    :param directory: directory of the archive file
     :param filename: filename of the input file used to compute \
         the archive name
     """
-    filename = filename[:-1] if filename.endswith("/") else filename
+    filename = filename.rstrip("/")
     # base result on the first filename matching pattern; this also prevents
     # wildcards in filenames :)
     archive_name = basename(glob(filename)[0])
     return archive_name
 
 
-def parse_arguments() -> None:
+def parse_arguments():
     """prepares the argument parser"""
     parser = ArgumentParser()
     parser.add_argument("fname", help="File(s) to davify.", nargs="*", default=None)
     parser.add_argument(
         "--lifetime",
         help="Suggested file lifetime (default: '1 week'). "
         "'forever' suggests that the file is never "
@@ -243,32 +247,35 @@
                 webdav_file_pattern=FILENAME_PATTERN,
                 file_url_pattern=FILE_URL_PATTERN,
             )
         else:
             with TemporaryDirectory() as tempdirname:
                 filename = os_join(
                     tempdirname,
-                    args.archive_name
-                    if args.archive_name
-                    else get_archive_name(args.fname[0]) + TAR_FILE_EXT,
+                    (
+                        args.archive_name
+                        if args.archive_name
+                        else get_archive_name(args.fname[0]) + TAR_FILE_EXT
+                    ),
                 )
                 archive_files(filename, args.fname)
                 file_url_dict = upload(
                     filename,
                     args.lifetime,
                     webdav_file_pattern=FILENAME_PATTERN,
                     file_url_pattern=FILE_URL_PATTERN,
                 )
 
         if args.hash:
-            sha1 = sha1(open(filename, "rb").read()).hexdigest()
-            sha3 = sha3_224(open(filename, "rb").read()).hexdigest()
-            file_url_dict["hash"] = HASH_PATTERN.format(sha1=sha1, sha3=sha3)
+            sha1_hash = sha1(open(filename, "rb").read()).hexdigest()
+            sha3_hash = sha3_224(open(filename, "rb").read()).hexdigest()
+            file_url_dict["hash"] = HASH_PATTERN.format(sha1=sha1_hash, sha3=sha3_hash)
         else:
             file_url_dict["hash"] = ""
 
         print_notification_message(
             notification_message=MESSAGE, file_url_dict=file_url_dict
         )
 
+
 if __name__ == "__main__":
     cli()
```

### Comparing `davify-1.0.0/src/davify/config.py` & `davify-1.1.0/src/davify/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from configparser import ConfigParser
 
 from os.path import expanduser
 
 CONFIG = ConfigParser()
 CONFIG.read(expanduser("~/.davify"))
 
-_g = (
-    lambda option, default: CONFIG.get(section="default", option=option)
+_g = lambda option, default: (
+    CONFIG.get(section="default", option=option)
     if CONFIG.has_option(section="default", option=option)
     else default
 )
 
 FILENAME_PATTERN = _g(
     "filename_pattern", "{random_prefix}{lifetime_str}-{fname}{version_suffix}{ext}"
 )
```

### Comparing `davify-1.0.0/src/davify/keyring.py` & `davify-1.1.0/src/davify/keyring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 """
-Handles access to the WebDAV's server creditentials.
+Handles access to the WebDAV's server credentials.
 """
 
 from collections import namedtuple
 
 import secretstorage
 
 APPLICATION_NAME = "davify"
```

### Comparing `davify-1.0.0/src/davify/transform.py` & `davify-1.1.0/src/davify/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python
 
 """
 standard file name and data type transformations
 """
 
-from os.path import dirname, basename, join as os_join
-from datetime import timedelta
 from collections import OrderedDict
-
+from datetime import timedelta
+from os.path import dirname, basename, join as os_join
 
 #
 # static list of VALID_LIFE_TIMES and the corresponding
 # mapping to one letter codes
 #
 VALID_LIFE_TIMES = OrderedDict(
     [
```

