# Comparing `tmp/Beaker-1.9.0.tar.gz` & `tmp/Beaker-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Beaker-1.9.0.tar", last modified: Sun Jun 18 21:34:02 2017, max compression
+gzip compressed data, was "dist/Beaker-1.9.1.tar", last modified: Mon Apr  9 20:04:55 2018, max compression
```

## Comparing `Beaker-1.9.0.tar` & `Beaker-1.9.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 amol       (501) staff       (20)        0 2017-06-18 21:34:02.000000 Beaker-1.9.0/
-drwxr-xr-x   0 amol       (501) staff       (20)        0 2017-06-18 21:34:02.000000 Beaker-1.9.0/beaker/
--rw-r--r--   0 amol       (501) staff       (20)       22 2017-06-18 21:32:51.000000 Beaker-1.9.0/beaker/__init__.py
--rw-r--r--   0 amol       (501) staff       (20)     4256 2017-03-08 19:47:07.000000 Beaker-1.9.0/beaker/_compat.py
--rw-r--r--   0 amol       (501) staff       (20)    21822 2017-06-18 20:41:27.000000 Beaker-1.9.0/beaker/cache.py
--rw-r--r--   0 amol       (501) staff       (20)    23586 2017-06-18 20:41:27.000000 Beaker-1.9.0/beaker/container.py
--rw-r--r--   0 amol       (501) staff       (20)      898 2015-02-25 15:37:38.000000 Beaker-1.9.0/beaker/converters.py
--rw-r--r--   0 amol       (501) staff       (20)     3045 2015-11-22 13:54:40.000000 Beaker-1.9.0/beaker/cookie.py
-drwxr-xr-x   0 amol       (501) staff       (20)        0 2017-06-18 21:34:02.000000 Beaker-1.9.0/beaker/crypto/
--rw-r--r--   0 amol       (501) staff       (20)     2434 2017-03-08 19:45:16.000000 Beaker-1.9.0/beaker/crypto/__init__.py
--rw-r--r--   0 amol       (501) staff       (20)     1297 2017-03-08 19:45:16.000000 Beaker-1.9.0/beaker/crypto/jcecrypto.py
--rw-r--r--   0 amol       (501) staff       (20)      182 2017-03-08 19:45:16.000000 Beaker-1.9.0/beaker/crypto/noencryption.py
--rw-r--r--   0 amol       (501) staff       (20)     1586 2015-02-25 15:37:38.000000 Beaker-1.9.0/beaker/crypto/nsscrypto.py
--rw-r--r--   0 amol       (501) staff       (20)     3236 2016-01-23 10:54:31.000000 Beaker-1.9.0/beaker/crypto/pbkdf2.py
--rw-r--r--   0 amol       (501) staff       (20)     1333 2017-03-08 19:45:16.000000 Beaker-1.9.0/beaker/crypto/pyca_cryptography.py
--rw-r--r--   0 amol       (501) staff       (20)      984 2017-03-08 19:45:16.000000 Beaker-1.9.0/beaker/crypto/pycrypto.py
--rw-r--r--   0 amol       (501) staff       (20)      432 2015-02-25 15:37:38.000000 Beaker-1.9.0/beaker/crypto/util.py
--rw-r--r--   0 amol       (501) staff       (20)      443 2015-02-25 15:37:38.000000 Beaker-1.9.0/beaker/exceptions.py
-drwxr-xr-x   0 amol       (501) staff       (20)        0 2017-06-18 21:34:02.000000 Beaker-1.9.0/beaker/ext/
--rw-r--r--   0 amol       (501) staff       (20)        0 2015-02-25 15:37:38.000000 Beaker-1.9.0/beaker/ext/__init__.py
--rw-r--r--   0 amol       (501) staff       (20)     6205 2017-04-26 20:24:35.000000 Beaker-1.9.0/beaker/ext/database.py
--rw-r--r--   0 amol       (501) staff       (20)     3961 2015-02-25 15:37:38.000000 Beaker-1.9.0/beaker/ext/google.py
--rw-r--r--   0 amol       (501) staff       (20)     6980 2016-01-23 10:49:56.000000 Beaker-1.9.0/beaker/ext/memcached.py
--rw-r--r--   0 amol       (501) staff       (20)     5869 2017-06-18 20:41:27.000000 Beaker-1.9.0/beaker/ext/mongodb.py
--rw-r--r--   0 amol       (501) staff       (20)     4080 2017-06-18 20:41:27.000000 Beaker-1.9.0/beaker/ext/redisnm.py
--rw-r--r--   0 amol       (501) staff       (20)     4721 2015-02-25 15:37:38.000000 Beaker-1.9.0/beaker/ext/sqla.py
--rw-r--r--   0 amol       (501) staff       (20)     6482 2017-06-17 12:26:14.000000 Beaker-1.9.0/beaker/middleware.py
--rw-r--r--   0 amol       (501) staff       (20)    30697 2017-06-18 20:41:24.000000 Beaker-1.9.0/beaker/session.py
--rw-r--r--   0 amol       (501) staff       (20)    11300 2017-06-18 20:41:27.000000 Beaker-1.9.0/beaker/synchronization.py
--rw-r--r--   0 amol       (501) staff       (20)    16802 2017-06-18 20:41:27.000000 Beaker-1.9.0/beaker/util.py
-drwxr-xr-x   0 amol       (501) staff       (20)        0 2017-06-18 21:34:02.000000 Beaker-1.9.0/Beaker.egg-info/
--rw-r--r--   0 amol       (501) staff       (20)        1 2017-06-18 21:34:02.000000 Beaker-1.9.0/Beaker.egg-info/dependency_links.txt
--rw-r--r--   0 amol       (501) staff       (20)      496 2017-06-18 21:34:02.000000 Beaker-1.9.0/Beaker.egg-info/entry_points.txt
--rw-r--r--   0 amol       (501) staff       (20)        1 2015-02-25 14:52:31.000000 Beaker-1.9.0/Beaker.egg-info/not-zip-safe
--rw-r--r--   0 amol       (501) staff       (20)       47 2015-08-15 19:32:53.000000 Beaker-1.9.0/Beaker.egg-info/pbr.json
--rw-r--r--   0 amol       (501) staff       (20)     3575 2017-06-18 21:34:02.000000 Beaker-1.9.0/Beaker.egg-info/PKG-INFO
--rw-r--r--   0 amol       (501) staff       (20)      233 2017-06-18 21:34:02.000000 Beaker-1.9.0/Beaker.egg-info/requires.txt
--rw-r--r--   0 amol       (501) staff       (20)      848 2017-06-18 21:34:02.000000 Beaker-1.9.0/Beaker.egg-info/SOURCES.txt
--rw-r--r--   0 amol       (501) staff       (20)        7 2017-06-18 21:34:02.000000 Beaker-1.9.0/Beaker.egg-info/top_level.txt
--rw-r--r--   0 amol       (501) staff       (20)     3575 2017-06-18 21:34:02.000000 Beaker-1.9.0/PKG-INFO
--rw-r--r--   0 amol       (501) staff       (20)     1941 2015-01-28 11:40:24.000000 Beaker-1.9.0/README.rst
--rw-r--r--   0 amol       (501) staff       (20)      228 2017-06-18 21:34:02.000000 Beaker-1.9.0/setup.cfg
--rw-r--r--   0 amol       (501) staff       (20)     3340 2017-06-18 20:41:27.000000 Beaker-1.9.0/setup.py
+drwxr-xr-x   0 amol       (501) staff       (20)        0 2018-04-09 20:04:55.000000 Beaker-1.9.1/
+drwxr-xr-x   0 amol       (501) staff       (20)        0 2018-04-09 20:04:55.000000 Beaker-1.9.1/beaker/
+-rw-r--r--   0 amol       (501) staff       (20)       22 2018-04-09 19:38:13.000000 Beaker-1.9.1/beaker/__init__.py
+-rw-r--r--   0 amol       (501) staff       (20)     4256 2017-03-08 19:47:07.000000 Beaker-1.9.1/beaker/_compat.py
+-rw-r--r--   0 amol       (501) staff       (20)    21917 2018-04-09 19:37:09.000000 Beaker-1.9.1/beaker/cache.py
+-rw-r--r--   0 amol       (501) staff       (20)    24079 2018-04-09 19:37:09.000000 Beaker-1.9.1/beaker/container.py
+-rw-r--r--   0 amol       (501) staff       (20)      898 2015-02-25 15:37:38.000000 Beaker-1.9.1/beaker/converters.py
+-rw-r--r--   0 amol       (501) staff       (20)     3045 2015-11-22 13:54:40.000000 Beaker-1.9.1/beaker/cookie.py
+drwxr-xr-x   0 amol       (501) staff       (20)        0 2018-04-09 20:04:55.000000 Beaker-1.9.1/beaker/crypto/
+-rw-r--r--   0 amol       (501) staff       (20)     2434 2017-03-08 19:45:16.000000 Beaker-1.9.1/beaker/crypto/__init__.py
+-rw-r--r--   0 amol       (501) staff       (20)     1297 2017-03-08 19:45:16.000000 Beaker-1.9.1/beaker/crypto/jcecrypto.py
+-rw-r--r--   0 amol       (501) staff       (20)      182 2017-03-08 19:45:16.000000 Beaker-1.9.1/beaker/crypto/noencryption.py
+-rw-r--r--   0 amol       (501) staff       (20)     1586 2015-02-25 15:37:38.000000 Beaker-1.9.1/beaker/crypto/nsscrypto.py
+-rw-r--r--   0 amol       (501) staff       (20)     3236 2016-01-23 10:54:31.000000 Beaker-1.9.1/beaker/crypto/pbkdf2.py
+-rw-r--r--   0 amol       (501) staff       (20)     1333 2017-03-08 19:45:16.000000 Beaker-1.9.1/beaker/crypto/pyca_cryptography.py
+-rw-r--r--   0 amol       (501) staff       (20)      984 2017-03-08 19:45:16.000000 Beaker-1.9.1/beaker/crypto/pycrypto.py
+-rw-r--r--   0 amol       (501) staff       (20)      432 2015-02-25 15:37:38.000000 Beaker-1.9.1/beaker/crypto/util.py
+-rw-r--r--   0 amol       (501) staff       (20)      443 2015-02-25 15:37:38.000000 Beaker-1.9.1/beaker/exceptions.py
+drwxr-xr-x   0 amol       (501) staff       (20)        0 2018-04-09 20:04:55.000000 Beaker-1.9.1/beaker/ext/
+-rw-r--r--   0 amol       (501) staff       (20)        0 2015-02-25 15:37:38.000000 Beaker-1.9.1/beaker/ext/__init__.py
+-rw-r--r--   0 amol       (501) staff       (20)     6279 2018-04-09 19:37:09.000000 Beaker-1.9.1/beaker/ext/database.py
+-rw-r--r--   0 amol       (501) staff       (20)     3961 2015-02-25 15:37:38.000000 Beaker-1.9.1/beaker/ext/google.py
+-rw-r--r--   0 amol       (501) staff       (20)     6980 2016-01-23 10:49:56.000000 Beaker-1.9.1/beaker/ext/memcached.py
+-rw-r--r--   0 amol       (501) staff       (20)     6719 2017-06-19 06:58:30.000000 Beaker-1.9.1/beaker/ext/mongodb.py
+-rw-r--r--   0 amol       (501) staff       (20)     4512 2017-06-19 07:00:10.000000 Beaker-1.9.1/beaker/ext/redisnm.py
+-rw-r--r--   0 amol       (501) staff       (20)     4721 2015-02-25 15:37:38.000000 Beaker-1.9.1/beaker/ext/sqla.py
+-rw-r--r--   0 amol       (501) staff       (20)     6482 2017-06-17 12:26:14.000000 Beaker-1.9.1/beaker/middleware.py
+-rw-r--r--   0 amol       (501) staff       (20)    30698 2017-12-05 21:54:26.000000 Beaker-1.9.1/beaker/session.py
+-rw-r--r--   0 amol       (501) staff       (20)    11525 2018-04-09 19:37:09.000000 Beaker-1.9.1/beaker/synchronization.py
+-rw-r--r--   0 amol       (501) staff       (20)    17118 2018-02-12 13:50:33.000000 Beaker-1.9.1/beaker/util.py
+drwxr-xr-x   0 amol       (501) staff       (20)        0 2018-04-09 20:04:55.000000 Beaker-1.9.1/Beaker.egg-info/
+-rw-r--r--   0 amol       (501) staff       (20)        1 2018-04-09 20:04:55.000000 Beaker-1.9.1/Beaker.egg-info/dependency_links.txt
+-rw-r--r--   0 amol       (501) staff       (20)      496 2018-04-09 20:04:55.000000 Beaker-1.9.1/Beaker.egg-info/entry_points.txt
+-rw-r--r--   0 amol       (501) staff       (20)        1 2015-02-25 14:52:31.000000 Beaker-1.9.1/Beaker.egg-info/not-zip-safe
+-rw-r--r--   0 amol       (501) staff       (20)       47 2015-08-15 19:32:53.000000 Beaker-1.9.1/Beaker.egg-info/pbr.json
+-rw-r--r--   0 amol       (501) staff       (20)     3811 2018-04-09 20:04:55.000000 Beaker-1.9.1/Beaker.egg-info/PKG-INFO
+-rw-r--r--   0 amol       (501) staff       (20)      233 2018-04-09 20:04:55.000000 Beaker-1.9.1/Beaker.egg-info/requires.txt
+-rw-r--r--   0 amol       (501) staff       (20)      848 2018-04-09 20:04:55.000000 Beaker-1.9.1/Beaker.egg-info/SOURCES.txt
+-rw-r--r--   0 amol       (501) staff       (20)        7 2018-04-09 20:04:55.000000 Beaker-1.9.1/Beaker.egg-info/top_level.txt
+-rw-r--r--   0 amol       (501) staff       (20)     3811 2018-04-09 20:04:55.000000 Beaker-1.9.1/PKG-INFO
+-rw-r--r--   0 amol       (501) staff       (20)     1955 2017-12-05 21:54:26.000000 Beaker-1.9.1/README.rst
+-rw-r--r--   0 amol       (501) staff       (20)      207 2018-04-09 20:04:55.000000 Beaker-1.9.1/setup.cfg
+-rw-r--r--   0 amol       (501) staff       (20)     3773 2018-04-09 19:37:41.000000 Beaker-1.9.1/setup.py
```

### Comparing `Beaker-1.9.0/beaker/_compat.py` & `Beaker-1.9.1/beaker/_compat.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/cache.py` & `Beaker-1.9.1/beaker/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,14 +591,16 @@
             # TODO: This is probably a bug as length is checked before converting to UTF8
             # which will cause cache_key to grow in size.
             if len(cache_key) + len(namespace) > int(key_length):
                 cache_key = sha1(cache_key.encode('utf-8')).hexdigest()
 
             def go():
                 return func(*args, **kwargs)
