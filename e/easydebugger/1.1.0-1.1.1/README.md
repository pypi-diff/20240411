# Comparing `tmp/easydebugger-1.1.0.tar.gz` & `tmp/easydebugger-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydebugger-1.1.0.tar", last modified: Thu Apr 11 10:34:55 2024, max compression
+gzip compressed data, was "easydebugger-1.1.1.tar", last modified: Thu Apr 11 13:33:24 2024, max compression
```

## Comparing `easydebugger-1.1.0.tar` & `easydebugger-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 10:34:55.594994 easydebugger-1.1.0/
--rw-rw-rw-   0        0        0    35823 2024-04-08 15:41:48.000000 easydebugger-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      259 2024-04-11 10:34:55.592991 easydebugger-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    15173 2024-04-11 10:32:10.000000 easydebugger-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 10:34:55.581020 easydebugger-1.1.0/easydebugger/
--rw-rw-rw-   0        0        0     6097 2024-04-11 10:29:43.000000 easydebugger-1.1.0/easydebugger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:34:55.590990 easydebugger-1.1.0/easydebugger.egg-info/
--rw-rw-rw-   0        0        0      259 2024-04-11 10:34:55.000000 easydebugger-1.1.0/easydebugger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-04-11 10:34:55.000000 easydebugger-1.1.0/easydebugger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 10:34:55.000000 easydebugger-1.1.0/easydebugger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-11 10:34:55.000000 easydebugger-1.1.0/easydebugger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 10:34:55.595993 easydebugger-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      522 2024-04-11 10:34:29.000000 easydebugger-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:33:24.520147 easydebugger-1.1.1/
+-rw-rw-rw-   0        0        0    35823 2024-04-08 15:41:48.000000 easydebugger-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      259 2024-04-11 13:33:24.517144 easydebugger-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    15173 2024-04-11 10:32:10.000000 easydebugger-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 13:33:24.498247 easydebugger-1.1.1/easydebugger/
+-rw-rw-rw-   0        0        0     6097 2024-04-11 13:31:36.000000 easydebugger-1.1.1/easydebugger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:33:24.516144 easydebugger-1.1.1/easydebugger.egg-info/
+-rw-rw-rw-   0        0        0      259 2024-04-11 13:33:24.000000 easydebugger-1.1.1/easydebugger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-04-11 13:33:24.000000 easydebugger-1.1.1/easydebugger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 13:33:24.000000 easydebugger-1.1.1/easydebugger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-11 13:33:24.000000 easydebugger-1.1.1/easydebugger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 13:33:24.520147 easydebugger-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      522 2024-04-11 13:32:04.000000 easydebugger-1.1.1/setup.py
```

### Comparing `easydebugger-1.1.0/LICENSE` & `easydebugger-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easydebugger-1.1.0/README.md` & `easydebugger-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `easydebugger-1.1.0/easydebugger/__init__.py` & `easydebugger-1.1.1/easydebugger/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,55 +77,55 @@
         if label:
             print((" " * indent * 3) + format_text(colour_code, f" {symbol} {label} ", True), message)
         else:
             print(format_text(colour_code, f" {symbol} ", True), message)
 
 
 def error(message, code=""):
-    caller_line_number = inspect.stack()[2].lineno
+    caller_line_number = inspect.stack()[1].lineno
     symbol = "!"
     colour = ERROR
     display_message(symbol, code, message, caller_line_number, colour)
     history_log(symbol, colour, message, code, caller_line_number)
 
 
 def warn(message, code=""):
-    caller_line_number = inspect.stack()[2].lineno
+    caller_line_number = inspect.stack()[1].lineno
     symbol = "*"
     colour = WARN
     display_message(symbol, code, message, caller_line_number, colour)
     history_log(symbol, colour, message, code, caller_line_number)
         
 
 def success(message, code=""):
-    caller_line_number = inspect.stack()[2].lineno
+    caller_line_number = inspect.stack()[1].lineno
     symbol = "+"
     colour = SUCCESS
     display_message(symbol, code, message, caller_line_number, colour)
     history_log(symbol, colour, message, code, caller_line_number)
         
 
 def variable(value, name):
-    caller_line_number = inspect.stack()[2].lineno
+    caller_line_number = inspect.stack()[1].lineno
     symbol = "$"
     colour = VARIABLE
     display_message(symbol, name, value, caller_line_number, colour)
     history_log(symbol, colour, value, name, caller_line_number)
 
 
 def log(message, label=""):
-    caller_line_number = inspect.stack()[2].lineno
+    caller_line_number = inspect.stack()[1].lineno
     symbol = "="
     colour = LOG
     display_message(symbol, label, message, caller_line_number, colour)
     history_log(symbol, colour, message, label, caller_line_number)
 
 
 def start_timer(code):
-    caller_line_number = inspect.stack()[2].lineno
+    caller_line_number = inspect.stack()[1].lineno
     symbol = "#"
     colour = TIME
     
     start_time = t.time()
     timers[code] = start_time
     
     message = "Started timing"
@@ -137,15 +137,15 @@
 def end_timer(code):
     end_time = t.time()
     
     symbol = "#"
     colour = TIME
     
     if code in timers:
-        caller_line_number = inspect.stack()[2].lineno
+        caller_line_number = inspect.stack()[1].lineno
         
         start_time = timers[code]
         timers.pop(code)
         
         duration_in_seconds = end_time - start_time
         duration_in_millis = duration_in_seconds * 1000
         
@@ -154,15 +154,15 @@
         display_message(symbol, code, message, caller_line_number, colour)
         history_log(symbol, colour, message, code, caller_line_number)        
     else:
         display_message(symbol, code, "Timer doesn't exist!", caller_line_number, colour)
 
 
 def trace():
-    caller_line_number = inspect.stack()[2].lineno
+    caller_line_number = inspect.stack()[1].lineno
     symbol = "@"
     colour = TRACE
     
     function_name = inspect.stack()[1].function
     
     if function_name in traces:
         traces.pop(traces.index(function_name))
```

### Comparing `easydebugger-1.1.0/setup.py` & `easydebugger-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = "easydebugger"
-VERSION = '1.1.0'
+VERSION = '1.1.1'
 DESCRIPTION = 'A clean Python debugging tool'
 LONG_DESCRIPTION = 'A clean Python debugging tool. Documentation at https://github.com/Blob2763/easydebugger'
 
 # Setting up
 setup(
     name=NAME,
     version=VERSION,
```

