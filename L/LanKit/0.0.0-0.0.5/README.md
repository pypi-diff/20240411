# Comparing `tmp/LanKit-0.0.0.tar.gz` & `tmp/LanKit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LanKit-0.0.0.tar", last modified: Tue Apr  9 16:47:39 2024, max compression
+gzip compressed data, was "LanKit-0.0.5.tar", last modified: Thu Apr 11 16:00:43 2024, max compression
```

## Comparing `LanKit-0.0.0.tar` & `LanKit-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:47:39.923610 LanKit-0.0.0/
--rw-rw-rw-   0        0        0     1083 2024-03-23 14:37:27.000000 LanKit-0.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-09 16:47:39.846395 LanKit-0.0.0/LanKit/
-drwxrwxrwx   0        0        0        0 2024-04-09 16:47:39.898749 LanKit-0.0.0/LanKit/Lexer/
--rw-rw-rw-   0        0        0     4179 2024-04-09 15:42:33.000000 LanKit-0.0.0/LanKit/Lexer/Lexer.py
--rw-rw-rw-   0        0        0     4729 2024-04-09 15:41:12.000000 LanKit-0.0.0/LanKit/Lexer/Lexer.pyi
--rw-rw-rw-   0        0        0       20 2024-03-19 11:02:35.000000 LanKit-0.0.0/LanKit/Lexer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:47:39.910639 LanKit-0.0.0/LanKit/Parser/
--rw-rw-rw-   0        0        0     3575 2024-04-09 14:15:47.000000 LanKit-0.0.0/LanKit/Parser/Parser.py
--rw-rw-rw-   0        0        0     6210 2024-04-09 14:16:02.000000 LanKit-0.0.0/LanKit/Parser/Parser.pyi
--rw-rw-rw-   0        0        0       21 2024-03-27 18:11:11.000000 LanKit-0.0.0/LanKit/Parser/__init__.py
--rw-rw-rw-   0        0        0      106 2024-04-09 15:43:18.000000 LanKit-0.0.0/LanKit/__init__.py
--rw-rw-rw-   0        0        0      146 2024-03-20 14:09:38.000000 LanKit-0.0.0/LanKit/errors.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:47:39.914611 LanKit-0.0.0/LanKit.egg-info/
--rw-rw-rw-   0        0        0     1864 2024-04-09 16:47:39.000000 LanKit-0.0.0/LanKit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-09 16:47:39.000000 LanKit-0.0.0/LanKit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:47:39.000000 LanKit-0.0.0/LanKit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 16:47:39.000000 LanKit-0.0.0/LanKit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1864 2024-04-09 16:47:39.920613 LanKit-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-18 16:12:27.000000 LanKit-0.0.0/README.md
--rw-rw-rw-   0        0        0      845 2024-04-09 16:47:28.000000 LanKit-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 16:47:39.924631 LanKit-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0       96 2024-03-27 16:48:41.000000 LanKit-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:00:43.077403 LanKit-0.0.5/
+-rw-rw-rw-   0        0        0     1083 2024-03-23 14:37:27.000000 LanKit-0.0.5/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-11 16:00:43.039167 LanKit-0.0.5/LanKit/
+drwxrwxrwx   0        0        0        0 2024-04-11 16:00:43.066360 LanKit-0.0.5/LanKit/Lexer/
+-rw-rw-rw-   0        0        0     4182 2024-04-10 19:32:02.000000 LanKit-0.0.5/LanKit/Lexer/Lexer.py
+-rw-rw-rw-   0        0        0     4877 2024-04-10 19:31:21.000000 LanKit-0.0.5/LanKit/Lexer/Lexer.pyi
+-rw-rw-rw-   0        0        0       20 2024-03-19 11:02:35.000000 LanKit-0.0.5/LanKit/Lexer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:00:43.072356 LanKit-0.0.5/LanKit/Parser/
+-rw-rw-rw-   0        0        0     3585 2024-04-10 19:04:45.000000 LanKit-0.0.5/LanKit/Parser/Parser.py
+-rw-rw-rw-   0        0        0     6454 2024-04-10 19:28:43.000000 LanKit-0.0.5/LanKit/Parser/Parser.pyi
+-rw-rw-rw-   0        0        0       21 2024-03-27 18:11:11.000000 LanKit-0.0.5/LanKit/Parser/__init__.py
+-rw-rw-rw-   0        0        0      128 2024-04-10 16:50:23.000000 LanKit-0.0.5/LanKit/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-03-20 14:09:38.000000 LanKit-0.0.5/LanKit/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:00:43.074356 LanKit-0.0.5/LanKit.egg-info/
+-rw-rw-rw-   0        0        0     1864 2024-04-11 16:00:42.000000 LanKit-0.0.5/LanKit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-11 16:00:43.000000 LanKit-0.0.5/LanKit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 16:00:42.000000 LanKit-0.0.5/LanKit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-11 16:00:42.000000 LanKit-0.0.5/LanKit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1864 2024-04-11 16:00:43.076357 LanKit-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-02-18 16:12:27.000000 LanKit-0.0.5/README.md
+-rw-rw-rw-   0        0        0      845 2024-04-10 19:35:35.000000 LanKit-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 16:00:43.078359 LanKit-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       96 2024-03-27 16:48:41.000000 LanKit-0.0.5/setup.py
```

### Comparing `LanKit-0.0.0/LICENSE` & `LanKit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `LanKit-0.0.0/LanKit/Lexer/Lexer.py` & `LanKit-0.0.5/LanKit/Lexer/Lexer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 
 from typing import Callable
-from LanKit.errors import *
+from LanKit_dev.LanKit.errors import *
 
 
 LEXER_RULE = dict[str, list[str]]
 LEXER_IGNORE = tuple[list[str]]
 
 # Номер символа в коде
 LEXING_ERROR_CHAR_NUMBER = int
@@ -25,15 +25,15 @@
         self.name = self.value = self.objMatch = None
 
 
 class Lexer:
     __slots__ = ('rules', 'ignore', 'code', 'errorHandler', 'iterRuleHandler', 'iterIgnoreHandler')
 
 
-    def __std_error_handler(error: LEXING_ERROR_CHAR_NUMBER):
+    def __std_error_handler(self, error: LEXING_ERROR_CHAR_NUMBER):
         print(error)
 
 
     def __init__(self, rules: LEXER_RULE, ignore=LEXER_IGNORE) -> None:
         self.rules = rules
         self.ignore = ignore
 
@@ -62,15 +62,15 @@
                 resultMatch = self.__match_ignore(self.code[charnum:])
 
             # Если результат есть
             if resultMatch:
                 charnum += resultMatch.regs[0][1]
 
             elif self.errorHandler:
-                self.errorHandler('хуй пососи')
+                self.errorHandler(charnum)
                 raise LexingError(charnum)
 
             else:
                 raise LexingError(charnum)
         
         return tokens
```