+            # save org function name
+            go.__name__ = '_cached_%s' % (func.__name__,)
 
             return cache[0].get_value(cache_key, createfunc=go)
         cached._arg_namespace = namespace
         if region is not None:
             cached._arg_region = region
         return cached
     return decorate
```

### Comparing `Beaker-1.9.0/beaker/container.py` & `Beaker-1.9.1/beaker/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Container and Namespace classes"""
+import errno
+
 from ._compat import pickle, anydbm, add_metaclass, PYVER, unicode_text
 
 import beaker.util as util
 import logging
 import os
 import time
 
@@ -549,16 +551,22 @@
         else:
             for ext in ('db', 'dat', 'pag', 'dir'):
                 if os.access(file + os.extsep + ext, os.F_OK):
                     return True
 
         return False
 
+    def _ensuredir(self, filename):
+        dirname = os.path.dirname(filename)
+        if not os.path.exists(dirname):
+            util.verify_directory(dirname)
+
     def _checkfile(self):
         if not self.file_exists(self.file):
+            self._ensuredir(self.file)
             g = self.dbmmodule.open(self.file, 'c')
             g.close()
 
     def get_filenames(self):
         list = []
         if os.access(self.file, os.F_OK):
             list.append(self.file)
@@ -656,25 +664,29 @@
                 )
 
     def file_exists(self, file):
         return os.access(file, os.F_OK)
 
     def do_open(self, flags, replace):
         if not replace and self.file_exists(self.file):
-            fh = open(self.file, 'rb')
-            self.hash = pickle.load(fh)
-            fh.close()
+            try:
+                with open(self.file, 'rb') as fh:
+                    self.hash = pickle.load(fh)
+            except IOError as e:
+                # Ignore EACCES and ENOENT as it just means we are no longer
+                # able to access the file or that it no longer exists
+                if e.errno not in [errno.EACCES, errno.ENOENT]:
+                    raise
 
         self.flags = flags
 
     def do_close(self):
         if self.flags == 'c' or self.flags == 'w':
-            fh = open(self.file, 'wb')
-            pickle.dump(self.hash, fh)
-            fh.close()
+            pickled = pickle.dumps(self.hash)
+            util.safe_write(self.file, pickled)
 
         self.hash = {}
         self.flags = None
 
     def do_remove(self):
         try:
             os.remove(self.file)
```

### Comparing `Beaker-1.9.0/beaker/converters.py` & `Beaker-1.9.1/beaker/converters.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/cookie.py` & `Beaker-1.9.1/beaker/cookie.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/crypto/__init__.py` & `Beaker-1.9.1/beaker/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/crypto/jcecrypto.py` & `Beaker-1.9.1/beaker/crypto/jcecrypto.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/crypto/nsscrypto.py` & `Beaker-1.9.1/beaker/crypto/nsscrypto.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/crypto/pbkdf2.py` & `Beaker-1.9.1/beaker/crypto/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/crypto/pyca_cryptography.py` & `Beaker-1.9.1/beaker/crypto/pyca_cryptography.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/crypto/pycrypto.py` & `Beaker-1.9.1/beaker/crypto/pycrypto.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/ext/database.py` & `Beaker-1.9.1/beaker/ext/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,20 @@
     def do_open(self, flags, replace):
         # If we already loaded the data, don't bother loading it again
         if self.loaded:
             self.flags = flags
             return
 
         cache = self.cache
-        result = sa.select([cache.c.data],
+        result_proxy = sa.select([cache.c.data],
                            cache.c.namespace == self.namespace
-                          ).execute().fetchone()
+                          ).execute()
+        result = result_proxy.fetchone()
+        result_proxy.close()
+        
         if not result:
             self._is_new = True
             self.hash = {}
         else:
             self._is_new = False
             try:
                 self.hash = result['data']
```

### Comparing `Beaker-1.9.0/beaker/ext/google.py` & `Beaker-1.9.1/beaker/ext/google.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/ext/memcached.py` & `Beaker-1.9.1/beaker/ext/memcached.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/ext/mongodb.py` & `Beaker-1.9.1/beaker/ext/mongodb.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,23 @@
 from beaker.synchronization import SynchronizerImpl
 from beaker.util import SyncDict, machine_identifier
 from beaker.crypto.util import sha1
 from beaker._compat import string_type, PY2
 
 
 class MongoNamespaceManager(NamespaceManager):
-    """Provides the :class:`.NamespaceManager` API over MongoDB."""
+    """Provides the :class:`.NamespaceManager` API over MongoDB.
+
+    Provided ``url`` can be both a mongodb connection string or
+    an already existing MongoClient instance.
+
+    The data will be stored into ``beaker_cache`` collection of the
+    *default database*, so make sure your connection string or
+    MongoClient point to a default database.
+    """
     MAX_KEY_LENGTH = 1024
 
     clients = SyncDict()
 
     def __init__(self, namespace, url, **kw):
         super(MongoNamespaceManager, self).__init__(namespace)
         self.lock_dir = None  # MongoDB uses mongo itself for locking.
@@ -96,14 +104,26 @@
     def _clear_expired(self):
         now = time.time()
         self.db.backer_cache.delete_many({'_id': {'$regex': '^%s' % self.namespace},
                                           'expiration': {'$ne': None, '$lte': now}})
 
 
 class MongoSynchronizer(SynchronizerImpl):
+    """Provides a Writer/Reader lock based on MongoDB.
+
+    Provided ``url`` can be both a mongodb connection string or
+    an already existing MongoClient instance.
+
+    The data will be stored into ``beaker_locks`` collection of the
+    *default database*, so make sure your connection string or
+    MongoClient point to a default database.
+
+    Locks are identified by local machine, PID and threadid, so
+    are suitable for use in both local and distributed environments.
+    """
     # If a cache entry generation function can take a lot,
     # but 15 minutes is more than a reasonable time.
     LOCK_EXPIRATION = 900
     MACHINE_ID = machine_identifier()
 
     def __init__(self, identifier, url):
         super(MongoSynchronizer, self).__init__()
@@ -120,41 +140,44 @@
         self.db.beaker_locks.delete_many({'_id': self.identifier, 'timestamp': {'$lte': expired}})
         return now
 
     def _get_owner_id(self):
         return '%s-%s-%s' % (self.MACHINE_ID, os.getpid(), threading.current_thread().ident)
 
     def do_release_read_lock(self):
-        self.db.beaker_locks.update_one({'_id': self.identifier, 'readers': self._get_owner_id()},
-                                        {'$pull': {'readers': self._get_owner_id()}})
+        owner_id = self._get_owner_id()
+        self.db.beaker_locks.update_one({'_id': self.identifier, 'readers': owner_id},
+                                        {'$pull': {'readers': owner_id}})
 
     def do_acquire_read_lock(self, wait):
         now = self._clear_expired_locks()
+        owner_id = self._get_owner_id()
         while True:
             try:
                 self.db.beaker_locks.update_one({'_id': self.identifier, 'owner': None},
                                                 {'$set': {'timestamp': now},
-                                                 '$push': {'readers': self._get_owner_id()}},
+                                                 '$push': {'readers': owner_id}},
                                                 upsert=True)
                 return True
             except pymongo.errors.DuplicateKeyError:
                 if not wait:
                     return False
                 time.sleep(0.2)
 
     def do_release_write_lock(self):
         self.db.beaker_locks.delete_one({'_id': self.identifier, 'owner': self._get_owner_id()})
 
     def do_acquire_write_lock(self, wait):
         now = self._clear_expired_locks()
+        owner_id = self._get_owner_id()
         while True:
             try:
                 self.db.beaker_locks.update_one({'_id': self.identifier, 'owner': None,
                                                  'readers': []},
-                                                {'$set': {'owner': self._get_owner_id(),
+                                                {'$set': {'owner': owner_id,
                                                           'timestamp': now}},
                                                 upsert=True)
                 return True
             except pymongo.errors.DuplicateKeyError:
                 if not wait:
                     return False
                 time.sleep(0.2)
```

### Comparing `Beaker-1.9.0/beaker/ext/redisnm.py` & `Beaker-1.9.1/beaker/ext/redisnm.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,24 @@
 from beaker.synchronization import SynchronizerImpl
 from beaker.util import SyncDict, machine_identifier
 from beaker.crypto.util import sha1
 from beaker._compat import string_type, PY2
 
 
 class RedisNamespaceManager(NamespaceManager):
-    """Provides the :class:`.NamespaceManager` API over Redis."""
+    """Provides the :class:`.NamespaceManager` API over Redis.
+
+    Provided ``url`` can be both a redis connection string or
+    an already existing StrictRedis instance.
+
+    The data will be stored into redis keys, with their name
+    starting with ``beaker_cache:``. So make sure you provide
+    a specific database number if you don't want to mix them
+    with your own data.
+    """
     MAX_KEY_LENGTH = 1024
 
     clients = SyncDict()
 
     def __init__(self, namespace, url, **kw):
         super(RedisNamespaceManager, self).__init__(namespace)
         self.lock_dir = None  # Redis uses redis itself for locking.
@@ -77,14 +86,17 @@
     def keys(self):
         return self.client.keys('beaker_cache:%s:*' % self.namespace)
 
 
 class RedisSynchronizer(SynchronizerImpl):
     """Synchronizer based on redis.
 
