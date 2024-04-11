# Comparing `tmp/filetrack-0.0.5.tar.gz` & `tmp/filetrack-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filetrack-0.0.5.tar", last modified: Sat Apr  6 15:40:49 2024, max compression
+gzip compressed data, was "filetrack-0.0.6.tar", last modified: Wed Apr 10 12:08:37 2024, max compression
```

## Comparing `filetrack-0.0.5.tar` & `filetrack-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 15:40:49.623308 filetrack-0.0.5/
--rw-rw-rw-   0        0        0     1519 2024-04-03 13:43:42.000000 filetrack-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     4137 2024-04-06 15:40:49.622308 filetrack-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2024-04-06 12:02:19.000000 filetrack-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 15:40:49.589820 filetrack-0.0.5/filetrack/
--rw-rw-rw-   0        0        0     6446 2024-04-06 15:29:52.000000 filetrack-0.0.5/filetrack/Trackfile.py
--rw-rw-rw-   0        0        0     5243 2024-04-06 15:34:05.000000 filetrack-0.0.5/filetrack/__init__.py
--rw-rw-rw-   0        0        0       83 2024-04-03 13:43:42.000000 filetrack-0.0.5/filetrack/__main__.py
--rw-rw-rw-   0        0        0      729 2024-04-06 15:34:34.000000 filetrack-0.0.5/filetrack/command_line.py
-drwxrwxrwx   0        0        0        0 2024-04-06 15:40:49.619783 filetrack-0.0.5/filetrack.egg-info/
--rw-rw-rw-   0        0        0     4137 2024-04-06 15:40:49.000000 filetrack-0.0.5/filetrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2024-04-06 15:40:49.000000 filetrack-0.0.5/filetrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 15:40:49.000000 filetrack-0.0.5/filetrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-04-06 15:40:49.000000 filetrack-0.0.5/filetrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2024-04-06 15:40:49.000000 filetrack-0.0.5/filetrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-06 15:40:49.000000 filetrack-0.0.5/filetrack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1393 2024-04-06 07:21:50.000000 filetrack-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       14 2024-04-03 13:43:42.000000 filetrack-0.0.5/requirements-dev.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 07:21:29.000000 filetrack-0.0.5/requirements-opt.txt
--rw-rw-rw-   0        0        0       46 2024-04-06 07:21:08.000000 filetrack-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 15:40:49.624307 filetrack-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-06 15:40:49.619783 filetrack-0.0.5/tests/
--rw-rw-rw-   0        0        0     1050 2024-04-06 15:34:48.000000 filetrack-0.0.5/tests/test_command_line.py
--rw-rw-rw-   0        0        0      524 2024-04-06 15:38:46.000000 filetrack-0.0.5/tests/test_filetrack.py
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-04-10 12:08:37.207200 filetrack-0.0.6/
+-rw-r--r--   0 kyan001    (501) staff       (20)     1491 2024-03-07 11:39:07.000000 filetrack-0.0.6/LICENSE
+-rw-r--r--   0 kyan001    (501) staff       (20)     4039 2024-04-10 12:08:37.206982 filetrack-0.0.6/PKG-INFO
+-rw-r--r--   0 kyan001    (501) staff       (20)     1264 2024-04-10 11:03:45.000000 filetrack-0.0.6/README.md
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-04-10 12:08:37.205666 filetrack-0.0.6/filetrack/
+-rw-r--r--   0 kyan001    (501) staff       (20)     6403 2024-04-10 11:55:54.000000 filetrack-0.0.6/filetrack/Trackfile.py
+-rwxr-xr-x   0 kyan001    (501) staff       (20)     6212 2024-04-10 11:57:17.000000 filetrack-0.0.6/filetrack/__init__.py
+-rw-r--r--   0 kyan001    (501) staff       (20)       79 2024-03-07 11:39:07.000000 filetrack-0.0.6/filetrack/__main__.py
+-rw-r--r--   0 kyan001    (501) staff       (20)      708 2024-04-10 11:03:45.000000 filetrack-0.0.6/filetrack/command_line.py
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-04-10 12:08:37.206667 filetrack-0.0.6/filetrack.egg-info/
+-rw-r--r--   0 kyan001    (501) staff       (20)     4039 2024-04-10 12:08:37.000000 filetrack-0.0.6/filetrack.egg-info/PKG-INFO
+-rw-r--r--   0 kyan001    (501) staff       (20)      435 2024-04-10 12:08:37.000000 filetrack-0.0.6/filetrack.egg-info/SOURCES.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)        1 2024-04-10 12:08:37.000000 filetrack-0.0.6/filetrack.egg-info/dependency_links.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       58 2024-04-10 12:08:37.000000 filetrack-0.0.6/filetrack.egg-info/entry_points.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       77 2024-04-10 12:08:37.000000 filetrack-0.0.6/filetrack.egg-info/requires.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       15 2024-04-10 12:08:37.000000 filetrack-0.0.6/filetrack.egg-info/top_level.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)     1350 2024-04-10 11:03:45.000000 filetrack-0.0.6/pyproject.toml
+-rw-r--r--   0 kyan001    (501) staff       (20)       12 2024-03-07 11:39:07.000000 filetrack-0.0.6/requirements-dev.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)        8 2024-04-10 11:03:45.000000 filetrack-0.0.6/requirements-opt.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       43 2024-04-10 11:03:45.000000 filetrack-0.0.6/requirements.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       38 2024-04-10 12:08:37.207239 filetrack-0.0.6/setup.cfg
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-04-10 12:08:37.206519 filetrack-0.0.6/tests/
+-rw-r--r--   0 kyan001    (501) staff       (20)     1016 2024-04-10 11:03:45.000000 filetrack-0.0.6/tests/test_command_line.py
+-rw-r--r--   0 kyan001    (501) staff       (20)      501 2024-04-10 11:03:45.000000 filetrack-0.0.6/tests/test_filetrack.py
```

### Comparing `filetrack-0.0.5/LICENSE` & `filetrack-0.0.6/LICENSE`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2024, Kyan
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2024, Kyan
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `filetrack-0.0.5/PKG-INFO` & `filetrack-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-Metadata-Version: 2.1
-Name: filetrack
-Version: 0.0.5
-Summary: Tracking file changes according to the record file.
-Author-email: Kyan <kai@kyan001.com>
-License: BSD 3-Clause License
-        
-        Copyright (c) 2024, Kyan
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Project-URL: Homepage, https://github.com/kyan001/PyFileTrack
-Project-URL: Changelog, https://github.com/kyan001/PyFileTrack/blob/master/CHANGELOG.md
-Project-URL: Issue Tracker, https://github.com/kyan001/PyFileTrack/issues
-Project-URL: Source Code, https://github.com/kyan001/PyFileTrack
-Keywords: python3,file,track,cli
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: consoleiotools
-Requires-Dist: consolecmdtools
-Requires-Dist: fuzzyfinder
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Provides-Extra: opt
-Requires-Dist: tomlkit; extra == "opt"
-
-# FileTrack
-
-[CHANGELOG](CHANGELOG.md)
-
-[FileTrack](https://github.com/kyan001/PyFileTrack) is a filetracking cli tool that can track file changes in a certain folder.
-
-## Get Started
-
-```sh
-pip install filetrack  # Install
-
-filetrack  # Run FileTrack according filetrack.toml in current folder.
-filetrack -h/--help  # Show help message.
-filetrack -v/--version  # Show version.
-filetrack -c/--config $config_file  # Run FileTrack according to the config file.
-```
-
-## Installation
-
-```sh
-# pip
-pip install --user filetrack  # install filetrack
-pip install --upgrade filetrack # upgrade filetrack
-pip uninstall filetrack  # uninstall filetrack
-
-# pipx (recommanded)
-pipx install filetrack  # install filetrack through pipx
-pipx upgrade filetrack  # upgrade filetrack through pipx
-pipx uninstall filetrack  # uninstall filetrack through pipx
-```
-
-## Config File
-
-* Config file example: [filetrack.toml]
-
-## Knowledge Base
-
-* Trackings: File hashes to track changes.
-* TrackFile: The output file to hold file trackings.
-* TrackFile Format: Can choose from `TOML` or `JSON`
-* Target File Exts: Files that you wanna track with specific extensions. Leave it empty `[]` or `["*"]` to track all files.
-* Old TrackFile: Autodetect and parse old TrackFile to compared with.
+Metadata-Version: 2.1
+Name: filetrack
+Version: 0.0.6
+Summary: Tracking file changes according to the record file.
+Author-email: Kyan <kai@kyan001.com>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2024, Kyan
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://github.com/kyan001/PyFileTrack
+Project-URL: Changelog, https://github.com/kyan001/PyFileTrack/blob/master/CHANGELOG.md
+Project-URL: Issue Tracker, https://github.com/kyan001/PyFileTrack/issues
+Project-URL: Source Code, https://github.com/kyan001/PyFileTrack
+Keywords: python3,file,track,cli
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: consoleiotools
+Requires-Dist: consolecmdtools
+Requires-Dist: fuzzyfinder
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Provides-Extra: opt
+Requires-Dist: tomlkit; extra == "opt"
+
+# FileTrack
+
+[CHANGELOG](CHANGELOG.md)
+
+[FileTrack](https://github.com/kyan001/PyFileTrack) is a filetracking cli tool that can track file changes in a certain folder.
+
+## Get Started
+
+```sh
+pip install filetrack  # Install
+
+filetrack  # Run FileTrack according filetrack.toml in current folder.
+filetrack -h/--help  # Show help message.
+filetrack -v/--version  # Show version.
+filetrack -c/--config $config_file  # Run FileTrack according to the config file.
+```
+
+## Installation
+
+```sh
+# pip
+pip install --user filetrack  # install filetrack
+pip install --upgrade filetrack # upgrade filetrack
+pip uninstall filetrack  # uninstall filetrack
+
+# pipx (recommanded)
+pipx install filetrack  # install filetrack through pipx
+pipx upgrade filetrack  # upgrade filetrack through pipx
+pipx uninstall filetrack  # uninstall filetrack through pipx
+```
+
+## Config File
+
+* Config file example: [filetrack.toml]
+
+## Knowledge Base
+
+* Trackings: File hashes to track changes.
+* TrackFile: The output file to hold file trackings.
+* TrackFile Format: Can choose from `TOML` or `JSON`
+* Target File Exts: Files that you wanna track with specific extensions. Leave it empty `[]` or `["*"]` to track all files.
+* Old TrackFile: Autodetect and parse old TrackFile to compared with.
```

### Comparing `filetrack-0.0.5/README.md` & `filetrack-0.0.6/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# FileTrack
-
-[CHANGELOG](CHANGELOG.md)
-
-[FileTrack](https://github.com/kyan001/PyFileTrack) is a filetracking cli tool that can track file changes in a certain folder.
-
-## Get Started
-
-```sh
-pip install filetrack  # Install
-
-filetrack  # Run FileTrack according filetrack.toml in current folder.
-filetrack -h/--help  # Show help message.
-filetrack -v/--version  # Show version.
-filetrack -c/--config $config_file  # Run FileTrack according to the config file.
-```
-
-## Installation
-
-```sh
-# pip
-pip install --user filetrack  # install filetrack
-pip install --upgrade filetrack # upgrade filetrack
-pip uninstall filetrack  # uninstall filetrack
-
-# pipx (recommanded)
-pipx install filetrack  # install filetrack through pipx
-pipx upgrade filetrack  # upgrade filetrack through pipx
-pipx uninstall filetrack  # uninstall filetrack through pipx
-```
-
-## Config File
-
-* Config file example: [filetrack.toml]
-
-## Knowledge Base
-
-* Trackings: File hashes to track changes.
-* TrackFile: The output file to hold file trackings.
-* TrackFile Format: Can choose from `TOML` or `JSON`
-* Target File Exts: Files that you wanna track with specific extensions. Leave it empty `[]` or `["*"]` to track all files.
-* Old TrackFile: Autodetect and parse old TrackFile to compared with.
+# FileTrack
+
+[CHANGELOG](CHANGELOG.md)
+
+[FileTrack](https://github.com/kyan001/PyFileTrack) is a filetracking cli tool that can track file changes in a certain folder.
+
+## Get Started
+
+```sh
+pip install filetrack  # Install
+
+filetrack  # Run FileTrack according filetrack.toml in current folder.
+filetrack -h/--help  # Show help message.
+filetrack -v/--version  # Show version.
+filetrack -c/--config $config_file  # Run FileTrack according to the config file.
+```
+
+## Installation
+
+```sh
+# pip
+pip install --user filetrack  # install filetrack
+pip install --upgrade filetrack # upgrade filetrack
+pip uninstall filetrack  # uninstall filetrack
+
+# pipx (recommanded)
+pipx install filetrack  # install filetrack through pipx
+pipx upgrade filetrack  # upgrade filetrack through pipx
+pipx uninstall filetrack  # uninstall filetrack through pipx
+```
+
+## Config File
+
+* Config file example: [filetrack.toml]
+
+## Knowledge Base
+
+* Trackings: File hashes to track changes.
+* TrackFile: The output file to hold file trackings.
+* TrackFile Format: Can choose from `TOML` or `JSON`
+* Target File Exts: Files that you wanna track with specific extensions. Leave it empty `[]` or `["*"]` to track all files.
+* Old TrackFile: Autodetect and parse old TrackFile to compared with.
```

### Comparing `filetrack-0.0.5/filetrack/Trackfile.py` & `filetrack-0.0.6/filetrack/Trackfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,172 +1,171 @@
-import os
-import socket
-import pathlib
-import datetime
-
-import consoleiotools as cit
-import consolecmdtools as cct
-
-
-class Trackfile:
-    def __init__(self, trackfile_dir: str = os.getcwd(), prefix: str = "FileTrack-", format: str = "json", group_by: str = ""):
-        """Initialize Trackfile object.
-
-        Args:
-            trackfile_dir (str): The directory path of the trackfile.
-            prefix (str): The prefix of the trackfile.
-            format (str): The output format. Options: "json", "toml".
-            group_by (str): Group by. Default is "" meaning no group. Options: "host", "os", "".
-        """
-        self.prefix = prefix
-        self.trackfile_dir = trackfile_dir
-        self.format = format
-        if self.format.upper() == "TOML":
-            import tomlkit  # lazyload
-            self.suffix = ".toml"
-            self.formatter = tomlkit
-        elif self.format.upper() == "JSON":
-            import json  # lazyload
-            self.suffix = ".json"
-            self.formatter = json
-        else:
-            raise Exception(f"Output format `{self.format}` does not support")
-        self.group_by = group_by
-        self.trackings = {}
-
-    def __str__(self) -> str:
-        return self.path
-
-    @property
-    def files(self) -> list:
-        def filename_filter(path: str) -> bool:
-            filename = cct.get_path(path).basename
-            if filename.startswith(self.prefix) and filename.endswith(self.suffix):
-                if self.group_by == "host" and (self.hostname not in filename):
-                    return False
-                if self.group_by == "os" and (os.name not in filename):
-                    return False
-                return True
-            return False
-
-        trackfile_list = cct.get_paths(self.trackfile_dir, filter=filename_filter)
-        return sorted(trackfile_list)
-
-    @property
-    def latest(self) -> str:
-        print(self.files)
-        if not self.files:
-            return ""
-        return self.files[-1]
-
-    @property
-    def group(self):
-        match self.group_by:
-            case "host":
-                return self.hostname
-            case "os":
-                return os.name
-            case "":
-                return ""
-            case _:
-                cit.err(f"Unsupported group_by: {self.group_by}")
-                cit.bye()
-
-    @property
-    def filename(self):
-        now = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
-        return f"{self.prefix}{now}{'-' if self.group else ''}{self.group}{self.suffix}"
-
-    @property
-    def path(self):
-        return cct.get_path(os.path.join(self.trackfile_dir, self.filename))
-
-    def compare_with(self, trackfile: "Trackfile") -> tuple[list, list]:
-        trackings_1 = set(self.trackings.items())
-        trackings_2 = set(trackfile.trackings.items())
-        return [filename for filename, filehash in trackings_1 - trackings_2], [filename for filename, filehash in trackings_2 - trackings_1]
-
-    @property
-    def hostname(self) -> str:
-        """Get hostname and check if hostname is new."""
-        host = socket.gethostname().replace("-", "").replace(".", "")  # default hostname
-        return host
-
-    @cit.as_session("Cleanup Outdated TrackFiles")
-    def cleanup_outdated_trackfiles(self):
-        if len(self.files) > 1:
-            old_trackfiles = self.latest
-            cit.ask("Cleanup old TrackFiles?")
-            for trackfile in old_trackfiles:
-                cit.echo(cct.get_path(trackfile).basename, pre="*")
-            if cit.get_choice(["Yes", "No"]) == "Yes":
-                for filepath in old_trackfiles:
-                    os.remove(filepath)
-                cit.info("Cleanup done")
-            else:
-                cit.warn("Cleanup canceled")
-
-    @cit.as_session("Saving TrackFile")
-    def to_file(self):
-        with open(self.path, "w", encoding="UTF8") as f:
-            options = {}
-            if self.format == "JSON":
-                options = {"indent": 4, "ensure_ascii": False}
-            f.write(self.formatter.dumps(self.trackings, **options))
-            cit.info(f"New TrackFile created: [u]{self.path}[/]")
-
-    @cit.as_session("Loading Old TrackFile")
-    def from_file(self, path: str) -> bool:
-        """Parse a TrackFile and load trackings into instance.
-
-        Args:
-            path (str): Path to the TrackFile.
-
-        Returns:
-            bool: True if successful.
-        """
-        if not path:
-            return False
-        path = cct.get_path(path)
-        if not path.is_file:
-            cit.warn("No TrackFile loaded.")
-            return False
-        cit.info(f"Parsing TrackFile `{path}`")
-        with open(path, encoding="UTF8") as fl:
-            trackings = self.formatter.loads(fl.read())
-            cit.info(f"{len(trackings)} entries loaded")
-        self.trackings = trackings
-        return True
-
-    @cit.as_session("Generating New TrackFile")
-    def generate(self, target_dir: str = os.getcwd(), exts: list = [], hash_mode: str = "CRC32"):
-        """Generate file tracking information.
-
-        Args:
-            target_dir (str): Target directory to scan.
-            exts (list[str]): Accepted file extensions. Ex. ["mp3", "m4a"]. Default is [] meaning all files.
-            hash_mode (str): "CRC32", "MD5", "NAME", "PATH", "MTIME".
-
-        Returns:
-            dict: {filename: filehash}
-        """
-        paths = []
-        if not exts:
-            exts = ["*",]
-        for ext in exts:
-            target_file_pattern = f"*.{ext}"
-            cit.info(f"Target file pattern: {target_file_pattern}")
-            paths += list(pathlib.Path(target_dir).rglob(target_file_pattern))
-        for filepath in cit.track(paths, "Hashing...", unit="files"):
-            if hash_mode == "CRC32":
-                filehash = cct.crc32(filepath)
-            elif hash_mode == "MTIME":
-                filehash = int(os.path.getmtime(filepath))
-            elif hash_mode == "NAME":
-                filehash = os.path.basename(filepath)
-            elif hash_mode == "PATH":
-                filehash = filepath
-            elif hash_mode == "MD5":
-                filehash = cct.md5(filepath)
-            else:
-                filehash = None
-            self.trackings[os.path.basename(filepath)] = filehash
+import os
+import socket
+import pathlib
+import datetime
+
+import consoleiotools as cit
+import consolecmdtools as cct
+
+
+class Trackfile:
+    def __init__(self, trackfile_dir: str = os.getcwd(), prefix: str = "FileTrack-", format: str = "json", group_by: str = ""):
+        """Initialize Trackfile object.
+
+        Args:
+            trackfile_dir (str): The directory path of the trackfile.
+            prefix (str): The prefix of the trackfile.
+            format (str): The output format. Options: "json", "toml".
+            group_by (str): Group by. Default is "" meaning no group. Options: "host", "os", "".
+        """
+        self.prefix = prefix
+        self.trackfile_dir = trackfile_dir
+        self.format = format
+        if self.format.upper() == "TOML":
+            import tomlkit  # lazyload
+            self.suffix = ".toml"
+            self.formatter = tomlkit
+        elif self.format.upper() == "JSON":
+            import json  # lazyload
+            self.suffix = ".json"
+            self.formatter = json
+        else:
+            raise Exception(f"Output format `{self.format}` does not support")
+        self.group_by = group_by
+        self.trackings = {}
+
+    def __str__(self) -> str:
+        return self.path
+
+    @property
+    def files(self) -> list:
+        def filename_filter(path: str) -> bool:
+            filename = cct.get_path(path).basename
+            if filename.startswith(self.prefix) and filename.endswith(self.suffix):
+                if self.group_by == "host" and (self.hostname not in filename):
+                    return False
+                if self.group_by == "os" and (os.name not in filename):
+                    return False
+                return True
+            return False
+
+        trackfile_list = cct.get_paths(self.trackfile_dir, filter=filename_filter)
+        return sorted(trackfile_list)
+
+    @property
+    def latest(self) -> str:
+        if not self.files:
+            return ""
+        return self.files[-1]
+
+    @property
+    def group(self):
+        match self.group_by:
+            case "host":
+                return self.hostname
+            case "os":
+                return os.name
+            case "":
+                return ""
+            case _:
+                cit.err(f"Unsupported group_by: {self.group_by}")
+                cit.bye()
+
+    @property
+    def filename(self):
+        now = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
+        return f"{self.prefix}{now}{'-' if self.group else ''}{self.group}{self.suffix}"
+
+    @property
+    def path(self):
+        return cct.get_path(os.path.join(self.trackfile_dir, self.filename))
+
+    def compare_with(self, trackfile: "Trackfile") -> tuple[list, list]:
+        trackings_1 = set(self.trackings.items())
+        trackings_2 = set(trackfile.trackings.items())
+        return [filename for filename, filehash in trackings_1 - trackings_2], [filename for filename, filehash in trackings_2 - trackings_1]
+
+    @property
+    def hostname(self) -> str:
+        """Get hostname and check if hostname is new."""
+        host = socket.gethostname().replace("-", "").replace(".", "")  # default hostname
+        return host
+
+    @cit.as_session("Cleanup Outdated TrackFiles")
+    def cleanup_outdated_trackfiles(self):
+        if len(self.files) > 1:
+            old_trackfiles = self.files[:-1]  # exclude the latest one
+            cit.ask(f"Cleanup {len(old_trackfiles)} old TrackFiles?")
+            for trackfile in old_trackfiles:
+                cit.echo(cct.get_path(trackfile).basename, pre="*")
+            if cit.get_choice(["Yes", "No"]) == "Yes":
+                for filepath in old_trackfiles:
+                    os.remove(filepath)
+                cit.info("Cleanup done")
+            else:
+                cit.warn("Cleanup canceled")
+
+    @cit.as_session("Saving TrackFile")
+    def to_file(self):
+        with open(self.path, "w", encoding="UTF8") as f:
+            options = {}
+            if self.format == "JSON":
+                options = {"indent": 4, "ensure_ascii": False}
+            f.write(self.formatter.dumps(self.trackings, **options))
+            cit.info(f"New TrackFile created: [u]{self.path.basename}[/]")
+
+    @cit.as_session("Loading Old TrackFile")
+    def from_file(self, path: str) -> bool:
+        """Parse a TrackFile and load trackings into instance.
+
+        Args:
+            path (str): Path to the TrackFile.
+
+        Returns:
+            bool: True if successful.
+        """
+        if not path:
+            return False
+        path = cct.get_path(path)
+        if not path.is_file:
+            cit.warn("No TrackFile loaded.")
+            return False
+        cit.info(f"Parsing TrackFile `{path.basename}`")
+        with open(path, encoding="UTF8") as fl:
+            trackings = self.formatter.loads(fl.read())
+            cit.info(f"{len(trackings)} entries loaded")
+        self.trackings = trackings
+        return True
+
+    @cit.as_session("Generating New TrackFile")
+    def generate(self, target_dir: str = os.getcwd(), exts: list = ["*",], hash_mode: str = "CRC32"):
+        """Generate file tracking information.
+
+        Args:
+            target_dir (str): Target directory to scan.
+            exts (list[str]): Accepted file extensions. Ex. ["mp3", "m4a"]. Default is [] meaning all files.
+            hash_mode (str): "CRC32", "MD5", "NAME", "PATH", "MTIME".
+
+        Returns:
+            dict: {filename: filehash}
+        """
+        paths = []
+        for ext in exts:
+            target_file_pattern = f"*.{ext}"
+            cit.info(f"Target file pattern: {target_file_pattern}")
+            paths += list(pathlib.Path(target_dir).rglob(target_file_pattern))
+        cit.info(f"Found {len(paths)} target files")
+        if paths:
+            for filepath in cit.track(paths, "Hashing...", unit="files"):
+                if hash_mode == "CRC32":
+                    filehash = cct.crc32(filepath)
+                elif hash_mode == "MTIME":
+                    filehash = int(os.path.getmtime(filepath))
+                elif hash_mode == "NAME":
+                    filehash = os.path.basename(filepath)
+                elif hash_mode == "PATH":
+                    filehash = filepath
+                elif hash_mode == "MD5":
+                    filehash = cct.md5(filepath)
+                else:
+                    filehash = None
+                self.trackings[os.path.basename(filepath)] = filehash
```

### Comparing `filetrack-0.0.5/filetrack.egg-info/PKG-INFO` & `filetrack-0.0.6/filetrack.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-Metadata-Version: 2.1
-Name: filetrack
-Version: 0.0.5
-Summary: Tracking file changes according to the record file.
-Author-email: Kyan <kai@kyan001.com>
-License: BSD 3-Clause License
-        
-        Copyright (c) 2024, Kyan
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Project-URL: Homepage, https://github.com/kyan001/PyFileTrack
-Project-URL: Changelog, https://github.com/kyan001/PyFileTrack/blob/master/CHANGELOG.md
-Project-URL: Issue Tracker, https://github.com/kyan001/PyFileTrack/issues
-Project-URL: Source Code, https://github.com/kyan001/PyFileTrack
-Keywords: python3,file,track,cli
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: consoleiotools
-Requires-Dist: consolecmdtools
-Requires-Dist: fuzzyfinder
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Provides-Extra: opt
-Requires-Dist: tomlkit; extra == "opt"
-
-# FileTrack
-
-[CHANGELOG](CHANGELOG.md)
-
-[FileTrack](https://github.com/kyan001/PyFileTrack) is a filetracking cli tool that can track file changes in a certain folder.
-
-## Get Started
-
-```sh
-pip install filetrack  # Install
-
-filetrack  # Run FileTrack according filetrack.toml in current folder.
-filetrack -h/--help  # Show help message.
-filetrack -v/--version  # Show version.
-filetrack -c/--config $config_file  # Run FileTrack according to the config file.
-```
-
-## Installation
-
-```sh
-# pip
-pip install --user filetrack  # install filetrack
-pip install --upgrade filetrack # upgrade filetrack
-pip uninstall filetrack  # uninstall filetrack
-
-# pipx (recommanded)
-pipx install filetrack  # install filetrack through pipx
-pipx upgrade filetrack  # upgrade filetrack through pipx
-pipx uninstall filetrack  # uninstall filetrack through pipx
-```
-
-## Config File
-
-* Config file example: [filetrack.toml]
-
-## Knowledge Base
-
-* Trackings: File hashes to track changes.
-* TrackFile: The output file to hold file trackings.
-* TrackFile Format: Can choose from `TOML` or `JSON`
-* Target File Exts: Files that you wanna track with specific extensions. Leave it empty `[]` or `["*"]` to track all files.
-* Old TrackFile: Autodetect and parse old TrackFile to compared with.
+Metadata-Version: 2.1
+Name: filetrack
+Version: 0.0.6
+Summary: Tracking file changes according to the record file.
+Author-email: Kyan <kai@kyan001.com>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2024, Kyan
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://github.com/kyan001/PyFileTrack
+Project-URL: Changelog, https://github.com/kyan001/PyFileTrack/blob/master/CHANGELOG.md
+Project-URL: Issue Tracker, https://github.com/kyan001/PyFileTrack/issues
+Project-URL: Source Code, https://github.com/kyan001/PyFileTrack
+Keywords: python3,file,track,cli
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: consoleiotools
+Requires-Dist: consolecmdtools
+Requires-Dist: fuzzyfinder
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Provides-Extra: opt
+Requires-Dist: tomlkit; extra == "opt"
+
+# FileTrack
+
+[CHANGELOG](CHANGELOG.md)
+
+[FileTrack](https://github.com/kyan001/PyFileTrack) is a filetracking cli tool that can track file changes in a certain folder.
+
+## Get Started
+
+```sh
+pip install filetrack  # Install
+
+filetrack  # Run FileTrack according filetrack.toml in current folder.
+filetrack -h/--help  # Show help message.
+filetrack -v/--version  # Show version.
+filetrack -c/--config $config_file  # Run FileTrack according to the config file.
+```
+
+## Installation
+
+```sh
+# pip
+pip install --user filetrack  # install filetrack
+pip install --upgrade filetrack # upgrade filetrack
+pip uninstall filetrack  # uninstall filetrack
+
+# pipx (recommanded)
+pipx install filetrack  # install filetrack through pipx
+pipx upgrade filetrack  # upgrade filetrack through pipx
+pipx uninstall filetrack  # uninstall filetrack through pipx
+```
+
+## Config File
+
+* Config file example: [filetrack.toml]
+
+## Knowledge Base
+
+* Trackings: File hashes to track changes.
+* TrackFile: The output file to hold file trackings.
+* TrackFile Format: Can choose from `TOML` or `JSON`
+* Target File Exts: Files that you wanna track with specific extensions. Leave it empty `[]` or `["*"]` to track all files.
+* Old TrackFile: Autodetect and parse old TrackFile to compared with.
```

### Comparing `filetrack-0.0.5/pyproject.toml` & `filetrack-0.0.6/pyproject.toml`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-[build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "filetrack"
-description = "Tracking file changes according to the record file."
-requires-python = ">=3.8"
-readme = "README.md"
-keywords = ["python3", "file", "track", "cli"]
-license = {file = "LICENSE"}
-classifiers = [
-    "Intended Audience :: Developers",
-    "Intended Audience :: End Users/Desktop",
-    "License :: OSI Approved :: BSD License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-]
-dynamic = ["version", "dependencies", "optional-dependencies"]
-
-[[project.authors]]
-name = "Kyan"
-email = "kai@kyan001.com"
-
-[project.urls]
-Homepage = "https://github.com/kyan001/PyFileTrack"
-Changelog = "https://github.com/kyan001/PyFileTrack/blob/master/CHANGELOG.md"
-"Issue Tracker" = "https://github.com/kyan001/PyFileTrack/issues"
-"Source Code" = "https://github.com/kyan001/PyFileTrack"
-
-[project.scripts]
-filetrack = "filetrack.command_line:main"
-
-[tool.setuptools]
-py-modules = ["filetrack"]
-
-[tool.setuptools.dynamic]
-version = {attr = "filetrack.__version__"}
-dependencies = {file = "requirements.txt"}
-optional-dependencies = {dev = {file = "requirements-dev.txt"}, opt = {file = "requirements-opt.txt"}}
-
-[tool.setuptools.packages.find]
-exclude = ["contrib", "docs", "tests"]
+[build-system]
+requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "filetrack"
+description = "Tracking file changes according to the record file."
+requires-python = ">=3.8"
+readme = "README.md"
+keywords = ["python3", "file", "track", "cli"]
+license = {file = "LICENSE"}
+classifiers = [
+    "Intended Audience :: Developers",
+    "Intended Audience :: End Users/Desktop",
+    "License :: OSI Approved :: BSD License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+]
+dynamic = ["version", "dependencies", "optional-dependencies"]
+
+[[project.authors]]
+name = "Kyan"
+email = "kai@kyan001.com"
+
+[project.urls]
+Homepage = "https://github.com/kyan001/PyFileTrack"
+Changelog = "https://github.com/kyan001/PyFileTrack/blob/master/CHANGELOG.md"
+"Issue Tracker" = "https://github.com/kyan001/PyFileTrack/issues"
+"Source Code" = "https://github.com/kyan001/PyFileTrack"
+
+[project.scripts]
+filetrack = "filetrack.command_line:main"
+
+[tool.setuptools]
+py-modules = ["filetrack"]
+
+[tool.setuptools.dynamic]
+version = {attr = "filetrack.__version__"}
+dependencies = {file = "requirements.txt"}
+optional-dependencies = {dev = {file = "requirements-dev.txt"}, opt = {file = "requirements-opt.txt"}}
+
+[tool.setuptools.packages.find]
+exclude = ["contrib", "docs", "tests"]
```

