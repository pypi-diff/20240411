# Comparing `tmp/myprayer-3.0.2.tar.gz` & `tmp/myprayer-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myprayer-3.0.2.tar", max compression
+gzip compressed data, was "myprayer-3.1.0.tar", max compression
```

## Comparing `myprayer-3.0.2.tar` & `myprayer-3.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-01-12 21:15:48.289422 myprayer-3.0.2/LICENSE
--rw-r--r--   0        0        0     6183 2024-04-09 20:06:34.224611 myprayer-3.0.2/README.md
--rw-r--r--   0        0        0        0 2023-10-07 02:42:05.360576 myprayer-3.0.2/myprayer/__init__.py
--rw-r--r--   0        0        0     5112 2024-04-09 04:05:59.536272 myprayer-3.0.2/myprayer/cli/config.py
--rw-r--r--   0        0        0     2689 2024-04-09 03:00:44.536541 myprayer-3.0.2/myprayer/cli/constants.py
--rw-r--r--   0        0        0     1995 2024-04-09 04:05:52.042947 myprayer-3.0.2/myprayer/cli/day.py
--rw-r--r--   0        0        0      770 2024-01-12 20:59:39.011876 myprayer-3.0.2/myprayer/cli/enums.py
--rwxr-xr-x   0        0        0    12505 2024-04-09 20:04:16.913222 myprayer-3.0.2/myprayer/cli/main.py
--rw-r--r--   0        0        0     3420 2024-04-09 02:47:58.627693 myprayer-3.0.2/myprayer/cli/output.py
--rw-r--r--   0        0        0      634 2024-01-06 22:19:10.669762 myprayer-3.0.2/myprayer/cli/utils.py
--rw-r--r--   0        0        0      578 2024-04-09 20:04:29.639386 myprayer-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     7202 1970-01-01 00:00:00.000000 myprayer-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-12 21:15:48.289422 myprayer-3.1.0/LICENSE
+-rw-r--r--   0        0        0     5947 2024-04-10 17:44:41.666103 myprayer-3.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-10-07 02:42:05.360576 myprayer-3.1.0/myprayer/__init__.py
+-rw-r--r--   0        0        0     5112 2024-04-09 04:05:59.536272 myprayer-3.1.0/myprayer/cli/config.py
+-rw-r--r--   0        0        0     2673 2024-04-10 17:41:00.787999 myprayer-3.1.0/myprayer/cli/constants.py
+-rw-r--r--   0        0        0     3467 2024-04-10 20:54:55.058657 myprayer-3.1.0/myprayer/cli/day.py
+-rw-r--r--   0        0        0      770 2024-01-12 20:59:39.011876 myprayer-3.1.0/myprayer/cli/enums.py
+-rwxr-xr-x   0        0        0    11883 2024-04-10 21:16:03.916329 myprayer-3.1.0/myprayer/cli/main.py
+-rw-r--r--   0        0        0     3420 2024-04-09 02:47:58.627693 myprayer-3.1.0/myprayer/cli/output.py
+-rw-r--r--   0        0        0      634 2024-01-06 22:19:10.669762 myprayer-3.1.0/myprayer/cli/utils.py
+-rw-r--r--   0        0        0      578 2024-04-10 22:21:18.129357 myprayer-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6966 1970-01-01 00:00:00.000000 myprayer-3.1.0/PKG-INFO
```

### Comparing `myprayer-3.0.2/LICENSE` & `myprayer-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myprayer-3.0.2/README.md` & `myprayer-3.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 ## Dependencies
 
 - Python 3.8+
 - [Typer](https://github.com/tiangolo/typer) - CLI app framework
 - [Inquirer.py](https://github.com/magmax/python-inquirer) - user prompts
 - [Rich](https://github.com/willmcgugan/rich) - output formatting
-- [Requests](https://docs.python-requests.org/en/latest/) - HTTP client
 - [adhanpy](https://pypi.org/project/adhanpy/) - Prayer times calculation
 - [geopy](https://geopy.readthedocs.io/en/stable/) - Geocoding library
 - [tzlocal](https://pypi.org/project/tzlocal/) - Local timezone
 - [pydantic](https://pydantic-docs.helpmanual.io/) - Data validation
 - [tzdata](https://pypi.org/project/tzdata/) - Timezone data
 
 ### Install
@@ -68,15 +67,14 @@
  --day          -d        INTEGER RANGE [1<=x<=31]     Day (1-31) [default: (Current day)]            
  --month        -m        INTEGER RANGE [1<=x<=12]     Month [default: (Current month)]                       
  --year         -y        INTEGER                      Year [default: (Current year)]                          
  --method       -M        INTEGER                      Calculation method. [default: (Egyptian General Authority of Survey)]         
  --time-format  -t        [12|24]                      Time format. [default: 12]       
  --output       -o        [pretty|machine|table|json]  Output type. [default: table]            
  --next         -n                                     Show next prayer, has no effect if day, month, or year are given. [default: True]         
- --force        -f                                     Force update cache.       
  --help                                                Show this message and exit.  
 ```
 
 ### myparyer next
 
 ```
 Usage: myprayer next [OPTIONS]                                                                                                                                                                 
@@ -88,15 +86,14 @@
  --address      -a        TEXT                         Address.                               
  --latitude     -lat      FLOAT                        Latitude.                               
  --longitude    -lon      FLOAT                        Longitude. 
  --day          -d        INTEGER RANGE [1<=x<=31]     Day (1-31) [default: (Current day)]            
  --method       -M        INTEGER                      Calculation method. [default: (Egyptian General Authority of Survey)]         
  --time-format  -t        [12|24]                      Time format. [default: 12]       
  --output       -o        [pretty|machine|table|json]  Output type. [default: table]            
- --force        -f                                     Force update cache.       
  --help                                                Configure default settings
 ```
 
 
 ## Configuration
 
 Default settings like location, calculation method, and output format can be configured in `$XDG_CONFIG_HOME/myprayer/config.json` or `$HOME/.config/myprayer/config.json` using `myprayer config`.
```

### Comparing `myprayer-3.0.2/myprayer/cli/config.py` & `myprayer-3.1.0/myprayer/cli/config.py`

 * *Files identical despite different names*

### Comparing `myprayer-3.0.2/myprayer/cli/constants.py` & `myprayer-3.1.0/myprayer/cli/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 PRAYERS: Final[List[str]] = [
     "Fajr",
     "Sunrise",
     "Dhuhr",
     "Asr",
     "Maghrib",
     "Isha",
-    "Midnight",
 ]
 
 DEFAULT_PRAYERS: Final[List[str]] = ["Fajr", "Dhuhr", "Asr", "Maghrib", "Isha"]
 
 # Create dict for calculation methods
 CALCULATION_METHODS: Final[Dict[str, int]] = {
     "University of Islamic Sciences, Karachi": 1,
```

### Comparing `myprayer-3.0.2/myprayer/cli/enums.py` & `myprayer-3.1.0/myprayer/cli/enums.py`

 * *Files identical despite different names*

### Comparing `myprayer-3.0.2/myprayer/cli/main.py` & `myprayer-3.1.0/myprayer/cli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python
 
-__author__ = "Youssef Aswad"
-__version__ = "3.0.2"
-
 import json
-from datetime import datetime
+from datetime import datetime, timedelta
+from importlib.metadata import version as get_version
 
 import inquirer
 import typer
 import tzlocal
 from adhanpy.calculation import CalculationMethod
 from adhanpy.PrayerTimes import PrayerTimes
 from geopy import Nominatim
@@ -134,15 +132,14 @@
     ),
     next: bool = typer.Option(
         CONFIG.next,
         "--next",
         "-n",
         help="Show next prayer, has no effect if day, month, or year are given.",
     ),
-    force: bool = typer.Option(False, "--force", "-f", help="Force update cache."),
 ):
     if CONFIG.is_error:
         typer.echo(message=f"[ERROR] {CONFIG.error}", err=True)
         exit(1)
 
     # client = get_client(city, country, address, latitude, longitude, method, force)
 
@@ -157,30 +154,19 @@
 
     today = datetime.today().replace(tzinfo=tz)
     day = day or today.day
     month = month or today.month
     year = year or today.year
     date = datetime(year, month, day)
     # day_data = client.get_day(day, month, year)
-    prayer_times = PrayerTimes(
-        (latitude, longitude),
-        date,
-        CalculationMethod.EGYPTIAN,
-    )
 
-    prayers = [
-        Prayer("Fajr", prayer_times.fajr.astimezone(tz)),
-        Prayer("Sunrise", prayer_times.sunrise.astimezone(tz)),
-        Prayer("Dhuhr", prayer_times.dhuhr.astimezone(tz)),
-        Prayer("Asr", prayer_times.asr.astimezone(tz)),
-        Prayer("Maghrib", prayer_times.maghrib.astimezone(tz)),
-        Prayer("Isha", prayer_times.isha.astimezone(tz)),
-    ]
+    day_data = Day(latitude, longitude, CalculationMethod(method), date, SKIP)
 
-    day_data = Day(date, prayers, SKIP)
+    if day_data.has_passed():
+        day_data.next()
 
     output = DayOutput(day_data, time_format, next)
 
     if out_type == OutType.table:
         rprint(output.table())
     elif out_type == OutType.pretty:
         rprint(output.pretty())
@@ -236,52 +222,36 @@
     ),
     out_type: NextOutType = typer.Option(
         CONFIG.out_type,
         "--output",
         "-o",
         help="Output type.",
     ),
-    force: bool = typer.Option(False, "--force", "-f", help="Force update cache."),
 ):
     if CONFIG.is_error:
         typer.echo(message=f"[ERROR] {CONFIG.error}", err=True)
         exit(1)
 
     if city and country:
         latitude, longitude = get_coordinates(f"{city}, {country}")
     elif address:
         latitude, longitude = get_coordinates(address)
     elif latitude and longitude:
         pass
     else:
         latitude, longitude = CONFIG.location.latitude, CONFIG.location.longitude
 
-    today = datetime.today().replace(tzinfo=tz)
+    today = datetime.now(tz)
     # day_data = client.get_day(day, month, year)
-    prayer_times = PrayerTimes(
-        (latitude, longitude),
-        today,
-        method,
-    )
+    day_data = Day(latitude, longitude, CalculationMethod(method), today, SKIP)
 
-    prayers = [
-        Prayer("Fajr", prayer_times.fajr),
-        Prayer("Sunrise", prayer_times.sunrise),
-        Prayer("Dhuhr", prayer_times.dhuhr),
-        Prayer("Asr", prayer_times.asr),
-        Prayer("Maghrib", prayer_times.maghrib),
-        Prayer("Isha", prayer_times.isha),
-    ]
+    if day_data.has_passed():
+        day_data.next()
 
-    next_prayer = None
-    day_data = Day(today, prayers, SKIP)
-    for prayer in day_data.prayers:
-        if not prayer.has_passed():
-            next_prayer = prayer
-            break
+    next_prayer = day_data.get_next_prayer()
 
     if next_prayer is not None:
         time_left = format_time_left(next_prayer.time_left(), out_type)  # type: ignore
         if out_type == OutType.table:
             table = Table(show_header=True, header_style="bold magenta")
             table.add_column("Prayer")
             table.add_column("Time Left")
@@ -385,15 +355,14 @@
         inquirer.List(
             "method",
             message="Select a calculation method:",
             choices=CalculationMethod.__members__.keys(),
             default=utils.get_key(CalculationMethod.__members__, CalculationMethod(CONFIG.method)),  # type: ignore
         ),
     ]
-    
 
     method_choice = inquirer.prompt(method_question)
     method: int = CalculationMethod[method_choice["method"]].value  # type: ignore
     # Prompt for time format
     time_format: str = Prompt.ask(
         "Time format",
         choices=[TimeFormat.twelve, TimeFormat.twenty_four],
@@ -432,9 +401,29 @@
         prayers=prayers,
     )
     CONFIG.save(CONFIG_FILE)
 
     rprint(f"[green]✔[/green] Configuration saved to {CONFIG_FILE}.")
 
 
+def version_callback(value: bool):
+    if value:
+        print(f"{APP_NAME} {get_version(APP_NAME)}")
+        raise typer.Exit()
+
+
+@app.callback()
+def version(
+    version: bool = typer.Option(
+        None,
+        "--version",
+        "-v",
+        callback=version_callback,
+        is_eager=True,
+        help="Print the version and exit.",
+    )
+):
+    pass
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `myprayer-3.0.2/myprayer/cli/output.py` & `myprayer-3.1.0/myprayer/cli/output.py`

 * *Files identical despite different names*

### Comparing `myprayer-3.0.2/myprayer/cli/utils.py` & `myprayer-3.1.0/myprayer/cli/utils.py`

 * *Files identical despite different names*

### Comparing `myprayer-3.0.2/pyproject.toml` & `myprayer-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "myprayer"
-version = "3.0.2"
+version = "3.1.0"
 description = "A CLI tool to get prayer times"
 authors = ["Youssef Aswad <youssefaswad@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/YoussefAswad/myprayer"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `myprayer-3.0.2/PKG-INFO` & `myprayer-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myprayer
-Version: 3.0.2
+Version: 3.1.0
 Summary: A CLI tool to get prayer times
 Home-page: https://github.com/YoussefAswad/myprayer
 License: MIT
 Author: Youssef Aswad
 Author-email: youssefaswad@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -41,15 +41,14 @@
 
 ## Dependencies
 
 - Python 3.8+
 - [Typer](https://github.com/tiangolo/typer) - CLI app framework
 - [Inquirer.py](https://github.com/magmax/python-inquirer) - user prompts
 - [Rich](https://github.com/willmcgugan/rich) - output formatting
-- [Requests](https://docs.python-requests.org/en/latest/) - HTTP client
 - [adhanpy](https://pypi.org/project/adhanpy/) - Prayer times calculation
 - [geopy](https://geopy.readthedocs.io/en/stable/) - Geocoding library
 - [tzlocal](https://pypi.org/project/tzlocal/) - Local timezone
 - [pydantic](https://pydantic-docs.helpmanual.io/) - Data validation
 - [tzdata](https://pypi.org/project/tzdata/) - Timezone data
 
 ### Install
@@ -95,15 +94,14 @@
  --day          -d        INTEGER RANGE [1<=x<=31]     Day (1-31) [default: (Current day)]            
  --month        -m        INTEGER RANGE [1<=x<=12]     Month [default: (Current month)]                       
  --year         -y        INTEGER                      Year [default: (Current year)]                          
  --method       -M        INTEGER                      Calculation method. [default: (Egyptian General Authority of Survey)]         
  --time-format  -t        [12|24]                      Time format. [default: 12]       
  --output       -o        [pretty|machine|table|json]  Output type. [default: table]            
  --next         -n                                     Show next prayer, has no effect if day, month, or year are given. [default: True]         
- --force        -f                                     Force update cache.       
  --help                                                Show this message and exit.  
 ```
 
 ### myparyer next
 
 ```
 Usage: myprayer next [OPTIONS]                                                                                                                                                                 
@@ -115,15 +113,14 @@
  --address      -a        TEXT                         Address.                               
  --latitude     -lat      FLOAT                        Latitude.                               
  --longitude    -lon      FLOAT                        Longitude. 
  --day          -d        INTEGER RANGE [1<=x<=31]     Day (1-31) [default: (Current day)]            
  --method       -M        INTEGER                      Calculation method. [default: (Egyptian General Authority of Survey)]         
  --time-format  -t        [12|24]                      Time format. [default: 12]       
  --output       -o        [pretty|machine|table|json]  Output type. [default: table]            
- --force        -f                                     Force update cache.       
  --help                                                Configure default settings
 ```
 
 
 ## Configuration
 
 Default settings like location, calculation method, and output format can be configured in `$XDG_CONFIG_HOME/myprayer/config.json` or `$HOME/.config/myprayer/config.json` using `myprayer config`.
```