+    Provided ``url`` can be both a redis connection string or
+    an already existing StrictRedis instance.
+
     This Synchronizer only supports 1 reader or 1 writer at time, not concurrent readers.
     """
     # If a cache entry generation function can take a lot,
     # but 15 minutes is more than a reasonable time.
     LOCK_EXPIRATION = 900
     MACHINE_ID = machine_identifier()
```

### Comparing `Beaker-1.9.0/beaker/ext/sqla.py` & `Beaker-1.9.1/beaker/ext/sqla.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/middleware.py` & `Beaker-1.9.1/beaker/middleware.py`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/beaker/session.py` & `Beaker-1.9.1/beaker/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,14 +797,15 @@
         self._session().delete()
 
     def persist(self):
         """Persist the session to the storage
 
         Always saves the whole session if save() or delete() have been called.
         If they haven't:
+
         - If autosave is set to true, saves the the entire session regardless.
         - If save_accessed_time is set to true or unset, only saves the updated
           access time.
         - If save_accessed_time is set to false, doesn't save anything.
 
         """
         if self.__dict__['_params'].get('auto'):
```

### Comparing `Beaker-1.9.0/beaker/synchronization.py` & `Beaker-1.9.1/beaker/synchronization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Synchronization functions.
 
 File- and mutex-based mutual exclusion synchronizers are provided,
 as well as a name-based mutex which locks within an application
 based on a string name.
 
 """
