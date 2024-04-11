# Comparing `tmp/connect_four_lib-1.1.1.tar.gz` & `tmp/connect_four_lib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_four_lib-1.1.1.tar", max compression
+gzip compressed data, was "connect_four_lib-1.2.0.tar", max compression
```

## Comparing `connect_four_lib-1.1.1.tar` & `connect_four_lib-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0      472 2024-03-19 11:04:50.279681 connect_four_lib-1.1.1/README.md
--rw-r--r--   0        0        0      533 2024-03-19 11:04:50.279681 connect_four_lib-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-19 11:04:50.279681 connect_four_lib-1.1.1/src/connect_four_lib/__init__.py
--rw-r--r--   0        0        0       67 2024-03-19 11:04:50.279681 connect_four_lib-1.1.1/src/connect_four_lib/config.py
--rw-r--r--   0        0        0     3890 2024-03-19 11:04:50.279681 connect_four_lib-1.1.1/src/connect_four_lib/connect_four_engine.py
--rw-r--r--   0        0        0     2371 2024-03-19 11:04:50.279681 connect_four_lib-1.1.1/src/connect_four_lib/connect_four_heuristic.py
--rw-r--r--   0        0        0     4585 2024-03-19 11:04:50.279681 connect_four_lib-1.1.1/src/connect_four_lib/connect_four_judge.py
--rw-r--r--   0        0        0      571 2024-03-19 11:04:50.279681 connect_four_lib-1.1.1/src/connect_four_lib/game_state.py
--rw-r--r--   0        0        0     1233 2024-03-19 11:04:50.279681 connect_four_lib-1.1.1/src/connect_four_lib/judge.py
--rw-r--r--   0        0        0      643 2024-03-19 11:04:50.279681 connect_four_lib-1.1.1/src/connect_four_lib/point.py
--rw-r--r--   0        0        0      426 2024-03-19 11:04:50.279681 connect_four_lib-1.1.1/src/connect_four_lib/utils/speed.py
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 connect_four_lib-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      472 2024-04-11 14:47:55.886272 connect_four_lib-1.2.0/README.md
+-rw-r--r--   0        0        0      557 2024-04-11 14:47:55.886272 connect_four_lib-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 14:47:55.886272 connect_four_lib-1.2.0/src/connect_four_lib/__init__.py
+-rw-r--r--   0        0        0       67 2024-04-11 14:47:55.886272 connect_four_lib-1.2.0/src/connect_four_lib/config.py
+-rw-r--r--   0        0        0     3887 2024-04-11 14:47:55.890272 connect_four_lib-1.2.0/src/connect_four_lib/connect_four_engine.py
+-rw-r--r--   0        0        0     2371 2024-04-11 14:47:55.890272 connect_four_lib-1.2.0/src/connect_four_lib/connect_four_heuristic.py
+-rw-r--r--   0        0        0     4578 2024-04-11 14:47:55.890272 connect_four_lib-1.2.0/src/connect_four_lib/connect_four_judge.py
+-rw-r--r--   0        0        0      643 2024-04-11 14:47:55.890272 connect_four_lib-1.2.0/src/connect_four_lib/point.py
+-rw-r--r--   0        0        0      426 2024-04-11 14:47:55.890272 connect_four_lib-1.2.0/src/connect_four_lib/utils/speed.py
+-rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 connect_four_lib-1.2.0/PKG-INFO
```

### Comparing `connect_four_lib-1.1.1/pyproject.toml` & `connect_four_lib-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "connect-four-lib"
-version = "1.1.1"
+version = "1.2.0"
 description = "A library for connect 4 game"
 authors = ["game-ai-platform-team"]
 readme = "README.md"
 packages = [{ include = "connect_four_lib/**/*.py", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+duo-game-lib = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.12.1"
 isort = "^5.13.2"
 pylint = "^3.0.3"
 pytest = "^7.4.4"
 pytest-cov = "^4.1.0"
```

### Comparing `connect_four_lib-1.1.1/src/connect_four_lib/connect_four_engine.py` & `connect_four_lib-1.2.0/src/connect_four_lib/connect_four_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import random
 import time
 
+from duo_game_lib.game_state import GameState
+
 from connect_four_lib.config import INFINITY
 from connect_four_lib.connect_four_judge import ConnectFourJudge
-from connect_four_lib.game_state import GameState
 
 
 class ConnectFourEngine:
     def __init__(
         self,
         difficulty: int = 1000,
         judge: ConnectFourJudge | None = None,
```

### Comparing `connect_four_lib-1.1.1/src/connect_four_lib/connect_four_heuristic.py` & `connect_four_lib-1.2.0/src/connect_four_lib/connect_four_heuristic.py`

 * *Files identical despite different names*

### Comparing `connect_four_lib-1.1.1/src/connect_four_lib/connect_four_judge.py` & `connect_four_lib-1.2.0/src/connect_four_lib/connect_four_judge.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from duo_game_lib.game_state import GameState
+from duo_game_lib.judge import Judge
+
 from connect_four_lib.connect_four_heuristic import ConnectFourHeuristic
-from connect_four_lib.game_state import GameState
-from connect_four_lib.judge import Judge
 from connect_four_lib.point import Point
 
 
 class ConnectFourJudge(Judge):
     def __init__(
         self,
         moves: list[int] | None = None,
```

### Comparing `connect_four_lib-1.1.1/src/connect_four_lib/point.py` & `connect_four_lib-1.2.0/src/connect_four_lib/point.py`

 * *Files identical despite different names*

### Comparing `connect_four_lib-1.1.1/PKG-INFO` & `connect_four_lib-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: connect-four-lib
-Version: 1.1.1
+Version: 1.2.0
 Summary: A library for connect 4 game
 Author: game-ai-platform-team
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: duo-game-lib (>=0.1.0,<0.2.0)
 Description-Content-Type: text/markdown
 
 # connect-four-lib
 
 [![codecov](https://codecov.io/gh/game-ai-platform-team/connect-four-lib/graph/badge.svg?token=MNLla272Cv)](https://codecov.io/gh/game-ai-platform-team/connect-four-lib)
 [![CI/CD](https://github.com/game-ai-platform-team/connect-four-lib/actions/workflows/cicd.yml/badge.svg)](https://github.com/game-ai-platform-team/connect-four-lib/actions/workflows/cicd.yml)
```

