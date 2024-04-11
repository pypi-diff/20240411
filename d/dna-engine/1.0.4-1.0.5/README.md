# Comparing `tmp/dna_engine-1.0.4.tar.gz` & `tmp/dna_engine-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dna_engine-1.0.4.tar", last modified: Thu Apr 11 16:34:30 2024, max compression
+gzip compressed data, was "dna_engine-1.0.5.tar", last modified: Thu Apr 11 16:48:36 2024, max compression
```

## Comparing `dna_engine-1.0.4.tar` & `dna_engine-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 16:34:30.701445 dna_engine-1.0.4/
--rw-rw-rw-   0        0        0      609 2024-04-11 16:34:30.693015 dna_engine-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 dna_engine-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 16:34:30.614136 dna_engine-1.0.4/dna_engine/
--rw-rw-rw-   0        0        0      464 2023-10-09 13:45:02.000000 dna_engine-1.0.4/dna_engine/__init__.py
--rw-rw-rw-   0        0        0    21404 2024-04-11 16:29:54.000000 dna_engine-1.0.4/dna_engine/actor.py
--rw-rw-rw-   0        0        0     4860 2023-10-09 14:12:49.000000 dna_engine-1.0.4/dna_engine/audio_manager.py
--rw-rw-rw-   0        0        0     3196 2023-10-09 14:09:43.000000 dna_engine-1.0.4/dna_engine/background.py
--rw-rw-rw-   0        0        0    13485 2023-12-06 21:14:50.000000 dna_engine-1.0.4/dna_engine/game.py
--rw-rw-rw-   0        0        0     7100 2023-08-14 17:41:11.000000 dna_engine-1.0.4/dna_engine/input_manager.py
--rw-rw-rw-   0        0        0    11332 2024-04-11 16:32:50.000000 dna_engine-1.0.4/dna_engine/text.py
-drwxrwxrwx   0        0        0        0 2024-04-11 16:34:30.691484 dna_engine-1.0.4/dna_engine/tilemaps/
--rw-rw-rw-   0        0        0       74 2023-10-09 13:47:19.000000 dna_engine-1.0.4/dna_engine/tilemaps/__init__.py
--rw-rw-rw-   0        0        0     2140 2023-08-17 14:19:22.000000 dna_engine-1.0.4/dna_engine/tilemaps/tile.py
--rw-rw-rw-   0        0        0     3374 2023-10-09 13:47:41.000000 dna_engine-1.0.4/dna_engine/tilemaps/tile_map.py
--rw-rw-rw-   0        0        0    10427 2024-04-11 11:10:24.000000 dna_engine-1.0.4/dna_engine/world.py
-drwxrwxrwx   0        0        0        0 2024-04-11 16:34:30.641626 dna_engine-1.0.4/dna_engine.egg-info/
--rw-rw-rw-   0        0        0      609 2024-04-11 16:34:30.000000 dna_engine-1.0.4/dna_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-04-11 16:34:30.000000 dna_engine-1.0.4/dna_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 16:34:30.000000 dna_engine-1.0.4/dna_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-11 16:34:30.000000 dna_engine-1.0.4/dna_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-11 16:34:30.000000 dna_engine-1.0.4/dna_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 16:34:30.702511 dna_engine-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1173 2024-04-11 16:22:41.000000 dna_engine-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:48:36.969632 dna_engine-1.0.5/
+-rw-rw-rw-   0        0        0      609 2024-04-11 16:48:36.961936 dna_engine-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 dna_engine-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 16:48:36.927424 dna_engine-1.0.5/dna_engine/
+-rw-rw-rw-   0        0        0      464 2023-10-09 13:45:02.000000 dna_engine-1.0.5/dna_engine/__init__.py
+-rw-rw-rw-   0        0        0    21046 2024-04-11 16:47:42.000000 dna_engine-1.0.5/dna_engine/actor.py
+-rw-rw-rw-   0        0        0     4860 2023-10-09 14:12:49.000000 dna_engine-1.0.5/dna_engine/audio_manager.py
+-rw-rw-rw-   0        0        0     3196 2023-10-09 14:09:43.000000 dna_engine-1.0.5/dna_engine/background.py
+-rw-rw-rw-   0        0        0    13485 2023-12-06 21:14:50.000000 dna_engine-1.0.5/dna_engine/game.py
+-rw-rw-rw-   0        0        0     7100 2023-08-14 17:41:11.000000 dna_engine-1.0.5/dna_engine/input_manager.py
+-rw-rw-rw-   0        0        0    11332 2024-04-11 16:32:50.000000 dna_engine-1.0.5/dna_engine/text.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:48:36.957410 dna_engine-1.0.5/dna_engine/tilemaps/
+-rw-rw-rw-   0        0        0       74 2023-10-09 13:47:19.000000 dna_engine-1.0.5/dna_engine/tilemaps/__init__.py
+-rw-rw-rw-   0        0        0     2140 2023-08-17 14:19:22.000000 dna_engine-1.0.5/dna_engine/tilemaps/tile.py
+-rw-rw-rw-   0        0        0     3374 2023-10-09 13:47:41.000000 dna_engine-1.0.5/dna_engine/tilemaps/tile_map.py
+-rw-rw-rw-   0        0        0    10427 2024-04-11 11:10:24.000000 dna_engine-1.0.5/dna_engine/world.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:48:36.946982 dna_engine-1.0.5/dna_engine.egg-info/
+-rw-rw-rw-   0        0        0      609 2024-04-11 16:48:36.000000 dna_engine-1.0.5/dna_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-04-11 16:48:36.000000 dna_engine-1.0.5/dna_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 16:48:36.000000 dna_engine-1.0.5/dna_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-11 16:48:36.000000 dna_engine-1.0.5/dna_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-11 16:48:36.000000 dna_engine-1.0.5/dna_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 16:48:36.970759 dna_engine-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2024-04-11 16:48:17.000000 dna_engine-1.0.5/setup.py
```

### Comparing `dna_engine-1.0.4/PKG-INFO` & `dna_engine-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dna_engine
-Version: 1.0.4
+Version: 1.0.5
 Summary: PyGame Abstraction Library
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pygame,game development,beginner,education
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dna_engine-1.0.4/dna_engine/actor.py` & `dna_engine-1.0.5/dna_engine/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,24 +368,14 @@
         :type rotate_by: float
         """
         self.__rotation -= rotate_by
         if self.__rotation <= -360 or self.__rotation >= 360:
             self.__rotation = 0
         self.__generate_sprite()
 
-    @dispatch('Actor')
-    def look_at(self, look_at_object : Actor) -> None:
-        """
-        [Overload] Rotates this Actor to face a specific location on-screen.
-
-        :param look_at_object: The Actor which this Actor should face towards.
-        :type look_at_object: Actor
-        """
-        self.look_at(look_at_object.get_position())
-
 
     @dispatch(pygame.Vector2)
     def look_at(self, look_at_position : pygame.Vector2) -> None:
         """
         Rotates this Actor to face a specific location on-screen.
 
         :param look_at_position: The location on-screen that this Actor should face.