-
+import errno
 import os
 import sys
 import tempfile
 
 try:
     import threading as _threading
 except ImportError:
@@ -221,22 +221,28 @@
             lock_dir = lock_dir
 
         self.filename = util.encoded_path(
                             lock_dir,
                             [identifier],
                             extension='.lock'
                         )
+        self.lock_dir = os.path.dirname(self.filename)
 
     def _filedesc(self):
         return self._filedescriptor.get()
     _filedesc = property(_filedesc)
 
+    def _ensuredir(self):
+        if not os.path.exists(self.lock_dir):
+            util.verify_directory(self.lock_dir)
+
     def _open(self, mode):
         filedescriptor = self._filedesc
         if filedescriptor is None:
+            self._ensuredir()
             filedescriptor = os.open(self.filename, mode)
             self._filedescriptor.put(filedescriptor)
         return filedescriptor
 
     def do_acquire_read_lock(self, wait):
         filedescriptor = self._open(os.O_CREAT | os.O_RDONLY)
         if not wait:
@@ -282,15 +288,15 @@
 class ConditionSynchronizer(SynchronizerImpl):
     """a synchronizer using a Condition."""
 
     def __init__(self, identifier):
         super(ConditionSynchronizer, self).__init__()
 
         # counts how many asynchronous methods are executing
