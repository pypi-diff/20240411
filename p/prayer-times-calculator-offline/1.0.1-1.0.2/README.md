# Comparing `tmp/prayer_times_calculator_offline-1.0.1.tar.gz` & `tmp/prayer_times_calculator_offline-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prayer_times_calculator_offline-1.0.1.tar", last modified: Sun Apr  7 18:38:53 2024, max compression
+gzip compressed data, was "prayer_times_calculator_offline-1.0.2.tar", last modified: Thu Apr 11 13:16:49 2024, max compression
```

## Comparing `prayer_times_calculator_offline-1.0.1.tar` & `prayer_times_calculator_offline-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 cfair     (1000) users      (100)        0 2024-04-07 18:38:53.964519 prayer_times_calculator_offline-1.0.1/
--rw-r--r--   0 cfair     (1000) users      (100)     1052 2024-04-05 16:47:19.000000 prayer_times_calculator_offline-1.0.1/LICENSE
--rw-r--r--   0 cfair     (1000) users      (100)       16 2024-04-05 16:47:19.000000 prayer_times_calculator_offline-1.0.1/MANIFEST.in
--rw-r--r--   0 cfair     (1000) users      (100)     3142 2024-04-07 18:38:53.964519 prayer_times_calculator_offline-1.0.1/PKG-INFO
--rw-r--r--   0 cfair     (1000) users      (100)     2816 2024-04-07 18:38:04.000000 prayer_times_calculator_offline-1.0.1/README.MD
-drwxr-xr-x   0 cfair     (1000) users      (100)        0 2024-04-07 18:38:53.963519 prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline/
--rw-r--r--   0 cfair     (1000) users      (100)      237 2024-04-07 18:06:09.000000 prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline/__init__.py
--rw-r--r--   0 cfair     (1000) users      (100)      491 2024-04-05 16:47:19.000000 prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline/exceptions.py
--rw-r--r--   0 cfair     (1000) users      (100)    13227 2024-04-07 18:16:28.000000 prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline/interop.py
--rw-r--r--   0 cfair     (1000) users      (100)     1644 2024-04-07 18:16:07.000000 prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline/methods.py
--rw-r--r--   0 cfair     (1000) users      (100)    15822 2024-04-07 18:11:56.000000 prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline/praytimes.py
-drwxr-xr-x   0 cfair     (1000) users      (100)        0 2024-04-07 18:38:53.964519 prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline.egg-info/
--rw-r--r--   0 cfair     (1000) users      (100)     3142 2024-04-07 18:38:53.000000 prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline.egg-info/PKG-INFO
--rw-r--r--   0 cfair     (1000) users      (100)      485 2024-04-07 18:38:53.000000 prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline.egg-info/SOURCES.txt
--rw-r--r--   0 cfair     (1000) users      (100)        1 2024-04-07 18:38:53.000000 prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline.egg-info/dependency_links.txt
--rw-r--r--   0 cfair     (1000) users      (100)       32 2024-04-07 18:38:53.000000 prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline.egg-info/top_level.txt
--rw-r--r--   0 cfair     (1000) users      (100)      338 2024-04-07 18:38:48.000000 prayer_times_calculator_offline-1.0.1/pyproject.toml
--rw-r--r--   0 cfair     (1000) users      (100)       38 2024-04-07 18:38:53.964519 prayer_times_calculator_offline-1.0.1/setup.cfg
+drwxr-xr-x   0 cfair     (1000) users      (100)        0 2024-04-11 13:16:49.128608 prayer_times_calculator_offline-1.0.2/
+-rw-r--r--   0 cfair     (1000) users      (100)     1052 2024-04-05 16:47:19.000000 prayer_times_calculator_offline-1.0.2/LICENSE
+-rw-r--r--   0 cfair     (1000) users      (100)       16 2024-04-05 16:47:19.000000 prayer_times_calculator_offline-1.0.2/MANIFEST.in
+-rw-r--r--   0 cfair     (1000) users      (100)     3147 2024-04-11 13:16:49.128608 prayer_times_calculator_offline-1.0.2/PKG-INFO
+-rw-r--r--   0 cfair     (1000) users      (100)     2821 2024-04-11 13:14:33.000000 prayer_times_calculator_offline-1.0.2/README.MD
+drwxr-xr-x   0 cfair     (1000) users      (100)        0 2024-04-11 13:16:49.128608 prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline/
+-rw-r--r--   0 cfair     (1000) users      (100)      237 2024-04-07 18:06:09.000000 prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline/__init__.py
+-rw-r--r--   0 cfair     (1000) users      (100)      491 2024-04-05 16:47:19.000000 prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline/exceptions.py
+-rw-r--r--   0 cfair     (1000) users      (100)    13183 2024-04-11 13:14:33.000000 prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline/interop.py
+-rw-r--r--   0 cfair     (1000) users      (100)     1644 2024-04-07 18:16:07.000000 prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline/methods.py
+-rw-r--r--   0 cfair     (1000) users      (100)    15822 2024-04-07 18:11:56.000000 prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline/praytimes.py
+drwxr-xr-x   0 cfair     (1000) users      (100)        0 2024-04-11 13:16:49.128608 prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline.egg-info/
+-rw-r--r--   0 cfair     (1000) users      (100)     3147 2024-04-11 13:16:49.000000 prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline.egg-info/PKG-INFO
+-rw-r--r--   0 cfair     (1000) users      (100)      485 2024-04-11 13:16:49.000000 prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline.egg-info/SOURCES.txt
+-rw-r--r--   0 cfair     (1000) users      (100)        1 2024-04-11 13:16:49.000000 prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline.egg-info/dependency_links.txt
+-rw-r--r--   0 cfair     (1000) users      (100)       32 2024-04-11 13:16:49.000000 prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline.egg-info/top_level.txt
+-rw-r--r--   0 cfair     (1000) users      (100)      338 2024-04-11 13:15:12.000000 prayer_times_calculator_offline-1.0.2/pyproject.toml
+-rw-r--r--   0 cfair     (1000) users      (100)       38 2024-04-11 13:16:49.128608 prayer_times_calculator_offline-1.0.2/setup.cfg
```

### Comparing `prayer_times_calculator_offline-1.0.1/LICENSE` & `prayer_times_calculator_offline-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prayer_times_calculator_offline-1.0.1/PKG-INFO` & `prayer_times_calculator_offline-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prayer_times_calculator_offline
-Version: 1.0.1
+Version: 1.0.2
 Summary: Prayer Times Calculator - Offline
 Author-email: "cpfair, Umair Chagani" <cpf@cpfx.ca>
 License: MIT
 Project-URL: Homepage, https://github.com/cfair/prayer-times-calculator-offline
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -14,19 +14,17 @@
 
 
 Equivalence to the `prayer-times-calculator` library was checked by emperical comparison of 50,000 requests (each with randomized parameters). The original intention was to replicate the output exactly, however please note the following exceptions where `prayer-times-calculator-offline` will return a different result than `prayer-times-calculator` for the same call:
 
 * Asr calculation is stable; at time of writing, AlAdhan's API uses the [API server's local time](https://github.com/islamic-network/prayer-times/blob/f7ed3a2467fbced252a0914c8b202c8b61ca58b9/src/PrayerTimes/PrayerTimes.php#L538) as part of the Asr calculation, causing the returned time to drift as the server's day progresses.
 * ISO8601 date components are correct; at time of writing, AlAdhan's API sometime returns ISO8601 timestamps with correct times but incorrect dates.
   * E.g. [this API call](https://api.aladhan.com/v1/timings/28-06-2042?latitude=78.76131061889032&longitude=72.35356426766558&method=21&iso8601=true&school=1&midnightMode=1&latitudeAdjustmentMethod=3&tune=1%2C3%2C-1%2C5%2C4%2C4%2C-2%2C-2%2C1) where all timestamps are returned with the same date component, making Isha appear to happen before Maghrib and Fajr appear to happen after Sunrise
-* Portugal Maghrib tuning applied correctly; At time of writing, AlAdhan's API maps the [Asr tuning value to Maghrib](https://github.com/islamic-network/api.aladhan.com/blob/f3d57f7c7b54f5bb9592efdb984fbbea41093f82/api/Utils/PrayerTimesHelper.php#L306)
+* Portugal Maghrib tuning applied correctly; ~At time of writing, AlAdhan's API maps the [Asr tuning value to Maghrib.](https://github.com/islamic-network/api.aladhan.com/blob/f3d57f7c7b54f5bb9592efdb984fbbea41093f82/api/Utils/PrayerTimesHelper.php#L306)~ Since [fixed in API](https://github.com/islamic-network/api.aladhan.com/pull/75)
 * Local time output (`iso8601=False`) is not supported, as it is not required for use in HomeAssistant (which deals only with UTC internally)
 * 'None' is supported as a high-latitude adjustment method
 * Angles of 0 are supported for the "custom" calculation method; at time of writing, AlAdhan's API silently ignores such angles and uses a different default angle in their place.
 * Floating point computations take place on your CPU, which may vary from the AlAdhan API server's CPU; there may be 1-minute differences if these computational variations span a rounding break. Hijri date calculation may also be affected, including the 30-minute Isha offset during Ramadan when using the Makkah calculation method.
 
 
-*The remainder of this README is based on that from prayer-times-calculator.*
-
 ## Usage
 
 Please refer to the [usage section of `prayer-times-calculator`](https://github.com/uchagani/prayer-times-calculator?tab=readme-ov-file#usage).
```

### Comparing `prayer_times_calculator_offline-1.0.1/README.MD` & `prayer_times_calculator_offline-1.0.2/README.MD`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 
 
 Equivalence to the `prayer-times-calculator` library was checked by emperical comparison of 50,000 requests (each with randomized parameters). The original intention was to replicate the output exactly, however please note the following exceptions where `prayer-times-calculator-offline` will return a different result than `prayer-times-calculator` for the same call:
 
 * Asr calculation is stable; at time of writing, AlAdhan's API uses the [API server's local time](https://github.com/islamic-network/prayer-times/blob/f7ed3a2467fbced252a0914c8b202c8b61ca58b9/src/PrayerTimes/PrayerTimes.php#L538) as part of the Asr calculation, causing the returned time to drift as the server's day progresses.
 * ISO8601 date components are correct; at time of writing, AlAdhan's API sometime returns ISO8601 timestamps with correct times but incorrect dates.
   * E.g. [this API call](https://api.aladhan.com/v1/timings/28-06-2042?latitude=78.76131061889032&longitude=72.35356426766558&method=21&iso8601=true&school=1&midnightMode=1&latitudeAdjustmentMethod=3&tune=1%2C3%2C-1%2C5%2C4%2C4%2C-2%2C-2%2C1) where all timestamps are returned with the same date component, making Isha appear to happen before Maghrib and Fajr appear to happen after Sunrise
-* Portugal Maghrib tuning applied correctly; At time of writing, AlAdhan's API maps the [Asr tuning value to Maghrib](https://github.com/islamic-network/api.aladhan.com/blob/f3d57f7c7b54f5bb9592efdb984fbbea41093f82/api/Utils/PrayerTimesHelper.php#L306)
+* Portugal Maghrib tuning applied correctly; ~At time of writing, AlAdhan's API maps the [Asr tuning value to Maghrib.](https://github.com/islamic-network/api.aladhan.com/blob/f3d57f7c7b54f5bb9592efdb984fbbea41093f82/api/Utils/PrayerTimesHelper.php#L306)~ Since [fixed in API](https://github.com/islamic-network/api.aladhan.com/pull/75)
 * Local time output (`iso8601=False`) is not supported, as it is not required for use in HomeAssistant (which deals only with UTC internally)
 * 'None' is supported as a high-latitude adjustment method
 * Angles of 0 are supported for the "custom" calculation method; at time of writing, AlAdhan's API silently ignores such angles and uses a different default angle in their place.
 * Floating point computations take place on your CPU, which may vary from the AlAdhan API server's CPU; there may be 1-minute differences if these computational variations span a rounding break. Hijri date calculation may also be affected, including the 30-minute Isha offset during Ramadan when using the Makkah calculation method.
 
 
-*The remainder of this README is based on that from prayer-times-calculator.*
-
 ## Usage
 
 Please refer to the [usage section of `prayer-times-calculator`](https://github.com/uchagani/prayer-times-calculator?tab=readme-ov-file#usage).
```

### Comparing `prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline/interop.py` & `prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline/interop.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,15 +356,14 @@
             self._date, (self._latitude, self._longitude), timezone=0, format="Float"
         )
 
         response: dict[str, typing.Any] = {}
 
         for k, v in times_float.items():
             ts = datetime.combine(self._date, time()) + timedelta(hours=v)
-            print(k, v, ts, times_float[k])
 
             # Rounding
             ts = (ts + timedelta(seconds=30) - timedelta.resolution).replace(
                 second=0, microsecond=0
             )
             response[k[0].upper() + k[1:]] = ts.replace(tzinfo=timezone.utc).isoformat()
```

### Comparing `prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline/methods.py` & `prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline/methods.py`

 * *Files identical despite different names*

### Comparing `prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline/praytimes.py` & `prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline/praytimes.py`

 * *Files identical despite different names*

### Comparing `prayer_times_calculator_offline-1.0.1/prayer_times_calculator_offline.egg-info/PKG-INFO` & `prayer_times_calculator_offline-1.0.2/prayer_times_calculator_offline.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prayer_times_calculator_offline
-Version: 1.0.1
+Version: 1.0.2
 Summary: Prayer Times Calculator - Offline
 Author-email: "cpfair, Umair Chagani" <cpf@cpfx.ca>
 License: MIT
 Project-URL: Homepage, https://github.com/cfair/prayer-times-calculator-offline
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -14,19 +14,17 @@
 
 
 Equivalence to the `prayer-times-calculator` library was checked by emperical comparison of 50,000 requests (each with randomized parameters). The original intention was to replicate the output exactly, however please note the following exceptions where `prayer-times-calculator-offline` will return a different result than `prayer-times-calculator` for the same call:
 
 * Asr calculation is stable; at time of writing, AlAdhan's API uses the [API server's local time](https://github.com/islamic-network/prayer-times/blob/f7ed3a2467fbced252a0914c8b202c8b61ca58b9/src/PrayerTimes/PrayerTimes.php#L538) as part of the Asr calculation, causing the returned time to drift as the server's day progresses.
 * ISO8601 date components are correct; at time of writing, AlAdhan's API sometime returns ISO8601 timestamps with correct times but incorrect dates.
   * E.g. [this API call](https://api.aladhan.com/v1/timings/28-06-2042?latitude=78.76131061889032&longitude=72.35356426766558&method=21&iso8601=true&school=1&midnightMode=1&latitudeAdjustmentMethod=3&tune=1%2C3%2C-1%2C5%2C4%2C4%2C-2%2C-2%2C1) where all timestamps are returned with the same date component, making Isha appear to happen before Maghrib and Fajr appear to happen after Sunrise
-* Portugal Maghrib tuning applied correctly; At time of writing, AlAdhan's API maps the [Asr tuning value to Maghrib](https://github.com/islamic-network/api.aladhan.com/blob/f3d57f7c7b54f5bb9592efdb984fbbea41093f82/api/Utils/PrayerTimesHelper.php#L306)
+* Portugal Maghrib tuning applied correctly; ~At time of writing, AlAdhan's API maps the [Asr tuning value to Maghrib.](https://github.com/islamic-network/api.aladhan.com/blob/f3d57f7c7b54f5bb9592efdb984fbbea41093f82/api/Utils/PrayerTimesHelper.php#L306)~ Since [fixed in API](https://github.com/islamic-network/api.aladhan.com/pull/75)
 * Local time output (`iso8601=False`) is not supported, as it is not required for use in HomeAssistant (which deals only with UTC internally)
 * 'None' is supported as a high-latitude adjustment method
 * Angles of 0 are supported for the "custom" calculation method; at time of writing, AlAdhan's API silently ignores such angles and uses a different default angle in their place.
 * Floating point computations take place on your CPU, which may vary from the AlAdhan API server's CPU; there may be 1-minute differences if these computational variations span a rounding break. Hijri date calculation may also be affected, including the 30-minute Isha offset during Ramadan when using the Makkah calculation method.
 
 
-*The remainder of this README is based on that from prayer-times-calculator.*
-
 ## Usage
 
 Please refer to the [usage section of `prayer-times-calculator`](https://github.com/uchagani/prayer-times-calculator?tab=readme-ov-file#usage).
```

