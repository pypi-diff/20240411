# Comparing `tmp/dna_engine-1.0.2.tar.gz` & `tmp/dna_engine-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dna_engine-1.0.2.tar", last modified: Thu Apr 11 11:00:48 2024, max compression
+gzip compressed data, was "dna_engine-1.0.3.tar", last modified: Thu Apr 11 11:11:21 2024, max compression
```

## Comparing `dna_engine-1.0.2.tar` & `dna_engine-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 11:00:48.046718 dna_engine-1.0.2/
--rw-rw-rw-   0        0        0      609 2024-04-11 11:00:48.045300 dna_engine-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 dna_engine-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 11:00:47.970231 dna_engine-1.0.2/dna_engine/
--rw-rw-rw-   0        0        0      464 2023-10-09 13:45:02.000000 dna_engine-1.0.2/dna_engine/__init__.py
--rw-rw-rw-   0        0        0    21149 2023-10-09 14:12:15.000000 dna_engine-1.0.2/dna_engine/actor.py
--rw-rw-rw-   0        0        0     4860 2023-10-09 14:12:49.000000 dna_engine-1.0.2/dna_engine/audio_manager.py
--rw-rw-rw-   0        0        0     3196 2023-10-09 14:09:43.000000 dna_engine-1.0.2/dna_engine/background.py
--rw-rw-rw-   0        0        0    13485 2023-12-06 21:14:50.000000 dna_engine-1.0.2/dna_engine/game.py
--rw-rw-rw-   0        0        0     7100 2023-08-14 17:41:11.000000 dna_engine-1.0.2/dna_engine/input_manager.py
--rw-rw-rw-   0        0        0    11193 2023-12-05 20:27:47.000000 dna_engine-1.0.2/dna_engine/text.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:00:48.043049 dna_engine-1.0.2/dna_engine/tilemaps/
--rw-rw-rw-   0        0        0       74 2023-10-09 13:47:19.000000 dna_engine-1.0.2/dna_engine/tilemaps/__init__.py
--rw-rw-rw-   0        0        0     2140 2023-08-17 14:19:22.000000 dna_engine-1.0.2/dna_engine/tilemaps/tile.py
--rw-rw-rw-   0        0        0     3374 2023-10-09 13:47:41.000000 dna_engine-1.0.2/dna_engine/tilemaps/tile_map.py
--rw-rw-rw-   0        0        0    10407 2023-10-09 14:07:52.000000 dna_engine-1.0.2/dna_engine/world.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:00:47.987835 dna_engine-1.0.2/dna_engine.egg-info/
--rw-rw-rw-   0        0        0      609 2024-04-11 11:00:47.000000 dna_engine-1.0.2/dna_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-04-11 11:00:47.000000 dna_engine-1.0.2/dna_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 11:00:47.000000 dna_engine-1.0.2/dna_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-11 11:00:47.000000 dna_engine-1.0.2/dna_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-11 11:00:47.000000 dna_engine-1.0.2/dna_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 11:00:48.047250 dna_engine-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1153 2024-04-11 11:00:40.000000 dna_engine-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:11:21.605044 dna_engine-1.0.3/
+-rw-rw-rw-   0        0        0      609 2024-04-11 11:11:21.603450 dna_engine-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 dna_engine-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 11:11:21.567637 dna_engine-1.0.3/dna_engine/
+-rw-rw-rw-   0        0        0      464 2023-10-09 13:45:02.000000 dna_engine-1.0.3/dna_engine/__init__.py
+-rw-rw-rw-   0        0        0    21149 2023-10-09 14:12:15.000000 dna_engine-1.0.3/dna_engine/actor.py
+-rw-rw-rw-   0        0        0     4860 2023-10-09 14:12:49.000000 dna_engine-1.0.3/dna_engine/audio_manager.py
+-rw-rw-rw-   0        0        0     3196 2023-10-09 14:09:43.000000 dna_engine-1.0.3/dna_engine/background.py
+-rw-rw-rw-   0        0        0    13485 2023-12-06 21:14:50.000000 dna_engine-1.0.3/dna_engine/game.py
+-rw-rw-rw-   0        0        0     7100 2023-08-14 17:41:11.000000 dna_engine-1.0.3/dna_engine/input_manager.py
+-rw-rw-rw-   0        0        0    11193 2023-12-05 20:27:47.000000 dna_engine-1.0.3/dna_engine/text.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:11:21.599856 dna_engine-1.0.3/dna_engine/tilemaps/
+-rw-rw-rw-   0        0        0       74 2023-10-09 13:47:19.000000 dna_engine-1.0.3/dna_engine/tilemaps/__init__.py
+-rw-rw-rw-   0        0        0     2140 2023-08-17 14:19:22.000000 dna_engine-1.0.3/dna_engine/tilemaps/tile.py
+-rw-rw-rw-   0        0        0     3374 2023-10-09 13:47:41.000000 dna_engine-1.0.3/dna_engine/tilemaps/tile_map.py
+-rw-rw-rw-   0        0        0    10427 2024-04-11 11:10:24.000000 dna_engine-1.0.3/dna_engine/world.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:11:21.591875 dna_engine-1.0.3/dna_engine.egg-info/
+-rw-rw-rw-   0        0        0      609 2024-04-11 11:11:21.000000 dna_engine-1.0.3/dna_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-04-11 11:11:21.000000 dna_engine-1.0.3/dna_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 11:11:21.000000 dna_engine-1.0.3/dna_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-11 11:11:21.000000 dna_engine-1.0.3/dna_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-11 11:11:21.000000 dna_engine-1.0.3/dna_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 11:11:21.605044 dna_engine-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2024-04-11 11:11:05.000000 dna_engine-1.0.3/setup.py
```

### Comparing `dna_engine-1.0.2/PKG-INFO` & `dna_engine-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dna_engine
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyGame Abstraction Library
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pygame,game development,beginner,education
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dna_engine-1.0.2/dna_engine/actor.py` & `dna_engine-1.0.3/dna_engine/actor.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.2/dna_engine/audio_manager.py` & `dna_engine-1.0.3/dna_engine/audio_manager.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.2/dna_engine/background.py` & `dna_engine-1.0.3/dna_engine/background.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.2/dna_engine/game.py` & `dna_engine-1.0.3/dna_engine/game.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.2/dna_engine/input_manager.py` & `dna_engine-1.0.3/dna_engine/input_manager.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.2/dna_engine/text.py` & `dna_engine-1.0.3/dna_engine/text.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.2/dna_engine/tilemaps/tile.py` & `dna_engine-1.0.3/dna_engine/tilemaps/tile.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.2/dna_engine/tilemaps/tile_map.py` & `dna_engine-1.0.3/dna_engine/tilemaps/tile_map.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.2/dna_engine/world.py` & `dna_engine-1.0.3/dna_engine/world.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from pygame.surface import Surface
 
 
 from .game import Game
 from .tilemaps.tile import Tile
 from .background import Background
