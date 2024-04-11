# Comparing `tmp/apoplast-2.0.7.tar.gz` & `tmp/apoplast-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apoplast-2.0.7.tar", max compression
+gzip compressed data, was "apoplast-2.0.8.tar", max compression
```

## Comparing `apoplast-2.0.7.tar` & `apoplast-2.0.8.tar`

### file list

```diff
@@ -1,593 +1,593 @@
--rw-r--r--   0        0        0      757 2024-04-11 20:36:05.381259 apoplast-2.0.7/pyproject.toml
--rwxr-xr-x   0        0        0      540 2024-04-11 17:29:17.329381 apoplast-2.0.7/readme.md
--rwxr-xr-x   0        0        0     1431 2024-04-11 20:25:17.648072 apoplast-2.0.7/venue.S.HTML
--rwxr-xr-x   0        0        0      427 2024-02-04 21:45:08.055173 apoplast-2.0.7/venues/stages/apoplast/___license/license.s.HTML
--rw-r--r--   0        0        0      370 2024-04-11 17:19:27.770864 apoplast-2.0.7/venues/stages/apoplast/___license/list/coms.s.HTML
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 apoplast-2.0.7/venues/stages/apoplast/___license/list/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      112 2024-02-04 21:44:43.992353 apoplast-2.0.7/venues/stages/apoplast/___license/list/vegan.s.HTML
--rwxr-xr-x   0        0        0      379 2024-04-08 03:42:51.464524 apoplast-2.0.7/venues/stages/apoplast/__bin/apoplast_1
--rwxr-xr-x   0        0        0        0 2024-04-11 20:16:42.949103 apoplast-2.0.7/venues/stages/apoplast/__init__.py
--rwxr-xr-x   0        0        0      772 2024-04-10 01:40:13.241532 apoplast-2.0.7/venues/stages/apoplast/__itinerary/apoplast.S.HTML
--rwxr-xr-x   0        0        0      405 2024-04-08 03:26:57.443923 apoplast-2.0.7/venues/stages/apoplast/__itinerary/book/Vitamin B.S.HTML
--rwxr-xr-x   0        0        0       63 2024-04-08 03:27:04.947828 apoplast-2.0.7/venues/stages/apoplast/__itinerary/book/Vitamin K.S.HTML
--rwxr-xr-x   0        0        0  6858198 2024-04-11 17:28:33.233991 apoplast-2.0.7/venues/stages/apoplast/__status/db/records.json
--rwxr-xr-x   0        0        0    50398 2024-04-10 05:20:39.085373 apoplast-2.0.7/venues/stages/apoplast/__status/db_API/records.json
--rwxr-xr-x   0        0        0     1457 2024-04-11 17:25:09.951874 apoplast-2.0.7/venues/stages/apoplast/__status/status.proc.py
--rwxr-xr-x   0        0        0     1169 2024-04-10 05:16:26.771953 apoplast-2.0.7/venues/stages/apoplast/__status/status_API.proc.py
--rwxr-xr-x   0        0        0      428 2024-04-10 05:17:06.307551 apoplast-2.0.7/venues/stages/apoplast/_ellipses/__init__.py
--rw-r--r--   0        0        0      595 2024-04-10 05:17:08.375530 apoplast-2.0.7/venues/stages/apoplast/_ellipses/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      891 2024-02-04 20:02:36.038251 apoplast-2.0.7/venues/stages/apoplast/_ellipses/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1172 2024-04-11 17:13:36.374807 apoplast-2.0.7/venues/stages/apoplast/_interfaces/clique/__init__.py
--rw-r--r--   0        0        0     1530 2024-04-11 17:13:40.986742 apoplast-2.0.7/venues/stages/apoplast/_interfaces/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      297 2024-04-08 03:41:14.873594 apoplast-2.0.7/venues/stages/apoplast/_interfaces/clique/group/__init__.py
--rwxr-xr-x   0        0        0      703 2024-04-08 03:43:34.852041 apoplast-2.0.7/venues/stages/apoplast/_interfaces/clique/group/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        2 2024-04-11 17:08:27.110508 apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/__init__.py
--rw-r--r--   0        0        0      157 2024-04-11 17:13:41.498735 apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1198 2024-04-11 17:13:41.498735 apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/__pycache__/clique.cpython-310.pyc
--rw-r--r--   0        0        0      245 2024-04-11 17:13:41.498735 apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/__pycache__/off.cpython-310.pyc
--rw-r--r--   0        0        0      345 2024-04-11 17:13:41.498735 apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      251 2024-04-11 17:13:41.498735 apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/__pycache__/status.cpython-310.pyc
--rw-r--r--   0        0        0      728 2024-04-11 17:12:41.519615 apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/clique.py
--rw-r--r--   0        0        0       45 2024-04-11 17:08:40.814410 apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/customs.S.HTML
--rw-r--r--   0        0        0       25 2024-04-11 17:10:34.789623 apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/off.py
--rw-r--r--   0        0        0      102 2024-04-11 17:10:28.957663 apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/on.py
--rw-r--r--   0        0        0       25 2024-04-11 17:12:20.871941 apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/status.py
--rw-r--r--   0        0        0     1009 2024-04-09 21:23:47.661473 apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1203 2024-04-10 01:56:49.759392 apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/__pycache__/clique.cpython-310.pyc
--rw-r--r--   0        0        0     1175 2024-04-09 22:04:41.609395 apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/__pycache__/harbor.cpython-310.pyc
--rw-r--r--   0        0        0      818 2024-04-09 22:06:02.852384 apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/__pycache__/off.cpython-310.pyc
--rw-r--r--   0        0        0      870 2024-04-09 21:57:44.518681 apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      870 2024-04-10 01:38:51.770292 apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/clique.py
--rwxr-xr-x   0        0        0     1535 2024-04-09 22:04:27.465571 apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/harbor.py
--rwxr-xr-x   0        0        0      500 2024-04-09 22:05:47.060581 apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/off.py
--rwxr-xr-x   0        0        0      624 2024-04-09 21:57:42.582706 apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/on.py
--rwxr-xr-x   0        0        0     1314 2024-04-09 21:54:23.433322 apoplast-2.0.7/venues/stages/apoplast/_variables/__init__.py
--rw-r--r--   0        0        0     1307 2024-04-09 21:54:34.813170 apoplast-2.0.7/venues/stages/apoplast/_variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      118 2024-02-04 18:06:33.920433 apoplast-2.0.7/venues/stages/apoplast/clouds/affiliates_Amazon/affiliates.s.HTML
--rwxr-xr-x   0        0        0      111 2024-03-31 01:44:52.099453 apoplast-2.0.7/venues/stages/apoplast/clouds/clouds.S.HTML
--rwxr-xr-x   0        0        0      607 2024-02-04 21:46:15.410669 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/__pycache__/source.cpython-310.pyc
--rwxr-xr-x   0        0        0      738 2023-11-16 23:18:39.357737 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/__pycache__/source.cpython-311.pyc
--rwxr-xr-x   0        0        0     1036 2024-03-31 22:06:11.113782 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__init__.py
--rwxr-xr-x   0        0        0     1277 2024-03-31 22:08:36.588698 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2127 2023-11-17 00:20:13.313296 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2023-10-12 21:45:50.642367 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/BRANDED.cpython-311.pyc
--rwxr-xr-x   0        0        0      450 2023-10-12 21:45:50.642367 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/FOUNDATIONAL.cpython-311.pyc
--rwxr-xr-x   0        0        0      545 2024-02-04 21:46:15.409669 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-310.pyc
--rwxr-xr-x   0        0        0      778 2023-10-29 21:44:27.877088 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-311.pyc
--rwxr-xr-x   0        0        0      508 2024-02-04 21:46:15.410669 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-310.pyc
--rwxr-xr-x   0        0        0      677 2023-11-17 17:51:16.699708 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-311.pyc
--rwxr-xr-x   0        0        0      429 2023-10-29 21:44:17.338209 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/branded.py
--rwxr-xr-x   0        0        0      264 2023-11-17 17:51:13.692733 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/foundational.py
--rwxr-xr-x   0        0        0      419 2023-11-17 00:19:37.192708 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/status/API_status_branded_1.py
--rwxr-xr-x   0        0        0      465 2023-11-17 00:19:37.195707 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/status/API_status_foundational_1.py
--rwxr-xr-x   0        0        0      370 2023-11-16 23:17:45.538337 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/source.py
--rwxr-xr-x   0        0        0     1009 2023-11-22 01:31:31.581903 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/__init__.py
--rwxr-xr-x   0        0        0     1214 2024-02-04 21:46:15.411669 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2082 2023-11-22 01:32:30.716226 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0    37079 2023-12-09 20:38:41.901230 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON
--rwxr-xr-x   0        0        0    37079 2023-11-22 01:40:03.461042 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON
--rwxr-xr-x   0        0        0     7242 2023-10-19 22:27:22.121247 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/beet_juice_2412474.JSON
--rwxr-xr-x   0        0        0     8522 2023-10-12 21:13:07.386564 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/beet_juice_2642759.JSON
--rwxr-xr-x   0        0        0    33964 2023-11-22 01:38:38.653013 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/impossible_beef_2664238.JSON
--rwxr-xr-x   0        0        0    17926 2023-09-25 16:28:17.430256 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/problems/impossible_2468423.JSON
--rwxr-xr-x   0        0        0      104 2023-11-26 02:04:47.345653 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/problems/problems.r.HTML
--rwxr-xr-x   0        0        0    10678 2023-11-22 01:32:41.686100 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/vegan_pizza_2672996.JSON
--rwxr-xr-x   0        0        0    10670 2023-10-24 03:17:57.735576 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/walnuts_1882785.JSON
--rwxr-xr-x   0        0        0   189146 2023-10-12 22:00:16.639151 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON
--rwxr-xr-x   0        0        0      255 2023-11-17 18:04:07.057375 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/mergers.r.HTML
--rwxr-xr-x   0        0        0       88 2023-11-22 01:27:20.472779 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/priorities.r.HTML
--rwxr-xr-x   0        0        0      457 2023-12-09 23:06:15.605787 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/status_1.py
--rwxr-xr-x   0        0        0      614 2023-12-15 19:53:16.754046 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/food.s.HTML
--rwxr-xr-x   0        0        0       28 2023-11-22 04:54:08.017554 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/foodNutrient/__init__.py
--rwxr-xr-x   0        0        0       28 2023-11-22 02:45:04.164448 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/labelNutrient/__init__.py
--rwxr-xr-x   0        0        0     1783 2023-11-23 18:42:09.922568 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__init__.py
--rwxr-xr-x   0        0        0     1324 2024-02-04 21:46:15.413668 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2050 2023-11-23 18:42:13.005533 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      571 2024-02-04 21:46:15.416669 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/assertions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1065 2023-11-22 00:03:16.653487 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/assertions.cpython-311.pyc
--rwxr-xr-x   0        0        0      583 2023-11-22 00:01:06.946973 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/assertions.py
--rwxr-xr-x   0        0        0     4126 2023-11-22 20:58:41.034879 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__init__.py
--rwxr-xr-x   0        0        0     3007 2024-02-04 21:46:15.415669 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     5397 2023-11-22 21:04:24.375937 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1229 2023-11-22 20:47:39.030385 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_mass_1.py
--rwxr-xr-x   0        0        0      877 2023-11-22 20:23:41.394700 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_volume_1.py
--rwxr-xr-x   0        0        0      415 2023-11-22 20:49:55.692835 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/__init__.py
--rwxr-xr-x   0        0        0      547 2024-02-04 21:46:15.416669 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      946 2023-11-22 20:50:32.179422 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1374 2023-11-22 20:23:29.910831 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/status_1.py
--rwxr-xr-x   0        0        0     5029 2024-01-08 21:02:44.875367 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/__init__.py
--rwxr-xr-x   0        0        0     2923 2024-02-04 21:46:15.412669 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4846 2024-02-04 19:05:42.507811 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     2606 2024-02-04 20:24:03.556661 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_1.py
--rwxr-xr-x   0        0        0     1610 2023-12-09 20:39:39.205746 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_2.py
--rwxr-xr-x   0        0        0     1236 2023-12-17 01:49:13.793860 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_2412474.py
--rwxr-xr-x   0        0        0     1078 2023-12-17 00:42:09.947955 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_3.py
--rwxr-xr-x   0        0        0      812 2023-12-09 20:39:39.218746 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_loop_1.py
--rwxr-xr-x   0        0        0     3302 2023-12-15 23:15:41.332733 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__init__.py
--rwxr-xr-x   0        0        0     2102 2024-02-04 22:00:53.434098 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3367 2023-12-15 23:15:51.961647 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0        4 2023-11-26 00:02:13.258869 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/energy/__init__.py
--rwxr-xr-x   0        0        0     3116 2023-12-17 00:12:42.461151 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__init__.py
--rwxr-xr-x   0        0        0     2324 2024-02-04 22:00:53.448098 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3653 2023-12-17 00:13:04.029904 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     4031 2023-11-26 01:50:19.679543 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/form/__init__.py
--rwxr-xr-x   0        0        0     2394 2024-02-04 22:00:53.442098 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/form/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4016 2023-11-26 01:51:17.420831 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/form/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1231 2024-03-31 22:06:29.601567 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/form/status_mass_1.py
--rwxr-xr-x   0        0        0     1159 2023-11-26 00:30:32.288953 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/form/status_volume_1.py
--rwxr-xr-x   0        0        0     1427 2023-11-27 04:58:37.292037 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__init__.py
--rwxr-xr-x   0        0        0     1112 2024-02-04 22:00:53.443098 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1591 2023-11-27 18:18:50.779625 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1676 2023-11-26 01:00:29.154907 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_IU_1.py
--rwxr-xr-x   0        0        0     1875 2024-03-31 22:07:48.608961 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_energy_1.py
--rwxr-xr-x   0        0        0     1579 2023-11-26 01:00:16.204059 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_mass_1.py
--rwxr-xr-x   0        0        0     2077 2023-11-26 01:09:26.265614 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__init__.py
--rwxr-xr-x   0        0        0     2087 2024-02-04 22:00:53.444098 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3142 2023-11-26 01:10:28.190888 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1224 2023-11-26 01:10:07.049136 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__init__.py
--rwxr-xr-x   0        0        0     1225 2024-02-04 22:00:53.446098 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1831 2023-11-26 01:10:28.192888 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1494 2023-11-26 23:54:17.527847 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__init__.py
--rwxr-xr-x   0        0        0     1190 2024-02-04 22:00:53.446098 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1791 2023-11-26 23:54:20.036817 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1389 2024-03-29 23:33:34.229759 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__init__.py
--rwxr-xr-x   0        0        0     1386 2024-03-29 23:33:56.513497 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1842 2023-11-27 18:18:50.784625 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      679 2024-02-04 22:00:53.444098 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-310.pyc
--rwxr-xr-x   0        0        0     1040 2023-11-26 02:05:12.327391 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-311.pyc
--rwxr-xr-x   0        0        0     1899 2023-11-26 00:58:42.572156 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/food_nutrient_calculator.cpython-311.pyc
--rwxr-xr-x   0        0        0      617 2024-02-04 22:00:53.445098 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-310.pyc
--rwxr-xr-x   0        0        0      845 2023-11-26 01:09:01.315906 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-311.pyc
--rwxr-xr-x   0        0        0      849 2023-11-22 04:50:34.615973 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/label_nutrient_calculator.cpython-311.pyc
--rwxr-xr-x   0        0        0      622 2023-11-26 02:01:26.676025 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/food_nutrient.py
--rwxr-xr-x   0        0        0      468 2023-11-22 04:50:10.260249 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/label_nutrient.py
--rwxr-xr-x   0        0        0      503 2023-11-26 00:52:57.775193 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/ingredient.r.HTML
--rwxr-xr-x   0        0        0      706 2023-11-22 20:45:42.034711 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/ingredient_prototype_1.r.HTML
--rwxr-xr-x   0        0        0      485 2023-11-26 01:53:47.219931 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/__init__.py
--rwxr-xr-x   0        0        0      656 2024-02-04 22:00:53.443098 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      957 2023-11-26 01:53:50.019895 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     2092 2023-11-24 04:45:08.346598 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_mass_1.py
--rwxr-xr-x   0        0        0      687 2023-11-26 00:51:56.712908 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_volume_1.py
--rwxr-xr-x   0        0        0     1058 2023-11-26 00:49:48.022415 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/example.r.HTML
--rwxr-xr-x   0        0        0      863 2023-11-23 23:49:12.698629 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__init__.py
--rwxr-xr-x   0        0        0      807 2024-02-04 22:00:53.447098 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1012 2023-11-23 23:49:23.582505 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      575 2023-11-23 23:46:06.183759 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__init__.py
--rwxr-xr-x   0        0        0      897 2024-02-04 22:00:53.447098 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1272 2023-11-23 23:46:09.669719 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1019 2023-11-23 23:47:00.051144 apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/status_1.py
--rwxr-xr-x   0        0        0     1791 2024-03-31 18:10:18.994424 apoplast-2.0.7/venues/stages/apoplast/clouds/goodness_certifications/certifications.py
--rwxr-xr-x   0        0        0      641 2024-03-31 20:50:04.634053 apoplast-2.0.7/venues/stages/apoplast/clouds/goodness_certifications/vegan.s.HTML
--rwxr-xr-x   0        0        0     1046 2024-03-31 02:07:55.069366 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/NIH.s.HTML
--rwxr-xr-x   0        0        0      547 2024-02-04 22:01:04.036019 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/__pycache__/source.cpython-310.pyc
--rwxr-xr-x   0        0        0      670 2023-10-25 01:34:03.568051 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/__pycache__/source.cpython-311.pyc
--rwxr-xr-x   0        0        0     1137 2024-03-31 22:06:43.569405 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__init__.py
--rw-r--r--   0        0        0     1141 2024-04-10 05:16:32.027900 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1889 2023-11-17 00:20:13.309296 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      826 2024-02-04 22:01:04.041019 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/assertions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1399 2023-10-25 01:34:03.568051 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/assertions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1087 2023-10-25 01:29:58.565739 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/assertions.py
--rwxr-xr-x   0        0        0      392 2023-11-17 00:20:01.903426 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/status/API_status_1.py
--rwxr-xr-x   0        0        0      316 2023-10-25 01:28:37.971623 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/source.py
--rwxr-xr-x   0        0        0      848 2023-11-27 22:36:33.129934 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/__init__.py
--rwxr-xr-x   0        0        0     1050 2024-02-04 21:46:18.952642 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1918 2023-11-27 22:37:23.089492 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0    44597 2023-10-13 17:10:19.838169 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/coated tablets/multivitamin_276336.JSON
--rwxr-xr-x   0        0        0    22180 2023-10-25 17:22:33.578905 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/other/chia_seeds_214893.JSON
--rwxr-xr-x   0        0        0     6430 2023-10-13 17:09:44.373557 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/powder/mane_270619.JSON
--rwxr-xr-x   0        0        0    72594 2023-10-25 01:46:01.092818 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/powder/nutritional_shake_220884.JSON
--rwxr-xr-x   0        0        0    57378 2023-10-13 17:05:59.829003 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/powder packets/multivitamin_246811.JSON
--rwxr-xr-x   0        0        0    22710 2023-10-13 17:08:42.546230 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/calcium_261967.JSON
--rwxr-xr-x   0        0        0    43725 2023-10-13 17:08:08.961596 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/multivitamin_249664.JSON
--rwxr-xr-x   0        0        0     7107 2023-10-13 17:07:29.648024 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/vegan_capsules/probiotics_248267.JSON
--rwxr-xr-x   0        0        0       98 2023-11-27 03:46:15.367425 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/__init__.py
--rwxr-xr-x   0        0        0      285 2024-02-04 21:46:18.226647 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      383 2023-11-27 04:14:12.512606 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1152 2023-11-27 04:24:46.432108 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__init__.py
--rwxr-xr-x   0        0        0      907 2024-02-04 21:46:18.227648 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1201 2023-11-27 04:25:03.266909 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      923 2023-11-27 04:25:24.402660 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/status_powder_packets_246811.py
--rwxr-xr-x   0        0        0       56 2023-11-27 04:49:39.293420 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/interpret/servingSizeUnit/__init__.py
--rwxr-xr-x   0        0        0     4087 2024-03-31 22:07:01.073202 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py
--rwxr-xr-x   0        0        0     3020 2024-03-31 22:08:36.760697 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4873 2023-12-16 03:49:29.728760 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      730 2023-11-27 22:52:02.622639 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/_loop/status_1.py
--rwxr-xr-x   0        0        0     1580 2024-03-11 02:00:19.620159 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336.py
--rwxr-xr-x   0        0        0   136857 2024-04-11 17:28:32.781997 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336_nature.JSON
--rwxr-xr-x   0        0        0   100726 2024-04-11 17:28:32.757998 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/chia_seeds_214893_nature.JSON
--rwxr-xr-x   0        0        0      762 2024-03-11 02:02:48.750472 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/status_chia_seeds_214893.py
--rwxr-xr-x   0        0        0    28773 2024-04-11 17:28:32.661999 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/mane_270619_nature.JSON
--rwxr-xr-x   0        0        0      748 2023-12-19 18:33:07.683544 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/status_mane_270619.py
--rwxr-xr-x   0        0        0     2753 2023-12-15 23:31:38.763948 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__init__.py
--rwxr-xr-x   0        0        0     2408 2024-02-04 22:00:53.505098 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3688 2023-12-15 23:31:44.199904 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     2583 2024-03-30 21:02:16.032550 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__init__.py
--rwxr-xr-x   0        0        0     2183 2024-03-30 21:02:46.768381 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3443 2023-12-15 23:31:44.195904 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      832 2023-11-27 20:26:53.811823 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/essential_nutrients.s.HTML
--rwxr-xr-x   0        0        0      281 2023-11-27 20:27:05.759787 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/essential_nutrients_priorities.s.HTML
--rwxr-xr-x   0        0        0      323 2023-11-27 04:41:57.157899 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/__init__.py
--rwxr-xr-x   0        0        0      560 2024-02-04 21:46:18.215648 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      672 2023-11-27 04:42:26.984546 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      676 2023-11-27 23:18:44.963779 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__init__.py
--rwxr-xr-x   0        0        0      870 2024-02-04 21:46:18.227648 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1333 2023-11-27 23:19:04.631610 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      510 2023-11-22 19:45:00.248952 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/status_other_214893.py
--rwxr-xr-x   0        0        0      512 2023-11-25 23:13:17.621118 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/form.r.HTML
--rwxr-xr-x   0        0        0     3759 2023-11-27 23:36:21.498654 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__init__.py
--rwxr-xr-x   0        0        0     2314 2024-02-04 21:46:18.228648 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4306 2023-11-27 23:36:25.653617 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0        0 2023-11-27 22:52:26.655429 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_1.py
--rwxr-xr-x   0        0        0     1841 2024-04-09 20:04:26.544534 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py
--rwxr-xr-x   0        0        0     1711 2023-11-27 23:47:05.617116 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py
--rwxr-xr-x   0        0        0     3210 2023-11-27 23:13:13.104637 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__init__.py
--rwxr-xr-x   0        0        0     2634 2024-02-04 21:46:18.224648 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4650 2023-11-27 23:13:23.844544 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      983 2023-11-27 23:17:35.529377 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py
--rwxr-xr-x   0        0        0      814 2023-11-22 18:01:32.907312 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_gram_1.py
--rwxr-xr-x   0        0        0      818 2023-11-22 19:42:51.390406 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_220884.py
--rwxr-xr-x   0        0        0      903 2023-11-22 19:46:12.236140 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_270619.py
--rwxr-xr-x   0        0        0     1333 2023-11-22 20:15:00.085618 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_packets_246811.py
--rwxr-xr-x   0        0        0      701 2023-11-22 20:21:05.755467 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_tablet_261967.py
--rwxr-xr-x   0        0        0      725 2023-11-22 19:30:39.266645 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py
--rwxr-xr-x   0        0        0     4631 2024-03-11 02:07:04.511863 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__init__.py
--rwxr-xr-x   0        0        0     2830 2024-03-11 02:07:07.519836 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4500 2024-02-04 19:05:43.260805 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1687 2024-03-11 02:13:24.344258 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py
--rwxr-xr-x   0        0        0        0 2023-11-27 05:04:38.944743 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/amount--/mass/__init__.py
--rwxr-xr-x   0        0        0     1514 2024-03-11 01:32:01.379383 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/measured_ingredient.s.HTML
--rwxr-xr-x   0        0        0     1656 2024-03-30 21:01:47.824701 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__init__.py
--rwxr-xr-x   0        0        0     1845 2024-03-30 21:02:46.768381 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2911 2023-11-27 05:46:33.775695 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      826 2024-03-11 02:03:57.637692 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py
--rwxr-xr-x   0        0        0      561 2023-11-27 05:48:16.117464 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/measured_ingredients.r.HTML
--rwxr-xr-x   0        0        0     1116 2023-11-27 05:48:52.161031 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__init__.py
--rwxr-xr-x   0        0        0     1078 2024-02-04 22:00:53.503098 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1442 2023-11-27 05:50:31.795832 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      657 2023-11-27 05:50:29.870855 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py
--rwxr-xr-x   0        0        0      511 2023-11-27 18:44:30.266270 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/__init__.py
--rwxr-xr-x   0        0        0      877 2024-02-04 22:00:56.631074 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1171 2023-11-27 18:44:33.989225 apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      527 2024-04-09 15:54:15.319774 apoplast-2.0.7/venues/stages/apoplast/data_nodes/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      233 2024-04-09 15:54:11.135807 apoplast-2.0.7/venues/stages/apoplast/data_nodes/clique.py
--rwxr-xr-x   0        0        0       96 2024-04-08 03:49:12.700230 apoplast-2.0.7/venues/stages/apoplast/data_nodes/data_nodes.S.HTML
--rwxr-xr-x   0        0        0       13 2024-04-08 04:26:53.388706 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/.gitignore
--rwxr-xr-x   0        0        0      677 2024-04-09 16:44:28.185484 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/connect.cpython-310.pyc
--rwxr-xr-x   0        0        0      826 2024-04-08 04:23:35.323211 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/off.cpython-310.pyc
--rw-r--r--   0        0        0     1856 2024-04-09 21:23:47.537474 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1522 2024-04-08 04:11:40.756704 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/open.cpython-310.pyc
--rwxr-xr-x   0        0        0     1500 2024-04-09 19:46:47.950169 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      554 2024-04-09 16:42:34.370813 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/connect.py
--rwxr-xr-x   0        0        0      632 2024-04-08 04:23:34.295224 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/off.py
--rwxr-xr-x   0        0        0     2119 2024-04-09 21:02:16.663855 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/on.py
--rwxr-xr-x   0        0        0        0 2024-04-08 04:30:53.369730 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/saves/dump.py
--rwxr-xr-x   0        0        0        0 2024-04-08 04:30:49.193781 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/saves/export.py
--rwxr-xr-x   0        0        0     1701 2024-04-09 19:46:45.714191 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/status.py
--rwxr-xr-x   0        0        0      454 2024-03-31 01:44:39.427583 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/__itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0     1542 2024-04-09 19:46:25.206393 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      118 2024-03-31 03:53:00.212849 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/cautionary_ingredients/cautionary_ingredients.1.json
--rwxr-xr-x   0        0        0     5140 2024-03-31 03:54:30.968103 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/essential_nutrients/essential_nutrients.1.json
--rwxr-xr-x   0        0        0      481 2024-03-31 03:53:37.064550 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/exports.S.HTML
--rwxr-xr-x   0        0        0       35 2024-04-09 20:14:48.596372 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/_saves/save.py
--rwxr-xr-x   0        0        0     1104 2024-04-09 19:46:23.838407 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/clique.py
--rwxr-xr-x   0        0        0      798 2024-03-31 03:45:22.693513 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/collections/_land/__pycache__/insert_document.cpython-310.pyc
--rwxr-xr-x   0        0        0      796 2024-03-31 03:43:31.086721 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/collections/_land/insert_document.py
--rwxr-xr-x   0        0        0      170 2024-04-08 03:47:20.717500 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/cautionary_ingredients.S.HTML
--rwxr-xr-x   0        0        0        2 2024-03-31 03:51:33.881524 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/collection/export.py
--rwxr-xr-x   0        0        0        0 2024-04-08 03:46:10.538293 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/document/insert.py
--rwxr-xr-x   0        0        0       27 2024-04-08 03:47:50.181167 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/collections/collections.S.HTML
--rwxr-xr-x   0        0        0        0 2024-03-31 03:51:29.633556 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/collections/essential_nutrients/export.py
--rwxr-xr-x   0        0        0     1523 2024-04-08 03:56:03.579528 apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/ingredients.S.HTML
--rwxr-xr-x   0        0        0       14 2024-03-31 22:10:20.784048 apoplast-2.0.7/venues/stages/apoplast/emojis.S.HTML
--rwxr-xr-x   0        0        0     1030 2024-02-04 21:46:14.886673 apoplast-2.0.7/venues/stages/apoplast/insure/__pycache__/equalities.cpython-310.pyc
--rwxr-xr-x   0        0        0     1871 2023-11-27 23:25:41.951185 apoplast-2.0.7/venues/stages/apoplast/insure/__pycache__/equalities.cpython-311.pyc
--rwxr-xr-x   0        0        0      453 2024-02-04 21:46:15.408669 apoplast-2.0.7/venues/stages/apoplast/insure/__pycache__/equality.cpython-310.pyc
--rwxr-xr-x   0        0        0      694 2023-11-22 19:22:56.114817 apoplast-2.0.7/venues/stages/apoplast/insure/__pycache__/equality.cpython-311.pyc
--rwxr-xr-x   0        0        0     1058 2024-02-04 21:46:17.800651 apoplast-2.0.7/venues/stages/apoplast/insure/__pycache__/override_print.cpython-310.pyc
--rwxr-xr-x   0        0        0     2001 2023-11-27 01:34:12.790621 apoplast-2.0.7/venues/stages/apoplast/insure/__pycache__/override_print.cpython-311.pyc
--rwxr-xr-x   0        0        0     1085 2023-11-27 23:25:39.844204 apoplast-2.0.7/venues/stages/apoplast/insure/equalities.py
--rwxr-xr-x   0        0        0      234 2023-11-22 18:56:47.658330 apoplast-2.0.7/venues/stages/apoplast/insure/equality.py
--rwxr-xr-x   0        0        0      729 2023-11-27 01:34:09.516659 apoplast-2.0.7/venues/stages/apoplast/insure/override_print.py
--rwxr-xr-x   0        0        0      374 2023-11-22 19:22:12.923299 apoplast-2.0.7/venues/stages/apoplast/insure/status_equalitites_1.py
--rwxr-xr-x   0        0        0     1480 2024-02-04 21:46:15.401669 apoplast-2.0.7/venues/stages/apoplast/measures/_interpret/__pycache__/unit_kind.cpython-310.pyc
--rwxr-xr-x   0        0        0     2547 2023-11-27 23:52:18.152450 apoplast-2.0.7/venues/stages/apoplast/measures/_interpret/__pycache__/unit_kind.cpython-311.pyc
--rwxr-xr-x   0        0        0       61 2023-10-24 19:09:48.581050 apoplast-2.0.7/venues/stages/apoplast/measures/_interpret/interpret.r.html
--rwxr-xr-x   0        0        0      670 2023-11-22 03:00:29.040898 apoplast-2.0.7/venues/stages/apoplast/measures/_interpret/status_unit_kind.py
--rwxr-xr-x   0        0        0     1678 2023-11-27 23:51:26.564890 apoplast-2.0.7/venues/stages/apoplast/measures/_interpret/unit_kind.py
--rwxr-xr-x   0        0        0        0 2023-11-22 02:29:15.950254 apoplast-2.0.7/venues/stages/apoplast/measures/biological_activity/__init__.py
--rwxr-xr-x   0        0        0       59 2024-02-26 21:23:18.202627 apoplast-2.0.7/venues/stages/apoplast/measures/electric_current/electric_current.S.HTML
--rwxr-xr-x   0        0        0     1142 2023-11-18 02:03:26.122070 apoplast-2.0.7/venues/stages/apoplast/measures/energy/energy.r.HTML
--rwxr-xr-x   0        0        0     1174 2023-11-27 05:11:29.583845 apoplast-2.0.7/venues/stages/apoplast/measures/energy/swap/__init__.py
--rwxr-xr-x   0        0        0     1027 2024-02-04 21:46:14.884672 apoplast-2.0.7/venues/stages/apoplast/measures/energy/swap/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1761 2023-11-27 05:11:32.899806 apoplast-2.0.7/venues/stages/apoplast/measures/energy/swap/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      386 2023-11-22 03:06:00.365118 apoplast-2.0.7/venues/stages/apoplast/measures/energy/swap/status_1.py
--rwxr-xr-x   0        0        0       71 2023-11-18 02:08:27.601504 apoplast-2.0.7/venues/stages/apoplast/measures/length/length.r.HTML
--rwxr-xr-x   0        0        0       95 2023-09-10 01:33:12.464335 apoplast-2.0.7/venues/stages/apoplast/measures/mass/e_note.py
--rwxr-xr-x   0        0        0       12 2023-10-24 23:00:23.774371 apoplast-2.0.7/venues/stages/apoplast/measures/mass/mass.r.html
--rwxr-xr-x   0        0        0     2329 2023-11-27 23:53:01.539080 apoplast-2.0.7/venues/stages/apoplast/measures/mass/swap/__init__.py
--rwxr-xr-x   0        0        0     1735 2024-02-04 21:46:14.882673 apoplast-2.0.7/venues/stages/apoplast/measures/mass/swap/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3229 2023-11-27 23:53:04.757052 apoplast-2.0.7/venues/stages/apoplast/measures/mass/swap/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1153 2023-11-21 20:24:21.450301 apoplast-2.0.7/venues/stages/apoplast/measures/mass/swap/status_1.py
--rwxr-xr-x   0        0        0     2419 2023-10-25 22:32:32.500043 apoplast-2.0.7/venues/stages/apoplast/measures/mass/system international.r.html
--rwxr-xr-x   0        0        0      768 2023-10-24 19:13:36.766543 apoplast-2.0.7/venues/stages/apoplast/measures/mass/us customary.r.html
--rwxr-xr-x   0        0        0      523 2023-11-18 02:19:07.769055 apoplast-2.0.7/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__init__.py
--rwxr-xr-x   0        0        0      643 2024-02-04 21:46:14.890673 apoplast-2.0.7/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      945 2023-11-18 02:33:55.200495 apoplast-2.0.7/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      342 2023-11-18 02:17:02.598121 apoplast-2.0.7/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/status_1.py
--rwxr-xr-x   0        0        0      861 2023-11-18 02:32:14.965350 apoplast-2.0.7/venues/stages/apoplast/measures/mass_equivalents/jargon.r.HTML
--rwxr-xr-x   0        0        0     2242 2023-12-09 18:56:13.594964 apoplast-2.0.7/venues/stages/apoplast/measures/mass_equivalents/mass equivalents.r.HTML
--rwxr-xr-x   0        0        0     2431 2024-02-26 20:25:18.856520 apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/__init__.py
--rwxr-xr-x   0        0        0     1665 2024-02-26 20:26:53.162839 apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3068 2023-11-26 02:13:59.845148 apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1428 2023-11-26 02:08:37.997986 apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/status_1.py
--rwxr-xr-x   0        0        0      901 2023-11-21 19:30:34.527895 apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/status_2.py
--rwxr-xr-x   0        0        0     1115 2023-11-21 19:30:34.540895 apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/status_3.py
--rwxr-xr-x   0        0        0      470 2023-11-26 02:09:05.917648 apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/status_sci_note_1.py
--rwxr-xr-x   0        0        0      170 2023-12-10 03:06:16.513154 apoplast-2.0.7/venues/stages/apoplast/measures/number/fraction_point/fraction_point.s.HTML
--rwxr-xr-x   0        0        0      539 2024-02-04 21:46:14.908672 apoplast-2.0.7/venues/stages/apoplast/measures/number/integer/__pycache__/string_is_integer.cpython-310.pyc
--rwxr-xr-x   0        0        0      749 2023-11-18 02:07:47.470846 apoplast-2.0.7/venues/stages/apoplast/measures/number/integer/__pycache__/string_is_integer.cpython-311.pyc
--rwxr-xr-x   0        0        0      560 2023-11-18 02:07:34.289958 apoplast-2.0.7/venues/stages/apoplast/measures/number/integer/status_string_is_integer.py
--rwxr-xr-x   0        0        0      368 2023-11-18 02:05:23.482071 apoplast-2.0.7/venues/stages/apoplast/measures/number/integer/string_is_integer.py
--rwxr-xr-x   0        0        0      899 2024-02-04 21:46:14.887673 apoplast-2.0.7/venues/stages/apoplast/measures/number/percentage/__pycache__/from_fraction.cpython-310.pyc
--rwxr-xr-x   0        0        0     1702 2023-11-21 19:30:05.993226 apoplast-2.0.7/venues/stages/apoplast/measures/number/percentage/__pycache__/from_fraction.cpython-311.pyc
--rwxr-xr-x   0        0        0      951 2023-11-21 19:30:01.342280 apoplast-2.0.7/venues/stages/apoplast/measures/number/percentage/from_fraction.py
--rwxr-xr-x   0        0        0      553 2023-11-18 02:34:50.110026 apoplast-2.0.7/venues/stages/apoplast/measures/number/percentage/status_1.py
--rwxr-xr-x   0        0        0     2211 2024-02-26 21:02:23.732405 apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note/__init__.py
--rwxr-xr-x   0        0        0     1448 2024-02-26 21:09:35.283275 apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3224 2024-02-26 21:13:28.392460 apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note/_status/status_multiples_of_3_1.py
--rwxr-xr-x   0        0        0      612 2024-02-26 21:07:29.400784 apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note/sci_note.S.HTML
--rwxr-xr-x   0        0        0      644 2024-02-26 21:07:36.720697 apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note/sci_note_possibilities.S.HTML
--rwxr-xr-x   0        0        0     1342 2024-02-26 21:09:10.127577 apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note/sci_note_thoughts.S.HTML
--rwxr-xr-x   0        0        0      363 2024-03-29 23:32:14.486695 apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note_2/__init__.py
--rwxr-xr-x   0        0        0      663 2024-03-29 23:33:54.137525 apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      936 2024-02-26 21:51:34.751894 apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note_2/status_1.py
--rwxr-xr-x   0        0        0       58 2023-10-24 22:59:09.790207 apoplast-2.0.7/venues/stages/apoplast/measures/temperature/temperature.r.html
--rwxr-xr-x   0        0        0     2205 2023-11-18 04:45:15.145783 apoplast-2.0.7/venues/stages/apoplast/measures/volume/swap/__init__.py
--rwxr-xr-x   0        0        0     1483 2024-02-04 21:46:15.385669 apoplast-2.0.7/venues/stages/apoplast/measures/volume/swap/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2595 2023-11-18 05:19:23.119351 apoplast-2.0.7/venues/stages/apoplast/measures/volume/swap/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1666 2023-11-18 04:42:26.127221 apoplast-2.0.7/venues/stages/apoplast/measures/volume/swap/status_1.py
--rwxr-xr-x   0        0        0      510 2023-10-19 17:30:50.062721 apoplast-2.0.7/venues/stages/apoplast/measures/volume/volume.html
--rwxr-xr-x   0        0        0      911 2023-11-18 02:37:48.804499 apoplast-2.0.7/venues/stages/apoplast/measures/weight/weight.r.html
--rwxr-xr-x   0        0        0        0 2023-12-16 03:24:46.171106 apoplast-2.0.7/venues/stages/apoplast/proposals/humans/__init__.py
--rwxr-xr-x   0        0        0      364 2023-11-18 01:10:16.872199 apoplast-2.0.7/venues/stages/apoplast/proposals/humans/_journal/vitamin e.r.HTML
--rwxr-xr-x   0        0        0      219 2023-11-18 02:14:35.364374 apoplast-2.0.7/venues/stages/apoplast/proposals/humans/people.s.HTML
--rwxr-xr-x   0        0        0      207 2023-12-16 03:26:47.079100 apoplast-2.0.7/venues/stages/apoplast/proposals/proposals structure.s.HTML
--rwxr-xr-x   0        0        0      958 2024-01-19 20:01:27.849061 apoplast-2.0.7/venues/stages/apoplast/proposals/proposals.s.HTML
--rwxr-xr-x   0        0        0      540 2024-03-31 22:10:19.048060 apoplast-2.0.7/venues/stages/apoplast/room.md
--rwxr-xr-x   0        0        0      338 2024-04-08 03:36:01.989225 apoplast-2.0.7/venues/stages/apoplast/room.s.HTML
--rwxr-xr-x   0        0        0      224 2023-11-17 23:54:21.748981 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/FDA.s.HTML
--rwxr-xr-x   0        0        0      421 2023-11-22 20:41:38.805470 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/_journal/journal.r.HTML
--rwxr-xr-x   0        0        0        0 2023-11-22 06:06:19.241831 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/_journal/structures/calcium.r.HTML
--rwxr-xr-x   0        0        0      216 2023-11-24 01:35:08.490720 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/_journal/structures/lipids/lipids.r.HTML
--rwxr-xr-x   0        0        0       11 2023-11-22 06:06:47.781502 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/_journal/structures/protein/protein.r.HTML
--rwxr-xr-x   0        0        0     1351 2023-11-18 00:49:44.295684 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin a.r.HTML
--rwxr-xr-x   0        0        0      807 2023-11-18 00:12:47.288622 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin b.r.HTML
--rwxr-xr-x   0        0        0       93 2023-11-24 01:36:24.952841 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin c.r.HTML
--rwxr-xr-x   0        0        0     1298 2023-11-17 23:45:28.778499 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin d.r.HTML
--rwxr-xr-x   0        0        0      149 2023-11-18 01:08:23.546163 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin e.r.HTML
--rwxr-xr-x   0        0        0      219 2023-11-16 23:54:05.601068 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/channel/river.s.HTML
--rwxr-xr-x   0        0        0      543 2024-02-04 19:20:12.996206 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/forward channel.s.HTML
--rwxr-xr-x   0        0        0      935 2023-11-24 02:38:32.442999 apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/structures.s.HTML
--rwxr-xr-x   0        0        0      786 2024-02-04 21:46:15.977664 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/access.cpython-310.pyc
--rwxr-xr-x   0        0        0     1067 2023-12-15 20:42:35.611119 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/access.cpython-311.pyc
--rwxr-xr-x   0        0        0      699 2024-02-04 21:46:15.978664 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/path.cpython-310.pyc
--rwxr-xr-x   0        0        0     1092 2023-12-15 20:12:11.634659 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/path.cpython-311.pyc
--rwxr-xr-x   0        0        0      102 2023-12-15 18:50:56.704859 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/cautions/cautions.JSON
--rwxr-xr-x   0        0        0       35 2023-12-16 23:46:18.398267 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/cautions/cautions.s.HTML
--rwxr-xr-x   0        0        0     3706 2023-11-25 18:53:45.691756 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/1.JSON
--rwxr-xr-x   0        0        0     3955 2023-11-27 20:39:58.077599 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/2.JSON
--rwxr-xr-x   0        0        0     3864 2023-12-15 19:16:15.734307 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/essentials.JSON
--rwxr-xr-x   0        0        0     1643 2023-12-15 20:42:05.183385 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/access.py
--rwxr-xr-x   0        0        0      598 2023-12-15 20:11:06.457198 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/path.py
--rwxr-xr-x   0        0        0      957 2024-03-11 03:50:37.039618 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py
--rwxr-xr-x   0        0        0      665 2024-03-11 03:53:05.197685 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      855 2023-12-15 23:01:07.547799 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      425 2023-12-15 20:37:53.477587 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/status_1.py
--rwxr-xr-x   0        0        0     1040 2024-03-11 03:59:22.473027 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__init__.py
--rwxr-xr-x   0        0        0      907 2024-03-29 23:34:10.581332 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1146 2023-12-15 20:38:04.629490 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1127 2024-03-11 03:56:08.423385 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/status_1.py
--rwxr-xr-x   0        0        0      521 2023-12-15 20:03:32.715951 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__init__.py
--rwxr-xr-x   0        0        0      895 2024-02-04 21:46:17.267655 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1282 2023-12-15 20:03:59.450730 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      452 2023-12-15 20:03:32.730951 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/status_actual/status_1.py
--rwxr-xr-x   0        0        0      994 2023-12-15 20:03:32.744950 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/__init__.py
--rwxr-xr-x   0        0        0     2132 2023-11-27 20:33:10.870623 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1160 2023-12-15 20:37:53.503587 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/__init__.py
--rwxr-xr-x   0        0        0     2262 2023-11-25 19:20:33.032957 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      735 2023-12-15 20:03:32.775950 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/__init__.py
--rwxr-xr-x   0        0        0     1466 2023-11-24 01:19:42.973352 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      749 2023-12-15 20:03:32.790950 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/__init__.py
--rwxr-xr-x   0        0        0     1582 2023-12-15 18:48:20.744152 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0       93 2023-11-25 18:51:12.376547 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/sculpt.r.HTML
--rwxr-xr-x   0        0        0      251 2023-12-15 20:03:32.804950 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/status_1.py
--rwxr-xr-x   0        0        0      424 2023-12-15 22:29:15.419867 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/assertions/one/__init__.py
--rwxr-xr-x   0        0        0      609 2024-02-04 22:00:53.441098 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/assertions/one/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      893 2023-12-15 22:39:49.023943 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/assertions/one/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      504 2023-12-15 20:03:32.608952 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/assertions/recipe/__init__.py
--rwxr-xr-x   0        0        0      768 2023-12-15 22:31:10.731971 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__init__.py
--rwxr-xr-x   0        0        0     1000 2024-02-04 22:00:53.442098 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1474 2023-12-15 22:39:49.023943 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1030 2023-12-17 01:34:38.227857 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__init__.py
--rwxr-xr-x   0        0        0     1102 2024-02-04 21:46:16.701659 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1758 2023-12-17 01:34:53.335684 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      668 2023-12-17 01:36:56.858274 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_1.py
--rwxr-xr-x   0        0        0      603 2023-12-17 01:38:18.265344 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_2.py
--rwxr-xr-x   0        0        0      551 2023-12-15 22:31:10.745971 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__init__.py
--rwxr-xr-x   0        0        0      799 2024-02-04 21:46:17.060656 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1170 2023-12-15 22:31:23.050875 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      798 2023-12-15 20:03:32.879949 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/status_1.py
--rwxr-xr-x   0        0        0      254 2023-11-23 22:33:02.113155 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/grove.s.HTML
--rwxr-xr-x   0        0        0     4712 2024-03-31 22:07:23.909086 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__init__.py
--rwxr-xr-x   0        0        0     1645 2024-03-31 22:08:36.700698 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3030 2023-12-15 22:31:23.142875 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      945 2023-11-26 03:02:03.332197 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/has_uniters.r.HTML
--rwxr-xr-x   0        0        0     1055 2023-12-15 22:31:10.773971 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/status_1.py
--rwxr-xr-x   0        0        0      222 2023-12-09 18:50:30.819756 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/measures/measures.s.HTML
--rwxr-xr-x   0        0        0      176 2023-12-15 20:03:32.925949 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/measures/seek_fraction_string/__init__.py
--rwxr-xr-x   0        0        0      164 2023-12-15 20:03:32.938949 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/measures/seek_fraction_string/status_1.py
--rwxr-xr-x   0        0        0     2879 2023-12-17 01:45:25.376468 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__init__.py
--rwxr-xr-x   0        0        0     2351 2024-02-04 21:46:15.976664 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3863 2023-12-17 01:45:27.972438 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     9652 2023-12-15 19:06:54.650929 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/note.txt
--rwxr-xr-x   0        0        0      542 2023-12-15 23:08:39.155150 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/nurture.s.HTML
--rwxr-xr-x   0        0        0     1297 2023-12-15 23:05:28.423694 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/status_cautions_1.py
--rwxr-xr-x   0        0        0      696 2023-12-15 22:31:10.815971 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/status_essentials_1.py
--rwxr-xr-x   0        0        0     1424 2023-12-15 23:01:30.390616 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/print/__init__.py
--rwxr-xr-x   0        0        0     1458 2024-02-04 21:46:17.005657 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/print/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2465 2023-12-15 23:01:32.768597 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/print/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1235 2023-12-17 01:00:44.139172 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__init__.py
--rwxr-xr-x   0        0        0     1002 2024-02-04 21:46:16.030664 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1378 2023-12-17 01:00:55.887037 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      572 2023-12-15 22:31:10.859970 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek/status_1.py
--rwxr-xr-x   0        0        0      469 2023-12-15 20:03:33.024948 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/__init__.py
--rwxr-xr-x   0        0        0      739 2024-02-04 21:46:16.728659 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1101 2023-12-15 20:03:58.148740 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     3891 2023-12-08 03:23:39.720308 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/essentials.JSON
--rwxr-xr-x   0        0        0      833 2023-12-15 23:06:34.419160 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/status_1.py
--rwxr-xr-x   0        0        0     1237 2023-12-15 22:31:10.873970 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__init__.py
--rwxr-xr-x   0        0        0     1116 2024-02-04 21:46:16.111663 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1834 2023-12-15 22:31:20.150898 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      568 2023-12-15 20:03:33.071948 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/status_1.py
--rwxr-xr-x   0        0        0     1056 2023-12-17 00:41:11.531623 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__init__.py
--rwxr-xr-x   0        0        0     1243 2024-02-04 21:46:16.029664 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1985 2023-12-17 00:41:23.756483 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      507 2023-12-15 20:03:33.104947 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/status_1.py
--rwxr-xr-x   0        0        0      794 2023-12-15 22:31:10.903970 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__init__.py
--rwxr-xr-x   0        0        0     1055 2024-02-04 21:46:17.013657 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1550 2023-12-15 22:31:23.110875 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2023-12-15 22:31:10.916970 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/status_1.py
--rwxr-xr-x   0        0        0      633 2023-12-15 22:31:10.928970 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__init__.py
--rwxr-xr-x   0        0        0     1148 2024-02-04 21:46:17.006657 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1680 2023-12-15 22:31:23.097875 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      180 2023-11-23 19:14:43.750059 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/grove prototype.r.HTML
--rwxr-xr-x   0        0        0     1903 2023-12-15 22:31:10.942969 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__init__.py
--rwxr-xr-x   0        0        0     2203 2024-02-04 21:46:16.469661 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3647 2023-12-15 22:31:21.710886 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      918 2023-12-15 20:35:42.040737 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__init__.py
--rwxr-xr-x   0        0        0      813 2024-02-04 21:46:16.469661 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1127 2023-12-15 20:36:59.502059 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      536 2023-12-15 20:35:49.922668 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_1.py
--rwxr-xr-x   0        0        0      624 2023-12-15 20:36:03.137552 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_2.py
--rwxr-xr-x   0        0        0      966 2023-12-15 20:42:05.241384 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/status_1.py
--rwxr-xr-x   0        0        0     1389 2023-12-15 20:03:33.244946 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__init__.py
--rwxr-xr-x   0        0        0     1325 2024-02-04 21:46:16.470661 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2194 2023-12-15 20:03:57.290748 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      719 2023-12-15 20:36:28.059334 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__init__.py
--rwxr-xr-x   0        0        0      615 2024-02-04 21:46:16.471661 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      929 2023-12-15 20:36:59.505059 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      529 2023-12-15 20:36:38.211246 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/status_1.py
--rwxr-xr-x   0        0        0      615 2023-12-15 20:36:51.162132 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/status_2.py
--rwxr-xr-x   0        0        0      692 2023-11-24 00:44:01.444936 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/ingredient/nutrient_pattern.s.HTML
--rwxr-xr-x   0        0        0     1012 2024-03-29 20:58:01.155250 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/ingredient scan.s.HTML
--rwxr-xr-x   0        0        0     4982 2024-03-29 23:50:17.061986 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__init__.py
--rwxr-xr-x   0        0        0     2377 2024-03-29 23:51:14.241315 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3660 2023-12-15 20:03:55.578762 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0        3 2023-11-27 20:33:45.784509 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/add_measured_ingredient.r.HTML
--rwxr-xr-x   0        0        0     1082 2023-12-15 20:03:33.325946 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py
--rwxr-xr-x   0        0        0     2212 2024-03-29 23:53:03.560032 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_1.py
--rwxr-xr-x   0        0        0     2200 2024-03-29 23:53:32.283694 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_2.py
--rwxr-xr-x   0        0        0     3932 2024-03-29 23:52:06.320703 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/status_1.py
--rwxr-xr-x   0        0        0     1136 2023-12-15 23:10:16.248364 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/__init__.py
--rwxr-xr-x   0        0        0      976 2024-02-04 21:46:15.975664 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1378 2023-12-15 23:11:10.322927 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      561 2024-02-04 21:46:15.979664 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/measures.cpython-310.pyc
--rwxr-xr-x   0        0        0      715 2023-12-15 20:03:55.424763 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/measures.cpython-311.pyc
--rwxr-xr-x   0        0        0      375 2023-12-15 20:03:33.404945 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/measures.py
--rwxr-xr-x   0        0        0      324 2023-12-15 23:11:21.661835 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/status_1.py
--rwxr-xr-x   0        0        0      812 2023-12-15 23:12:52.091103 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/status_cautionary_1.py
--rwxr-xr-x   0        0        0     3271 2024-03-30 21:01:29.376796 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__init__.py
--rwxr-xr-x   0        0        0     1590 2024-03-30 21:02:46.028385 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2481 2023-12-15 23:20:29.920394 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1644 2023-12-17 01:39:47.249328 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__init__.py
--rwxr-xr-x   0        0        0     1525 2024-02-04 22:00:53.448098 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2202 2023-12-17 01:47:38.718946 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     3497 2024-03-29 23:49:19.694659 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/land.s.HTML
--rwxr-xr-x   0        0        0      439 2023-12-15 20:03:33.447945 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/__init__.py
--rwxr-xr-x   0        0        0      815 2024-02-04 22:00:54.280092 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1095 2023-12-15 20:03:55.450763 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      614 2023-12-15 20:03:33.461945 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/status_1.py
--rwxr-xr-x   0        0        0     2794 2024-03-29 23:51:11.921342 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__init__.py
--rwxr-xr-x   0        0        0     1774 2024-03-29 23:53:51.883464 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2771 2023-12-15 20:03:55.426763 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      407 2023-12-15 20:03:33.492944 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/status/status_1.py
--rwxr-xr-x   0        0        0     2290 2023-12-15 20:50:14.984241 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__init__.py
--rwxr-xr-x   0        0        0     1885 2024-02-04 22:00:53.451098 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2945 2023-12-15 20:50:23.774168 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      780 2024-02-04 22:00:53.485098 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/__pycache__/course_2.cpython-310.pyc
--rwxr-xr-x   0        0        0     1182 2023-12-15 22:29:32.153737 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/__pycache__/course_2.cpython-311.pyc
--rwxr-xr-x   0        0        0      551 2023-12-15 20:50:37.247054 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/course_2.py
--rwxr-xr-x   0        0        0      950 2023-11-27 02:53:23.082794 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/multiply_measures.s.HTML
--rwxr-xr-x   0        0        0     2582 2024-03-30 00:06:40.890240 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_1.py
--rwxr-xr-x   0        0        0     2923 2024-03-30 00:05:43.491040 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_2.py
--rwxr-xr-x   0        0        0     1039 2023-12-15 20:03:33.561944 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_loop_1.py
--rwxr-xr-x   0        0        0     1313 2024-03-30 00:01:21.450188 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__init__.py
--rwxr-xr-x   0        0        0     1150 2024-03-30 00:01:26.518128 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1601 2023-12-15 20:03:54.816768 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1477 2024-03-30 00:13:11.765040 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_1.py
--rwxr-xr-x   0        0        0     1475 2024-03-30 00:08:56.548392 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_2.py
--rwxr-xr-x   0        0        0     1319 2024-03-30 00:09:21.776054 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_3.py
--rwxr-xr-x   0        0        0      776 2023-12-15 20:03:33.638943 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__init__.py
--rwxr-xr-x   0        0        0      842 2024-02-04 22:00:53.483098 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1336 2023-12-15 20:03:54.814768 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1728 2023-12-15 20:03:33.654943 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/status_1.py
--rwxr-xr-x   0        0        0      275 2023-11-26 22:20:49.328242 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/selected_unit/__init__.py
--rwxr-xr-x   0        0        0      102 2023-12-15 19:52:46.524296 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/names.s.HTML
--rwxr-xr-x   0        0        0     1200 2024-03-07 04:13:37.347239 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__init__.py
--rwxr-xr-x   0        0        0     1259 2024-03-11 01:21:46.158376 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1632 2024-02-04 19:33:07.617350 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1207 2023-12-16 05:02:53.973031 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_empty/status_1.py
--rwxr-xr-x   0        0        0     2315 2024-03-30 00:02:05.729668 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_0.py
--rwxr-xr-x   0        0        0     6474 2024-03-30 00:18:21.421112 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_1.py
--rwxr-xr-x   0        0        0     3862 2024-03-30 00:17:10.781998 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_2.py
--rwxr-xr-x   0        0        0     2473 2024-02-04 20:24:03.569661 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_3.py
--rwxr-xr-x   0        0        0   215864 2024-04-11 17:28:28.862053 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.JSON
--rwxr-xr-x   0        0        0     2506 2024-03-11 02:02:18.286816 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.py
--rwxr-xr-x   0        0        0   131410 2024-04-11 17:28:28.150062 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.JSON
--rwxr-xr-x   0        0        0     1863 2024-03-11 01:24:01.392835 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.py
--rwxr-xr-x   0        0        0   127961 2024-04-11 17:28:28.470058 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.JSON
--rwxr-xr-x   0        0        0     1755 2023-12-16 05:04:27.952247 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.py
--rwxr-xr-x   0        0        0     1606 2023-12-16 05:04:52.885039 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1_supp_1.py
--rwxr-xr-x   0        0        0     1707 2024-02-04 22:00:53.495098 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/__pycache__/ingredient.cpython-310.pyc
--rwxr-xr-x   0        0        0     3758 2023-12-16 05:01:10.617894 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/__pycache__/ingredient.cpython-311.pyc
--rwxr-xr-x   0        0        0     2844 2023-12-16 05:01:05.865934 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/ingredient.py
--rwxr-xr-x   0        0        0      471 2023-12-15 22:41:08.357326 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/__init__.py
--rwxr-xr-x   0        0        0      902 2024-02-04 22:00:53.486098 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1185 2023-12-15 22:41:31.485147 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0        0 2023-12-09 18:24:24.688260 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/slice/__init__.py
--rwxr-xr-x   0        0        0        0 2023-12-16 04:48:59.742994 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/cautionary_ingredients/formulate.py
--rwxr-xr-x   0        0        0     2968 2024-03-11 01:21:46.166376 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/__pycache__/formulate.cpython-310.pyc
--rwxr-xr-x   0        0        0     4840 2023-12-16 04:55:55.440526 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/__pycache__/formulate.cpython-311.pyc
--rwxr-xr-x   0        0        0     3439 2024-03-07 04:11:50.688393 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/formulate.py
--rwxr-xr-x   0        0        0     1876 2023-11-26 22:19:07.302481 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/recipe structure.s.HTML
--rwxr-xr-x   0        0        0      968 2024-02-04 19:27:25.533932 apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/recipe.s.HTML
--rwxr-xr-x   0        0        0      101 2023-11-17 21:50:38.225811 apoplast-2.0.7/venues/stages/apoplast/shows/natures/__init__.py
--rwxr-xr-x   0        0        0      328 2024-02-04 21:46:15.412669 apoplast-2.0.7/venues/stages/apoplast/shows/natures/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      440 2023-11-21 19:25:30.099428 apoplast-2.0.7/venues/stages/apoplast/shows/natures/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      633 2024-02-04 21:46:15.413668 apoplast-2.0.7/venues/stages/apoplast/shows/natures/__pycache__/assertions.cpython-310.pyc
--rwxr-xr-x   0        0        0      934 2023-11-21 23:22:13.005761 apoplast-2.0.7/venues/stages/apoplast/shows/natures/__pycache__/assertions.cpython-311.pyc
--rwxr-xr-x   0        0        0      371 2023-11-21 23:21:15.613421 apoplast-2.0.7/venues/stages/apoplast/shows/natures/assertions.py
--rwxr-xr-x   0        0        0       84 2023-11-22 02:42:38.990104 apoplast-2.0.7/venues/stages/apoplast/shows/natures/measured_ingredient/assertions.py
--rwxr-xr-x   0        0        0      332 2024-03-29 20:56:02.996705 apoplast-2.0.7/venues/stages/apoplast/shows/natures/nature.s.HTML
--rwxr-xr-x   0        0        0     3867 2023-11-28 02:28:19.579319 apoplast-2.0.7/venues/stages/apoplast/shows/natures/pattern/nature/nature.S.HTML
--rwxr-xr-x   0        0        0     2209 2023-11-25 23:54:11.701513 apoplast-2.0.7/venues/stages/apoplast/shows/natures/pattern/nature: form.S.HTML
--rwxr-xr-x   0        0        0      139 2023-11-28 02:28:25.915261 apoplast-2.0.7/venues/stages/apoplast/shows/natures/pattern/pattern.S.HTML
--rwxr-xr-x   0        0        0      115 2023-11-16 20:19:44.647903 apoplast-2.0.7/venues/stages/apoplast/shows/natures/pattern/pattern: measured ingredients.S.HTML
--rwxr-xr-x   0        0        0        5 2023-11-16 20:58:52.759569 apoplast-2.0.7/venues/stages/apoplast/shows/natures/pattern/pattern: unmeasured ingredients.S.HTML
--rwxr-xr-x   0        0        0      843 2024-03-31 01:49:28.876629 apoplast-2.0.7/venues/stages/apoplast/shows/shows.s.HTML
--rwxr-xr-x   0        0        0     1523 2024-03-31 02:20:59.032310 apoplast-2.0.7/venues/stages/apoplast/shows_v2/land/grove/grove.S.HTML
--rwxr-xr-x   0        0        0       58 2024-03-31 02:19:44.581133 apoplast-2.0.7/venues/stages/apoplast/shows_v2/land/grove/info/info.S.HTML
--rwxr-xr-x   0        0        0       73 2024-03-31 02:21:06.092232 apoplast-2.0.7/venues/stages/apoplast/shows_v2/land/grove/measures/measures.S.HTML
--rwxr-xr-x   0        0        0       59 2024-03-31 02:21:27.675994 apoplast-2.0.7/venues/stages/apoplast/shows_v2/land/grove/natures/natures.S.HTML
--rwxr-xr-x   0        0        0     1508 2024-03-31 02:23:11.418860 apoplast-2.0.7/venues/stages/apoplast/shows_v2/land/grove/unites/unites.S.HTML
--rwxr-xr-x   0        0        0      131 2024-03-31 02:19:06.373559 apoplast-2.0.7/venues/stages/apoplast/shows_v2/land/land.S.HTML
--rwxr-xr-x   0        0        0      459 2024-03-31 02:16:52.687064 apoplast-2.0.7/venues/stages/apoplast/shows_v2/land/measures/measures.S.HTML
--rwxr-xr-x   0        0        0      412 2024-03-31 02:09:01.592689 apoplast-2.0.7/venues/stages/apoplast/shows_v2/land/natures/natures.S.HTML
--rwxr-xr-x   0        0        0      405 2024-03-31 01:56:16.948471 apoplast-2.0.7/venues/stages/apoplast/shows_v2/nature/measured_ingredients/measured_ingredients.S.HTML
--rwxr-xr-x   0        0        0     1018 2024-03-31 01:54:44.445413 apoplast-2.0.7/venues/stages/apoplast/shows_v2/nature/measures/measures.S.HTML
--rwxr-xr-x   0        0        0      426 2024-03-31 01:58:10.379316 apoplast-2.0.7/venues/stages/apoplast/shows_v2/nature/nature.S.HTML
--rwxr-xr-x   0        0        0      294 2024-03-31 01:56:52.156113 apoplast-2.0.7/venues/stages/apoplast/shows_v2/nature/unmeasured_ingredients/UI.S.HTML
--rwxr-xr-x   0        0        0      106 2024-03-31 01:57:56.055462 apoplast-2.0.7/venues/stages/apoplast/shows_v2/shows.S.HTML
--rwxr-xr-x   0        0        0      232 2024-03-31 01:52:52.946549 apoplast-2.0.7/venues/stages/apoplast/shows_v2/treasure/treasure.S.HTML
--rwxr-xr-x   0        0        0       63 2023-11-16 19:27:45.065885 apoplast-2.0.7/venues/stages/apoplast/status_1.py
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 apoplast-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0      772 2024-04-11 20:37:05.700600 apoplast-2.0.8/pyproject.toml
+-rwxr-xr-x   0        0        0      540 2024-04-11 17:29:17.329381 apoplast-2.0.8/readme.md
+-rwxr-xr-x   0        0        0     1431 2024-04-11 20:25:17.648072 apoplast-2.0.8/venue.S.HTML
+-rwxr-xr-x   0        0        0      427 2024-02-04 21:45:08.055173 apoplast-2.0.8/venues/stages/apoplast/___license/license.s.HTML
+-rw-r--r--   0        0        0      370 2024-04-11 17:19:27.770864 apoplast-2.0.8/venues/stages/apoplast/___license/list/coms.s.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 apoplast-2.0.8/venues/stages/apoplast/___license/list/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      112 2024-02-04 21:44:43.992353 apoplast-2.0.8/venues/stages/apoplast/___license/list/vegan.s.HTML
+-rwxr-xr-x   0        0        0      379 2024-04-08 03:42:51.464524 apoplast-2.0.8/venues/stages/apoplast/__bin/apoplast_1
+-rwxr-xr-x   0        0        0        0 2024-04-11 20:16:42.949103 apoplast-2.0.8/venues/stages/apoplast/__init__.py
+-rwxr-xr-x   0        0        0      772 2024-04-10 01:40:13.241532 apoplast-2.0.8/venues/stages/apoplast/__itinerary/apoplast.S.HTML
+-rwxr-xr-x   0        0        0      405 2024-04-08 03:26:57.443923 apoplast-2.0.8/venues/stages/apoplast/__itinerary/book/Vitamin B.S.HTML
+-rwxr-xr-x   0        0        0       63 2024-04-08 03:27:04.947828 apoplast-2.0.8/venues/stages/apoplast/__itinerary/book/Vitamin K.S.HTML
+-rwxr-xr-x   0        0        0  6858198 2024-04-11 17:28:33.233991 apoplast-2.0.8/venues/stages/apoplast/__status/db/records.json
+-rwxr-xr-x   0        0        0    50398 2024-04-10 05:20:39.085373 apoplast-2.0.8/venues/stages/apoplast/__status/db_API/records.json
+-rwxr-xr-x   0        0        0     1457 2024-04-11 17:25:09.951874 apoplast-2.0.8/venues/stages/apoplast/__status/status.proc.py
+-rwxr-xr-x   0        0        0     1169 2024-04-10 05:16:26.771953 apoplast-2.0.8/venues/stages/apoplast/__status/status_API.proc.py
+-rwxr-xr-x   0        0        0      428 2024-04-10 05:17:06.307551 apoplast-2.0.8/venues/stages/apoplast/_ellipses/__init__.py
+-rw-r--r--   0        0        0      595 2024-04-10 05:17:08.375530 apoplast-2.0.8/venues/stages/apoplast/_ellipses/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      891 2024-02-04 20:02:36.038251 apoplast-2.0.8/venues/stages/apoplast/_ellipses/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1172 2024-04-11 17:13:36.374807 apoplast-2.0.8/venues/stages/apoplast/_interfaces/clique/__init__.py
+-rw-r--r--   0        0        0     1530 2024-04-11 17:13:40.986742 apoplast-2.0.8/venues/stages/apoplast/_interfaces/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      297 2024-04-08 03:41:14.873594 apoplast-2.0.8/venues/stages/apoplast/_interfaces/clique/group/__init__.py
+-rwxr-xr-x   0        0        0      703 2024-04-08 03:43:34.852041 apoplast-2.0.8/venues/stages/apoplast/_interfaces/clique/group/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        2 2024-04-11 17:08:27.110508 apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-11 17:13:41.498735 apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1198 2024-04-11 17:13:41.498735 apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/__pycache__/clique.cpython-310.pyc
+-rw-r--r--   0        0        0      245 2024-04-11 17:13:41.498735 apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/__pycache__/off.cpython-310.pyc
+-rw-r--r--   0        0        0      345 2024-04-11 17:13:41.498735 apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/__pycache__/on.cpython-310.pyc
+-rw-r--r--   0        0        0      251 2024-04-11 17:13:41.498735 apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/__pycache__/status.cpython-310.pyc
+-rw-r--r--   0        0        0      728 2024-04-11 17:12:41.519615 apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/clique.py
+-rw-r--r--   0        0        0       45 2024-04-11 17:08:40.814410 apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/customs.S.HTML
+-rw-r--r--   0        0        0       25 2024-04-11 17:10:34.789623 apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/off.py
+-rw-r--r--   0        0        0      102 2024-04-11 17:10:28.957663 apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/on.py
+-rw-r--r--   0        0        0       25 2024-04-11 17:12:20.871941 apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/status.py
+-rw-r--r--   0        0        0     1009 2024-04-09 21:23:47.661473 apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1203 2024-04-10 01:56:49.759392 apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/__pycache__/clique.cpython-310.pyc
+-rw-r--r--   0        0        0     1175 2024-04-09 22:04:41.609395 apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/__pycache__/harbor.cpython-310.pyc
+-rw-r--r--   0        0        0      818 2024-04-09 22:06:02.852384 apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/__pycache__/off.cpython-310.pyc
+-rw-r--r--   0        0        0      870 2024-04-09 21:57:44.518681 apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/__pycache__/on.cpython-310.pyc
+-rw-r--r--   0        0        0      870 2024-04-10 01:38:51.770292 apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/clique.py
+-rwxr-xr-x   0        0        0     1535 2024-04-09 22:04:27.465571 apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/harbor.py
+-rwxr-xr-x   0        0        0      500 2024-04-09 22:05:47.060581 apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/off.py
+-rwxr-xr-x   0        0        0      624 2024-04-09 21:57:42.582706 apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/on.py
+-rwxr-xr-x   0        0        0     1314 2024-04-09 21:54:23.433322 apoplast-2.0.8/venues/stages/apoplast/_variables/__init__.py
+-rw-r--r--   0        0        0     1307 2024-04-09 21:54:34.813170 apoplast-2.0.8/venues/stages/apoplast/_variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      118 2024-02-04 18:06:33.920433 apoplast-2.0.8/venues/stages/apoplast/clouds/affiliates_Amazon/affiliates.s.HTML
+-rwxr-xr-x   0        0        0      111 2024-03-31 01:44:52.099453 apoplast-2.0.8/venues/stages/apoplast/clouds/clouds.S.HTML
+-rwxr-xr-x   0        0        0      607 2024-02-04 21:46:15.410669 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/__pycache__/source.cpython-310.pyc
+-rwxr-xr-x   0        0        0      738 2023-11-16 23:18:39.357737 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/__pycache__/source.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1036 2024-03-31 22:06:11.113782 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__init__.py
+-rwxr-xr-x   0        0        0     1277 2024-03-31 22:08:36.588698 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2127 2023-11-17 00:20:13.313296 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2023-10-12 21:45:50.642367 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/BRANDED.cpython-311.pyc
+-rwxr-xr-x   0        0        0      450 2023-10-12 21:45:50.642367 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/FOUNDATIONAL.cpython-311.pyc
+-rwxr-xr-x   0        0        0      545 2024-02-04 21:46:15.409669 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-310.pyc
+-rwxr-xr-x   0        0        0      778 2023-10-29 21:44:27.877088 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-311.pyc
+-rwxr-xr-x   0        0        0      508 2024-02-04 21:46:15.410669 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-310.pyc
+-rwxr-xr-x   0        0        0      677 2023-11-17 17:51:16.699708 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-311.pyc
+-rwxr-xr-x   0        0        0      429 2023-10-29 21:44:17.338209 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/branded.py
+-rwxr-xr-x   0        0        0      264 2023-11-17 17:51:13.692733 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/foundational.py
+-rwxr-xr-x   0        0        0      419 2023-11-17 00:19:37.192708 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/status/API_status_branded_1.py
+-rwxr-xr-x   0        0        0      465 2023-11-17 00:19:37.195707 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/status/API_status_foundational_1.py
+-rwxr-xr-x   0        0        0      370 2023-11-16 23:17:45.538337 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/source.py
+-rwxr-xr-x   0        0        0     1009 2023-11-22 01:31:31.581903 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/__init__.py
+-rwxr-xr-x   0        0        0     1214 2024-02-04 21:46:15.411669 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2082 2023-11-22 01:32:30.716226 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0    37079 2023-12-09 20:38:41.901230 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON
+-rwxr-xr-x   0        0        0    37079 2023-11-22 01:40:03.461042 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON
+-rwxr-xr-x   0        0        0     7242 2023-10-19 22:27:22.121247 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/beet_juice_2412474.JSON
+-rwxr-xr-x   0        0        0     8522 2023-10-12 21:13:07.386564 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/beet_juice_2642759.JSON
+-rwxr-xr-x   0        0        0    33964 2023-11-22 01:38:38.653013 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/impossible_beef_2664238.JSON
+-rwxr-xr-x   0        0        0    17926 2023-09-25 16:28:17.430256 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/problems/impossible_2468423.JSON
+-rwxr-xr-x   0        0        0      104 2023-11-26 02:04:47.345653 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/problems/problems.r.HTML
+-rwxr-xr-x   0        0        0    10678 2023-11-22 01:32:41.686100 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/vegan_pizza_2672996.JSON
+-rwxr-xr-x   0        0        0    10670 2023-10-24 03:17:57.735576 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/walnuts_1882785.JSON
+-rwxr-xr-x   0        0        0   189146 2023-10-12 22:00:16.639151 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON
+-rwxr-xr-x   0        0        0      255 2023-11-17 18:04:07.057375 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/mergers.r.HTML
+-rwxr-xr-x   0        0        0       88 2023-11-22 01:27:20.472779 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/priorities.r.HTML
+-rwxr-xr-x   0        0        0      457 2023-12-09 23:06:15.605787 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/status_1.py
+-rwxr-xr-x   0        0        0      614 2023-12-15 19:53:16.754046 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/food.s.HTML
+-rwxr-xr-x   0        0        0       28 2023-11-22 04:54:08.017554 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/foodNutrient/__init__.py
+-rwxr-xr-x   0        0        0       28 2023-11-22 02:45:04.164448 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/labelNutrient/__init__.py
+-rwxr-xr-x   0        0        0     1783 2023-11-23 18:42:09.922568 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__init__.py
+-rwxr-xr-x   0        0        0     1324 2024-02-04 21:46:15.413668 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2050 2023-11-23 18:42:13.005533 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      571 2024-02-04 21:46:15.416669 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/assertions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1065 2023-11-22 00:03:16.653487 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/assertions.cpython-311.pyc
+-rwxr-xr-x   0        0        0      583 2023-11-22 00:01:06.946973 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/assertions.py
+-rwxr-xr-x   0        0        0     4126 2023-11-22 20:58:41.034879 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__init__.py
+-rwxr-xr-x   0        0        0     3007 2024-02-04 21:46:15.415669 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     5397 2023-11-22 21:04:24.375937 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1229 2023-11-22 20:47:39.030385 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_mass_1.py
+-rwxr-xr-x   0        0        0      877 2023-11-22 20:23:41.394700 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_volume_1.py
+-rwxr-xr-x   0        0        0      415 2023-11-22 20:49:55.692835 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/__init__.py
+-rwxr-xr-x   0        0        0      547 2024-02-04 21:46:15.416669 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      946 2023-11-22 20:50:32.179422 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1374 2023-11-22 20:23:29.910831 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/status_1.py
+-rwxr-xr-x   0        0        0     5029 2024-01-08 21:02:44.875367 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/__init__.py
+-rwxr-xr-x   0        0        0     2923 2024-02-04 21:46:15.412669 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4846 2024-02-04 19:05:42.507811 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2606 2024-02-04 20:24:03.556661 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_1.py
+-rwxr-xr-x   0        0        0     1610 2023-12-09 20:39:39.205746 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_2.py
+-rwxr-xr-x   0        0        0     1236 2023-12-17 01:49:13.793860 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_2412474.py
+-rwxr-xr-x   0        0        0     1078 2023-12-17 00:42:09.947955 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_3.py
+-rwxr-xr-x   0        0        0      812 2023-12-09 20:39:39.218746 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_loop_1.py
+-rwxr-xr-x   0        0        0     3302 2023-12-15 23:15:41.332733 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__init__.py
+-rwxr-xr-x   0        0        0     2102 2024-02-04 22:00:53.434098 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3367 2023-12-15 23:15:51.961647 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0        4 2023-11-26 00:02:13.258869 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/energy/__init__.py
+-rwxr-xr-x   0        0        0     3116 2023-12-17 00:12:42.461151 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__init__.py
+-rwxr-xr-x   0        0        0     2324 2024-02-04 22:00:53.448098 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3653 2023-12-17 00:13:04.029904 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4031 2023-11-26 01:50:19.679543 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/form/__init__.py
+-rwxr-xr-x   0        0        0     2394 2024-02-04 22:00:53.442098 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/form/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4016 2023-11-26 01:51:17.420831 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/form/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1231 2024-03-31 22:06:29.601567 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/form/status_mass_1.py
+-rwxr-xr-x   0        0        0     1159 2023-11-26 00:30:32.288953 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/form/status_volume_1.py
+-rwxr-xr-x   0        0        0     1427 2023-11-27 04:58:37.292037 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__init__.py
+-rwxr-xr-x   0        0        0     1112 2024-02-04 22:00:53.443098 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1591 2023-11-27 18:18:50.779625 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1676 2023-11-26 01:00:29.154907 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_IU_1.py
+-rwxr-xr-x   0        0        0     1875 2024-03-31 22:07:48.608961 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_energy_1.py
+-rwxr-xr-x   0        0        0     1579 2023-11-26 01:00:16.204059 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_mass_1.py
+-rwxr-xr-x   0        0        0     2077 2023-11-26 01:09:26.265614 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__init__.py
+-rwxr-xr-x   0        0        0     2087 2024-02-04 22:00:53.444098 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3142 2023-11-26 01:10:28.190888 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1224 2023-11-26 01:10:07.049136 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__init__.py
+-rwxr-xr-x   0        0        0     1225 2024-02-04 22:00:53.446098 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1831 2023-11-26 01:10:28.192888 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1494 2023-11-26 23:54:17.527847 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__init__.py
+-rwxr-xr-x   0        0        0     1190 2024-02-04 22:00:53.446098 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1791 2023-11-26 23:54:20.036817 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1389 2024-03-29 23:33:34.229759 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__init__.py
+-rwxr-xr-x   0        0        0     1386 2024-03-29 23:33:56.513497 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1842 2023-11-27 18:18:50.784625 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      679 2024-02-04 22:00:53.444098 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1040 2023-11-26 02:05:12.327391 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1899 2023-11-26 00:58:42.572156 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/food_nutrient_calculator.cpython-311.pyc
+-rwxr-xr-x   0        0        0      617 2024-02-04 22:00:53.445098 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-310.pyc
+-rwxr-xr-x   0        0        0      845 2023-11-26 01:09:01.315906 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-311.pyc
+-rwxr-xr-x   0        0        0      849 2023-11-22 04:50:34.615973 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/label_nutrient_calculator.cpython-311.pyc
+-rwxr-xr-x   0        0        0      622 2023-11-26 02:01:26.676025 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/food_nutrient.py
+-rwxr-xr-x   0        0        0      468 2023-11-22 04:50:10.260249 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/label_nutrient.py
+-rwxr-xr-x   0        0        0      503 2023-11-26 00:52:57.775193 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/ingredient.r.HTML
+-rwxr-xr-x   0        0        0      706 2023-11-22 20:45:42.034711 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/ingredient_prototype_1.r.HTML
+-rwxr-xr-x   0        0        0      485 2023-11-26 01:53:47.219931 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/__init__.py
+-rwxr-xr-x   0        0        0      656 2024-02-04 22:00:53.443098 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      957 2023-11-26 01:53:50.019895 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2092 2023-11-24 04:45:08.346598 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_mass_1.py
+-rwxr-xr-x   0        0        0      687 2023-11-26 00:51:56.712908 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_volume_1.py
+-rwxr-xr-x   0        0        0     1058 2023-11-26 00:49:48.022415 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/example.r.HTML
+-rwxr-xr-x   0        0        0      863 2023-11-23 23:49:12.698629 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__init__.py
+-rwxr-xr-x   0        0        0      807 2024-02-04 22:00:53.447098 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1012 2023-11-23 23:49:23.582505 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      575 2023-11-23 23:46:06.183759 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__init__.py
+-rwxr-xr-x   0        0        0      897 2024-02-04 22:00:53.447098 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1272 2023-11-23 23:46:09.669719 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1019 2023-11-23 23:47:00.051144 apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/status_1.py
+-rwxr-xr-x   0        0        0     1791 2024-03-31 18:10:18.994424 apoplast-2.0.8/venues/stages/apoplast/clouds/goodness_certifications/certifications.py
+-rwxr-xr-x   0        0        0      641 2024-03-31 20:50:04.634053 apoplast-2.0.8/venues/stages/apoplast/clouds/goodness_certifications/vegan.s.HTML
+-rwxr-xr-x   0        0        0     1046 2024-03-31 02:07:55.069366 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/NIH.s.HTML
+-rwxr-xr-x   0        0        0      547 2024-02-04 22:01:04.036019 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/__pycache__/source.cpython-310.pyc
+-rwxr-xr-x   0        0        0      670 2023-10-25 01:34:03.568051 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/__pycache__/source.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1137 2024-03-31 22:06:43.569405 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__init__.py
+-rw-r--r--   0        0        0     1141 2024-04-10 05:16:32.027900 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1889 2023-11-17 00:20:13.309296 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      826 2024-02-04 22:01:04.041019 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/assertions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1399 2023-10-25 01:34:03.568051 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/assertions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1087 2023-10-25 01:29:58.565739 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/assertions.py
+-rwxr-xr-x   0        0        0      392 2023-11-17 00:20:01.903426 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/status/API_status_1.py
+-rwxr-xr-x   0        0        0      316 2023-10-25 01:28:37.971623 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/source.py
+-rwxr-xr-x   0        0        0      848 2023-11-27 22:36:33.129934 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/__init__.py
+-rwxr-xr-x   0        0        0     1050 2024-02-04 21:46:18.952642 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1918 2023-11-27 22:37:23.089492 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0    44597 2023-10-13 17:10:19.838169 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/coated tablets/multivitamin_276336.JSON
+-rwxr-xr-x   0        0        0    22180 2023-10-25 17:22:33.578905 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/other/chia_seeds_214893.JSON
+-rwxr-xr-x   0        0        0     6430 2023-10-13 17:09:44.373557 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/powder/mane_270619.JSON
+-rwxr-xr-x   0        0        0    72594 2023-10-25 01:46:01.092818 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/powder/nutritional_shake_220884.JSON
+-rwxr-xr-x   0        0        0    57378 2023-10-13 17:05:59.829003 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/powder packets/multivitamin_246811.JSON
+-rwxr-xr-x   0        0        0    22710 2023-10-13 17:08:42.546230 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/calcium_261967.JSON
+-rwxr-xr-x   0        0        0    43725 2023-10-13 17:08:08.961596 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/multivitamin_249664.JSON
+-rwxr-xr-x   0        0        0     7107 2023-10-13 17:07:29.648024 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/vegan_capsules/probiotics_248267.JSON
+-rwxr-xr-x   0        0        0       98 2023-11-27 03:46:15.367425 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/__init__.py
+-rwxr-xr-x   0        0        0      285 2024-02-04 21:46:18.226647 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      383 2023-11-27 04:14:12.512606 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1152 2023-11-27 04:24:46.432108 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__init__.py
+-rwxr-xr-x   0        0        0      907 2024-02-04 21:46:18.227648 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1201 2023-11-27 04:25:03.266909 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      923 2023-11-27 04:25:24.402660 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/status_powder_packets_246811.py
+-rwxr-xr-x   0        0        0       56 2023-11-27 04:49:39.293420 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/interpret/servingSizeUnit/__init__.py
+-rwxr-xr-x   0        0        0     4087 2024-03-31 22:07:01.073202 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py
+-rwxr-xr-x   0        0        0     3020 2024-03-31 22:08:36.760697 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4873 2023-12-16 03:49:29.728760 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      730 2023-11-27 22:52:02.622639 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/_loop/status_1.py
+-rwxr-xr-x   0        0        0     1580 2024-03-11 02:00:19.620159 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336.py
+-rwxr-xr-x   0        0        0   136857 2024-04-11 17:28:32.781997 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336_nature.JSON
+-rwxr-xr-x   0        0        0   100726 2024-04-11 17:28:32.757998 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/chia_seeds_214893_nature.JSON
+-rwxr-xr-x   0        0        0      762 2024-03-11 02:02:48.750472 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/status_chia_seeds_214893.py
+-rwxr-xr-x   0        0        0    28773 2024-04-11 17:28:32.661999 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/mane_270619_nature.JSON
+-rwxr-xr-x   0        0        0      748 2023-12-19 18:33:07.683544 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/status_mane_270619.py
+-rwxr-xr-x   0        0        0     2753 2023-12-15 23:31:38.763948 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__init__.py
+-rwxr-xr-x   0        0        0     2408 2024-02-04 22:00:53.505098 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3688 2023-12-15 23:31:44.199904 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2583 2024-03-30 21:02:16.032550 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__init__.py
+-rwxr-xr-x   0        0        0     2183 2024-03-30 21:02:46.768381 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3443 2023-12-15 23:31:44.195904 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      832 2023-11-27 20:26:53.811823 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/essential_nutrients.s.HTML
+-rwxr-xr-x   0        0        0      281 2023-11-27 20:27:05.759787 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/essential_nutrients_priorities.s.HTML
+-rwxr-xr-x   0        0        0      323 2023-11-27 04:41:57.157899 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/__init__.py
+-rwxr-xr-x   0        0        0      560 2024-02-04 21:46:18.215648 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      672 2023-11-27 04:42:26.984546 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      676 2023-11-27 23:18:44.963779 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__init__.py
+-rwxr-xr-x   0        0        0      870 2024-02-04 21:46:18.227648 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1333 2023-11-27 23:19:04.631610 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      510 2023-11-22 19:45:00.248952 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/status_other_214893.py
+-rwxr-xr-x   0        0        0      512 2023-11-25 23:13:17.621118 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/form.r.HTML
+-rwxr-xr-x   0        0        0     3759 2023-11-27 23:36:21.498654 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__init__.py
+-rwxr-xr-x   0        0        0     2314 2024-02-04 21:46:18.228648 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4306 2023-11-27 23:36:25.653617 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0        0 2023-11-27 22:52:26.655429 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_1.py
+-rwxr-xr-x   0        0        0     1841 2024-04-09 20:04:26.544534 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py
+-rwxr-xr-x   0        0        0     1711 2023-11-27 23:47:05.617116 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py
+-rwxr-xr-x   0        0        0     3210 2023-11-27 23:13:13.104637 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__init__.py
+-rwxr-xr-x   0        0        0     2634 2024-02-04 21:46:18.224648 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4650 2023-11-27 23:13:23.844544 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      983 2023-11-27 23:17:35.529377 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py
+-rwxr-xr-x   0        0        0      814 2023-11-22 18:01:32.907312 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_gram_1.py
+-rwxr-xr-x   0        0        0      818 2023-11-22 19:42:51.390406 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_220884.py
+-rwxr-xr-x   0        0        0      903 2023-11-22 19:46:12.236140 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_270619.py
+-rwxr-xr-x   0        0        0     1333 2023-11-22 20:15:00.085618 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_packets_246811.py
+-rwxr-xr-x   0        0        0      701 2023-11-22 20:21:05.755467 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_tablet_261967.py
+-rwxr-xr-x   0        0        0      725 2023-11-22 19:30:39.266645 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py
+-rwxr-xr-x   0        0        0     4631 2024-03-11 02:07:04.511863 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__init__.py
+-rwxr-xr-x   0        0        0     2830 2024-03-11 02:07:07.519836 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4500 2024-02-04 19:05:43.260805 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1687 2024-03-11 02:13:24.344258 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py
+-rwxr-xr-x   0        0        0        0 2023-11-27 05:04:38.944743 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/amount--/mass/__init__.py
+-rwxr-xr-x   0        0        0     1514 2024-03-11 01:32:01.379383 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/measured_ingredient.s.HTML
+-rwxr-xr-x   0        0        0     1656 2024-03-30 21:01:47.824701 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__init__.py
+-rwxr-xr-x   0        0        0     1845 2024-03-30 21:02:46.768381 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2911 2023-11-27 05:46:33.775695 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      826 2024-03-11 02:03:57.637692 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py
+-rwxr-xr-x   0        0        0      561 2023-11-27 05:48:16.117464 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/measured_ingredients.r.HTML
+-rwxr-xr-x   0        0        0     1116 2023-11-27 05:48:52.161031 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__init__.py
+-rwxr-xr-x   0        0        0     1078 2024-02-04 22:00:53.503098 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1442 2023-11-27 05:50:31.795832 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      657 2023-11-27 05:50:29.870855 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py
+-rwxr-xr-x   0        0        0      511 2023-11-27 18:44:30.266270 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/__init__.py
+-rwxr-xr-x   0        0        0      877 2024-02-04 22:00:56.631074 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1171 2023-11-27 18:44:33.989225 apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      527 2024-04-09 15:54:15.319774 apoplast-2.0.8/venues/stages/apoplast/data_nodes/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      233 2024-04-09 15:54:11.135807 apoplast-2.0.8/venues/stages/apoplast/data_nodes/clique.py
+-rwxr-xr-x   0        0        0       96 2024-04-08 03:49:12.700230 apoplast-2.0.8/venues/stages/apoplast/data_nodes/data_nodes.S.HTML
+-rwxr-xr-x   0        0        0       13 2024-04-08 04:26:53.388706 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/.gitignore
+-rwxr-xr-x   0        0        0      677 2024-04-09 16:44:28.185484 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/connect.cpython-310.pyc
+-rwxr-xr-x   0        0        0      826 2024-04-08 04:23:35.323211 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/off.cpython-310.pyc
+-rw-r--r--   0        0        0     1856 2024-04-09 21:23:47.537474 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1522 2024-04-08 04:11:40.756704 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/open.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1500 2024-04-09 19:46:47.950169 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      554 2024-04-09 16:42:34.370813 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/connect.py
+-rwxr-xr-x   0        0        0      632 2024-04-08 04:23:34.295224 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/off.py
+-rwxr-xr-x   0        0        0     2119 2024-04-09 21:02:16.663855 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/on.py
+-rwxr-xr-x   0        0        0        0 2024-04-08 04:30:53.369730 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/saves/dump.py
+-rwxr-xr-x   0        0        0        0 2024-04-08 04:30:49.193781 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/saves/export.py
+-rwxr-xr-x   0        0        0     1701 2024-04-09 19:46:45.714191 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/status.py
+-rwxr-xr-x   0        0        0      454 2024-03-31 01:44:39.427583 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/__itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0     1542 2024-04-09 19:46:25.206393 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      118 2024-03-31 03:53:00.212849 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/cautionary_ingredients/cautionary_ingredients.1.json
+-rwxr-xr-x   0        0        0     5140 2024-03-31 03:54:30.968103 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/essential_nutrients/essential_nutrients.1.json
+-rwxr-xr-x   0        0        0      481 2024-03-31 03:53:37.064550 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/exports.S.HTML
+-rwxr-xr-x   0        0        0       35 2024-04-09 20:14:48.596372 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/_saves/save.py
+-rwxr-xr-x   0        0        0     1104 2024-04-09 19:46:23.838407 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/clique.py
+-rwxr-xr-x   0        0        0      798 2024-03-31 03:45:22.693513 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/collections/_land/__pycache__/insert_document.cpython-310.pyc
+-rwxr-xr-x   0        0        0      796 2024-03-31 03:43:31.086721 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/collections/_land/insert_document.py
+-rwxr-xr-x   0        0        0      170 2024-04-08 03:47:20.717500 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/cautionary_ingredients.S.HTML
+-rwxr-xr-x   0        0        0        2 2024-03-31 03:51:33.881524 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/collection/export.py
+-rwxr-xr-x   0        0        0        0 2024-04-08 03:46:10.538293 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/collections/cautionary_ingredients/document/insert.py
+-rwxr-xr-x   0        0        0       27 2024-04-08 03:47:50.181167 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/collections/collections.S.HTML
+-rwxr-xr-x   0        0        0        0 2024-03-31 03:51:29.633556 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/collections/essential_nutrients/export.py
+-rwxr-xr-x   0        0        0     1523 2024-04-08 03:56:03.579528 apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/ingredients.S.HTML
+-rwxr-xr-x   0        0        0       14 2024-03-31 22:10:20.784048 apoplast-2.0.8/venues/stages/apoplast/emojis.S.HTML
+-rwxr-xr-x   0        0        0     1030 2024-02-04 21:46:14.886673 apoplast-2.0.8/venues/stages/apoplast/insure/__pycache__/equalities.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1871 2023-11-27 23:25:41.951185 apoplast-2.0.8/venues/stages/apoplast/insure/__pycache__/equalities.cpython-311.pyc
+-rwxr-xr-x   0        0        0      453 2024-02-04 21:46:15.408669 apoplast-2.0.8/venues/stages/apoplast/insure/__pycache__/equality.cpython-310.pyc
+-rwxr-xr-x   0        0        0      694 2023-11-22 19:22:56.114817 apoplast-2.0.8/venues/stages/apoplast/insure/__pycache__/equality.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1058 2024-02-04 21:46:17.800651 apoplast-2.0.8/venues/stages/apoplast/insure/__pycache__/override_print.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2001 2023-11-27 01:34:12.790621 apoplast-2.0.8/venues/stages/apoplast/insure/__pycache__/override_print.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1085 2023-11-27 23:25:39.844204 apoplast-2.0.8/venues/stages/apoplast/insure/equalities.py
+-rwxr-xr-x   0        0        0      234 2023-11-22 18:56:47.658330 apoplast-2.0.8/venues/stages/apoplast/insure/equality.py
+-rwxr-xr-x   0        0        0      729 2023-11-27 01:34:09.516659 apoplast-2.0.8/venues/stages/apoplast/insure/override_print.py
+-rwxr-xr-x   0        0        0      374 2023-11-22 19:22:12.923299 apoplast-2.0.8/venues/stages/apoplast/insure/status_equalitites_1.py
+-rwxr-xr-x   0        0        0     1480 2024-02-04 21:46:15.401669 apoplast-2.0.8/venues/stages/apoplast/measures/_interpret/__pycache__/unit_kind.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2547 2023-11-27 23:52:18.152450 apoplast-2.0.8/venues/stages/apoplast/measures/_interpret/__pycache__/unit_kind.cpython-311.pyc
+-rwxr-xr-x   0        0        0       61 2023-10-24 19:09:48.581050 apoplast-2.0.8/venues/stages/apoplast/measures/_interpret/interpret.r.html
+-rwxr-xr-x   0        0        0      670 2023-11-22 03:00:29.040898 apoplast-2.0.8/venues/stages/apoplast/measures/_interpret/status_unit_kind.py
+-rwxr-xr-x   0        0        0     1678 2023-11-27 23:51:26.564890 apoplast-2.0.8/venues/stages/apoplast/measures/_interpret/unit_kind.py
+-rwxr-xr-x   0        0        0        0 2023-11-22 02:29:15.950254 apoplast-2.0.8/venues/stages/apoplast/measures/biological_activity/__init__.py
+-rwxr-xr-x   0        0        0       59 2024-02-26 21:23:18.202627 apoplast-2.0.8/venues/stages/apoplast/measures/electric_current/electric_current.S.HTML
+-rwxr-xr-x   0        0        0     1142 2023-11-18 02:03:26.122070 apoplast-2.0.8/venues/stages/apoplast/measures/energy/energy.r.HTML
+-rwxr-xr-x   0        0        0     1174 2023-11-27 05:11:29.583845 apoplast-2.0.8/venues/stages/apoplast/measures/energy/swap/__init__.py
+-rwxr-xr-x   0        0        0     1027 2024-02-04 21:46:14.884672 apoplast-2.0.8/venues/stages/apoplast/measures/energy/swap/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1761 2023-11-27 05:11:32.899806 apoplast-2.0.8/venues/stages/apoplast/measures/energy/swap/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      386 2023-11-22 03:06:00.365118 apoplast-2.0.8/venues/stages/apoplast/measures/energy/swap/status_1.py
+-rwxr-xr-x   0        0        0       71 2023-11-18 02:08:27.601504 apoplast-2.0.8/venues/stages/apoplast/measures/length/length.r.HTML
+-rwxr-xr-x   0        0        0       95 2023-09-10 01:33:12.464335 apoplast-2.0.8/venues/stages/apoplast/measures/mass/e_note.py
+-rwxr-xr-x   0        0        0       12 2023-10-24 23:00:23.774371 apoplast-2.0.8/venues/stages/apoplast/measures/mass/mass.r.html
+-rwxr-xr-x   0        0        0     2329 2023-11-27 23:53:01.539080 apoplast-2.0.8/venues/stages/apoplast/measures/mass/swap/__init__.py
+-rwxr-xr-x   0        0        0     1735 2024-02-04 21:46:14.882673 apoplast-2.0.8/venues/stages/apoplast/measures/mass/swap/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3229 2023-11-27 23:53:04.757052 apoplast-2.0.8/venues/stages/apoplast/measures/mass/swap/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1153 2023-11-21 20:24:21.450301 apoplast-2.0.8/venues/stages/apoplast/measures/mass/swap/status_1.py
+-rwxr-xr-x   0        0        0     2419 2023-10-25 22:32:32.500043 apoplast-2.0.8/venues/stages/apoplast/measures/mass/system international.r.html
+-rwxr-xr-x   0        0        0      768 2023-10-24 19:13:36.766543 apoplast-2.0.8/venues/stages/apoplast/measures/mass/us customary.r.html
+-rwxr-xr-x   0        0        0      523 2023-11-18 02:19:07.769055 apoplast-2.0.8/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__init__.py
+-rwxr-xr-x   0        0        0      643 2024-02-04 21:46:14.890673 apoplast-2.0.8/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      945 2023-11-18 02:33:55.200495 apoplast-2.0.8/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      342 2023-11-18 02:17:02.598121 apoplast-2.0.8/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/status_1.py
+-rwxr-xr-x   0        0        0      861 2023-11-18 02:32:14.965350 apoplast-2.0.8/venues/stages/apoplast/measures/mass_equivalents/jargon.r.HTML
+-rwxr-xr-x   0        0        0     2242 2023-12-09 18:56:13.594964 apoplast-2.0.8/venues/stages/apoplast/measures/mass_equivalents/mass equivalents.r.HTML
+-rwxr-xr-x   0        0        0     2431 2024-02-26 20:25:18.856520 apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/__init__.py
+-rwxr-xr-x   0        0        0     1665 2024-02-26 20:26:53.162839 apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3068 2023-11-26 02:13:59.845148 apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1428 2023-11-26 02:08:37.997986 apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/status_1.py
+-rwxr-xr-x   0        0        0      901 2023-11-21 19:30:34.527895 apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/status_2.py
+-rwxr-xr-x   0        0        0     1115 2023-11-21 19:30:34.540895 apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/status_3.py
+-rwxr-xr-x   0        0        0      470 2023-11-26 02:09:05.917648 apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/status_sci_note_1.py
+-rwxr-xr-x   0        0        0      170 2023-12-10 03:06:16.513154 apoplast-2.0.8/venues/stages/apoplast/measures/number/fraction_point/fraction_point.s.HTML
+-rwxr-xr-x   0        0        0      539 2024-02-04 21:46:14.908672 apoplast-2.0.8/venues/stages/apoplast/measures/number/integer/__pycache__/string_is_integer.cpython-310.pyc
+-rwxr-xr-x   0        0        0      749 2023-11-18 02:07:47.470846 apoplast-2.0.8/venues/stages/apoplast/measures/number/integer/__pycache__/string_is_integer.cpython-311.pyc
+-rwxr-xr-x   0        0        0      560 2023-11-18 02:07:34.289958 apoplast-2.0.8/venues/stages/apoplast/measures/number/integer/status_string_is_integer.py
+-rwxr-xr-x   0        0        0      368 2023-11-18 02:05:23.482071 apoplast-2.0.8/venues/stages/apoplast/measures/number/integer/string_is_integer.py
+-rwxr-xr-x   0        0        0      899 2024-02-04 21:46:14.887673 apoplast-2.0.8/venues/stages/apoplast/measures/number/percentage/__pycache__/from_fraction.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1702 2023-11-21 19:30:05.993226 apoplast-2.0.8/venues/stages/apoplast/measures/number/percentage/__pycache__/from_fraction.cpython-311.pyc
+-rwxr-xr-x   0        0        0      951 2023-11-21 19:30:01.342280 apoplast-2.0.8/venues/stages/apoplast/measures/number/percentage/from_fraction.py
+-rwxr-xr-x   0        0        0      553 2023-11-18 02:34:50.110026 apoplast-2.0.8/venues/stages/apoplast/measures/number/percentage/status_1.py
+-rwxr-xr-x   0        0        0     2211 2024-02-26 21:02:23.732405 apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note/__init__.py
+-rwxr-xr-x   0        0        0     1448 2024-02-26 21:09:35.283275 apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3224 2024-02-26 21:13:28.392460 apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note/_status/status_multiples_of_3_1.py
+-rwxr-xr-x   0        0        0      612 2024-02-26 21:07:29.400784 apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note/sci_note.S.HTML
+-rwxr-xr-x   0        0        0      644 2024-02-26 21:07:36.720697 apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note/sci_note_possibilities.S.HTML
+-rwxr-xr-x   0        0        0     1342 2024-02-26 21:09:10.127577 apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note/sci_note_thoughts.S.HTML
+-rwxr-xr-x   0        0        0      363 2024-03-29 23:32:14.486695 apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note_2/__init__.py
+-rwxr-xr-x   0        0        0      663 2024-03-29 23:33:54.137525 apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      936 2024-02-26 21:51:34.751894 apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note_2/status_1.py
+-rwxr-xr-x   0        0        0       58 2023-10-24 22:59:09.790207 apoplast-2.0.8/venues/stages/apoplast/measures/temperature/temperature.r.html
+-rwxr-xr-x   0        0        0     2205 2023-11-18 04:45:15.145783 apoplast-2.0.8/venues/stages/apoplast/measures/volume/swap/__init__.py
+-rwxr-xr-x   0        0        0     1483 2024-02-04 21:46:15.385669 apoplast-2.0.8/venues/stages/apoplast/measures/volume/swap/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2595 2023-11-18 05:19:23.119351 apoplast-2.0.8/venues/stages/apoplast/measures/volume/swap/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1666 2023-11-18 04:42:26.127221 apoplast-2.0.8/venues/stages/apoplast/measures/volume/swap/status_1.py
+-rwxr-xr-x   0        0        0      510 2023-10-19 17:30:50.062721 apoplast-2.0.8/venues/stages/apoplast/measures/volume/volume.html
+-rwxr-xr-x   0        0        0      911 2023-11-18 02:37:48.804499 apoplast-2.0.8/venues/stages/apoplast/measures/weight/weight.r.html
+-rwxr-xr-x   0        0        0        0 2023-12-16 03:24:46.171106 apoplast-2.0.8/venues/stages/apoplast/proposals/humans/__init__.py
+-rwxr-xr-x   0        0        0      364 2023-11-18 01:10:16.872199 apoplast-2.0.8/venues/stages/apoplast/proposals/humans/_journal/vitamin e.r.HTML
+-rwxr-xr-x   0        0        0      219 2023-11-18 02:14:35.364374 apoplast-2.0.8/venues/stages/apoplast/proposals/humans/people.s.HTML
+-rwxr-xr-x   0        0        0      207 2023-12-16 03:26:47.079100 apoplast-2.0.8/venues/stages/apoplast/proposals/proposals structure.s.HTML
+-rwxr-xr-x   0        0        0      958 2024-01-19 20:01:27.849061 apoplast-2.0.8/venues/stages/apoplast/proposals/proposals.s.HTML
+-rwxr-xr-x   0        0        0      540 2024-03-31 22:10:19.048060 apoplast-2.0.8/venues/stages/apoplast/room.md
+-rwxr-xr-x   0        0        0      338 2024-04-08 03:36:01.989225 apoplast-2.0.8/venues/stages/apoplast/room.s.HTML
+-rwxr-xr-x   0        0        0      224 2023-11-17 23:54:21.748981 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/FDA.s.HTML
+-rwxr-xr-x   0        0        0      421 2023-11-22 20:41:38.805470 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/_journal/journal.r.HTML
+-rwxr-xr-x   0        0        0        0 2023-11-22 06:06:19.241831 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/_journal/structures/calcium.r.HTML
+-rwxr-xr-x   0        0        0      216 2023-11-24 01:35:08.490720 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/_journal/structures/lipids/lipids.r.HTML
+-rwxr-xr-x   0        0        0       11 2023-11-22 06:06:47.781502 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/_journal/structures/protein/protein.r.HTML
+-rwxr-xr-x   0        0        0     1351 2023-11-18 00:49:44.295684 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin a.r.HTML
+-rwxr-xr-x   0        0        0      807 2023-11-18 00:12:47.288622 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin b.r.HTML
+-rwxr-xr-x   0        0        0       93 2023-11-24 01:36:24.952841 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin c.r.HTML
+-rwxr-xr-x   0        0        0     1298 2023-11-17 23:45:28.778499 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin d.r.HTML
+-rwxr-xr-x   0        0        0      149 2023-11-18 01:08:23.546163 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin e.r.HTML
+-rwxr-xr-x   0        0        0      219 2023-11-16 23:54:05.601068 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/channel/river.s.HTML
+-rwxr-xr-x   0        0        0      543 2024-02-04 19:20:12.996206 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/forward channel.s.HTML
+-rwxr-xr-x   0        0        0      935 2023-11-24 02:38:32.442999 apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/structures.s.HTML
+-rwxr-xr-x   0        0        0      786 2024-02-04 21:46:15.977664 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/access.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1067 2023-12-15 20:42:35.611119 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/access.cpython-311.pyc
+-rwxr-xr-x   0        0        0      699 2024-02-04 21:46:15.978664 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/path.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1092 2023-12-15 20:12:11.634659 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/path.cpython-311.pyc
+-rwxr-xr-x   0        0        0      102 2023-12-15 18:50:56.704859 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/cautions/cautions.JSON
+-rwxr-xr-x   0        0        0       35 2023-12-16 23:46:18.398267 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/cautions/cautions.s.HTML
+-rwxr-xr-x   0        0        0     3706 2023-11-25 18:53:45.691756 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/1.JSON
+-rwxr-xr-x   0        0        0     3955 2023-11-27 20:39:58.077599 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/2.JSON
+-rwxr-xr-x   0        0        0     3864 2023-12-15 19:16:15.734307 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/essentials.JSON
+-rwxr-xr-x   0        0        0     1643 2023-12-15 20:42:05.183385 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/access.py
+-rwxr-xr-x   0        0        0      598 2023-12-15 20:11:06.457198 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/path.py
+-rwxr-xr-x   0        0        0      957 2024-03-11 03:50:37.039618 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py
+-rwxr-xr-x   0        0        0      665 2024-03-11 03:53:05.197685 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      855 2023-12-15 23:01:07.547799 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      425 2023-12-15 20:37:53.477587 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/status_1.py
+-rwxr-xr-x   0        0        0     1040 2024-03-11 03:59:22.473027 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__init__.py
+-rwxr-xr-x   0        0        0      907 2024-03-29 23:34:10.581332 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1146 2023-12-15 20:38:04.629490 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1127 2024-03-11 03:56:08.423385 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/status_1.py
+-rwxr-xr-x   0        0        0      521 2023-12-15 20:03:32.715951 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__init__.py
+-rwxr-xr-x   0        0        0      895 2024-02-04 21:46:17.267655 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1282 2023-12-15 20:03:59.450730 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      452 2023-12-15 20:03:32.730951 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/status_actual/status_1.py
+-rwxr-xr-x   0        0        0      994 2023-12-15 20:03:32.744950 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/__init__.py
+-rwxr-xr-x   0        0        0     2132 2023-11-27 20:33:10.870623 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1160 2023-12-15 20:37:53.503587 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/__init__.py
+-rwxr-xr-x   0        0        0     2262 2023-11-25 19:20:33.032957 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      735 2023-12-15 20:03:32.775950 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/__init__.py
+-rwxr-xr-x   0        0        0     1466 2023-11-24 01:19:42.973352 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      749 2023-12-15 20:03:32.790950 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/__init__.py
+-rwxr-xr-x   0        0        0     1582 2023-12-15 18:48:20.744152 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0       93 2023-11-25 18:51:12.376547 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/sculpt.r.HTML
+-rwxr-xr-x   0        0        0      251 2023-12-15 20:03:32.804950 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/status_1.py
+-rwxr-xr-x   0        0        0      424 2023-12-15 22:29:15.419867 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/assertions/one/__init__.py
+-rwxr-xr-x   0        0        0      609 2024-02-04 22:00:53.441098 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/assertions/one/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      893 2023-12-15 22:39:49.023943 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/assertions/one/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      504 2023-12-15 20:03:32.608952 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/assertions/recipe/__init__.py
+-rwxr-xr-x   0        0        0      768 2023-12-15 22:31:10.731971 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__init__.py
+-rwxr-xr-x   0        0        0     1000 2024-02-04 22:00:53.442098 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1474 2023-12-15 22:39:49.023943 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1030 2023-12-17 01:34:38.227857 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__init__.py
+-rwxr-xr-x   0        0        0     1102 2024-02-04 21:46:16.701659 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1758 2023-12-17 01:34:53.335684 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      668 2023-12-17 01:36:56.858274 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_1.py
+-rwxr-xr-x   0        0        0      603 2023-12-17 01:38:18.265344 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_2.py
+-rwxr-xr-x   0        0        0      551 2023-12-15 22:31:10.745971 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__init__.py
+-rwxr-xr-x   0        0        0      799 2024-02-04 21:46:17.060656 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1170 2023-12-15 22:31:23.050875 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      798 2023-12-15 20:03:32.879949 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/status_1.py
+-rwxr-xr-x   0        0        0      254 2023-11-23 22:33:02.113155 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/grove.s.HTML
+-rwxr-xr-x   0        0        0     4712 2024-03-31 22:07:23.909086 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__init__.py
+-rwxr-xr-x   0        0        0     1645 2024-03-31 22:08:36.700698 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3030 2023-12-15 22:31:23.142875 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      945 2023-11-26 03:02:03.332197 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/has_uniters.r.HTML
+-rwxr-xr-x   0        0        0     1055 2023-12-15 22:31:10.773971 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/status_1.py
+-rwxr-xr-x   0        0        0      222 2023-12-09 18:50:30.819756 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/measures/measures.s.HTML
+-rwxr-xr-x   0        0        0      176 2023-12-15 20:03:32.925949 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/measures/seek_fraction_string/__init__.py
+-rwxr-xr-x   0        0        0      164 2023-12-15 20:03:32.938949 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/measures/seek_fraction_string/status_1.py
+-rwxr-xr-x   0        0        0     2879 2023-12-17 01:45:25.376468 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__init__.py
+-rwxr-xr-x   0        0        0     2351 2024-02-04 21:46:15.976664 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3863 2023-12-17 01:45:27.972438 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     9652 2023-12-15 19:06:54.650929 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/note.txt
+-rwxr-xr-x   0        0        0      542 2023-12-15 23:08:39.155150 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/nurture.s.HTML
+-rwxr-xr-x   0        0        0     1297 2023-12-15 23:05:28.423694 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/status_cautions_1.py
+-rwxr-xr-x   0        0        0      696 2023-12-15 22:31:10.815971 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/status_essentials_1.py
+-rwxr-xr-x   0        0        0     1424 2023-12-15 23:01:30.390616 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/print/__init__.py
+-rwxr-xr-x   0        0        0     1458 2024-02-04 21:46:17.005657 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/print/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2465 2023-12-15 23:01:32.768597 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/print/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1235 2023-12-17 01:00:44.139172 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__init__.py
+-rwxr-xr-x   0        0        0     1002 2024-02-04 21:46:16.030664 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1378 2023-12-17 01:00:55.887037 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      572 2023-12-15 22:31:10.859970 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek/status_1.py
+-rwxr-xr-x   0        0        0      469 2023-12-15 20:03:33.024948 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/__init__.py
+-rwxr-xr-x   0        0        0      739 2024-02-04 21:46:16.728659 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1101 2023-12-15 20:03:58.148740 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3891 2023-12-08 03:23:39.720308 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/essentials.JSON
+-rwxr-xr-x   0        0        0      833 2023-12-15 23:06:34.419160 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/status_1.py
+-rwxr-xr-x   0        0        0     1237 2023-12-15 22:31:10.873970 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__init__.py
+-rwxr-xr-x   0        0        0     1116 2024-02-04 21:46:16.111663 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1834 2023-12-15 22:31:20.150898 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      568 2023-12-15 20:03:33.071948 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/status_1.py
+-rwxr-xr-x   0        0        0     1056 2023-12-17 00:41:11.531623 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__init__.py
+-rwxr-xr-x   0        0        0     1243 2024-02-04 21:46:16.029664 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1985 2023-12-17 00:41:23.756483 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      507 2023-12-15 20:03:33.104947 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/status_1.py
+-rwxr-xr-x   0        0        0      794 2023-12-15 22:31:10.903970 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__init__.py
+-rwxr-xr-x   0        0        0     1055 2024-02-04 21:46:17.013657 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1550 2023-12-15 22:31:23.110875 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2023-12-15 22:31:10.916970 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/status_1.py
+-rwxr-xr-x   0        0        0      633 2023-12-15 22:31:10.928970 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__init__.py
+-rwxr-xr-x   0        0        0     1148 2024-02-04 21:46:17.006657 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1680 2023-12-15 22:31:23.097875 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      180 2023-11-23 19:14:43.750059 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/grove prototype.r.HTML
+-rwxr-xr-x   0        0        0     1903 2023-12-15 22:31:10.942969 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__init__.py
+-rwxr-xr-x   0        0        0     2203 2024-02-04 21:46:16.469661 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3647 2023-12-15 22:31:21.710886 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      918 2023-12-15 20:35:42.040737 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__init__.py
+-rwxr-xr-x   0        0        0      813 2024-02-04 21:46:16.469661 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1127 2023-12-15 20:36:59.502059 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      536 2023-12-15 20:35:49.922668 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_1.py
+-rwxr-xr-x   0        0        0      624 2023-12-15 20:36:03.137552 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_2.py
+-rwxr-xr-x   0        0        0      966 2023-12-15 20:42:05.241384 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/status_1.py
+-rwxr-xr-x   0        0        0     1389 2023-12-15 20:03:33.244946 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__init__.py
+-rwxr-xr-x   0        0        0     1325 2024-02-04 21:46:16.470661 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2194 2023-12-15 20:03:57.290748 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      719 2023-12-15 20:36:28.059334 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__init__.py
+-rwxr-xr-x   0        0        0      615 2024-02-04 21:46:16.471661 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      929 2023-12-15 20:36:59.505059 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      529 2023-12-15 20:36:38.211246 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/status_1.py
+-rwxr-xr-x   0        0        0      615 2023-12-15 20:36:51.162132 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/status_2.py
+-rwxr-xr-x   0        0        0      692 2023-11-24 00:44:01.444936 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/ingredient/nutrient_pattern.s.HTML
+-rwxr-xr-x   0        0        0     1012 2024-03-29 20:58:01.155250 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/ingredient scan.s.HTML
+-rwxr-xr-x   0        0        0     4982 2024-03-29 23:50:17.061986 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__init__.py
+-rwxr-xr-x   0        0        0     2377 2024-03-29 23:51:14.241315 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3660 2023-12-15 20:03:55.578762 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0        3 2023-11-27 20:33:45.784509 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/add_measured_ingredient.r.HTML
+-rwxr-xr-x   0        0        0     1082 2023-12-15 20:03:33.325946 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py
+-rwxr-xr-x   0        0        0     2212 2024-03-29 23:53:03.560032 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_1.py
+-rwxr-xr-x   0        0        0     2200 2024-03-29 23:53:32.283694 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_2.py
+-rwxr-xr-x   0        0        0     3932 2024-03-29 23:52:06.320703 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/status_1.py
+-rwxr-xr-x   0        0        0     1136 2023-12-15 23:10:16.248364 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/__init__.py
+-rwxr-xr-x   0        0        0      976 2024-02-04 21:46:15.975664 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1378 2023-12-15 23:11:10.322927 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      561 2024-02-04 21:46:15.979664 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/measures.cpython-310.pyc
+-rwxr-xr-x   0        0        0      715 2023-12-15 20:03:55.424763 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/measures.cpython-311.pyc
+-rwxr-xr-x   0        0        0      375 2023-12-15 20:03:33.404945 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/measures.py
+-rwxr-xr-x   0        0        0      324 2023-12-15 23:11:21.661835 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/status_1.py
+-rwxr-xr-x   0        0        0      812 2023-12-15 23:12:52.091103 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/status_cautionary_1.py
+-rwxr-xr-x   0        0        0     3271 2024-03-30 21:01:29.376796 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__init__.py
+-rwxr-xr-x   0        0        0     1590 2024-03-30 21:02:46.028385 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2481 2023-12-15 23:20:29.920394 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1644 2023-12-17 01:39:47.249328 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__init__.py
+-rwxr-xr-x   0        0        0     1525 2024-02-04 22:00:53.448098 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2202 2023-12-17 01:47:38.718946 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3497 2024-03-29 23:49:19.694659 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/land.s.HTML
+-rwxr-xr-x   0        0        0      439 2023-12-15 20:03:33.447945 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/__init__.py
+-rwxr-xr-x   0        0        0      815 2024-02-04 22:00:54.280092 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1095 2023-12-15 20:03:55.450763 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      614 2023-12-15 20:03:33.461945 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/status_1.py
+-rwxr-xr-x   0        0        0     2794 2024-03-29 23:51:11.921342 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__init__.py
+-rwxr-xr-x   0        0        0     1774 2024-03-29 23:53:51.883464 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2771 2023-12-15 20:03:55.426763 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      407 2023-12-15 20:03:33.492944 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/status/status_1.py
+-rwxr-xr-x   0        0        0     2290 2023-12-15 20:50:14.984241 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__init__.py
+-rwxr-xr-x   0        0        0     1885 2024-02-04 22:00:53.451098 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2945 2023-12-15 20:50:23.774168 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      780 2024-02-04 22:00:53.485098 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/__pycache__/course_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1182 2023-12-15 22:29:32.153737 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/__pycache__/course_2.cpython-311.pyc
+-rwxr-xr-x   0        0        0      551 2023-12-15 20:50:37.247054 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/course_2.py
+-rwxr-xr-x   0        0        0      950 2023-11-27 02:53:23.082794 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/multiply_measures.s.HTML
+-rwxr-xr-x   0        0        0     2582 2024-03-30 00:06:40.890240 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_1.py
+-rwxr-xr-x   0        0        0     2923 2024-03-30 00:05:43.491040 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_2.py
+-rwxr-xr-x   0        0        0     1039 2023-12-15 20:03:33.561944 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_loop_1.py
+-rwxr-xr-x   0        0        0     1313 2024-03-30 00:01:21.450188 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__init__.py
+-rwxr-xr-x   0        0        0     1150 2024-03-30 00:01:26.518128 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1601 2023-12-15 20:03:54.816768 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1477 2024-03-30 00:13:11.765040 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_1.py
+-rwxr-xr-x   0        0        0     1475 2024-03-30 00:08:56.548392 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_2.py
+-rwxr-xr-x   0        0        0     1319 2024-03-30 00:09:21.776054 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_3.py
+-rwxr-xr-x   0        0        0      776 2023-12-15 20:03:33.638943 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__init__.py
+-rwxr-xr-x   0        0        0      842 2024-02-04 22:00:53.483098 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1336 2023-12-15 20:03:54.814768 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1728 2023-12-15 20:03:33.654943 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/status_1.py
+-rwxr-xr-x   0        0        0      275 2023-11-26 22:20:49.328242 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/selected_unit/__init__.py
+-rwxr-xr-x   0        0        0      102 2023-12-15 19:52:46.524296 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/names.s.HTML
+-rwxr-xr-x   0        0        0     1200 2024-03-07 04:13:37.347239 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__init__.py
+-rwxr-xr-x   0        0        0     1259 2024-03-11 01:21:46.158376 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1632 2024-02-04 19:33:07.617350 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1207 2023-12-16 05:02:53.973031 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_empty/status_1.py
+-rwxr-xr-x   0        0        0     2315 2024-03-30 00:02:05.729668 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_0.py
+-rwxr-xr-x   0        0        0     6474 2024-03-30 00:18:21.421112 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_1.py
+-rwxr-xr-x   0        0        0     3862 2024-03-30 00:17:10.781998 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_2.py
+-rwxr-xr-x   0        0        0     2473 2024-02-04 20:24:03.569661 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_3.py
+-rwxr-xr-x   0        0        0   215864 2024-04-11 17:28:28.862053 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.JSON
+-rwxr-xr-x   0        0        0     2506 2024-03-11 02:02:18.286816 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.py
+-rwxr-xr-x   0        0        0   131410 2024-04-11 17:28:28.150062 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.JSON
+-rwxr-xr-x   0        0        0     1863 2024-03-11 01:24:01.392835 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.py
+-rwxr-xr-x   0        0        0   127961 2024-04-11 17:28:28.470058 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.JSON
+-rwxr-xr-x   0        0        0     1755 2023-12-16 05:04:27.952247 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.py
+-rwxr-xr-x   0        0        0     1606 2023-12-16 05:04:52.885039 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1_supp_1.py
+-rwxr-xr-x   0        0        0     1707 2024-02-04 22:00:53.495098 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/__pycache__/ingredient.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3758 2023-12-16 05:01:10.617894 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/__pycache__/ingredient.cpython-311.pyc
+-rwxr-xr-x   0        0        0     2844 2023-12-16 05:01:05.865934 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/ingredient.py
+-rwxr-xr-x   0        0        0      471 2023-12-15 22:41:08.357326 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/__init__.py
+-rwxr-xr-x   0        0        0      902 2024-02-04 22:00:53.486098 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1185 2023-12-15 22:41:31.485147 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0        0 2023-12-09 18:24:24.688260 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/slice/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-12-16 04:48:59.742994 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/cautionary_ingredients/formulate.py
+-rwxr-xr-x   0        0        0     2968 2024-03-11 01:21:46.166376 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/__pycache__/formulate.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4840 2023-12-16 04:55:55.440526 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/__pycache__/formulate.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3439 2024-03-07 04:11:50.688393 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/formulate.py
+-rwxr-xr-x   0        0        0     1876 2023-11-26 22:19:07.302481 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/recipe structure.s.HTML
+-rwxr-xr-x   0        0        0      968 2024-02-04 19:27:25.533932 apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/recipe.s.HTML
+-rwxr-xr-x   0        0        0      101 2023-11-17 21:50:38.225811 apoplast-2.0.8/venues/stages/apoplast/shows/natures/__init__.py
+-rwxr-xr-x   0        0        0      328 2024-02-04 21:46:15.412669 apoplast-2.0.8/venues/stages/apoplast/shows/natures/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      440 2023-11-21 19:25:30.099428 apoplast-2.0.8/venues/stages/apoplast/shows/natures/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      633 2024-02-04 21:46:15.413668 apoplast-2.0.8/venues/stages/apoplast/shows/natures/__pycache__/assertions.cpython-310.pyc
+-rwxr-xr-x   0        0        0      934 2023-11-21 23:22:13.005761 apoplast-2.0.8/venues/stages/apoplast/shows/natures/__pycache__/assertions.cpython-311.pyc
+-rwxr-xr-x   0        0        0      371 2023-11-21 23:21:15.613421 apoplast-2.0.8/venues/stages/apoplast/shows/natures/assertions.py
+-rwxr-xr-x   0        0        0       84 2023-11-22 02:42:38.990104 apoplast-2.0.8/venues/stages/apoplast/shows/natures/measured_ingredient/assertions.py
+-rwxr-xr-x   0        0        0      332 2024-03-29 20:56:02.996705 apoplast-2.0.8/venues/stages/apoplast/shows/natures/nature.s.HTML
+-rwxr-xr-x   0        0        0     3867 2023-11-28 02:28:19.579319 apoplast-2.0.8/venues/stages/apoplast/shows/natures/pattern/nature/nature.S.HTML
+-rwxr-xr-x   0        0        0     2209 2023-11-25 23:54:11.701513 apoplast-2.0.8/venues/stages/apoplast/shows/natures/pattern/nature: form.S.HTML
+-rwxr-xr-x   0        0        0      139 2023-11-28 02:28:25.915261 apoplast-2.0.8/venues/stages/apoplast/shows/natures/pattern/pattern.S.HTML
+-rwxr-xr-x   0        0        0      115 2023-11-16 20:19:44.647903 apoplast-2.0.8/venues/stages/apoplast/shows/natures/pattern/pattern: measured ingredients.S.HTML
+-rwxr-xr-x   0        0        0        5 2023-11-16 20:58:52.759569 apoplast-2.0.8/venues/stages/apoplast/shows/natures/pattern/pattern: unmeasured ingredients.S.HTML
+-rwxr-xr-x   0        0        0      843 2024-03-31 01:49:28.876629 apoplast-2.0.8/venues/stages/apoplast/shows/shows.s.HTML
+-rwxr-xr-x   0        0        0     1523 2024-03-31 02:20:59.032310 apoplast-2.0.8/venues/stages/apoplast/shows_v2/land/grove/grove.S.HTML
+-rwxr-xr-x   0        0        0       58 2024-03-31 02:19:44.581133 apoplast-2.0.8/venues/stages/apoplast/shows_v2/land/grove/info/info.S.HTML
+-rwxr-xr-x   0        0        0       73 2024-03-31 02:21:06.092232 apoplast-2.0.8/venues/stages/apoplast/shows_v2/land/grove/measures/measures.S.HTML
+-rwxr-xr-x   0        0        0       59 2024-03-31 02:21:27.675994 apoplast-2.0.8/venues/stages/apoplast/shows_v2/land/grove/natures/natures.S.HTML
+-rwxr-xr-x   0        0        0     1508 2024-03-31 02:23:11.418860 apoplast-2.0.8/venues/stages/apoplast/shows_v2/land/grove/unites/unites.S.HTML
+-rwxr-xr-x   0        0        0      131 2024-03-31 02:19:06.373559 apoplast-2.0.8/venues/stages/apoplast/shows_v2/land/land.S.HTML
+-rwxr-xr-x   0        0        0      459 2024-03-31 02:16:52.687064 apoplast-2.0.8/venues/stages/apoplast/shows_v2/land/measures/measures.S.HTML
+-rwxr-xr-x   0        0        0      412 2024-03-31 02:09:01.592689 apoplast-2.0.8/venues/stages/apoplast/shows_v2/land/natures/natures.S.HTML
+-rwxr-xr-x   0        0        0      405 2024-03-31 01:56:16.948471 apoplast-2.0.8/venues/stages/apoplast/shows_v2/nature/measured_ingredients/measured_ingredients.S.HTML
+-rwxr-xr-x   0        0        0     1018 2024-03-31 01:54:44.445413 apoplast-2.0.8/venues/stages/apoplast/shows_v2/nature/measures/measures.S.HTML
+-rwxr-xr-x   0        0        0      426 2024-03-31 01:58:10.379316 apoplast-2.0.8/venues/stages/apoplast/shows_v2/nature/nature.S.HTML
+-rwxr-xr-x   0        0        0      294 2024-03-31 01:56:52.156113 apoplast-2.0.8/venues/stages/apoplast/shows_v2/nature/unmeasured_ingredients/UI.S.HTML
+-rwxr-xr-x   0        0        0      106 2024-03-31 01:57:56.055462 apoplast-2.0.8/venues/stages/apoplast/shows_v2/shows.S.HTML
+-rwxr-xr-x   0        0        0      232 2024-03-31 01:52:52.946549 apoplast-2.0.8/venues/stages/apoplast/shows_v2/treasure/treasure.S.HTML
+-rwxr-xr-x   0        0        0       63 2023-11-16 19:27:45.065885 apoplast-2.0.8/venues/stages/apoplast/status_1.py
+-rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 apoplast-2.0.8/PKG-INFO
```

### Comparing `apoplast-2.0.7/readme.md` & `apoplast-2.0.8/readme.md`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venue.S.HTML` & `apoplast-2.0.8/venue.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/___license/list/gpl-3.0-standalone.html` & `apoplast-2.0.8/venues/stages/apoplast/___license/list/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/__itinerary/apoplast.S.HTML` & `apoplast-2.0.8/venues/stages/apoplast/__itinerary/apoplast.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/__status/db/records.json` & `apoplast-2.0.8/venues/stages/apoplast/__status/db/records.json`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/__status/db_API/records.json` & `apoplast-2.0.8/venues/stages/apoplast/__status/db_API/records.json`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/__status/status.proc.py` & `apoplast-2.0.8/venues/stages/apoplast/__status/status.proc.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/__status/status_API.proc.py` & `apoplast-2.0.8/venues/stages/apoplast/__status/status_API.proc.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_ellipses/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/_ellipses/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_ellipses/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/_ellipses/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/clique/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/clique/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/clique/group/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/__pycache__/clique.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/customs/clique.py` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/customs/clique.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/__pycache__/clique.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/__pycache__/harbor.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/__pycache__/harbor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/__pycache__/off.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/__pycache__/on.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/clique.py` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/clique.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/harbor.py` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/harbor.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_interfaces/sanic/on.py` & `apoplast-2.0.8/venues/stages/apoplast/_interfaces/sanic/on.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_variables/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/_variables/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/_variables/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/__pycache__/source.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/__pycache__/source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/__pycache__/source.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/__pycache__/source.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/BRANDED.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/BRANDED.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/beet_juice_2412474.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/beet_juice_2412474.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/beet_juice_2642759.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/beet_juice_2642759.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/impossible_beef_2664238.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/impossible_beef_2664238.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/problems/impossible_2468423.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/problems/impossible_2468423.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/vegan_pizza_2672996.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/vegan_pizza_2672996.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/branded/walnuts_1882785.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/branded/walnuts_1882785.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/food.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/food.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/assertions.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/assertions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/assertions.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/__pycache__/assertions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/assertions.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/assertions.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_mass_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_volume_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/interpret/status_volume_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/label_splitter/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/interpret/packageWeight/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_2.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_2412474.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_2412474.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_3.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_3.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_loop_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/_status/status_loop_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/cautionary_ingredients/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/essential_nutrients/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/form/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/form/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/form/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/form/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/form/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/form/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/form/status_mass_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/form/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/form/status_volume_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/form/status_volume_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_IU_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_IU_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_energy_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_energy_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_mass_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/_status/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/energy/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/mass/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/food_nutrient_calculator.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/food_nutrient_calculator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/label_nutrient_calculator.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/__pycache__/label_nutrient_calculator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/food_nutrient.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/amount/per_package/food_nutrient.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/ingredient_prototype_1.r.HTML` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredient/ingredient_prototype_1.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_mass_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_volume_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/_status/status_volume_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/example.r.HTML` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/example.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/for_each/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/food_USDA/nature/measured_ingredients_list/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/goodness_certifications/certifications.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/goodness_certifications/certifications.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/goodness_certifications/vegan.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/clouds/goodness_certifications/vegan.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/NIH.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/NIH.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/__pycache__/source.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/__pycache__/source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/__pycache__/source.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/__pycache__/source.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/assertions.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/assertions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/assertions.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/__pycache__/assertions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/assertions.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/deliveries/one/assertions.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/coated tablets/multivitamin_276336.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/coated tablets/multivitamin_276336.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/other/chia_seeds_214893.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/other/chia_seeds_214893.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/powder/mane_270619.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/powder/mane_270619.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/powder/nutritional_shake_220884.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/powder/nutritional_shake_220884.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/powder packets/multivitamin_246811.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/powder packets/multivitamin_246811.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/calcium_261967.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/calcium_261967.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/multivitamin_249664.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/tablets/multivitamin_249664.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/examples/vegan_capsules/probiotics_248267.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/examples/vegan_capsules/probiotics_248267.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/status_powder_packets_246811.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/interpret/ingredientRows/for_each/status_powder_packets_246811.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/_loop/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/_loop/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336_nature.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/coated_tablets/status_multivitamin_276336_nature.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/chia_seeds_214893_nature.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/chia_seeds_214893_nature.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/status_chia_seeds_214893.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/other/status_chia_seeds_214893.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/mane_270619_nature.JSON` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/mane_270619_nature.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/status_mane_270619.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/_status/powder/status_mane_270619.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/cautionary_ingredients/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/essential_nutrients.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/essential_nutrients/essential_nutrients.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/amount/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/form.r.HTML` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/form.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_246811.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/serving_size/amount/status_276336.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_coated_tablet_276336.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_gram_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_gram_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_220884.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_220884.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_270619.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_270619.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_packets_246811.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_powder_packets_246811.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_tablet_261967.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_tablet_261967.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/form/unit/status_vegan_capsule_248267.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/measured_ingredient.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredient/measured_ingredient.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/_status/status_chia_seeds_214893.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/measured_ingredients.r.HTML` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/measured_ingredients.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/clouds/supp_NIH/nature/measured_ingredients/seek_name/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/__pycache__/clique.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/connect.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/connect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/off.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/on.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/open.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/open.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/status.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/connect.py` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/connect.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/off.py` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/off.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/on.py` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/on.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/DB/status.py` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/DB/status.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/__pycache__/clique.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/essential_nutrients/essential_nutrients.1.json` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/_saves/exports/essential_nutrients/essential_nutrients.1.json`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/clique.py` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/clique.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/collections/_land/__pycache__/insert_document.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/collections/_land/__pycache__/insert_document.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/collections/_land/insert_document.py` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/collections/_land/insert_document.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/data_nodes/ingredients/ingredients.S.HTML` & `apoplast-2.0.8/venues/stages/apoplast/data_nodes/ingredients/ingredients.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/insure/__pycache__/equalities.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/insure/__pycache__/equalities.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/insure/__pycache__/equalities.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/insure/__pycache__/equalities.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/insure/__pycache__/equality.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/insure/__pycache__/equality.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/insure/__pycache__/override_print.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/insure/__pycache__/override_print.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/insure/__pycache__/override_print.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/insure/__pycache__/override_print.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/insure/equalities.py` & `apoplast-2.0.8/venues/stages/apoplast/insure/equalities.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/insure/override_print.py` & `apoplast-2.0.8/venues/stages/apoplast/insure/override_print.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/_interpret/__pycache__/unit_kind.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/_interpret/__pycache__/unit_kind.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/_interpret/__pycache__/unit_kind.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/_interpret/__pycache__/unit_kind.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/_interpret/status_unit_kind.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/_interpret/status_unit_kind.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/_interpret/unit_kind.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/_interpret/unit_kind.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/energy/energy.r.HTML` & `apoplast-2.0.8/venues/stages/apoplast/measures/energy/energy.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/energy/swap/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/energy/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/energy/swap/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/energy/swap/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/energy/swap/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/energy/swap/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/mass/swap/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/mass/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/mass/swap/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/mass/swap/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/mass/swap/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/mass/swap/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/mass/swap/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/mass/swap/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/mass/system international.r.html` & `apoplast-2.0.8/venues/stages/apoplast/measures/mass/system international.r.html`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/mass/us customary.r.html` & `apoplast-2.0.8/venues/stages/apoplast/measures/mass/us customary.r.html`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/mass_equivalents/jargon.r.HTML` & `apoplast-2.0.8/venues/stages/apoplast/measures/mass_equivalents/jargon.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/mass_equivalents/mass equivalents.r.HTML` & `apoplast-2.0.8/venues/stages/apoplast/measures/mass_equivalents/mass equivalents.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/status_2.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/decimal/reduce/status_3.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/decimal/reduce/status_3.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/integer/__pycache__/string_is_integer.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/integer/__pycache__/string_is_integer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/integer/__pycache__/string_is_integer.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/integer/__pycache__/string_is_integer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/integer/status_string_is_integer.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/integer/status_string_is_integer.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/percentage/__pycache__/from_fraction.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/percentage/__pycache__/from_fraction.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/percentage/__pycache__/from_fraction.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/percentage/__pycache__/from_fraction.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/percentage/from_fraction.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/percentage/from_fraction.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/percentage/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/percentage/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note/_status/status_multiples_of_3_1.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note/_status/status_multiples_of_3_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note/sci_note.S.HTML` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note/sci_note.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note/sci_note_possibilities.S.HTML` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note/sci_note_possibilities.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note/sci_note_thoughts.S.HTML` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note/sci_note_thoughts.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note_2/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/number/sci_note_2/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/number/sci_note_2/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/volume/swap/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/volume/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/volume/swap/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/volume/swap/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/volume/swap/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/measures/volume/swap/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/volume/swap/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/measures/volume/swap/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/measures/weight/weight.r.html` & `apoplast-2.0.8/venues/stages/apoplast/measures/weight/weight.r.html`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/proposals/proposals.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/proposals/proposals.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/room.md` & `apoplast-2.0.8/venues/stages/apoplast/room.md`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin a.r.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin a.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin b.r.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin b.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin d.r.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/_journal/structures/vitamin d.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/forward channel.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/forward channel.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/forward_channel/structures.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/forward_channel/structures.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/access.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/access.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/access.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/access.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/path.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/path.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/__pycache__/path.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/1.JSON` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/1.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/2.JSON` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/archive/2.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/essentials.JSON` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/_bases/essentials/essentials.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/access.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/access.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/path.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/path.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/list/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/scan/seek_next_region/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/adapt_every/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/add/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/DB/sculpt/essential/erase/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/assertions/one/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/assertions/one/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/assertions/one/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/assertions/one/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/assertions/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_2.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/erase_ingredient/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/essential_is_story_1/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/has_uniters.r.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/has_uniters.r.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/has_uniters/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/note.txt` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/note.txt`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/nurture.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/nurture.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/status_cautions_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/status_cautions_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/status_essentials_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/nurture/status_essentials_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/print/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/print/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/print/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/print/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/print/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/print/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/essentials.JSON` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/essentials.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_count/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_measured_ingredient_name/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_name_or_accepts/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/seek_uniter/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove/sort/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_2.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/seek/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/nurture/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/print/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/status_2.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/grove_prototype/seek/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/ingredient/nutrient_pattern.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/ingredient/nutrient_pattern.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/ingredient scan.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/ingredient scan.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_empty_grove/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_2.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_and_meq/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/add_measured_ingredient/status_m_eq_and_ba/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/measures.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/measures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/measures.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/__pycache__/measures.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/build/status_cautionary_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/build/status_cautionary_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/calculate_portions/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/cultivate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/land.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/land.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/aggregate/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/measures/sums/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/__pycache__/course_2.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/__pycache__/course_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/__pycache__/course_2.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/__pycache__/course_2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/course_2.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/courses/course_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/multiply_measures.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/multiply_measures.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_2.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_loop_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/land/multiply_amount/status_loop_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/merge/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_2.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_3.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/merge/status_3.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan/measures/multiply/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__init__.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__init__.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_empty/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_empty/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_0.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_0.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_2.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_2.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_3.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_food/status_3.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.JSON` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_foods_and_supps/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.JSON` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_rational_amounts/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.JSON` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.JSON`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1_supp_1.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/_status/status_supp/status_1_supp_1.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/__pycache__/ingredient.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/__pycache__/ingredient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/__pycache__/ingredient.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/__pycache__/ingredient.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/ingredient.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/assertions/ingredient.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/__pycache__/__init__.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/__pycache__/__init__.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/calculate/grove_mass_and_mass_eq_sum/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/__pycache__/formulate.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/__pycache__/formulate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/__pycache__/formulate.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/__pycache__/formulate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/formulate.py` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/formulate/essential_nutrients/formulate.py`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/recipe structure.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/recipe structure.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/ingredient_scan_recipe/recipe.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/ingredient_scan_recipe/recipe.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/natures/__pycache__/assertions.cpython-310.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/natures/__pycache__/assertions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/natures/__pycache__/assertions.cpython-311.pyc` & `apoplast-2.0.8/venues/stages/apoplast/shows/natures/__pycache__/assertions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/natures/pattern/nature/nature.S.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/natures/pattern/nature/nature.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/natures/pattern/nature: form.S.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/natures/pattern/nature: form.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows/shows.s.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows/shows.s.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows_v2/land/grove/grove.S.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows_v2/land/grove/grove.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows_v2/land/grove/unites/unites.S.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows_v2/land/grove/unites/unites.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/venues/stages/apoplast/shows_v2/nature/measures/measures.S.HTML` & `apoplast-2.0.8/venues/stages/apoplast/shows_v2/nature/measures/measures.S.HTML`

 * *Files identical despite different names*

### Comparing `apoplast-2.0.7/PKG-INFO` & `apoplast-2.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: apoplast
-Version: 2.0.7
+Version: 2.0.8
 Summary: 
+License: >1
 Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
```

