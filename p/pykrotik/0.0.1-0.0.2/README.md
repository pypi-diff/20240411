# Comparing `tmp/pykrotik-0.0.1.tar.gz` & `tmp/pykrotik-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykrotik-0.0.1.tar", last modified: Wed Apr 10 04:59:20 2024, max compression
+gzip compressed data, was "pykrotik-0.0.2.tar", last modified: Thu Apr 11 04:51:04 2024, max compression
```

## Comparing `pykrotik-0.0.1.tar` & `pykrotik-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:59:20.430766 pykrotik-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      170 2024-04-10 04:59:20.426372 pykrotik-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2024-04-10 04:46:21.000000 pykrotik-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:59:20.352908 pykrotik-0.0.1/pykrotik/
--rwxrwxrwx   0 root         (0) root         (0)    33298 2024-04-10 04:01:40.000000 pykrotik-0.0.1/pykrotik/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 04:59:20.419968 pykrotik-0.0.1/pykrotik.egg-info/
--rw-r--r--   0 root         (0) root         (0)      170 2024-04-10 04:59:20.000000 pykrotik-0.0.1/pykrotik.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      213 2024-04-10 04:59:20.000000 pykrotik-0.0.1/pykrotik.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 04:59:20.000000 pykrotik-0.0.1/pykrotik.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 04:59:20.000000 pykrotik-0.0.1/pykrotik.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-10 04:59:20.000000 pykrotik-0.0.1/pykrotik.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      137 2024-04-10 04:55:44.000000 pykrotik-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 04:59:20.431285 pykrotik-0.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-10 02:42:46.000000 pykrotik-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:51:04.348539 pykrotik-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-11 04:51:04.347710 pykrotik-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2024-04-10 16:25:46.000000 pykrotik-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:51:04.337662 pykrotik-0.0.2/pykrotik/
+-rw-r--r--   0 root         (0) root         (0)    33864 2024-04-11 00:51:40.000000 pykrotik-0.0.2/pykrotik/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:51:04.344867 pykrotik-0.0.2/pykrotik.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-11 04:51:04.000000 pykrotik-0.0.2/pykrotik.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      232 2024-04-11 04:51:04.000000 pykrotik-0.0.2/pykrotik.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 04:51:04.000000 pykrotik-0.0.2/pykrotik.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-11 04:51:04.000000 pykrotik-0.0.2/pykrotik.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-11 04:51:04.000000 pykrotik-0.0.2/pykrotik.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      335 2024-04-11 04:50:58.000000 pykrotik-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 04:51:04.348767 pykrotik-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 16:25:46.000000 pykrotik-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:51:04.343865 pykrotik-0.0.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     9887 2024-04-11 04:48:09.000000 pykrotik-0.0.2/tests/test_init.py
```

### Comparing `pykrotik-0.0.1/README.md` & `pykrotik-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pykrotik-0.0.1/pykrotik/__init__.py` & `pykrotik-0.0.2/pykrotik/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,20 +65,32 @@
 
     # the chain the firewall filter belongs to
     chain: str
     # comment attached to the ip firewall filter
     comment: str = pydantic.Field(default="")
     # flag that dictates whether an ip firewall filter is active
     disabled: bool = pydantic.Field(default=False)
+    # dst address for the firewall fitler
+    dst_address: str | None = pydantic.Field(default=None, alias=str("dst-address"))
+    # dst address list for the firewall fitler
+    dst_address_list: str | None = pydantic.Field(
+        default=None, alias=str("dst-address-list")
+    )
     # the id for an ip firewall filter (NOTE: prefixed with '*')
     id: str | None = pydantic.Field(default=None, alias=str(".id"))
     # flag that dictates whether filter is logged
     log: bool = pydantic.Field(default=False)
     # log prefix for logged filter
     log_prefix: str = pydantic.Field(default="", alias=str("log-prefix"))
+    # src address for the firewall fitler
+    src_address: str | None = pydantic.Field(default=None, alias=str("src-address"))
+    # src address list for the firewall fitler
+    src_address_list: str | None = pydantic.Field(
+        default=None, alias=str("src-address-list")
+    )
 
 
 class IpFirewallAcceptFilter(BaseIpFirewallFilter):
     """
     Firewall filter for an 'accept' action
     """
```

