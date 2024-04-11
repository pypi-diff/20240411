# Comparing `tmp/dna_engine-1.0.3.tar.gz` & `tmp/dna_engine-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dna_engine-1.0.3.tar", last modified: Thu Apr 11 11:11:21 2024, max compression
+gzip compressed data, was "dna_engine-1.0.4.tar", last modified: Thu Apr 11 16:34:30 2024, max compression
```

## Comparing `dna_engine-1.0.3.tar` & `dna_engine-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 11:11:21.605044 dna_engine-1.0.3/
--rw-rw-rw-   0        0        0      609 2024-04-11 11:11:21.603450 dna_engine-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 dna_engine-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 11:11:21.567637 dna_engine-1.0.3/dna_engine/
--rw-rw-rw-   0        0        0      464 2023-10-09 13:45:02.000000 dna_engine-1.0.3/dna_engine/__init__.py
--rw-rw-rw-   0        0        0    21149 2023-10-09 14:12:15.000000 dna_engine-1.0.3/dna_engine/actor.py
--rw-rw-rw-   0        0        0     4860 2023-10-09 14:12:49.000000 dna_engine-1.0.3/dna_engine/audio_manager.py
--rw-rw-rw-   0        0        0     3196 2023-10-09 14:09:43.000000 dna_engine-1.0.3/dna_engine/background.py
--rw-rw-rw-   0        0        0    13485 2023-12-06 21:14:50.000000 dna_engine-1.0.3/dna_engine/game.py
--rw-rw-rw-   0        0        0     7100 2023-08-14 17:41:11.000000 dna_engine-1.0.3/dna_engine/input_manager.py
--rw-rw-rw-   0        0        0    11193 2023-12-05 20:27:47.000000 dna_engine-1.0.3/dna_engine/text.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:11:21.599856 dna_engine-1.0.3/dna_engine/tilemaps/
--rw-rw-rw-   0        0        0       74 2023-10-09 13:47:19.000000 dna_engine-1.0.3/dna_engine/tilemaps/__init__.py
--rw-rw-rw-   0        0        0     2140 2023-08-17 14:19:22.000000 dna_engine-1.0.3/dna_engine/tilemaps/tile.py
--rw-rw-rw-   0        0        0     3374 2023-10-09 13:47:41.000000 dna_engine-1.0.3/dna_engine/tilemaps/tile_map.py
--rw-rw-rw-   0        0        0    10427 2024-04-11 11:10:24.000000 dna_engine-1.0.3/dna_engine/world.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:11:21.591875 dna_engine-1.0.3/dna_engine.egg-info/
--rw-rw-rw-   0        0        0      609 2024-04-11 11:11:21.000000 dna_engine-1.0.3/dna_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-04-11 11:11:21.000000 dna_engine-1.0.3/dna_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 11:11:21.000000 dna_engine-1.0.3/dna_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-11 11:11:21.000000 dna_engine-1.0.3/dna_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-11 11:11:21.000000 dna_engine-1.0.3/dna_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 11:11:21.605044 dna_engine-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1153 2024-04-11 11:11:05.000000 dna_engine-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:34:30.701445 dna_engine-1.0.4/
+-rw-rw-rw-   0        0        0      609 2024-04-11 16:34:30.693015 dna_engine-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-15 14:37:57.000000 dna_engine-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 16:34:30.614136 dna_engine-1.0.4/dna_engine/
+-rw-rw-rw-   0        0        0      464 2023-10-09 13:45:02.000000 dna_engine-1.0.4/dna_engine/__init__.py
+-rw-rw-rw-   0        0        0    21404 2024-04-11 16:29:54.000000 dna_engine-1.0.4/dna_engine/actor.py
+-rw-rw-rw-   0        0        0     4860 2023-10-09 14:12:49.000000 dna_engine-1.0.4/dna_engine/audio_manager.py
+-rw-rw-rw-   0        0        0     3196 2023-10-09 14:09:43.000000 dna_engine-1.0.4/dna_engine/background.py
+-rw-rw-rw-   0        0        0    13485 2023-12-06 21:14:50.000000 dna_engine-1.0.4/dna_engine/game.py
+-rw-rw-rw-   0        0        0     7100 2023-08-14 17:41:11.000000 dna_engine-1.0.4/dna_engine/input_manager.py
+-rw-rw-rw-   0        0        0    11332 2024-04-11 16:32:50.000000 dna_engine-1.0.4/dna_engine/text.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:34:30.691484 dna_engine-1.0.4/dna_engine/tilemaps/
+-rw-rw-rw-   0        0        0       74 2023-10-09 13:47:19.000000 dna_engine-1.0.4/dna_engine/tilemaps/__init__.py
+-rw-rw-rw-   0        0        0     2140 2023-08-17 14:19:22.000000 dna_engine-1.0.4/dna_engine/tilemaps/tile.py
+-rw-rw-rw-   0        0        0     3374 2023-10-09 13:47:41.000000 dna_engine-1.0.4/dna_engine/tilemaps/tile_map.py
+-rw-rw-rw-   0        0        0    10427 2024-04-11 11:10:24.000000 dna_engine-1.0.4/dna_engine/world.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:34:30.641626 dna_engine-1.0.4/dna_engine.egg-info/
+-rw-rw-rw-   0        0        0      609 2024-04-11 16:34:30.000000 dna_engine-1.0.4/dna_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-04-11 16:34:30.000000 dna_engine-1.0.4/dna_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 16:34:30.000000 dna_engine-1.0.4/dna_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-11 16:34:30.000000 dna_engine-1.0.4/dna_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-11 16:34:30.000000 dna_engine-1.0.4/dna_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 16:34:30.702511 dna_engine-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2024-04-11 16:22:41.000000 dna_engine-1.0.4/setup.py
```

### Comparing `dna_engine-1.0.3/PKG-INFO` & `dna_engine-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dna_engine
-Version: 1.0.3
+Version: 1.0.4
 Summary: PyGame Abstraction Library
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pygame,game development,beginner,education
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dna_engine-1.0.3/dna_engine/actor.py` & `dna_engine-1.0.4/dna_engine/actor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import pygame;
 from math import atan2, pi
 from abc import ABC, abstractmethod