+from .text import Text
 
 
 class World(ABC):
     """
     The base class from which all user-defined Worlds should derive.
 	- All derived World classes must implement the Start() method. 
 	- Handles the updating and rendering of Actors automatically.
@@ -249,15 +250,15 @@
         # If a piece of Text already exists at this location, use that text object instead of creating a new one.
         for text in self.__text:
             if text.get_x() == x and text.get_y() == y:
                 text.set_message(message)
                 return
             
         # Otherwise, create a new Text object
-        self.add_text(dna.Text(message), x, y)
+        self.add_text(Text(message), x, y)
 
 
     def get_background(self) -> Background:
         """
         Gets the Background for this World.
 
         :return: The Background object used by this World, if one exists. Otherwise returns 'null'.
```

### Comparing `dna_engine-1.0.2/dna_engine.egg-info/PKG-INFO` & `dna_engine-1.0.3/dna_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dna-engine
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyGame Abstraction Library
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pygame,game development,beginner,education
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dna_engine-1.0.2/setup.py` & `dna_engine-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.2' 
+VERSION = '1.0.3' 
 DESCRIPTION = 'PyGame Abstraction Library'
 LONG_DESCRIPTION = 'A library of code which presents users with a simple, extensible program structure to make simple, 2D games with. Requires Python 3.10 or above.'
 
 # Setting up
 setup(
        # the name must match the folder name
         name="dna_engine",
```