```

### Comparing `dna_engine-1.0.4/dna_engine/audio_manager.py` & `dna_engine-1.0.5/dna_engine/audio_manager.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.4/dna_engine/background.py` & `dna_engine-1.0.5/dna_engine/background.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.4/dna_engine/game.py` & `dna_engine-1.0.5/dna_engine/game.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.4/dna_engine/input_manager.py` & `dna_engine-1.0.5/dna_engine/input_manager.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.4/dna_engine/text.py` & `dna_engine-1.0.5/dna_engine/text.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.4/dna_engine/tilemaps/tile.py` & `dna_engine-1.0.5/dna_engine/tilemaps/tile.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.4/dna_engine/tilemaps/tile_map.py` & `dna_engine-1.0.5/dna_engine/tilemaps/tile_map.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.4/dna_engine/world.py` & `dna_engine-1.0.5/dna_engine/world.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.4/dna_engine.egg-info/PKG-INFO` & `dna_engine-1.0.5/dna_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dna-engine
-Version: 1.0.4
+Version: 1.0.5
 Summary: PyGame Abstraction Library
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pygame,game development,beginner,education
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dna_engine-1.0.4/setup.py` & `dna_engine-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.4' 
+VERSION = '1.0.5' 
 DESCRIPTION = 'PyGame Abstraction Library'
 LONG_DESCRIPTION = 'A library of code which presents users with a simple, extensible program structure to make simple, 2D games with. Requires Python 3.10 or above.'
 
 # Setting up
 setup(
        # the name must match the folder name
         name="dna_engine",
```

