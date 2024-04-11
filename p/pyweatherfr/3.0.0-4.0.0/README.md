# Comparing `tmp/pyweatherfr-3.0.0.tar.gz` & `tmp/pyweatherfr-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-3.0.0.tar", last modified: Tue Apr  9 18:19:18 2024, max compression
+gzip compressed data, was "pyweatherfr-4.0.0.tar", last modified: Thu Apr 11 04:51:14 2024, max compression
```

## Comparing `pyweatherfr-3.0.0.tar` & `pyweatherfr-4.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:18.031257 pyweatherfr-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-09 18:19:18.031257 pyweatherfr-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:18.031257 pyweatherfr-3.0.0/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    36888 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:19:18.031257 pyweatherfr-3.0.0/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-09 18:19:18.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 18:19:18.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:19:18.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 18:19:18.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:19:17.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 18:19:18.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 18:19:18.000000 pyweatherfr-3.0.0/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:19:18.031257 pyweatherfr-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-09 18:19:12.000000 pyweatherfr-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:51:14.879785 pyweatherfr-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-11 04:51:14.879785 pyweatherfr-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:51:14.879785 pyweatherfr-4.0.0/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30674 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:51:14.879785 pyweatherfr-4.0.0/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 04:51:14.000000 pyweatherfr-4.0.0/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 04:51:14.879785 pyweatherfr-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-11 04:51:07.000000 pyweatherfr-4.0.0/setup.py
```

### Comparing `pyweatherfr-3.0.0/LICENSE.txt` & `pyweatherfr-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-3.0.0/PKG-INFO` & `pyweatherfr-4.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 3.0.0
+Version: 4.0.0
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -14,15 +14,13 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 License-File: LICENSE.txt
 Requires-Dist: columnar
 Requires-Dist: termcolor
 Requires-Dist: colorama
-Requires-Dist: unidecode
-Requires-Dist: requests
 Requires-Dist: openmeteo_requests
 Requires-Dist: requests_cache
-Requires-Dist: pandas
 Requires-Dist: retry_requests
+Requires-Dist: geopy
 
 The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme
```

### Comparing `pyweatherfr-3.0.0/README.md` & `pyweatherfr-4.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 # :sunny: :umbrella: :cloud: pyweatherfr
 
-pyweatherfr affiche les prévisions méteo pour les communes françaises dans votre terminal. Il utilise les API de méteoFrance, https://www.prevision-meteo.ch et https://geolocation-db.com/json.
+pyweatherfr affiche les prévisions méteo pour les communes françaises dans votre terminal. Il utilise l'API de MéteoFrance
 
 
 # 🚀 Comment utiliser **pyweatherfr**
 
+pyweatherfr affiche les prévisions météo sur 4 jours en se basant sur l'ip
+
 pyweatherfr \[VILLE\]
 
 exemple : ``pyweatherfr Grenoble`` affiche les prévisions météo pour Grenoble sur 4 jours
 
+exemple : ``pyweatherfr 38700`` affiche les prévisions météo pour le code postal 38700
+
 pyweatherfr -n \[VILLE\]
 
 exemple : ``pyweatherfr -n Grenoble`` affiche les données météo pour Grenoble 
 
-pyweatherfr \[TOWN\] -j [INT(0-3)]
+pyweatherfr -g \[COORDONNEES_GPS\]
+
+exemple : `` pyweatherfr -g 45 5`` affiche les prévisions météo pour les coordonnées GPS (latitude : 45 et longitude : 5)
+
+pyweatherfr \[TOWN\] -j [INT]
 
 exemple : ``pyweatherfr Grenoble -j 1`` affiche les prévisions météo détaillées pour Grenoble à J+1
 
 exemple : ``pyweatherfr Grenoble -j -2`` affiche les données météo détaillées pour Grenoble à J-2
 
-exemple : ``pyweatherfr 38700`` affiche les prévisions météo pour le code postal 38700
+attention : le paramètre peut être compris entre - 100 et 3
 
-pyweatherfr -g \[COORDONNEES_GPS\]
+pyweatherfr \[TOWN\] -p [INT]
+
+exemple : ``pyweatherfr Grenoble -p 10`` affiche les données météo détaillées pour Grenoble de J-10 à J-1
 
-exemple : `` pyweatherfr -g 45 5`` affiche les prévisions météo pour les coordonnées GPS (latitude : 45 et longitude : 5)
 
 
 ## Autres options
 
   - ``-h/--help``    montrer l'aide
   - ``-u/--update``  update pyweatherfr
   - ``-c/--condensate``  condense la sortie
