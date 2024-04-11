# Comparing `tmp/pykrotik-0.0.2.tar.gz` & `tmp/pykrotik-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykrotik-0.0.2.tar", last modified: Thu Apr 11 04:51:04 2024, max compression
+gzip compressed data, was "pykrotik-0.0.3.tar", last modified: Thu Apr 11 05:22:44 2024, max compression
```

## Comparing `pykrotik-0.0.2.tar` & `pykrotik-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:51:04.348539 pykrotik-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      254 2024-04-11 04:51:04.347710 pykrotik-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2024-04-10 16:25:46.000000 pykrotik-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:51:04.337662 pykrotik-0.0.2/pykrotik/
--rw-r--r--   0 root         (0) root         (0)    33864 2024-04-11 00:51:40.000000 pykrotik-0.0.2/pykrotik/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:51:04.344867 pykrotik-0.0.2/pykrotik.egg-info/
--rw-r--r--   0 root         (0) root         (0)      254 2024-04-11 04:51:04.000000 pykrotik-0.0.2/pykrotik.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      232 2024-04-11 04:51:04.000000 pykrotik-0.0.2/pykrotik.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 04:51:04.000000 pykrotik-0.0.2/pykrotik.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-11 04:51:04.000000 pykrotik-0.0.2/pykrotik.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-11 04:51:04.000000 pykrotik-0.0.2/pykrotik.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      335 2024-04-11 04:50:58.000000 pykrotik-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 04:51:04.348767 pykrotik-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 16:25:46.000000 pykrotik-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 04:51:04.343865 pykrotik-0.0.2/tests/
--rw-r--r--   0 root         (0) root         (0)     9887 2024-04-11 04:48:09.000000 pykrotik-0.0.2/tests/test_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:22:44.427713 pykrotik-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-11 05:22:44.426840 pykrotik-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2024-04-10 16:25:46.000000 pykrotik-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:22:44.417094 pykrotik-0.0.3/pykrotik/
+-rw-r--r--   0 root         (0) root         (0)    35349 2024-04-11 05:21:36.000000 pykrotik-0.0.3/pykrotik/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:22:44.425675 pykrotik-0.0.3/pykrotik.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-11 05:22:44.000000 pykrotik-0.0.3/pykrotik.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      232 2024-04-11 05:22:44.000000 pykrotik-0.0.3/pykrotik.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 05:22:44.000000 pykrotik-0.0.3/pykrotik.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-11 05:22:44.000000 pykrotik-0.0.3/pykrotik.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-11 05:22:44.000000 pykrotik-0.0.3/pykrotik.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      335 2024-04-11 05:22:32.000000 pykrotik-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 05:22:44.427935 pykrotik-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 16:25:46.000000 pykrotik-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:22:44.424602 pykrotik-0.0.3/tests/
+-rw-r--r--   0 root         (0) root         (0)     9887 2024-04-11 05:19:02.000000 pykrotik-0.0.3/tests/test_init.py
```

### Comparing `pykrotik-0.0.2/README.md` & `pykrotik-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pykrotik-0.0.2/pykrotik/__init__.py` & `pykrotik-0.0.3/pykrotik/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -720,14 +720,26 @@
         )
         words = ["/ip/dns/static/add", *to_attribute_words(data)]
         response = await self.connection.send(*words)
         response.raise_for_error()
         id = response.sentences[-1].attributes["ret"]
         ip_dns_record.id = id
 
+    async def set_ip_dns_record(self, ip_dns_record: IpDnsRecord):
+        """
+        Edits an IPV4 dns record to routeros
+        """
+        data = ip_dns_record.model_dump(
+            by_alias=True, exclude_none=True, exclude={"id"}
+        )
+        data = {"numbers": ip_dns_record.id, **data}
+        words = ["/ip/dns/static/set", *to_attribute_words(data)]
+        response = await self.connection.send(*words)
+        response.raise_for_error()
+
     async def set_ip_dns_record_comment(self, ip_dns_record: IpDnsRecord, comment: str):
         """
         Sets the comment for an IPV4 dns record
         """
         data = {"numbers": ip_dns_record.id, "comment": comment}
         words = ["/ip/dns/static/comment", *to_attribute_words(data)]
         response = await self.connection.send(*words)
@@ -784,14 +796,26 @@
         )
         words = ["/ip/firewall/filter/add", *to_attribute_words(data)]
         response = await self.connection.send(*words)
         response.raise_for_error()
         id = response.sentences[-1].attributes["ret"]
         ip_firewall_filter.id = id
 
+    async def set_ip_firewall_filter(self, ip_firewall_filter: IpFirewallFilter):
+        """
+        Edits an IPV4 firewall filter to routeros
+        """
+        data = ip_firewall_filter.model_dump(
+            by_alias=True, exclude_none=True, exclude={"id"}
+        )
+        data = {"numbers": ip_firewall_filter.id, **data}
+        words = ["/ip/firewall/filter/set", *to_attribute_words(data)]
+        response = await self.connection.send(*words)
+        response.raise_for_error()
+
     async def set_ip_firewall_filter_comment(
         self, ip_firewall_filter: IpFirewallFilter, comment: str
     ):
         """
         Sets the comment for an IPV4 firewall filter
         """
         data = {"numbers": ip_firewall_filter.id, "comment": comment}
@@ -841,16 +865,30 @@
         Adds an IPV4 firewall address list to routeros
         """
         data = ip_firewall_address_list.model_dump(
             by_alias=True, exclude_none=True, exclude={"id"}
         )
         words = ["/ip/firewall/address-list/add", *to_attribute_words(data)]
         response = await self.connection.send(*words)
+        response.raise_for_error()
         id = response.sentences[-1].attributes["ret"]
         ip_firewall_address_list.id = id
+
+    async def set_ip_firewall_address_list(
+        self, ip_firewall_address_list: IpFirewallAddressList
+    ):
+        """
+        Edits an IPV4 dns record to routeros
+        """
+        data = ip_firewall_address_list.model_dump(
+            by_alias=True, exclude_none=True, exclude={"id"}
+        )
+        data = {"numbers": ip_firewall_address_list.id, **data}
+        words = ["/ip/firewall/address-list/set", *to_attribute_words(data)]
+        response = await self.connection.send(*words)
         response.raise_for_error()
 
     async def set_ip_firewall_address_list_comment(
         self, ip_firewall_address_list: IpFirewallAddressList, comment: str
     ):
         """
         Sets the comment for an IPV4 address list
```

### Comparing `pykrotik-0.0.2/tests/test_init.py` & `pykrotik-0.0.3/tests/test_init.py`

 * *Files identical despite different names*

