# Comparing `tmp/easydebugger-1.0.1.tar.gz` & `tmp/easydebugger-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydebugger-1.0.1.tar", last modified: Sun Apr  7 21:08:23 2024, max compression
+gzip compressed data, was "easydebugger-1.1.0.tar", last modified: Thu Apr 11 10:34:55 2024, max compression
```

## Comparing `easydebugger-1.0.1.tar` & `easydebugger-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 21:08:23.490339 easydebugger-1.0.1/
--rw-rw-rw-   0        0        0    35823 2024-04-07 16:20:32.000000 easydebugger-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      259 2024-04-07 21:08:23.485353 easydebugger-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    12460 2024-04-07 21:07:02.000000 easydebugger-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 21:08:23.430386 easydebugger-1.0.1/easydebugger/
--rw-rw-rw-   0        0        0     6105 2024-04-07 15:16:44.000000 easydebugger-1.0.1/easydebugger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:08:23.482187 easydebugger-1.0.1/easydebugger.egg-info/
--rw-rw-rw-   0        0        0      259 2024-04-07 21:08:23.000000 easydebugger-1.0.1/easydebugger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-04-07 21:08:23.000000 easydebugger-1.0.1/easydebugger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 21:08:23.000000 easydebugger-1.0.1/easydebugger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-07 21:08:23.000000 easydebugger-1.0.1/easydebugger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 21:08:23.491339 easydebugger-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      509 2024-04-07 21:08:04.000000 easydebugger-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:34:55.594994 easydebugger-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2024-04-08 15:41:48.000000 easydebugger-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      259 2024-04-11 10:34:55.592991 easydebugger-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    15173 2024-04-11 10:32:10.000000 easydebugger-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 10:34:55.581020 easydebugger-1.1.0/easydebugger/
+-rw-rw-rw-   0        0        0     6097 2024-04-11 10:29:43.000000 easydebugger-1.1.0/easydebugger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:34:55.590990 easydebugger-1.1.0/easydebugger.egg-info/
+-rw-rw-rw-   0        0        0      259 2024-04-11 10:34:55.000000 easydebugger-1.1.0/easydebugger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-04-11 10:34:55.000000 easydebugger-1.1.0/easydebugger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 10:34:55.000000 easydebugger-1.1.0/easydebugger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-11 10:34:55.000000 easydebugger-1.1.0/easydebugger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 10:34:55.595993 easydebugger-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      522 2024-04-11 10:34:29.000000 easydebugger-1.1.0/setup.py
```

### Comparing `easydebugger-1.0.1/LICENSE` & `easydebugger-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easydebugger-1.0.1/README.md` & `easydebugger-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # easydebugger
-
 a Python debugging tool made by blob2763
 