-        self.async = 0
+        self.asynch = 0
 
         # pointer to thread that is the current sync operation
         self.current_sync_operation = None
 
         # condition object to lock on
         self.condition = _threading.Condition(_threading.Lock())
 
@@ -303,34 +309,34 @@
             if wait:
                 while self.current_sync_operation is not None:
                     self.condition.wait()
             else:
                 if self.current_sync_operation is not None:
                     return False
 
-            self.async += 1
+            self.asynch += 1
         finally:
             self.condition.release()
 
         if not wait:
             return True
 
     def do_release_read_lock(self):
         self.condition.acquire()
         try:
-            self.async -= 1
+            self.asynch -= 1
 
             # check if we are the last asynchronous reader thread
             # out the door.
-            if self.async == 0:
+            if self.asynch == 0:
                 # yes. so if a sync operation is waiting, notifyAll to wake
                 # it up
                 if self.current_sync_operation is not None:
                     self.condition.notifyAll()
-            elif self.async < 0:
+            elif self.asynch < 0:
                 raise LockError("Synchronizer error - too many "
                                 "release_read_locks called")
         finally:
             self.condition.release()
 
     def do_acquire_write_lock(self, wait=True):
         self.condition.acquire()
@@ -350,15 +356,15 @@
 
             # establish ourselves as the current sync
             # this indicates to other read/write operations
             # that they should wait until this is None again
             self.current_sync_operation = _threading.currentThread()
 
             # now wait again for asyncs to finish
