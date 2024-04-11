# Comparing `tmp/chomper-0.2.0.tar.gz` & `tmp/chomper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chomper-0.2.0.tar", last modified: Sat Nov 26 10:21:16 2022, max compression
+gzip compressed data, was "chomper-0.3.0.tar", last modified: Thu Apr 11 19:47:18 2024, max compression
```

## Comparing `chomper-0.2.0.tar` & `chomper-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,46 @@
-drwxr-xr-x   0 yawenji    (501) staff       (20)        0 2022-11-26 10:21:16.431573 chomper-0.2.0/
--rw-r--r--   0 yawenji    (501) staff       (20)     1061 2022-09-07 17:36:57.000000 chomper-0.2.0/LICENSE
--rw-r--r--   0 yawenji    (501) staff       (20)     2999 2022-11-26 10:21:16.431662 chomper-0.2.0/PKG-INFO
--rw-r--r--   0 yawenji    (501) staff       (20)     2304 2022-11-26 10:18:07.000000 chomper-0.2.0/README.md
--rw-r--r--   0 yawenji    (501) staff       (20)       85 2022-07-18 14:24:42.000000 chomper-0.2.0/pyproject.toml
--rw-r--r--   0 yawenji    (501) staff       (20)     1307 2022-11-26 10:21:16.432204 chomper-0.2.0/setup.cfg
-drwxr-xr-x   0 yawenji    (501) staff       (20)        0 2022-11-26 10:21:16.427004 chomper-0.2.0/src/
-drwxr-xr-x   0 yawenji    (501) staff       (20)        0 2022-11-26 10:21:16.430544 chomper-0.2.0/src/chomper/
--rw-r--r--   0 yawenji    (501) staff       (20)       49 2022-11-26 09:57:19.000000 chomper-0.2.0/src/chomper/__init__.py
--rw-r--r--   0 yawenji    (501) staff       (20)     1643 2022-11-21 06:45:25.000000 chomper-0.2.0/src/chomper/arch.py
--rw-r--r--   0 yawenji    (501) staff       (20)      668 2022-10-21 06:30:40.000000 chomper-0.2.0/src/chomper/const.py
--rw-r--r--   0 yawenji    (501) staff       (20)    22431 2022-11-25 07:01:43.000000 chomper-0.2.0/src/chomper/core.py
--rw-r--r--   0 yawenji    (501) staff       (20)      183 2022-11-21 06:43:15.000000 chomper-0.2.0/src/chomper/exceptions.py
--rw-r--r--   0 yawenji    (501) staff       (20)     2332 2022-11-25 07:41:52.000000 chomper-0.2.0/src/chomper/hooks.py
--rw-r--r--   0 yawenji    (501) staff       (20)      437 2022-09-15 08:27:36.000000 chomper-0.2.0/src/chomper/log.py
--rw-r--r--   0 yawenji    (501) staff       (20)     2725 2022-10-21 06:30:40.000000 chomper-0.2.0/src/chomper/memory.py
--rw-r--r--   0 yawenji    (501) staff       (20)     1083 2022-11-21 06:45:25.000000 chomper-0.2.0/src/chomper/structs.py
--rw-r--r--   0 yawenji    (501) staff       (20)      108 2022-09-06 02:30:37.000000 chomper-0.2.0/src/chomper/utils.py
-drwxr-xr-x   0 yawenji    (501) staff       (20)        0 2022-11-26 10:21:16.431433 chomper-0.2.0/src/chomper.egg-info/
--rw-r--r--   0 yawenji    (501) staff       (20)     2999 2022-11-26 10:21:16.000000 chomper-0.2.0/src/chomper.egg-info/PKG-INFO
--rw-r--r--   0 yawenji    (501) staff       (20)      433 2022-11-26 10:21:16.000000 chomper-0.2.0/src/chomper.egg-info/SOURCES.txt
--rw-r--r--   0 yawenji    (501) staff       (20)        1 2022-11-26 10:21:16.000000 chomper-0.2.0/src/chomper.egg-info/dependency_links.txt
--rw-r--r--   0 yawenji    (501) staff       (20)       46 2022-11-26 10:21:16.000000 chomper-0.2.0/src/chomper.egg-info/requires.txt
--rw-r--r--   0 yawenji    (501) staff       (20)        8 2022-11-26 10:21:16.000000 chomper-0.2.0/src/chomper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 19:47:18.151381 chomper-0.3.0/
+-rw-rw-rw-   0        0        0     1061 2022-11-28 02:00:45.000000 chomper-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5064 2024-04-11 19:47:18.151381 chomper-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4267 2024-04-10 17:07:18.000000 chomper-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1261 2024-04-11 19:47:05.000000 chomper-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 19:47:18.151381 chomper-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 19:47:18.091865 chomper-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 19:47:18.127869 chomper-0.3.0/src/chomper/
+-rw-rw-rw-   0        0        0       52 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/__init__.py
+-rw-rw-rw-   0        0        0     1567 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/arch.py
+-rw-rw-rw-   0        0        0      730 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/const.py
+-rw-rw-rw-   0        0        0    28598 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/core.py
+-rw-rw-rw-   0        0        0      183 2024-03-29 14:18:10.000000 chomper-0.3.0/src/chomper/exceptions.py
+-rw-rw-rw-   0        0        0      437 2024-03-29 14:18:10.000000 chomper-0.3.0/src/chomper/log.py
+-rw-rw-rw-   0        0        0     3629 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/memory.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:47:18.142383 chomper-0.3.0/src/chomper/os/
+-rw-rw-rw-   0        0        0        0 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:47:18.144381 chomper-0.3.0/src/chomper/os/android/
+-rw-rw-rw-   0        0        0       27 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/os/android/__init__.py
+-rw-rw-rw-   0        0        0     1297 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/os/android/hooks.py
+-rw-rw-rw-   0        0        0     6485 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/os/android/loader.py
+-rw-rw-rw-   0        0        0      513 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/os/android/os.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:47:18.148381 chomper-0.3.0/src/chomper/os/ios/
+-rw-rw-rw-   0        0        0       23 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/os/ios/__init__.py
+-rw-rw-rw-   0        0        0    10059 2024-04-11 19:35:42.000000 chomper-0.3.0/src/chomper/os/ios/hooks.py
+-rw-rw-rw-   0        0        0     8829 2024-04-11 19:38:16.000000 chomper-0.3.0/src/chomper/os/ios/loader.py
+-rw-rw-rw-   0        0        0    18934 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/os/ios/modules.py
+-rw-rw-rw-   0        0        0      428 2024-04-11 19:35:42.000000 chomper-0.3.0/src/chomper/os/ios/options.py
+-rw-rw-rw-   0        0        0     5312 2024-04-11 19:35:42.000000 chomper-0.3.0/src/chomper/os/ios/os.py
+-rw-rw-rw-   0        0        0      359 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/os/ios/structs.py
+-rw-rw-rw-   0        0        0     5376 2024-04-11 19:35:42.000000 chomper-0.3.0/src/chomper/os/ios/syscall.py
+-rw-rw-rw-   0        0        0        0 2024-03-29 14:18:10.000000 chomper-0.3.0/src/chomper/py.typed
+-rw-rw-rw-   0        0        0     3414 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/types.py
+-rw-rw-rw-   0        0        0      392 2024-04-10 16:34:07.000000 chomper-0.3.0/src/chomper/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:47:18.150380 chomper-0.3.0/src/chomper.egg-info/
+-rw-rw-rw-   0        0        0     5064 2024-04-11 19:47:18.000000 chomper-0.3.0/src/chomper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2024-04-11 19:47:18.000000 chomper-0.3.0/src/chomper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 19:47:18.000000 chomper-0.3.0/src/chomper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-11 19:47:18.000000 chomper-0.3.0/src/chomper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-11 19:47:18.000000 chomper-0.3.0/src/chomper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 19:47:18.150380 chomper-0.3.0/tests/
+-rw-rw-rw-   0        0        0     3103 2024-04-10 16:34:07.000000 chomper-0.3.0/tests/test_emulator.py
+-rw-rw-rw-   0        0        0     2416 2024-04-10 16:34:07.000000 chomper-0.3.0/tests/test_examples.py
+-rw-rw-rw-   0        0        0     1138 2024-04-10 16:34:07.000000 chomper-0.3.0/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0     7008 2024-04-11 19:35:42.000000 chomper-0.3.0/tests/test_libc.py
+-rw-rw-rw-   0        0        0      307 2024-02-14 13:38:00.000000 chomper-0.3.0/tests/test_utils.py
```

### Comparing `chomper-0.2.0/LICENSE` & `chomper-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chomper-0.2.0/src/chomper/const.py` & `chomper-0.3.0/src/chomper/const.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-import sys
-
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
-# Endian type
-BIG_ENDIAN: Literal["big"] = "big"
-LITTLE_ENDIAN: Literal["little"] = "little"
-
-# Supported arch
-ARCH_ARM = 1
-ARCH_ARM64 = 2
-
-# The address of thread local storage (TLS)
-TLS_ADDRESS = 0x10000
-TLS_SIZE = 0x400
-
-# Trap area
-TRAP_ADDRESS = 0x20000
-TRAP_SIZE = 0x10000
-
-# Temporary use
-TEMP_ADDRESS = 0x30000
-
-# The address of stack
-STACK_ADDRESS = 0x50000
-STACK_SIZE = 0x50000
-
-# The address of module
-MODULE_ADDRESS = 0x1000000
-
-# The address of heap
-HEAP_ADDRESS = 0x80000000
-
-# Minimum size of memory pool
-MINIMUM_POOL_SIZE = 8**5
+import sys
+
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
+# Endian type
+EndianType = Literal["little", "big"]
+
+BIG_ENDIAN: Literal["big"] = "big"
+LITTLE_ENDIAN: Literal["little"] = "little"
+
+# Supported arch
+ARCH_ARM = 1
+ARCH_ARM64 = 2
+
+MODE_ARM = 1
+MODE_THUMB = 2
+
+# Supported os type
+OS_ANDROID = 1
+OS_IOS = 2
+
+# The address of thread local storage (TLS)
+TLS_ADDRESS = 0x10000
+TLS_SIZE = 0x10000
+
+# The address of stack
+STACK_ADDRESS = 0x50000
+STACK_SIZE = 0x50000
+
+# The address of module
+MODULE_ADDRESS = 0x10000000
+
+# The address of heap
+HEAP_ADDRESS = 0x8000000
+
+# Minimum size of memory pool
+MINIMUM_POOL_SIZE = 2**16
```

