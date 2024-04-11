# Comparing `tmp/space_avenger-0.1.0.tar.gz` & `tmp/space_avenger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_avenger-0.1.0.tar", last modified: Thu Apr 11 11:02:03 2024, max compression
+gzip compressed data, was "space_avenger-0.1.2.tar", last modified: Thu Apr 11 11:12:46 2024, max compression
```

## Comparing `space_avenger-0.1.0.tar` & `space_avenger-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 haseeb    (1000) haseeb    (1000)        0 2024-04-11 11:02:03.915222 space_avenger-0.1.0/
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)       79 2024-04-11 10:58:07.000000 space_avenger-0.1.0/MANIFEST.in
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)      203 2024-04-11 11:02:03.915222 space_avenger-0.1.0/PKG-INFO
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)     2796 2024-04-09 09:38:06.000000 space_avenger-0.1.0/README.md
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)       38 2024-04-11 11:02:03.915222 space_avenger-0.1.0/setup.cfg
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)      675 2024-04-11 10:57:39.000000 space_avenger-0.1.0/setup.py
-drwxrwxr-x   0 haseeb    (1000) haseeb    (1000)        0 2024-04-11 11:02:03.911221 space_avenger-0.1.0/src/
-drwxrwxr-x   0 haseeb    (1000) haseeb    (1000)        0 2024-04-11 11:02:03.911221 space_avenger-0.1.0/src/space_avenger/
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)        0 2024-04-11 10:53:44.000000 space_avenger-0.1.0/src/space_avenger/__init__.py
-drwxrwxr-x   0 haseeb    (1000) haseeb    (1000)        0 2024-04-11 11:02:03.915222 space_avenger-0.1.0/src/space_avenger/assets/
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)  1140747 2024-03-06 21:42:59.000000 space_avenger-0.1.0/src/space_avenger/assets/background_music.mp3
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    68146 2024-03-06 21:01:24.000000 space_avenger-0.1.0/src/space_avenger/assets/bullet.png
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)     3866 2023-04-05 06:40:28.000000 space_avenger-0.1.0/src/space_avenger/assets/enemy-flyer.png
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)     5354 2023-04-05 06:40:28.000000 space_avenger-0.1.0/src/space_avenger/assets/enemy-seeker.png
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    99933 2023-04-05 06:40:28.000000 space_avenger-0.1.0/src/space_avenger/assets/explosion.png
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    42350 2024-03-06 21:44:27.000000 space_avenger-0.1.0/src/space_avenger/assets/explosion_sound.mp3
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    90669 2024-03-12 23:50:00.000000 space_avenger-0.1.0/src/space_avenger/assets/final-round.png
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    77459 2024-03-06 21:46:18.000000 space_avenger-0.1.0/src/space_avenger/assets/game_lose_sound.mp3
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    30230 2024-03-06 21:45:52.000000 space_avenger-0.1.0/src/space_avenger/assets/game_win_sound.mp3
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    31315 2023-04-05 06:40:28.000000 space_avenger-0.1.0/src/space_avenger/assets/message-lose.png
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    43995 2023-04-05 06:40:28.000000 space_avenger-0.1.0/src/space_avenger/assets/message-win.png
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    90366 2024-03-06 21:09:12.000000 space_avenger-0.1.0/src/space_avenger/assets/spaceship.png
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)   412644 2024-03-06 19:49:51.000000 space_avenger-0.1.0/src/space_avenger/assets/stars-bg.png
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    14848 2024-04-11 10:57:06.000000 space_avenger-0.1.0/src/space_avenger/space_avenger.py
-drwxrwxr-x   0 haseeb    (1000) haseeb    (1000)        0 2024-04-11 11:02:03.911221 space_avenger-0.1.0/src/space_avenger.egg-info/
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)      203 2024-04-11 11:02:03.000000 space_avenger-0.1.0/src/space_avenger.egg-info/PKG-INFO
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)      882 2024-04-11 11:02:03.000000 space_avenger-0.1.0/src/space_avenger.egg-info/SOURCES.txt
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)        1 2024-04-11 11:02:03.000000 space_avenger-0.1.0/src/space_avenger.egg-info/dependency_links.txt
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)       58 2024-04-11 11:02:03.000000 space_avenger-0.1.0/src/space_avenger.egg-info/entry_points.txt
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)        7 2024-04-11 11:02:03.000000 space_avenger-0.1.0/src/space_avenger.egg-info/requires.txt
--rw-rw-r--   0 haseeb    (1000) haseeb    (1000)       14 2024-04-11 11:02:03.000000 space_avenger-0.1.0/src/space_avenger.egg-info/top_level.txt
+drwxrwxr-x   0 haseeb    (1000) haseeb    (1000)        0 2024-04-11 11:12:46.907251 space_avenger-0.1.2/
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)       79 2024-04-11 10:58:07.000000 space_avenger-0.1.2/MANIFEST.in
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)      203 2024-04-11 11:12:46.907251 space_avenger-0.1.2/PKG-INFO
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)     2796 2024-04-09 09:38:06.000000 space_avenger-0.1.2/README.md
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)       38 2024-04-11 11:12:46.907251 space_avenger-0.1.2/setup.cfg
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)      675 2024-04-11 11:12:11.000000 space_avenger-0.1.2/setup.py
+drwxrwxr-x   0 haseeb    (1000) haseeb    (1000)        0 2024-04-11 11:12:46.903252 space_avenger-0.1.2/src/
+drwxrwxr-x   0 haseeb    (1000) haseeb    (1000)        0 2024-04-11 11:12:46.903252 space_avenger-0.1.2/src/space_avenger/
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)        0 2024-04-11 10:53:44.000000 space_avenger-0.1.2/src/space_avenger/__init__.py
+drwxrwxr-x   0 haseeb    (1000) haseeb    (1000)        0 2024-04-11 11:12:46.907251 space_avenger-0.1.2/src/space_avenger/assets/
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)  1140747 2024-03-06 21:42:59.000000 space_avenger-0.1.2/src/space_avenger/assets/background_music.mp3
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    68146 2024-03-06 21:01:24.000000 space_avenger-0.1.2/src/space_avenger/assets/bullet.png
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)     3866 2023-04-05 06:40:28.000000 space_avenger-0.1.2/src/space_avenger/assets/enemy-flyer.png
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)     5354 2023-04-05 06:40:28.000000 space_avenger-0.1.2/src/space_avenger/assets/enemy-seeker.png
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    99933 2023-04-05 06:40:28.000000 space_avenger-0.1.2/src/space_avenger/assets/explosion.png
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    42350 2024-03-06 21:44:27.000000 space_avenger-0.1.2/src/space_avenger/assets/explosion_sound.mp3
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    90669 2024-03-12 23:50:00.000000 space_avenger-0.1.2/src/space_avenger/assets/final-round.png
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    77459 2024-03-06 21:46:18.000000 space_avenger-0.1.2/src/space_avenger/assets/game_lose_sound.mp3
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    30230 2024-03-06 21:45:52.000000 space_avenger-0.1.2/src/space_avenger/assets/game_win_sound.mp3
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    31315 2023-04-05 06:40:28.000000 space_avenger-0.1.2/src/space_avenger/assets/message-lose.png
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    43995 2023-04-05 06:40:28.000000 space_avenger-0.1.2/src/space_avenger/assets/message-win.png
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    90366 2024-03-06 21:09:12.000000 space_avenger-0.1.2/src/space_avenger/assets/spaceship.png
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)   412644 2024-03-06 19:49:51.000000 space_avenger-0.1.2/src/space_avenger/assets/stars-bg.png
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)    14848 2024-04-11 11:07:49.000000 space_avenger-0.1.2/src/space_avenger/main.py
+drwxrwxr-x   0 haseeb    (1000) haseeb    (1000)        0 2024-04-11 11:12:46.903252 space_avenger-0.1.2/src/space_avenger.egg-info/
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)      203 2024-04-11 11:12:46.000000 space_avenger-0.1.2/src/space_avenger.egg-info/PKG-INFO
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)      873 2024-04-11 11:12:46.000000 space_avenger-0.1.2/src/space_avenger.egg-info/SOURCES.txt
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)        1 2024-04-11 11:12:46.000000 space_avenger-0.1.2/src/space_avenger.egg-info/dependency_links.txt
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)       58 2024-04-11 11:12:46.000000 space_avenger-0.1.2/src/space_avenger.egg-info/entry_points.txt
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)        7 2024-04-11 11:12:46.000000 space_avenger-0.1.2/src/space_avenger.egg-info/requires.txt
+-rw-rw-r--   0 haseeb    (1000) haseeb    (1000)       14 2024-04-11 11:12:46.000000 space_avenger-0.1.2/src/space_avenger.egg-info/top_level.txt
```

### Comparing `space_avenger-0.1.0/README.md` & `space_avenger-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/setup.py` & `space_avenger-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="space_avenger",
-    version="0.1.0",
+    version="0.1.2",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     install_requires=[
         'pygame',
     ],
     entry_points={
```

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/background_music.mp3` & `space_avenger-0.1.2/src/space_avenger/assets/background_music.mp3`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/bullet.png` & `space_avenger-0.1.2/src/space_avenger/assets/bullet.png`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/enemy-flyer.png` & `space_avenger-0.1.2/src/space_avenger/assets/enemy-flyer.png`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/enemy-seeker.png` & `space_avenger-0.1.2/src/space_avenger/assets/enemy-seeker.png`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/explosion.png` & `space_avenger-0.1.2/src/space_avenger/assets/explosion.png`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/explosion_sound.mp3` & `space_avenger-0.1.2/src/space_avenger/assets/explosion_sound.mp3`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/final-round.png` & `space_avenger-0.1.2/src/space_avenger/assets/final-round.png`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/game_lose_sound.mp3` & `space_avenger-0.1.2/src/space_avenger/assets/game_lose_sound.mp3`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/game_win_sound.mp3` & `space_avenger-0.1.2/src/space_avenger/assets/game_win_sound.mp3`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/message-lose.png` & `space_avenger-0.1.2/src/space_avenger/assets/message-lose.png`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/message-win.png` & `space_avenger-0.1.2/src/space_avenger/assets/message-win.png`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/spaceship.png` & `space_avenger-0.1.2/src/space_avenger/assets/spaceship.png`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/assets/stars-bg.png` & `space_avenger-0.1.2/src/space_avenger/assets/stars-bg.png`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger/space_avenger.py` & `space_avenger-0.1.2/src/space_avenger/main.py`

 * *Files identical despite different names*

### Comparing `space_avenger-0.1.0/src/space_avenger.egg-info/SOURCES.txt` & `space_avenger-0.1.2/src/space_avenger.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 MANIFEST.in
 README.md
 setup.py
 src/space_avenger/__init__.py
-src/space_avenger/space_avenger.py
+src/space_avenger/main.py
 src/space_avenger.egg-info/PKG-INFO
 src/space_avenger.egg-info/SOURCES.txt
 src/space_avenger.egg-info/dependency_links.txt
 src/space_avenger.egg-info/entry_points.txt
 src/space_avenger.egg-info/requires.txt
 src/space_avenger.egg-info/top_level.txt
 src/space_avenger/assets/background_music.mp3
```