### Comparing `LanKit-0.0.0/LanKit/Lexer/Lexer.pyi` & `LanKit-0.0.5/LanKit/Lexer/Lexer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     value: str
     name: str
     objMatch: Match
 
 
 class NoneToken:
     """
-    Это токен (Token), но с константными, пустыми полями
+    * Это токен (Token), но с константными, пустыми полями
+    * Используется, как удобная для использования в match выражениях замена типу None
     """
     __slots__ = ('value', 'name', 'objMatch')
     name = None
     value = None
     objMatch = None
```

### Comparing `LanKit-0.0.0/LanKit/Parser/Parser.py` & `LanKit-0.0.5/LanKit/Parser/Parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from LanKit.Lexer import Token, NoneToken
+from LanKit_dev.LanKit.Lexer import Token, NoneToken
 
 
 class IsSet:
     def __init__(self) -> None:
         self.next: bool
 
 
@@ -73,15 +73,15 @@
 
 
     def jump(self, steps):
         self.pointer += steps
 
 
     def next(self, offset = 1):
-        if offset + self.pointer <= len(self.tokens):
+        if offset + self.pointer < len(self.tokens):
             self.isSet.next = True
             return self.tokens[offset + self.pointer]
         
         self.isSet.next = False
         return NoneToken()
```

### Comparing `LanKit-0.0.0/LanKit/Parser/Parser.pyi` & `LanKit-0.0.5/LanKit/Parser/Parser.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Предоставляет набор инструментов, для удобной
 реализации собственных парсеров
 """
 
-from typing import Any, Callable, Type, NamedTuple
+from typing import Any, Callable
 from LanKit.Lexer import Token, NoneToken
 from math import inf
 
 from abc import *
 
 
 PATTERN = list[Callable | str]
@@ -84,20 +84,19 @@
 
     # Инициализация
     testParser = Test()
     testParser.build(tokens)
     ```
     """
     def __init__(self, *args, **kwargs) -> None:
-        self.formList: list[Any]
-        self.pointer: int
-        self.isSet: IsSet
-        self.resultOffset: int
-        self.stopForm: bool
-        listNumber = 0
+        self.formList: list[Any]  # Результат форм
+        self.pointer: int  # Указатель на текущий токен
+        self.isSet: IsSet  # Информация о устанвках полей
+        self.resultOffset: int  # Результирующее смещение после form
+        self.notStopForm: bool  # Не выходить ли из парсинга паттерна? (form)
 
     @abstractmethod
     def build(self, tokens: list[Token]):
         """
         Запускает процесс парсинга
         """
```

### Comparing `LanKit-0.0.0/LanKit.egg-info/PKG-INFO` & `LanKit-0.0.5/LanKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LanKit
-Version: 0.0.0
+Version: 0.0.5
 Summary: Internal library of the Immeptor. Needed to create programming languages
 Author-email: Markada <markada.py@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Markada
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `LanKit-0.0.0/PKG-INFO` & `LanKit-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LanKit
-Version: 0.0.0
+Version: 0.0.5
 Summary: Internal library of the Immeptor. Needed to create programming languages
 Author-email: Markada <markada.py@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Markada
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `LanKit-0.0.0/pyproject.toml` & `LanKit-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LanKit"
-version = "0.0.0"
+version = "0.0.5"
 dependencies = []
 requires-python = ">=3.10"
 authors = [
   {name = "Markada", email = "markada.py@gmail.com"},
 ]
 description = "Internal library of the Immeptor. Needed to create programming languages"
 readme = "README.md"
```