-            if self.async > 0:
+            if self.asynch > 0:
                 if wait:
                     # wait
                     self.condition.wait()
                 else:
                     # we dont want to wait, so forget it
                     self.current_sync_operation = None
                     return False
```

### Comparing `Beaker-1.9.0/beaker/util.py` & `Beaker-1.9.1/beaker/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -488,7 +488,20 @@
 def machine_identifier():
     machine_hash = hashlib.md5()
     if not PY2:
         machine_hash.update(socket.gethostname().encode())
     else:
         machine_hash.update(socket.gethostname())
     return binascii.hexlify(machine_hash.digest()[0:3]).decode('ascii')
+
+
+def safe_write (filepath, contents):
+    if os.name == 'posix':
+        tempname = '%s.temp' % (filepath)
+        fh = open(tempname, 'wb')
+        fh.write(contents)
+        fh.close()
+        os.rename(tempname, filepath)
+    else:
+        fh = open(filepath, 'wb')
+        fh.write(contents)
+        fh.close()
```

### Comparing `Beaker-1.9.0/Beaker.egg-info/PKG-INFO` & `Beaker-1.9.1/Beaker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Beaker
-Version: 1.9.0
+Version: 1.9.1
 Summary: A Session and Caching library with WSGI Middleware
 Home-page: https://beaker.readthedocs.io/
 Author: Ben Bangert, Mike Bayer, Philip Jenvey, Alessandro Molina
 Author-email: ben@groovie.org, pjenvey@groovie.org, amol@turbogears.org
 License: BSD
 Description: =========================
         Cache and Session Library