```

### Comparing `pyweatherfr-3.0.0/pyweatherfr/args.py` & `pyweatherfr-4.0.0/pyweatherfr/args.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,42 +48,44 @@
         help="affichage des données météo par nom de ville ou code postal -si absent, la VILLE est déduite de l'ip-",
     )
     my_parser.add_argument(
         "-n",
         "--now",
         action="store_true",
         help="affichage des données météo détaillées actuelles",
-    )    
+    )
     my_parser.add_argument(
         "-j",
         "--jour",
         metavar="JOUR",
         action="store",
         type=int,
         default=1000,
         choices=range(-100, 4),
         help="affichage des données météo détaillées pour [JOUR] (0 pour le jour actuel, 1 pour le J+1, ..., -1 pour J-1, ...)",
-    ) 
+    )
+    my_parser.add_argument(
+        "-p",
+        "--past",
+        metavar="JOUR PASSE",
+        action="store",
+        type=int,
+        default=0,
+        choices=range(1, 100),
+        help="affichage des données météo génériques depuis [JOUR PASSE] (-10 pour J-10 à J-1, ...)",
+    )         
     my_group.add_argument(
         "-g",
         "--gps",
         metavar=("LATITUDE", "LONGITUDE"),
         action="store",
         nargs=2,
         type=str,
         help="affichage des données météo par coordonnées GPS",
-    )
-    my_group.add_argument(
-        "-s",
-        "--search",
-        action="store",
-        metavar="RECHERCHE",
-        type=str,
-        help="ville ou code postal à rechercher",
-    )        
+    )      
     my_parser.add_argument(
         "--nocolor",
         action="store_true",
         help="désactiver couleur et emojis en sortie -à utiliser en cas de problème d'affichage-",
     )
     my_parser.add_argument(
         "-c",
```

### Comparing `pyweatherfr-3.0.0/pyweatherfr/pyweatherfr.py` & `pyweatherfr-4.0.0/pyweatherfr/pyweatherfr.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 """
 pyweatherfr use case
 """
 
-from pyweatherfr.args import compute_args
 
+from pyweatherfr.args import compute_args
 
+import geopy,certifi,ssl
 import datetime
 import sys
-import requests
-import unidecode
 import json
 import urllib.request
 import os
-import time
-import re
 import openmeteo_requests
 import requests_cache
+import columnar
+import termcolor
+import pathlib
+import retry_requests
+import geopy
 
-import pandas as pd
-
-from columnar import columnar
-from termcolor import colored
-from pathlib import Path
-from retry_requests import retry
-
-incomplete_data = False
 
 DOSSIER_CONFIG_PYWEATHER = "pyweatherfr"
 
 SUN = "\U0001F31E"
 MI_SUN = "\U0001F324"
 CLOUD = "\U0001F325"
 MI_CLOUD_RAIN = "\U0001F326"
@@ -70,122 +64,71 @@
 WARNING_HUMIDITY=90
 
 def get_user_config_directory_pyweather():
     if os.name == "nt":
         appdata = os.getenv("LOCALAPPDATA")
         if appdata:
             ze_path = os.path.join(appdata, DOSSIER_CONFIG_PYWEATHER, "")
-            Path(ze_path).mkdir(parents=True, exist_ok=True)
+            pathlib.Path(ze_path).mkdir(parents=True, exist_ok=True)
             return ze_path
         appdata = os.getenv("APPDATA")
         if appdata:
             ze_path = os.path.join(appdata, DOSSIER_CONFIG_PYWEATHER, "")
-            Path(ze_path).mkdir(parents=True, exist_ok=True)
+            pathlib.Path(ze_path).mkdir(parents=True, exist_ok=True)
             return ze_path
         print(my_colored("erreur : impossible de créer le dossier de config", "red"))
         sys.exit(1)
     xdg_config_home = os.getenv("XDG_CONFIG_HOME")
     if xdg_config_home:
         ze_path = os.path.join(xdg_config_home, "")
-        Path(ze_path).mkdir(parents=True, exist_ok=True)
+        pathlib.Path(ze_path).mkdir(parents=True, exist_ok=True)
         return ze_path
     ze_path = os.path.join(
         os.path.expanduser("~"), ".config", DOSSIER_CONFIG_PYWEATHER, ""
     )
-    Path(ze_path).mkdir(parents=True, exist_ok=True)
+    pathlib.Path(ze_path).mkdir(parents=True, exist_ok=True)
     return ze_path
 
 
 def find():
 
-    global incomplete_data
-    global is_gps
-    incomplete_data = False
-    is_gps = False
-    doublon_cp = False
-
-    vjson = recuperation_data_villes()
-
-    if compute_args().search:
-        search_town(vjson)
-    elif compute_args().town:
-        url, doublon_cp = obtain_url_and_town_from_cp(vjson)
+    if compute_args().town:
+        ville, dpt, lat, long = obtain_url_and_town_from_cp()
     elif compute_args().gps:
-        is_gps = True
-        url = obtain_url_and_town_from_gps()
+        ville, dpt, lat, long = obtain_url_and_town_from_gps()
     else:
-        url = obtain_url_and_town_from_ip()
+        ville, dpt, lat, long = obtain_url_and_town_from_ip()
 
-    print_debug(
-        "recherche prévision depuis http://prevision-meteo.ch/services/json/" + url
-    )
-    r = requests.get("http://prevision-meteo.ch/services/json/" + url)
-    try:
-        if r.json().get("errors"):
-            display_error(r)
-    except Exception:
-        print(r)        
-    if is_gps:
-        infos = "(" + url + ")"
-        city = "."
-    else:
-        infos = obtain_info_town(vjson, url, r)
-        try:
-            city = r.json().get("city_info").get("name")
-        except Exception:
-            print(r)  
-        city = r.json().get("city_info").get("name")
     if compute_args().now:
-        previsions_courantes(r, infos, city)
+        previsions_courantes(ville, dpt, lat, long)
     elif compute_args().jour == 1000:
-        previsions_generiques(r, infos, city)
+        previsions_generiques(ville, dpt, lat, long)
     else:
-        previsions_detaillees(r, infos, city)
-    if incomplete_data == True:
-        print(
-            my_colored(
-                "attention : données incomplètes, vous pouvez essayer une autre ville pour plus de précision",
-                "yellow",
-            )
-        )
-    if doublon_cp:
-        print(
-            my_colored(
-                'attention : il existe plusieurs villes associées au code postal. Si besoin, jouez "pyweather -s '
-                + compute_args().town
-                + '"'
-                + " pour trouver la ville souhaitée ",
-                "yellow",
-            )
-        )
+        previsions_detaillees(ville, dpt, lat, long)
+
+
+
+def previsions_detaillees(ville, dpt, lat, long):
+    print_generic_data_town(ville, dpt, lat, long)
 
 
-def previsions_detaillees(r, infos, city):
-    gps, elevation, sunrise, sunset = obtain_data(r)
-    print_generic_data_town(infos, city, gps, elevation)
-    # Utilisation d'une expression régulière pour extraire les nombres
-    matches = re.findall(r"[-+]?\d*\.\d+|\d+", gps)
-
-    # Récupération des deux nombres extraits
-    latitude = float(matches[0])
-    longitude = float(matches[1])
     (
         hourly_temperature_2m,
         hourly_apparent_temperature,
         hourly_precipitation,
         hourly_wind_speed_10m,
         hourly_wind_gusts_10m,
         hourly_wind_direction_10m,
         surface_pressure,
         current_weather_code,
         snowfall,
         relative_humidity_2m,
         sunshine_duration,
         cloud_cover       
-    ) = specific_day(latitude, longitude, compute_args().jour)
+    ) = specific_day(lat, long, compute_args().jour)
     data = []
     for h in range(0, 24):
         warning = ""
         if (
             compute_args().jour == 0
             and 0 < h - int(datetime.datetime.now().strftime("%H")) <= 1
         ):