-from typing import overload
+from multipledispatch import dispatch
 from pygame.surface import Surface
 from pygame.locals import (RLEACCEL);
 
 import dna_engine as dna
 
 from . import game
 
@@ -224,76 +224,78 @@
             bounds = self.get_bounds()
             hit = self.get_world()._World__get_tile_map()._TileMap__get_tile_on_screen(bounds.centerx + x_offset, bounds.centery + y_offset)
             return hit
         
         return None
     
 
-    @overload
+    @dispatch(pygame.Vector2)
     def move(self, move_by : pygame.Vector2) -> None:
         """
         [Overload] Moves this Actor by the given amount.
 
         :param move_by: The x and y-axis co-ordinates this Actor should move by.
         :type move_by: pygame.Vector2
         """
         self.move(move_by[0], move_by[1])
 
 
-    @overload
+    @dispatch(int, int)
     def move(self, move_by_x : int, move_by_y : int) -> None:
         """
         [Overload] Moves this Actor by the given amount.
 
         :param move_by_x: The x-axis (horizontal) number of pixels to move by.
         :type move_by_x: int
         :param move_by_y: The y-axis (vertical) number of pixels to move by.
         :type move_by_y: int
         """
         self.move(float(move_by_x), float(move_by_y))
 
 
+    @dispatch(float, float)
     def move(self, move_by_x : float, move_by_y : float) -> None:
         """
         Moves this Actor by the given amount.
 
         :param move_by_x: The x-axis (horizontal) number of pixels to move by.
         :type move_by_x: float
 
         :param move_by_y: The y-axis (vertical) number of pixels to move by.
         :type move_by_y: float
         """
         self.__rect.move_ip(move_by_x, move_by_y);
         self.__position = self.__rect.center
     
 
-    @overload
+    @dispatch(int, int)
     def set_position(self, new_x : int, new_y : int) -> None:
         """
         [Overload] Sets the on-screen location of this Actor to the given co-ordinates.
 
         :param new_x: The horizontal (x-axis) co-ordinate of the desired new location.
         :type new_x: int
         :param new_y: The vertical (y-axis) co-ordinate of the desired new location.
         :type new_y: int
         """
         self.set_position(float(new_x), float(new_y))
     
 
