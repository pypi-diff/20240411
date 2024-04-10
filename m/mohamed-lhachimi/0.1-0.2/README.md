# Comparing `tmp/mohamed_lhachimi-0.1.tar.gz` & `tmp/mohamed_lhachimi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mohamed_lhachimi-0.1.tar", last modified: Wed Apr 10 21:36:19 2024, max compression
+gzip compressed data, was "mohamed_lhachimi-0.2.tar", last modified: Wed Apr 10 22:05:14 2024, max compression
```

## Comparing `mohamed_lhachimi-0.1.tar` & `mohamed_lhachimi-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 21:36:19.392896 mohamed_lhachimi-0.1/
--rw-rw-rw-   0        0        0      149 2024-04-10 21:36:19.390884 mohamed_lhachimi-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-10 21:24:27.000000 mohamed_lhachimi-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 21:36:19.377508 mohamed_lhachimi-0.1/mohamed_lhachimi/
--rw-rw-rw-   0        0        0       18 2024-04-10 21:29:47.000000 mohamed_lhachimi-0.1/mohamed_lhachimi/__init__.py
--rw-rw-rw-   0        0        0     1724 2024-04-10 21:21:14.000000 mohamed_lhachimi-0.1/mohamed_lhachimi/main.py
-drwxrwxrwx   0        0        0        0 2024-04-10 21:36:19.388879 mohamed_lhachimi-0.1/mohamed_lhachimi.egg-info/
--rw-rw-rw-   0        0        0      149 2024-04-10 21:36:19.000000 mohamed_lhachimi-0.1/mohamed_lhachimi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-04-10 21:36:19.000000 mohamed_lhachimi-0.1/mohamed_lhachimi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 21:36:19.000000 mohamed_lhachimi-0.1/mohamed_lhachimi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-10 21:36:19.000000 mohamed_lhachimi-0.1/mohamed_lhachimi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 21:36:19.392896 mohamed_lhachimi-0.1/setup.cfg
--rw-rw-rw-   0        0        0      219 2024-04-10 21:34:48.000000 mohamed_lhachimi-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 22:05:14.377231 mohamed_lhachimi-0.2/
+-rw-rw-rw-   0        0        0      267 2024-04-10 22:05:14.376232 mohamed_lhachimi-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2024-04-10 22:05:06.000000 mohamed_lhachimi-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 22:05:14.365841 mohamed_lhachimi-0.2/mohamed_lhachimi/
+-rw-rw-rw-   0        0        0       18 2024-04-10 21:29:47.000000 mohamed_lhachimi-0.2/mohamed_lhachimi/__init__.py
+-rw-rw-rw-   0        0        0     1724 2024-04-10 21:21:14.000000 mohamed_lhachimi-0.2/mohamed_lhachimi/main.py
+drwxrwxrwx   0        0        0        0 2024-04-10 22:05:14.370375 mohamed_lhachimi-0.2/mohamed_lhachimi.egg-info/
+-rw-rw-rw-   0        0        0      267 2024-04-10 22:05:14.000000 mohamed_lhachimi-0.2/mohamed_lhachimi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-04-10 22:05:14.000000 mohamed_lhachimi-0.2/mohamed_lhachimi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 22:05:14.000000 mohamed_lhachimi-0.2/mohamed_lhachimi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-10 22:05:14.000000 mohamed_lhachimi-0.2/mohamed_lhachimi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 22:05:14.377231 mohamed_lhachimi-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      431 2024-04-10 22:04:33.000000 mohamed_lhachimi-0.2/setup.py
```

### Comparing `mohamed_lhachimi-0.1/mohamed_lhachimi/main.py` & `mohamed_lhachimi-0.2/mohamed_lhachimi/main.py`

 * *Files identical despite different names*