@@ -31,21 +31,21 @@
         
         Features
         ========
         
         * Fast, robust performance
         * Multiple reader/single writer lock system to avoid duplicate simultaneous
           cache creation
-        * Cache back-ends include dbm, file, memory, memcached, and database (Using
-          SQLAlchemy for multiple-db vendor support)
-        * Signed cookie's to prevent session hijacking/spoofing
+        * Cache back-ends include dbm, file, memory, memcached, Redis, MongoDB, and
+          database (Using SQLAlchemy for multiple-db vendor support)
+        * Signed cookies to prevent session hijacking/spoofing
         * Cookie-only sessions to remove the need for a db or file backend (ideal
           for clustered systems)
         * Extensible Container object to support new back-ends
-        * Cache's can be divided into namespaces (to represent templates, objects,
+        * Caches can be divided into namespaces (to represent templates, objects,
           etc.) then keyed for different copies
         * Create functions for automatic call-backs to create new cache copies after
           expiration
         * Fine-grained toggling of back-ends, keys, and expiration per Cache object
         
         
         Documentation
@@ -54,22 +54,22 @@
         Documentation can be found on the `Official Beaker Docs site
         <http://beaker.groovie.org/>`_.
         
         
         Source
         ======
         
-        The latest developer version is available in a `github repository
+        The latest developer version is available in a `GitHub repository
         <https://github.com/bbangert/beaker>`_.
         
         Contributing
         ============
         
-        Bugs can be filed on github, **should be accompanied by a test case** to
-        retain current code coverage, and should be in a Pull request when ready to be
+        Bugs can be filed on GitHub, **should be accompanied by a test case** to
+        retain current code coverage, and should be in a pull request when ready to be
         accepted into the beaker code-base.
         
 Keywords: wsgi myghty session web cache middleware
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -78,10 +78,14 @@
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
```

### Comparing `Beaker-1.9.0/Beaker.egg-info/SOURCES.txt` & `Beaker-1.9.1/Beaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Beaker-1.9.0/PKG-INFO` & `Beaker-1.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Beaker
-Version: 1.9.0
+Version: 1.9.1
 Summary: A Session and Caching library with WSGI Middleware
 Home-page: https://beaker.readthedocs.io/
 Author: Ben Bangert, Mike Bayer, Philip Jenvey, Alessandro Molina
 Author-email: ben@groovie.org, pjenvey@groovie.org, amol@turbogears.org
 License: BSD
 Description: =========================
         Cache and Session Library
@@ -31,21 +31,21 @@
         
         Features
         ========
         
         * Fast, robust performance
         * Multiple reader/single writer lock system to avoid duplicate simultaneous
           cache creation
-        * Cache back-ends include dbm, file, memory, memcached, and database (Using
-          SQLAlchemy for multiple-db vendor support)
-        * Signed cookie's to prevent session hijacking/spoofing
+        * Cache back-ends include dbm, file, memory, memcached, Redis, MongoDB, and
+          database (Using SQLAlchemy for multiple-db vendor support)
+        * Signed cookies to prevent session hijacking/spoofing
         * Cookie-only sessions to remove the need for a db or file backend (ideal
           for clustered systems)
         * Extensible Container object to support new back-ends
-        * Cache's can be divided into namespaces (to represent templates, objects,
+        * Caches can be divided into namespaces (to represent templates, objects,
           etc.) then keyed for different copies
         * Create functions for automatic call-backs to create new cache copies after
           expiration
         * Fine-grained toggling of back-ends, keys, and expiration per Cache object
         
         
         Documentation
@@ -54,22 +54,22 @@
         Documentation can be found on the `Official Beaker Docs site
         <http://beaker.groovie.org/>`_.
         
         
         Source
         ======
         