-    @overload
+    @dispatch(pygame.Vector2)
     def set_position(self, new_position : pygame.Vector2) -> None:
         """
         [Overload] Sets the on-screen location of this Actor to the given co-ordinates.
 
         :param new_position: The x and y-axis co-ordinates this Actor should be set to.
         :type new_position: pygame.Vector2
         """
         self.set_position(new_position[0], new_position[1])
     
 
+    @dispatch(float, float)
     def set_position(self, new_x : float, new_y : float) -> None:
         """
         Sets the on-screen location of this Actor to the given co-ordinates.
 
         :param new_x: The horizontal (x-axis) co-ordinate of the desired new location.
         :type new_x: float
 
@@ -366,25 +368,26 @@
         :type rotate_by: float
         """
         self.__rotation -= rotate_by
         if self.__rotation <= -360 or self.__rotation >= 360:
             self.__rotation = 0
         self.__generate_sprite()
 
-    @overload
+    @dispatch('Actor')
     def look_at(self, look_at_object : Actor) -> None:
         """
         [Overload] Rotates this Actor to face a specific location on-screen.
 
         :param look_at_object: The Actor which this Actor should face towards.
         :type look_at_object: Actor
         """
         self.look_at(look_at_object.get_position())
 
 
+    @dispatch(pygame.Vector2)
     def look_at(self, look_at_position : pygame.Vector2) -> None:
         """
         Rotates this Actor to face a specific location on-screen.
 
         :param look_at_position: The location on-screen that this Actor should face.
         :type look_at_position: pygame.Vector2
         """
@@ -458,15 +461,15 @@
             self.__raw_image.set_colorkey((255,255,255), RLEACCEL)
             self.__rect = self.__raw_image.get_rect()
         except FileNotFoundError as err:
             raise FileNotFoundError(err)
 
         self.__generate_sprite()
 
-    @overload
+    @dispatch(int, int, int, int, int)
     def set_image_rect(self, width : int, height : int, red : int, green : int, blue : int) -> None:
         """
         [Overload] Sets this Actor's image to a new coloured rectangle.
 
         :param width: The width, in pixels, of the desired rectangle shape.
         :type width: int
 
@@ -484,15 +487,15 @@
         """
         red = max(0, min(red, 255))
         green = max(0, min(green, 255))
         blue = max(0, min(blue, 255))
         self.set_image_rect(width, height, pygame.Color(red, green, blue))
 
 
-    @overload
+    @dispatch(int, int, list[int, int, int])
     def set_image_rect(self, width : int, height : int, colour : list[int, int, int]) -> None:
         """
         [Overload] Sets this Actor's image to a new coloured rectangle.
 
         :param width: The width, in pixels, of the desired rectangle shape.
         :type width: int
 
@@ -507,14 +510,15 @@
 
         colour[0] = max(0, min(colour[0], 255))
         colour[1] = max(0, min(colour[1], 255))
         colour[2] = max(0, min(colour[2], 255))
         self.set_image_rect(width, height, pygame.Color(colour[0], colour[1], colour[2]))
 
 
+    @dispatch(int, int, pygame.Color)
     def set_image_rect(self, width : int, height : int, colour : pygame.Color) -> None:
         """
         Sets this Actor's image to a new coloured rectangle.
 
         :param width: The width, in pixels, of the desired rectangle shape.
         :type width: int
```

### Comparing `dna_engine-1.0.3/dna_engine/audio_manager.py` & `dna_engine-1.0.4/dna_engine/audio_manager.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.3/dna_engine/background.py` & `dna_engine-1.0.4/dna_engine/background.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.3/dna_engine/game.py` & `dna_engine-1.0.4/dna_engine/game.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.3/dna_engine/input_manager.py` & `dna_engine-1.0.4/dna_engine/input_manager.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.3/dna_engine/text.py` & `dna_engine-1.0.4/dna_engine/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pygame
 from pygame.surface import Surface
 from pygame.rect import Rect
 
 from typing import overload