@@ -215,15 +158,16 @@
         pression = f"{surface_pressure[h]:.1f}Hpa"
         if surface_pressure[h] >= WARNING_HP:
             warning = warning + " " + ELEPHANT
         if surface_pressure[h] <= WARNING_BP:
             warning = warning + " " + PLUME
         weather, emojiweather = traduction(current_weather_code[h])
         humidity = f"{relative_humidity_2m[h]:.0f}%"
-        soleil_nuage = f"{sunshine_duration[h]/60:.0f}% / {cloud_cover[h]:.0f}%"
+        duree_soleil = f"{sunshine_duration[h]/60:.0f}'"
+        couv_nuage = f" {cloud_cover[h]:.0f}%"        
         if compute_args().nocolor:
             data.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now().replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
@@ -234,15 +178,16 @@
                     weather,
                     temp,
                     pluie,
                     vent,
                     direction,
                     pression,
                     humidity,
-                    soleil_nuage,
+                    duree_soleil,
+                    couv_nuage,
                 ]
             )
         else:
             data.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now().replace(
@@ -255,51 +200,54 @@
                     emojiweather + " " + weather,
                     temp,
                     pluie,
                     vent,
                     direction,
                     pression,
                     humidity,
-                    soleil_nuage,
+                    duree_soleil,
+                    couv_nuage,
                     warning,
                 ]
             )
 
     if compute_args().nocolor:
         headers = [
             "date",
             "temps",
             "température (ressentie)",
             "précipitations",
             "vent (rafales)",
             "direction vent",
             "pression",
             "humidité",
-            "durée soleil / couverture nuage"
+            "durée soleil",
+            "couverture nuage"            
         ]
     else:
         headers = [
             "date",
             "temps",
             "température (ressentie)",
             "précipitations",
             "vent (rafales)",
             "direction vent",
             "pression",
             "humidité",
-            "durée soleil / couverture nuage",            
+            "durée soleil",
+            "couverture nuage",            
             "warnings",
         ]
 
     if data != []:
         if compute_args().condensate:
-            table = columnar(data, no_borders=True, wrap_max=0)
+            table = columnar.columnar(data, no_borders=True, wrap_max=0)
         else:
             print("")
-            table = columnar(data, headers, no_borders=False, wrap_max=0)
+            table = columnar.columnar(data, headers, no_borders=False, wrap_max=0)
         print(table)
 
 def calculer_direction(direction_vent_degres):
     if (
             direction_vent_degres <= 22.5
             or direction_vent_degres >= 360 - 22.5
         ):
@@ -365,35 +313,30 @@
         return ["pluie", RAIN]
     if current_weather_code >= 70 and current_weather_code <= 79:
         return ["neige", SNOW]
     if current_weather_code >= 80 and current_weather_code <= 99:
         return ["averse / orage", ORAGE_PLUIE]
 
 
-def previsions_courantes(r, infos, city):
-    gps, elevation, sunrise, sunset = obtain_data(r)
-    print_generic_data_town(infos, city, gps, elevation)
-
-    matches = re.findall(r"[-+]?\d*\.\d+|\d+", gps)
-    latitude = float(matches[0])
-    longitude = float(matches[1])
+def previsions_courantes(ville, dpt, lat, long):
+    print_generic_data_town(ville, dpt, lat, long)
 
     (
         current_temperature_2m,
         current_apparent_temperature,
         current_relative_humidity_2m,
         current_precipitation,
         current_surface_pressure,
         current_wind_speed_10m,
         current_wind_gusts_10m,
         current_wind_direction_10m,
         current_weather_code,
         snowfall
 
-    ) = current(latitude, longitude)
+    ) = current(lat, long)
     current_weather, emojiweather = traduction(current_weather_code)
     data = []
     direction = calculer_direction(current_wind_direction_10m)
 
     if compute_args().nocolor:
         data.append(
             [
@@ -462,47 +405,45 @@
                     f"{current_wind_speed_10m:.1f}km/h ({current_wind_gusts_10m:.1f}km/h) - "
                     + direction,
                     "",
                 ]
             )
         data.append(["temps", emojiweather + " " + current_weather, ""])
     if compute_args().condensate:
-        table = columnar(data, no_borders=True, wrap_max=0)
+        table = columnar.columnar(data, no_borders=True, wrap_max=0)
     else:
         print("")
-        table = columnar(data, no_borders=False, wrap_max=0)
+        table = columnar.columnar(data, no_borders=False, wrap_max=0)
     print(table)
 
 
-def previsions_generiques(r, infos, city):
-    gps, elevation, sunrise, sunset = obtain_data(r)
+def previsions_generiques(ville, dpt, lat, long):
 
-    print_generic_data_town(infos, city, gps, elevation)
+    print_generic_data_town(ville, dpt, lat, long)
 
-    matches = re.findall(r"[-+]?\d*\.\d+|\d+", gps)
-    latitude = float(matches[0])
-    longitude = float(matches[1])
 
     (
-        date_debut,
         daily_temperature_2m_min,
         daily_temperature_2m_max,
         daily_apparent_temperature_min,
         daily_apparent_temperature_max,
         daily_precipitation_sum,
         daily_wind_speed_10m_max,
         daily_wind_gusts_10m_max,
         daily_wind_direction_10m_dominant,
         weather_code,
         snowfall,
         precipitation_hours,
         sunshine_duration,
-    ) = resume(latitude, longitude)
+    ) = resume(lat, long)
     data2 = []
-    for i in [0, 1, 2, 3]:
+    fin = 3
+    if compute_args().past!=0:
+        fin=-1
+    for i in range(0,len(daily_precipitation_sum)):
         warning = ""
         pluie = f"{daily_precipitation_sum[i]:.1f}mm"
         if snowfall[i] >= WARNING_SNOW:
             warning = warning + " " + SNOW
         elif daily_precipitation_sum[i] >= WARNING_RAIN:
             warning = warning + " " + RAIN
         temp = f"{daily_temperature_2m_min[i]:.1f}° ({daily_apparent_temperature_min[i]:.1f}°) -> {daily_temperature_2m_max[i]:.1f}° ({daily_apparent_temperature_max[i]:.1f}°)"
