# Comparing `tmp/sentralify-1.2.4.tar.gz` & `tmp/sentralify-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentralify-1.2.4.tar", last modified: Thu Apr  4 09:11:43 2024, max compression
+gzip compressed data, was "sentralify-1.2.5.tar", last modified: Thu Apr 11 11:51:21 2024, max compression
```

## Comparing `sentralify-1.2.4.tar` & `sentralify-1.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-04 09:11:43.590543 sentralify-1.2.4/
--rw-r--r--   0 James     (1000) James     (1000)    35129 2024-02-09 23:22:38.000000 sentralify-1.2.4/LICENSE
--rw-r--r--   0 James     (1000) James     (1000)    57354 2024-04-04 09:11:43.590543 sentralify-1.2.4/PKG-INFO
--rw-r--r--   0 James     (1000) James     (1000)    16147 2024-04-04 09:11:42.000000 sentralify-1.2.4/README.md
--rw-r--r--   0 James     (1000) James     (1000)      884 2024-04-04 09:11:04.000000 sentralify-1.2.4/pyproject.toml
--rw-r--r--   0 James     (1000) James     (1000)       38 2024-04-04 09:11:43.590543 sentralify-1.2.4/setup.cfg
--rw-r--r--   0 James     (1000) James     (1000)       38 2024-02-12 20:14:52.000000 sentralify-1.2.4/setup.py
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-04 09:11:43.587210 sentralify-1.2.4/src/
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-04 09:11:43.590543 sentralify-1.2.4/src/sentralify/
--rw-r--r--   0 James     (1000) James     (1000)     4032 2024-04-04 09:11:42.000000 sentralify-1.2.4/src/sentralify/__init__.py
--rw-r--r--   0 James     (1000) James     (1000)    18560 2024-04-04 09:11:42.000000 sentralify-1.2.4/src/sentralify/generators.py
--rw-r--r--   0 James     (1000) James     (1000)    12504 2024-04-04 09:11:42.000000 sentralify-1.2.4/src/sentralify/scrapers.py
-drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-04 09:11:43.590543 sentralify-1.2.4/src/sentralify.egg-info/
--rw-r--r--   0 James     (1000) James     (1000)    57354 2024-04-04 09:11:43.000000 sentralify-1.2.4/src/sentralify.egg-info/PKG-INFO
--rw-r--r--   0 James     (1000) James     (1000)      313 2024-04-04 09:11:43.000000 sentralify-1.2.4/src/sentralify.egg-info/SOURCES.txt
--rw-r--r--   0 James     (1000) James     (1000)        1 2024-04-04 09:11:43.000000 sentralify-1.2.4/src/sentralify.egg-info/dependency_links.txt
--rw-r--r--   0 James     (1000) James     (1000)       97 2024-04-04 09:11:43.000000 sentralify-1.2.4/src/sentralify.egg-info/requires.txt
--rw-r--r--   0 James     (1000) James     (1000)       11 2024-04-04 09:11:43.000000 sentralify-1.2.4/src/sentralify.egg-info/top_level.txt
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-11 11:51:21.966943 sentralify-1.2.5/
+-rw-r--r--   0 James     (1000) James     (1000)    35129 2024-02-09 23:22:38.000000 sentralify-1.2.5/LICENSE
+-rw-r--r--   0 James     (1000) James     (1000)    57797 2024-04-11 11:51:21.966943 sentralify-1.2.5/PKG-INFO
+-rw-r--r--   0 James     (1000) James     (1000)    16590 2024-04-11 11:51:20.000000 sentralify-1.2.5/README.md
+-rw-r--r--   0 James     (1000) James     (1000)      884 2024-04-11 11:51:15.000000 sentralify-1.2.5/pyproject.toml
+-rw-r--r--   0 James     (1000) James     (1000)       38 2024-04-11 11:51:21.966943 sentralify-1.2.5/setup.cfg
+-rw-r--r--   0 James     (1000) James     (1000)       38 2024-02-12 20:14:52.000000 sentralify-1.2.5/setup.py
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-11 11:51:21.966943 sentralify-1.2.5/src/
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-11 11:51:21.966943 sentralify-1.2.5/src/sentralify/
+-rw-r--r--   0 James     (1000) James     (1000)     4095 2024-04-11 11:51:20.000000 sentralify-1.2.5/src/sentralify/__init__.py
+-rw-r--r--   0 James     (1000) James     (1000)    18560 2024-04-11 11:51:20.000000 sentralify-1.2.5/src/sentralify/generators.py
+-rw-r--r--   0 James     (1000) James     (1000)    12668 2024-04-11 11:51:20.000000 sentralify-1.2.5/src/sentralify/scrapers.py
+drwxr-xr-x   0 James     (1000) James     (1000)        0 2024-04-11 11:51:21.966943 sentralify-1.2.5/src/sentralify.egg-info/
+-rw-r--r--   0 James     (1000) James     (1000)    57797 2024-04-11 11:51:21.000000 sentralify-1.2.5/src/sentralify.egg-info/PKG-INFO
+-rw-r--r--   0 James     (1000) James     (1000)      313 2024-04-11 11:51:21.000000 sentralify-1.2.5/src/sentralify.egg-info/SOURCES.txt
+-rw-r--r--   0 James     (1000) James     (1000)        1 2024-04-11 11:51:21.000000 sentralify-1.2.5/src/sentralify.egg-info/dependency_links.txt
+-rw-r--r--   0 James     (1000) James     (1000)       97 2024-04-11 11:51:21.000000 sentralify-1.2.5/src/sentralify.egg-info/requires.txt
+-rw-r--r--   0 James     (1000) James     (1000)       11 2024-04-11 11:51:21.000000 sentralify-1.2.5/src/sentralify.egg-info/top_level.txt
```

### Comparing `sentralify-1.2.4/LICENSE` & `sentralify-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sentralify-1.2.4/PKG-INFO` & `sentralify-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentralify
-Version: 1.2.4
+Version: 1.2.5
 Summary: Scrape Sentral data and use it!
 Author-email: mario872 <jamesaglynn10@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -1009,13 +1009,19 @@
             }
         ]
     ]
 ]
 ```
 To get the your attendance status on the first day of the school year, you would call ```sentralify(config)['student_details']['attendance'][0][0][0]['status']```. The three zeros are the term, the week number in the term, and the day of the week.
 
+#### ICS Timetable
+If you, for example, wanted to import your timetable into your calendar, then you would export your timetable as an ICS file, and import it into, say, Google Calendar.
+This is how you can, for whatever reason, access your timetable in an ICS format using Sentralify.
+To parse the ICS data in python, you can use the [ics PyPi library](https://pypi.org/project/ics/).
+To access the ICS data use: `sentralify(config)['ics']`
+
 ### That's all folks!
 That's all of my documentation for now, I think I've covered everything, now it's up to you to take this project places!
 
 
 #### Why this doesn't use get-sentral's license
 I didn't use get-sentral's license, because although the idea for me to make this came from their archiving of get-sentral, I used no code from get-sentral, and implemented and researched all of the code myself. So, in my opinion this was made from the ground up, and I did not ['remix, transform, and build upon the material'](https://creativecommons.org/licenses/by-nc-sa/4.0/) provided by get-sentral.
```