+[![PyPI](https://img.shields.io/pypi/v/easydebugger?label=pypi)](https://pypi.org/project/easydebugger/)
+[![Downloads](https://pepy.tech/badge/easydebugger)](https://www.pepy.tech/projects/easydebugger)
+
+
 ## setting it up
 simple stuff for installing any library
 
 ### 1. installation
 install the library using `pip install easydebugger`
 
 ### 2. importing the library
@@ -90,16 +93,14 @@
 ```
 
 | parameter | required | default | description          |
 |-----------|----------|---------|----------------------|
 | `value`   | yes      | N/A     | the variable's value |
 | `name`    | yes      | N/A     | the variable's name  |
 
-in the future, i might add functionality to detect the variable name automatically. there will be be a way to override this because the detection is not always accurate
-
 ### timers
 you can time how long code takes to run using `ed.start_timer()` and `ed.end_timer()`
 
 ```py
 import easydebugger as ed
 import time as t
 
@@ -319,15 +320,64 @@
 ![image](https://github.com/Blob2763/easydebugger/assets/88489444/9aa1476e-1bd9-4fe7-bda4-dc64556d2591)
 
 #### parameters
 ```py
 ed.display_message(symbol, label, message, line_number, colour_code, indent)
 ```
 
-| parameter     | required | default  | description                                                                                                                   |
-|---------------|----------|--------- |-------------------------------------------------------------------------------------------------------------------------------|
-| `symbol`      | yes      | N/A      | the symbol used by the message. eg: `"!"` for `ed.error()`                                                                    |
-| `label`       | yes      | N/A      | the text next to the symbol                                                                                                   |
-| `message`     | yes      | N/A      | the main part of the debug message                                                                                            |
-| `line_number` | yes      | N/A      | the line number shown after the message                                                                                       |
-| `colour_code` | yes      | N/A      | the [8-bit ANSI colour code](https://en.wikipedia.org/wiki/ANSI_escape_code#8-bit) of the message. eg: `"9"` for `ed.error()` |
-| `indent`      | no       | `0`      | the text next to the symbol                                                                                                   |
+| parameter     | required | default  | description                                                                                                                                                      |
+|---------------|----------|--------- |------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `symbol`      | yes      | N/A      | the symbol used by the message. eg: `"!"` for `ed.error()`. symbols should be 1 character, but there is nothing stopping you from making longer ones if you want |
+| `label`       | yes      | N/A      | the text next to the symbol                                                                                                                                      |
+| `message`     | yes      | N/A      | the main part of the debug message                                                                                                                               |
+| `line_number` | yes      | N/A      | the line number shown after the message                                                                                                                          |
+| `colour_code` | yes      | N/A      | the [8-bit ANSI colour code](https://en.wikipedia.org/wiki/ANSI_escape_code#8-bit) of the message. eg: `"9"` for `ed.error()`                                    |
+| `indent`      | no       | `0`      | the indentation of the message (used in `ed.display_history()`. an indent of 1 is 3 spaces                                                                       |
+
+### changing colours
+you can change the colour of debug messages with its corresponding variable. colour codes are [8-bit ANSI colour codes](https://en.wikipedia.org/wiki/ANSI_escape_code#8-bit)
+```py
+import easydebugger as ed
+
+ed.error("red")
+ed.ERROR = "208"  # changes colour
+ed.error("orange")
+ed.error("also orange")
+```
+![image](https://github.com/Blob2763/easydebugger/assets/88489444/664abab9-c320-4271-8068-7f010018a3b8)
+
+the colour does not change back after you have used it
+
+here are the variables for each function:
+| function                                        | variable   | default value  |
+|-------------------------------------------------|------------|----------------|
+| `ed.error()`                                    | `ERROR`    | `"9"`          |
+| `ed.warn()`                                     | `WARN`     | `"220"`        |
+| `ed.success()`                                  | `SUCCESS`  | `"120"`        |
+| `ed.variable()`                                 | `VARIABLE` | `"208"`        |
+| `ed.log()`                                      | `LOG`      | `"15"`         |
+| `ed.start_timer()`                              | `TIME`     | `"93"`         |
+| `ed.end_timer()`                                | `TIME`     | `"93"`         |
+| `ed.trace()`                                    | `TRACE`    | `"27"`         |
+| `ed.display_history()`                          | `HISTORY`  | `"57"`         |
+| all functions above (and `ed.display_message()` | `ESCAPE`   | `u"\u001b[0m"` |
+
+`ed.ESCAPE` contains the escape characters to stop formatting at the end of a message. you shouldn't edit this variable, but you can if you want to
+```py
+import easydebugger as ed
+
+print(ed.ESCAPE)
+ed.ESCAPE = u"\u001b[48;5;225m"  # ANSI escape code to turn the background pink
+ed.error("error message")
+ed.warn("warn message")
+ed.success("success message")
+```
+![image](https://github.com/Blob2763/easydebugger/assets/88489444/6323a581-5f0e-4f4f-abcc-fd4f322be543)
+
+### start time
+`ed.START_TIME` is the UNIX time in seconds when the code started. it is used for timestamps in history, but you can use it in other places if you want
+
+## plans for the future
+im really happy with how this has turned out, but i still want to add more:
+- automatically try to detect variable name in `ed.variable()`
+- make some usage examples
+- an faq
```

### Comparing `easydebugger-1.0.1/easydebugger/__init__.py` & `easydebugger-1.1.0/easydebugger/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,55 +77,55 @@
         if label:
             print((" " * indent * 3) + format_text(colour_code, f" {symbol} {label} ", True), message)
         else:
             print(format_text(colour_code, f" {symbol} ", True), message)
 
 
 def error(message, code=""):
-    caller_line_number = inspect.stack()[-1].lineno
+    caller_line_number = inspect.stack()[2].lineno
     symbol = "!"
     colour = ERROR
     display_message(symbol, code, message, caller_line_number, colour)
     history_log(symbol, colour, message, code, caller_line_number)
 
 
 def warn(message, code=""):
-    caller_line_number = inspect.stack()[-1].lineno
+    caller_line_number = inspect.stack()[2].lineno
     symbol = "*"
     colour = WARN
     display_message(symbol, code, message, caller_line_number, colour)
     history_log(symbol, colour, message, code, caller_line_number)
         
 
 def success(message, code=""):
-    caller_line_number = inspect.stack()[-1].lineno
+    caller_line_number = inspect.stack()[2].lineno
     symbol = "+"
     colour = SUCCESS
     display_message(symbol, code, message, caller_line_number, colour)
     history_log(symbol, colour, message, code, caller_line_number)
         
 
 def variable(value, name):
-    caller_line_number = inspect.stack()[-1].lineno
+    caller_line_number = inspect.stack()[2].lineno
     symbol = "$"
     colour = VARIABLE
     display_message(symbol, name, value, caller_line_number, colour)
     history_log(symbol, colour, value, name, caller_line_number)
 
 
 def log(message, label=""):
-    caller_line_number = inspect.stack()[-1].lineno
+    caller_line_number = inspect.stack()[2].lineno
     symbol = "="
     colour = LOG
     display_message(symbol, label, message, caller_line_number, colour)
     history_log(symbol, colour, message, label, caller_line_number)
 
 
 def start_timer(code):
-    caller_line_number = inspect.stack()[-1].lineno
+    caller_line_number = inspect.stack()[2].lineno
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
-        caller_line_number = inspect.stack()[-1].lineno
+        caller_line_number = inspect.stack()[2].lineno
         
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
-    caller_line_number = inspect.stack()[-1].lineno
+    caller_line_number = inspect.stack()[2].lineno
     symbol = "@"
     colour = TRACE
     
     function_name = inspect.stack()[1].function
     
     if function_name in traces:
         traces.pop(traces.index(function_name))
```