@@ -525,15 +466,16 @@
         vent = f"{daily_wind_speed_10m_max[i]:.1f}km/h ({daily_wind_gusts_10m_max[i]:.1f}km/h)"
         direction=calculer_direction(daily_wind_direction_10m_dominant[i])
 
 
         vent = vent
         if daily_wind_speed_10m_max[i] >= WARNING_WIND or daily_wind_gusts_10m_max[i] >= WARNING_WIND_GUST:
             warning = warning + " " + WIND
-        duree = f"{precipitation_hours[i]:.0f}h / {sunshine_duration[i]/3600:.0f}h"
+        duree_pluie = f"{precipitation_hours[i]:.0f}h"
+        duree_soleil = f"{sunshine_duration[i]/3600:.1f}h"
         if compute_args().nocolor:
             data2.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now().replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
@@ -541,136 +483,91 @@
                         "%Y-%m-%d",
                     ),
                     weather,
                     temp,
                     pluie,
                     vent,
                     direction,
-                    duree
+                    duree_pluie,
+                    duree_soleil
                 ]
             )
             headers = [
                 "date",
                 "temps",
                 "température (ressentie)",
                 "précipitations",
                 "vent (rafales)",
                 "direction",
-                "durée pluie / soleil"
+                "durée pluie",
+                "durée soleil"
             ]
         else:
             data2.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now().replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
-                        + datetime.timedelta(hours=24 * i),
+                        + datetime.timedelta(hours=24 * i)
+                        + datetime.timedelta(days=-1*compute_args().past),
                         "%Y-%m-%d",
                     ),
                     emojiweather + " " + weather,
                     temp,
                     pluie,
                     vent,
                     direction,
-                    duree,
+                    duree_pluie,
+                    duree_soleil,
                     warning,
                 ]
             )
             headers = [
                 "date",
                 "temps",
                 "température (ressentie)",
                 "précipitations",
                 "vent (rafales)",
                 "direction vent",
-                "durée pluie / soleil",
+                "durée pluie",
+                "durée soleil",
                 "warning",
             ]
 
     if data2 != []:
         if compute_args().condensate:
-            table = columnar(data2, no_borders=True, wrap_max=0)
+            table = columnar.columnar(data2, no_borders=True, wrap_max=0)
         else:
             print("")
-            table = columnar(data2, headers, no_borders=False, wrap_max=0)
+            table = columnar.columnar(data2, headers, no_borders=False, wrap_max=0)
         print(table)
 
 
-def print_generic_data_town(infos, city, gps, elevation):
+def print_generic_data_town(ville, dpt, lat, long):
     print("")
 
     data = []
     if compute_args().nocolor:
-        data.append([re.sub(" \([0-9]+\)", "", city) + " " + infos])
-        data.append([gps + " / alt. " + elevation])
+        data.append(ville + " (" + dpt + ")")
+        data.append("lat.: " + lat + " / long.: " +long)
         data.append([datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")])
     else:
-        data.append([HOME, re.sub(" \([0-9]+\)", "", city) + " " + infos])
-        data.append([BOUSSOLE, gps + " / alt. " + elevation])
+        data.append([HOME, ville + " (" + dpt + ")"])
+        data.append([BOUSSOLE, "lat.: " + lat + " / long.: " +long])
         data.append([CLOCK, datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")])
 
     if compute_args().condensate:
-        table = columnar(data, no_borders=True, wrap_max=0)
+        table = columnar.columnar(data, no_borders=True, wrap_max=0)
     else:
-        table = columnar(data, no_borders=False, wrap_max=0)
+        table = columnar.columnar(data, no_borders=False, wrap_max=0)
 
     print(table)
 
 
-def obtain_data(r):
-    gps = (
-        "lat. "
-        + str(round(float(r.json().get("city_info").get("latitude")), 5))
-        + " / long. "
-        + str(round(float(r.json().get("city_info").get("longitude")), 5))
-    )
-    if not is_gps:
-        elevation = valueorNA(r.json().get("city_info").get("elevation")) + "m"
-    else:
-        elevation = valueorNA(r.json().get("forecast_info").get("elevation")) + "m"
-    sunrise = valueorNA(r.json().get("city_info").get("sunrise"))
-    sunset = valueorNA(r.json().get("city_info").get("sunset"))
-    return gps, elevation, sunrise, sunset
-
-
-def obtain_info_town(vjson, url, r):
-    print_debug(
-        "recherche informations de la VILLE depuis https://www.prevision-meteo.ch/services/json/list-cities"
-    )
-    try:
-        i = 0
-        while True:
-            if (
-                vjson.get(str(i)).get("country") is not None
-                and vjson.get(str(i)).get("country") == "FRA"
-            ):
-                if unidecode.unidecode(url.lower()) == unidecode.unidecode(
-                    vjson.get(str(i)).get("url").lower()
-                ):
-                    npa = vjson.get(str(i)).get("npa")
-                    print_debug("CODE_POSTAL : " + npa)
-                    infos = "(" + npa + ")"
-                    break
-            i = i + 1
-            infos = ""
-        return infos
-    except Exception:
-        print(my_colored("erreur : la VILLE n'est pas en France", "red"))
-        print(
-            my_colored(
-                "essayez de trouver un paramètre correct avec \"pyweatherfr -s '"
-                + compute_args().town
-                + "'\"",
-                "yellow",
-            )
-        )
-        sys.exit(1)
-
-
 def display_error(r):
     print(my_colored("erreur : pas de données trouvées", "red"))
     print_debug(r.json().get("errors")[0].get("code"))
     print_debug(r.json().get("errors")[0].get("text"))
     print_debug(r.json().get("errors")[0].get("description"))
     if compute_args().town:
         print(
@@ -688,222 +585,131 @@
                 "yellow",
             )
         )
     exit(1)
 
 
 def obtain_url_and_town_from_ip():
-    global is_gps
+
     with urllib.request.urlopen("https://geolocation-db.com/json") as url:
         print_debug(
             "recherche de la localisation depuis https://geolocation-db.com/json"
         )
         data = json.loads(url.read().decode())
         print_debug(str(data))
-        town = data["city"]
-        if town is None:
-            print(
-                my_colored(
-                    "attention : pas de ville trouvée avec l'ip, utilisation des coordonnées GPS...",
-                    "yellow",
-                )
-            )
-            print_debug(
-                "COORDONNEES_GPS :"
-                + "latitude="
-                + str(data["latitude"])
-                + " longitude="
-                + str(data["longitude"])
-            )
-            is_gps = True
-            url = "lat=" + str(data["latitude"]) + "lng=" + str(data["longitude"])
-            print_debug("URL : " + url)
-        else:
-            url = town
-            print_debug("URL : " + url)
-    return url
+        ville = data["city"]
+        lat = str(data["latitude"])
+        long = str(data["longitude"])
+        dpt = str(data["postal"])
+        return ville, dpt, lat, long 
+    
 
 
 def obtain_url_and_town_from_gps():
     print_debug(
         "COORDONNEES_GPS :"
         + "latitude="
         + str(compute_args().gps[0])
         + " longitude="
         + str(compute_args().gps[1])
     )
-    url = "lat=" + compute_args().gps[0] + "lng=" + compute_args().gps[1]
-    print_debug("URL : " + url)
-    return url
-
+    return "", "", str(compute_args().gps[0]), str(compute_args().gps[1])
 
-def obtain_url_and_town_from_cp(vjson):
-    town = compute_args().town
-    doublon = False
-    if town.isnumeric():
-        post = town
-        print_debug("CODE_POSTAL : " + str(post))
-        print_debug(
-            "recherche de la VILLE et de l'URL depuis https://www.prevision-meteo.ch/services/json/list-cities"
-        )
-        i = 0
-        try:
-            trouve = False
-            while True:
-                if (
-                    vjson.get(str(i)).get("country") is not None
-                    and vjson.get(str(i)).get("country") == "FRA"
-                ):
-                    if str(post) == vjson.get(str(i)).get("npa"):
-                        if not trouve:
-                            url = vjson.get(str(i)).get("url")
-                            print_debug("URL : " + url)
-                        if trouve:
-                            doublon = True
-                        trouve = True
-                i = i + 1
-        except Exception:
-            if not trouve:
-                print(
-                    my_colored(
-                        "erreur : pas de ville trouvée avec le code postal " + str(post),
-                        "red",
-                    )
-                )
-                print(
-                    my_colored(
-                        "essayez avec un autre code postal, ou avec le code postal principal de la ville ou encore le nom de la ville",
-                        "yellow",
-                    )
-                )
-                sys.exit(1)
-        return url, doublon
-    else:
-        url = unidecode.unidecode(town.lower()).replace(" ", "-")
-        print_debug("URL : " + url)
-        return url, doublon
-
-
-def search_town(vjson):
-    search = compute_args().search
-    print_debug(
-        "recherche de la ville depuis https://www.prevision-meteo.ch/services/json/list-cities"
-    )
-    trouve = False
-    i = 0
-    try:
-        while True:
-            if (
-                vjson.get(str(i)).get("country") is not None
-                and vjson.get(str(i)).get("country") == "FRA"
-            ):
-                name = re.sub(" \([0-9]+\)", "", vjson.get(str(i)).get("name")).replace(
-                    " ", "-"
-                )
-                npa = vjson.get(str(i)).get("npa")
-                url = vjson.get(str(i)).get("url")
-                if (
-                    str(search) == npa
-                    or unidecode.unidecode(search.lower()).replace(" ", "-")
-                    in unidecode.unidecode(name.lower().replace(" ", "-"))
-                    or unidecode.unidecode(name.lower().replace(" ", "-"))
-                    in unidecode.unidecode(search.lower().replace(" ", "-"))
-                ):
-                    trouve = True
-                    print(
-                        my_colored(
-                            "pour "
-                            + name
-                            + " ("
-                            + npa
-                            + "), exécutez 'pyweatherfr "
-                            + url
-                            + "' or 'pyweatherfr  "
-                            + npa
-                            + "'",
-                            "yellow",
-                        )
-                    )
-            i = i + 1
-    except Exception:
-        if not trouve:
-            print(my_colored("erreur : pas de ville trouvée", "red"))
-        sys.exit(1)
 
+def obtain_url_and_town_from_cp():
 
-def recuperation_data_villes():
-    tmp_json = "villes.json"
-    if (
-        compute_args().cache
-        or not os.path.exists(get_user_config_directory_pyweather() + tmp_json)
-        or (
-            time.time()
-            - os.stat(get_user_config_directory_pyweather() + tmp_json).st_mtime
-            > 86400 * 30
-        )
-    ):
-        print(
-            my_colored(
-                "cache des villes absent, expiré ou reset, en cours de téléchargement...",
-                "yellow",
-            )
-        )
-        vjson = requests.get(
-            "https://www.prevision-meteo.ch/services/json/list-cities"
-        ).json()
-        print_debug(
-            "enregistrement du cache dans "
-            + get_user_config_directory_pyweather()
-            + tmp_json
-        )
-        with open(get_user_config_directory_pyweather() + tmp_json, "w") as f:
-            json.dump(vjson, f)
-    else:
-        print_debug(
-            "recupération du cache depuis "
-            + get_user_config_directory_pyweather()
-            + tmp_json
-        )
-        with open(get_user_config_directory_pyweather() + tmp_json, "r") as f:
-            vjson = json.load(f)
-    return vjson
+    town = compute_args().town
+    ctx = ssl.create_default_context(cafile=certifi.where())
+    geopy.geocoders.options.default_ssl_context = ctx
+    
+    # Création d'un objet géocodeur Nominatim
+    geolocator = geopy.geocoders.Nominatim(user_agent="my_geocoder")
+    
+    # Géocodage d'une adresse
+    locations = geolocator.geocode(town + ", France",exactly_one=False,addressdetails=True)
+    
+    # Affichage des informations de localisation
+    choix = []
+    if locations == None:
+        print(my_colored("erreur : aucune ville trouvée", "red")) 
+        exit(1)    
+    for location in locations:
+        print_debug(str(location.raw))
+        ville = location.raw.get("address").get("village")
+        if ville == None:
+            ville = location.raw.get("address").get("municipality")
+        if ville == None:
+            ville = location.raw.get("address").get("city")
+        dpt = location.raw.get("address").get("county")
+        if dpt ==None:
+            dpt=""
+        cp = location.raw.get("address").get("postcode")
+        if cp == None:
+            cp = ""
+        lat = location.raw.get("lat")
+        long = location.raw.get("lon")
+        print_debug(ville+"-"+dpt+"-"+lat+"-"+long)
+        if ville.lower() == town.lower() or cp.lower() == town.lower(): 
+            if ville+"-"+dpt not in [item[0] for item in choix]:  # Vérifier si ville+"-"+dpt n'est pas déjà présent dans choix
+                choix.append([ville+"-"+dpt, ville, dpt, lat, long])
+    if len(choix)==1:
+        choice = choix[0]
+        ville = choice[1]
+        dpt = choice[2]
+        lat = choice[3]
+        long = choice[4]
+        return ville, dpt, lat, long    
+    if len(choix)==0:
+        print(my_colored("erreur : aucune ville trouvée", "red")) 
+        exit(1)
+    i=0    
+    for choice in choix:
+        i=i+1
+        print("["+str(i)+"] " + choice[1] + " (" + choice[2]+ ")")
+    toto = input("Quelle ville?")
+    choice = choix[int(toto)]
+    ville = choice[1]
+    dpt = choice[2]
+    lat = choice[3]
+    long = choice[4]
+    return ville, dpt, lat, long
 
 
 def my_colored(message, color):
     if compute_args().nocolor:
         return message
-    return colored(message, color)
+    return termcolor.colored(message, color)
 
 
 def print_debug(message):
     if compute_args().verbose:
         print("debug : " + message)
 
 
-def valueorNA(my_string):
-    global incomplete_data
-    if my_string is None or my_string == "NA":
-        incomplete_data = True
-        return "."
-    return my_string
 
 
 def resume(latitude, longitude):
     # Setup the Open-Meteo API client with cache and retry on error
     cache_session = requests_cache.CachedSession(
         get_user_config_directory_pyweather() + ".cache", expire_after=3600
     )
-    retry_session = retry(cache_session, retries=5, backoff_factor=0.2)
+    retry_session = retry_requests.retry(cache_session, retries=5, backoff_factor=0.2)
     openmeteo = openmeteo_requests.Client(session=retry_session)
 
     # Make sure all required weather variables are listed here
     # The order of variables in hourly or daily is important to assign them correctly below
     url = "https://api.open-meteo.com/v1/meteofrance"
+    date_debut = (datetime.datetime.now() + datetime.timedelta(days=-1*compute_args().past)).strftime("%Y-%m-%d")
+    date_fin = (datetime.datetime.now() + datetime.timedelta(days=3)).strftime("%Y-%m-%d")
+    if compute_args().past!=0:
+        date_fin = (datetime.datetime.now() + datetime.timedelta(days=-1)).strftime("%Y-%m-%d")    
     params = {
         "timezone": "Europe/Paris",
+        "start_date": date_debut,
+	    "end_date": date_fin,
         "latitude": latitude,
         "longitude": longitude,
         "daily": [
             "temperature_2m_max",
             "temperature_2m_min",
             "apparent_temperature_max",
             "apparent_temperature_min",
@@ -933,17 +739,15 @@
     daily_wind_speed_10m_max = daily.Variables(5).ValuesAsNumpy()
     daily_wind_gusts_10m_max = daily.Variables(6).ValuesAsNumpy()
     daily_wind_direction_10m_dominant = daily.Variables(7).ValuesAsNumpy()
     weather_code = daily.Variables(8).ValuesAsNumpy()
     snowfall = daily.Variables(9).ValuesAsNumpy()
     precipitation_hours= daily.Variables(10).ValuesAsNumpy()
     sunshine_duration= daily.Variables(11).ValuesAsNumpy()
-    date_debut = pd.to_datetime(daily.Time(), unit="s", utc=True)
     return (
-        date_debut,
         daily_temperature_2m_min,
         daily_temperature_2m_max,
         daily_apparent_temperature_min,
         daily_apparent_temperature_max,
         daily_precipitation_sum,
         daily_wind_speed_10m_max,
         daily_wind_gusts_10m_max,
@@ -955,15 +759,15 @@
     )
 
 
 def specific_day(latitude, longitude, day):
     cache_session = requests_cache.CachedSession(
         get_user_config_directory_pyweather() + ".cache", expire_after=3600
     )
-    retry_session = retry(cache_session, retries=5, backoff_factor=0.2)
+    retry_session = retry_requests.retry(cache_session, retries=5, backoff_factor=0.2)
     openmeteo = openmeteo_requests.Client(session=retry_session)
     url = "https://api.open-meteo.com/v1/meteofrance"
     params = {
         "timezone": "Europe/Paris",
         "latitude": latitude,
         "longitude": longitude,
         "hourly": [
@@ -1023,15 +827,15 @@
                 )
 
 
 def current(latitude, longitude):
     cache_session = requests_cache.CachedSession(
         get_user_config_directory_pyweather() + ".cache", expire_after=3600
     )
-    retry_session = retry(cache_session, retries=5, backoff_factor=0.2)
+    retry_session = retry_requests.retry(cache_session, retries=5, backoff_factor=0.2)
     openmeteo = openmeteo_requests.Client(session=retry_session)
 
     url = "https://api.open-meteo.com/v1/meteofrance"
     params = {
         "latitude": latitude,
         "longitude": longitude,
         "current": [
```

### Comparing `pyweatherfr-3.0.0/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-4.0.0/pyweatherfr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 3.0.0
+Version: 4.0.0
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -14,15 +14,13 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 License-File: LICENSE.txt
 Requires-Dist: columnar
 Requires-Dist: termcolor
 Requires-Dist: colorama
-Requires-Dist: unidecode
-Requires-Dist: requests
 Requires-Dist: openmeteo_requests
 Requires-Dist: requests_cache
-Requires-Dist: pandas
 Requires-Dist: retry_requests
+Requires-Dist: geopy
 
 The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme
```

### Comparing `pyweatherfr-3.0.0/setup.py` & `pyweatherfr-4.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="3.0.0",
+    version="4.0.0",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
-    install_requires=["columnar","termcolor", "colorama","unidecode","requests","openmeteo_requests","requests_cache","pandas","retry_requests"],
+    install_requires=["columnar","termcolor", "colorama","openmeteo_requests","requests_cache","retry_requests","geopy"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "pyweatherfr=pyweatherfr.__init__:pyweatherfr"
         ],
     },
     classifiers=[
```