### Comparing `sentralify-1.2.4/README.md` & `sentralify-1.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -315,13 +315,19 @@
             }
         ]
     ]
 ]
 ```
 To get the your attendance status on the first day of the school year, you would call ```sentralify(config)['student_details']['attendance'][0][0][0]['status']```. The three zeros are the term, the week number in the term, and the day of the week.
 
+#### ICS Timetable
+If you, for example, wanted to import your timetable into your calendar, then you would export your timetable as an ICS file, and import it into, say, Google Calendar.
+This is how you can, for whatever reason, access your timetable in an ICS format using Sentralify.
+To parse the ICS data in python, you can use the [ics PyPi library](https://pypi.org/project/ics/).
+To access the ICS data use: `sentralify(config)['ics']`
+
 ### That's all folks!
 That's all of my documentation for now, I think I've covered everything, now it's up to you to take this project places!
 
 
 #### Why this doesn't use get-sentral's license
 I didn't use get-sentral's license, because although the idea for me to make this came from their archiving of get-sentral, I used no code from get-sentral, and implemented and researched all of the code myself. So, in my opinion this was made from the ground up, and I did not ['remix, transform, and build upon the material'](https://creativecommons.org/licenses/by-nc-sa/4.0/) provided by get-sentral.
```

### Comparing `sentralify-1.2.4/pyproject.toml` & `sentralify-1.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sentralify"
-version = "1.2.4"
+version = "1.2.5"
 description = "Scrape Sentral data and use it!"
 readme = "README.md"
 authors = [{ name = "mario872", email = "jamesaglynn10@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `sentralify-1.2.4/src/sentralify/__init__.py` & `sentralify-1.2.5/src/sentralify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
     # A bunch of if blocks to determine whether or not to scrape parts of sentral
     if notices:
         notices = Sentral.generate_notices(scraper.save_notices(page))
         data['notices'] = notices
     if timetable:
         timetable = Sentral.generate_timetable(scraper.save_timetable(page))
         data['timetable'] = timetable
+        ics = scraper.save_ics(page)
+        data['ics'] = ics
     if calendar:
         calendar = Sentral.generate_calendar(scraper.save_calendar(page))
         data['calendar'] = calendar
         
     browser.close() # Close the browser, as  our work is done
     p.stop() # Stopping playwright instance
```

### Comparing `sentralify-1.2.4/src/sentralify/generators.py` & `sentralify-1.2.5/src/sentralify/generators.py`

 * *Files identical despite different names*

### Comparing `sentralify-1.2.4/src/sentralify/scrapers.py` & `sentralify-1.2.5/src/sentralify/scrapers.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - #
 # Imports
 
 import json
 import re
 from playwright.sync_api import expect
 from bs4 import BeautifulSoup
-import time
+import os
 
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - #
 # Main scrapers class
 
 class scrapers:
     def __init__(self, config: dict):
         """
@@ -215,32 +215,48 @@
 
     def save_timetable(self, page):
         """
         Saves the timetable using a backend url to get JSON, instead of having to use BeautifulSoup on this too.
         
         Args:
             page (playwright page): The current page / tab object the playwright is working in, for continuity between functions
-            student_id (int): The student id as an int
 
         Returns:
             dict: A dictionary with the timetable from the json on the page
         """
         
-        # Ok, so a quick explanation. The Sentral page for the timetable gets it's data from the url below.
-        # This data is really weirdly formatted, but hey, they're probably working with a backend they haven't changed in 3 years
-        # I mean, changing the frontend so that most people agree that it's worse, probably just to break a python package that takes data
-        # from Sentral made by a bunch of high schoolers (https://github.com/J-J-B-J/get-sentral [Great project, this was made because that got broken by the update]) is enough work anyway, right?
-        
-        # Oh man, that was a really long rant.
-        # Anyway, this just scrapes the page for the json, and converts it to a dictionary that python can acess.
+        # This just scrapes the page for the json, and converts it to a dictionary that python can acess.
         # I found this url after watching some kids at my school go into the network tab in dev tools in Chrome, and look at what Sentral was accessing. Thank you!
         
         page.goto(f"https://{self.config['base_url']}.sentral.com.au/s-Y7eXkn/portal2/timetable/getFullTimetableInDates/{str(self.student_id)}/undefined/true")
         return json.loads(BeautifulSoup(page.content(), "lxml").text)
 
+    def save_ics(self, page):
+        """
+        Saves the ics page and returns the html
+
+        Args:
+            page (playwright page): The current page / tab object the playwright is working in, for continuity between functions
+
+        Returns:
+            html: The html content on the page
+        """
+        
+        page.goto(f"https://{self.config['base_url']}.sentral.com.au/s-Y7eXkn/portal/#!/timetable/{str(self.student_id)}")
+        with page.expect_download() as download_info:
+            page.get_by_text("Export as ICS").first.click()
+        download = download_info.value
+
+        download.save_as("../timetable.ics")
+        with open('../timetable.ics', 'r') as timetable_ics:
+            timetable_ics_contents = timetable_ics.read()
+            
+        os.remove("../timetable.ics")
+        return timetable_ics_contents
+        
     def save_notices(self, page):
         """
         Saves the notices page and returns the html
 
         Args:
             page (playwright page): The current page / tab object the playwright is working in, for continuity between functions
```

### Comparing `sentralify-1.2.4/src/sentralify.egg-info/PKG-INFO` & `sentralify-1.2.5/src/sentralify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentralify
-Version: 1.2.4
+Version: 1.2.5
 Summary: Scrape Sentral data and use it!
 Author-email: mario872 <jamesaglynn10@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -1009,13 +1009,19 @@
             }
         ]
     ]
 ]
 ```
 To get the your attendance status on the first day of the school year, you would call ```sentralify(config)['student_details']['attendance'][0][0][0]['status']```. The three zeros are the term, the week number in the term, and the day of the week.
 
+#### ICS Timetable
+If you, for example, wanted to import your timetable into your calendar, then you would export your timetable as an ICS file, and import it into, say, Google Calendar.
+This is how you can, for whatever reason, access your timetable in an ICS format using Sentralify.
+To parse the ICS data in python, you can use the [ics PyPi library](https://pypi.org/project/ics/).
+To access the ICS data use: `sentralify(config)['ics']`
+
 ### That's all folks!
 That's all of my documentation for now, I think I've covered everything, now it's up to you to take this project places!
 
 
 #### Why this doesn't use get-sentral's license
 I didn't use get-sentral's license, because although the idea for me to make this came from their archiving of get-sentral, I used no code from get-sentral, and implemented and researched all of the code myself. So, in my opinion this was made from the ground up, and I did not ['remix, transform, and build upon the material'](https://creativecommons.org/licenses/by-nc-sa/4.0/) provided by get-sentral.
```