+from multipledispatch import dispatch
 import typing
 
 class Text():
     """
     The class which handles the rendering of text to the game screen.
 	- Supports system fonts and local fonts.
 	- Text can be scaled, rotated and positioned similarly to Actors.
@@ -58,39 +59,40 @@
             self.__surface, self.__rect = self.__font.render(self.__message, self.__colour, size=int(self.__font.size * self.__scale));
 
             self.__rect.x = x;
             self.__rect.y = y;
             self.__generate_render()
 
 
-    @overload
+    @dispatch(pygame.Vector2)
     def set_position(self, new_position : pygame.Vector2) -> None:
         """
         [Overload] Sets the on-screen location of this Text to the given co-ordinates.
 
         :param new_position: The horizontal (x-axis) and vertical (y_axis) co-ordinates of the desired new location.
         :type new_position: pygame.Vector2
         """
         self.set_position(new_position[0], new_position[1])
 
 
-    @overload
+    @dispatch(int, int)
     def set_position(self, new_x : int, new_y : int) -> None:
         """
         [Overload] Sets the on-screen location of this Text to the given co-ordinates.
 
         :param new_x: The horizontal (x-axis) co-ordinate of the desired new location.
         :type new_x: int
 
         :param new_y: The vertical (y-axis) co-ordinate of the desired new location.
         :type new_y: int
         """
         self.set_position(float(new_x), float(new_y))
 
 
+    @dispatch(float, float)
     def set_position(self, new_x : float, new_y : float) -> None:
         """
         Sets the on-screen location of this Text to the given co-ordinates.
 
         :param new_x: The horizontal (x-axis) co-ordinate of the desired new location.
         :type new_x: float
 
@@ -136,27 +138,28 @@
 
         :return: A floating-point value representing the y-axis co-ordinate of this Text.
         :rtype: float
         """
         return self.__position[1]
 
 
-    @overload
+    @dispatch(float, float)
     def set_origin(self, origin_x : float, origin_y : float) -> None:
         """
         [Overload] Sets the rendering origin of this Text. Values are clamped between 0.0 and 1.0.
 
         :param origin_x: The horizontal fractional co-ordinate of this Text's origin point.
         :type origin_x: float
         :param origin_y: The vertical fractional co-ordinate of this Text's origin point.
         :type origin_y: float
         """
         self.set_origin(pygame.Vector2(origin_x, origin_y))
 
 
+    @dispatch(pygame.Vector2)
     def set_origin(self, new_origin : pygame.Vector2) -> None:
         """
         Sets the rendering origin of this Text. Values are clamped between 0.0 and 1.0.
 
         :param new_origin: The horizontal and vertical fractional origin point of this Text.
         :type new_origin: pygame.Vector2
         """
```

### Comparing `dna_engine-1.0.3/dna_engine/tilemaps/tile.py` & `dna_engine-1.0.4/dna_engine/tilemaps/tile.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.3/dna_engine/tilemaps/tile_map.py` & `dna_engine-1.0.4/dna_engine/tilemaps/tile_map.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.3/dna_engine/world.py` & `dna_engine-1.0.4/dna_engine/world.py`

 * *Files identical despite different names*

### Comparing `dna_engine-1.0.3/dna_engine.egg-info/PKG-INFO` & `dna_engine-1.0.4/dna_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dna-engine
-Version: 1.0.3
+Version: 1.0.4
 Summary: PyGame Abstraction Library
 Author: Liam Burns
 Author-email: l.burns@dundeeandangus.ac.uk
 Keywords: python,pygame,game development,beginner,education
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dna_engine-1.0.3/setup.py` & `dna_engine-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.3' 
+VERSION = '1.0.4' 
 DESCRIPTION = 'PyGame Abstraction Library'
 LONG_DESCRIPTION = 'A library of code which presents users with a simple, extensible program structure to make simple, 2D games with. Requires Python 3.10 or above.'
 
 # Setting up
 setup(
        # the name must match the folder name
         name="dna_engine", 
         version=VERSION,
         author="Liam Burns",
         author_email="l.burns@dundeeandangus.ac.uk",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['pygame', 'pyinstaller'], # add any additional packages that 
+        install_requires=['pygame', 'pyinstaller', 'multipledispatch'], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'       
         
         keywords=['python', 'pygame', 'game development', 'beginner', 'education'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 3",
```