-        The latest developer version is available in a `github repository
+        The latest developer version is available in a `GitHub repository
         <https://github.com/bbangert/beaker>`_.
         
         Contributing
         ============
         
-        Bugs can be filed on github, **should be accompanied by a test case** to
-        retain current code coverage, and should be in a Pull request when ready to be
+        Bugs can be filed on GitHub, **should be accompanied by a test case** to
+        retain current code coverage, and should be in a pull request when ready to be
         accepted into the beaker code-base.
         
 Keywords: wsgi myghty session web cache middleware
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -78,10 +78,14 @@
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
```

### Comparing `Beaker-1.9.0/README.rst` & `Beaker-1.9.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
 Features
 ========
 
 * Fast, robust performance
 * Multiple reader/single writer lock system to avoid duplicate simultaneous
   cache creation
-* Cache back-ends include dbm, file, memory, memcached, and database (Using
-  SQLAlchemy for multiple-db vendor support)
-* Signed cookie's to prevent session hijacking/spoofing
+* Cache back-ends include dbm, file, memory, memcached, Redis, MongoDB, and
+  database (Using SQLAlchemy for multiple-db vendor support)
+* Signed cookies to prevent session hijacking/spoofing
 * Cookie-only sessions to remove the need for a db or file backend (ideal
   for clustered systems)
 * Extensible Container object to support new back-ends
-* Cache's can be divided into namespaces (to represent templates, objects,
+* Caches can be divided into namespaces (to represent templates, objects,
   etc.) then keyed for different copies
 * Create functions for automatic call-backs to create new cache copies after
   expiration
 * Fine-grained toggling of back-ends, keys, and expiration per Cache object
 
 
 Documentation
@@ -46,16 +46,16 @@
 Documentation can be found on the `Official Beaker Docs site
 <http://beaker.groovie.org/>`_.
 
 
 Source
 ======
 
-The latest developer version is available in a `github repository
+The latest developer version is available in a `GitHub repository
 <https://github.com/bbangert/beaker>`_.
 
 Contributing
 ============
 
-Bugs can be filed on github, **should be accompanied by a test case** to
-retain current code coverage, and should be in a Pull request when ready to be
+Bugs can be filed on GitHub, **should be accompanied by a test case** to
+retain current code coverage, and should be in a pull request when ready to be
 accepted into the beaker code-base.
```

### Comparing `Beaker-1.9.0/setup.py` & `Beaker-1.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,28 +19,37 @@
 
 INSTALL_REQUIRES = []
 if not hasattr(inspect, 'signature'):
     # On Python 2.6, 2.7 and 3.2 we need funcsigs dependency
     INSTALL_REQUIRES.append('funcsigs')
 
 
-TESTS_REQUIRE = ['nose', 'Mock', 'pycryptodome', 'cryptography']
+TESTS_REQUIRE = ['nose', 'Mock', 'pycryptodome']
 
 if py_version == (2, 6):
     TESTS_REQUIRE.append('WebTest<2.0.24')
 else:
     TESTS_REQUIRE.append('webtest')
 
 if py_version == (3, 2):
     TESTS_REQUIRE.append('coverage < 4.0')
 else:
     TESTS_REQUIRE.append('coverage')
 
+if py_version == (3, 3):
+    TESTS_REQUIRE.append('cryptography < 2.1.0')
+else:
+    TESTS_REQUIRE.append('cryptography')
+
 if not sys.platform.startswith('java') and not sys.platform == 'cli':
-    TESTS_REQUIRE.extend(['SQLALchemy', 'pymongo', 'redis'])
+    if py_version == (2, 6):
+        TESTS_REQUIRE.append('sqlalchemy < 1.2')
+    else:
+        TESTS_REQUIRE.append('sqlalchemy')
+    TESTS_REQUIRE.extend(['pymongo', 'redis'])
     try:
         import sqlite3
     except ImportError:
         TESTS_REQUIRE.append('pysqlite')
 
     if py_version[0] == 2:
         TESTS_REQUIRE.extend(['pylibmc', 'python-memcached'])
@@ -59,14 +68,18 @@
       'Programming Language :: Python :: 2.6',
       'Programming Language :: Python :: 2.7',
       'Programming Language :: Python :: 3',
       'Programming Language :: Python :: 3.2',
       'Programming Language :: Python :: 3.3',
       'Programming Language :: Python :: 3.4',
       'Programming Language :: Python :: 3.5',
+      'Programming Language :: Python :: 3.6',
+      'Programming Language :: Python :: 3.7',
+      'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
+      'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
       'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
       'Topic :: Internet :: WWW/HTTP :: WSGI',
       'Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware',
       ],
       keywords='wsgi myghty session web cache middleware',
       author='Ben Bangert, Mike Bayer, Philip Jenvey, Alessandro Molina',
       author_email='ben@groovie.org, pjenvey@groovie.org, amol@turbogears.org',
```

