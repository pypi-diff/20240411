# Comparing `tmp/adafruit-circuitpython-requests-3.2.3.tar.gz` & `tmp/adafruit-circuitpython-requests-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-requests-3.2.3.tar", last modified: Mon Apr  1 22:43:26 2024, max compression
+gzip compressed data, was "adafruit-circuitpython-requests-3.2.4.tar", last modified: Wed Apr 10 23:58:42 2024, max compression
```

## Comparing `adafruit-circuitpython-requests-3.2.3.tar` & `adafruit-circuitpython-requests-3.2.4.tar`

### file list

```diff
@@ -1,89 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.593120 adafruit-circuitpython-requests-3.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.597120 adafruit-circuitpython-requests-3.2.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.597120 adafruit-circuitpython-requests-3.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.github/workflows/release_pypi.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     6147 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.597120 adafruit-circuitpython-requests-3.2.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2642 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-01 22:43:26.000000 adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-01 22:43:26.000000 adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:43:26.000000 adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 22:43:26.000000 adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 22:43:26.000000 adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/adafruit_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.597120 adafruit-circuitpython-requests-3.2.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.601120 adafruit-circuitpython-requests-3.2.3/docs/_static/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4414 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/_static/favicon.ico.license
--rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/api.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      803 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/examples.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)      973 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.593120 adafruit-circuitpython-requests-3.2.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.601120 adafruit-circuitpython-requests-3.2.3/examples/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/cpython/requests_cpython_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/cpython/requests_cpython_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.601120 adafruit-circuitpython-requests-3.2.3/examples/esp32spi/
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/esp32spi/requests_esp32spi_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/esp32spi/requests_esp32spi_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.601120 adafruit-circuitpython-requests-3.2.3/examples/fona/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/fona/requests_fona_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/fona/requests_fona_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.601120 adafruit-circuitpython-requests-3.2.3/examples/wifi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_discord.py
--rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_fitbit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_mastodon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_premiereleague.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_steam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_twitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_youtube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_multiple_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/requests_wifi_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wifi/requests_wifi_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/examples/wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wiznet5k/requests_wiznet5k_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/examples/wiznet5k/requests_wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:26.605120 adafruit-circuitpython-requests-3.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/chunk_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/chunked_redirect_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/header_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/method_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/parse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-01 22:43:24.000000 adafruit-circuitpython-requests-3.2.3/tests/reuse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-01 22:43:17.000000 adafruit-circuitpython-requests-3.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.180429 adafruit-circuitpython-requests-3.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.164429 adafruit-circuitpython-requests-3.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.168429 adafruit-circuitpython-requests-3.2.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.168429 adafruit-circuitpython-requests-3.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.github/workflows/release_pypi.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1724 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6147 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1098 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.168429 adafruit-circuitpython-requests-3.2.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-10 23:58:42.180429 adafruit-circuitpython-requests-3.2.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2642 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.180429 adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-10 23:58:42.000000 adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-10 23:58:42.000000 adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:58:42.000000 adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 23:58:42.000000 adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 23:58:42.000000 adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/adafruit_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.172429 adafruit-circuitpython-requests-3.2.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.172429 adafruit-circuitpython-requests-3.2.4/docs/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4414 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/_static/favicon.ico.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/api.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      803 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/examples.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)      973 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.164429 adafruit-circuitpython-requests-3.2.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.172429 adafruit-circuitpython-requests-3.2.4/examples/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/cpython/requests_cpython_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/cpython/requests_cpython_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.172429 adafruit-circuitpython-requests-3.2.4/examples/esp32spi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/esp32spi/requests_esp32spi_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/esp32spi/requests_esp32spi_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.172429 adafruit-circuitpython-requests-3.2.4/examples/fona/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/fona/requests_fona_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/fona/requests_fona_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.172429 adafruit-circuitpython-requests-3.2.4/examples/wifi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.176429 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_fitbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_mastodon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_premiereleague.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_multiple_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/requests_wifi_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wifi/requests_wifi_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.176429 adafruit-circuitpython-requests-3.2.4/examples/wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wiznet5k/requests_wiznet5k_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/examples/wiznet5k/requests_wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:58:42.180429 adafruit-circuitpython-requests-3.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:58:42.180429 adafruit-circuitpython-requests-3.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/chunk_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/chunked_redirect_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/header_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/method_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/parse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-10 23:58:39.000000 adafruit-circuitpython-requests-3.2.4/tests/reuse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-10 23:58:32.000000 adafruit-circuitpython-requests-3.2.4/tox.ini
```

### Comparing `adafruit-circuitpython-requests-3.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-requests-3.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/.gitignore` & `adafruit-circuitpython-requests-3.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/.pre-commit-config.yaml` & `adafruit-circuitpython-requests-3.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/.pylintrc` & `adafruit-circuitpython-requests-3.2.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-requests-3.2.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/LICENSE` & `adafruit-circuitpython-requests-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-requests-3.2.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/LICENSES/MIT.txt` & `adafruit-circuitpython-requests-3.2.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-requests-3.2.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/PKG-INFO` & `adafruit-circuitpython-requests-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 3.2.3
+Version: 3.2.4
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-requests-3.2.3/README.rst` & `adafruit-circuitpython-requests-3.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/PKG-INFO` & `adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 3.2.3
+Version: 3.2.4
 Summary: A requests-like library for web interfacing
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Keywords: adafruit,blinka,circuitpython,micropython,requests,requests,,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-requests-3.2.3/adafruit_circuitpython_requests.egg-info/SOURCES.txt` & `adafruit-circuitpython-requests-3.2.4/adafruit_circuitpython_requests.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py
 examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py
 examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py
 examples/wifi/expanded/requests_wifi_api_premiereleague.py
 examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py
 examples/wifi/expanded/requests_wifi_api_steam.py
 examples/wifi/expanded/requests_wifi_api_twitch.py
-examples/wifi/expanded/requests_wifi_api_twitter.py
 examples/wifi/expanded/requests_wifi_api_youtube.py
 examples/wifi/expanded/requests_wifi_multiple_cookies.py
 examples/wiznet5k/requests_wiznet5k_advanced.py
 examples/wiznet5k/requests_wiznet5k_simpletest.py
 tests/chunk_test.py
 tests/chunked_redirect_test.py
 tests/concurrent_test.py
```

### Comparing `adafruit-circuitpython-requests-3.2.3/adafruit_requests.py` & `adafruit-circuitpython-requests-3.2.4/adafruit_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   https://github.com/adafruit/circuitpython/releases
 
 * Adafruit's Connection Manager library:
   https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager
 
 """
 
-__version__ = "3.2.3"
+__version__ = "3.2.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Requests.git"
 
 import errno
 import json as json_module
 import sys
 
 from adafruit_connection_manager import get_connection_manager
```

### Comparing `adafruit-circuitpython-requests-3.2.3/docs/_static/favicon.ico` & `adafruit-circuitpython-requests-3.2.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/docs/conf.py` & `adafruit-circuitpython-requests-3.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/docs/examples.rst` & `adafruit-circuitpython-requests-3.2.4/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/docs/index.rst` & `adafruit-circuitpython-requests-3.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/cpython/requests_cpython_advanced.py` & `adafruit-circuitpython-requests-3.2.4/examples/cpython/requests_cpython_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/cpython/requests_cpython_simpletest.py` & `adafruit-circuitpython-requests-3.2.4/examples/cpython/requests_cpython_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/esp32spi/requests_esp32spi_advanced.py` & `adafruit-circuitpython-requests-3.2.4/examples/esp32spi/requests_esp32spi_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/esp32spi/requests_esp32spi_simpletest.py` & `adafruit-circuitpython-requests-3.2.4/examples/esp32spi/requests_esp32spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/fona/requests_fona_advanced.py` & `adafruit-circuitpython-requests-3.2.4/examples/fona/requests_fona_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/fona/requests_fona_simpletest.py` & `adafruit-circuitpython-requests-3.2.4/examples/fona/requests_fona_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_adafruit_discord_active_online.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_discord.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_discord.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_fitbit.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_fitbit.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_github.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_github.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
-# Coded for Circuit Python 8.2.x
+# Coded for Circuit Python 9.x
 """Github API Example"""
 
 import os
 import time
 
 import adafruit_connection_manager
 import wifi
```

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_mastodon.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_mastodon.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_openskynetwork_public.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,153 +1,180 @@
-# SPDX-FileCopyrightText: 2023 DJDevon3
+# SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
-# Coded for Circuit Python 8.1
-# DJDevon3 ESP32-S3 OpenSkyNetwork_Private_API_Example
+# Coded for Circuit Python 8.2.x
+"""OpenSky-Network.org Public API Example"""
+# pylint: disable=import-error
 
-import json
 import os
-import ssl
 import time
 
-import circuitpython_base64 as base64
-import socketpool
+import adafruit_connection_manager
 import wifi
 
 import adafruit_requests
 
-# OpenSky-Network.org Login required for this API
-# REST API: https://openskynetwork.github.io/opensky-api/rest.html
-# All active flights JSON: https://opensky-network.org/api/states/all  # PICK ONE! :)
+# No login necessary for Public API. Drastically reduced daily limit vs Private
+# OpenSky-Networks.org REST API: https://openskynetwork.github.io/opensky-api/rest.html
+# All active flights JSON: https://opensky-network.org/api/states/all PICK ONE!
 # JSON order: transponder, callsign, country
 # ACTIVE transpondes only, for multiple "c822af&icao24=cb3993&icao24=c63923"
-transponder = "7c6b2d"
+TRANSPONDER = "3c5ef8"
 
-# Initialize WiFi Pool (There can be only 1 pool & top of script)
-pool = socketpool.SocketPool(wifi.radio)
+# Get WiFi details, ensure these are setup in settings.toml
+ssid = os.getenv("CIRCUITPY_WIFI_SSID")
+password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
+osnusername = os.getenv("OSN_USERNAME")  # Website Credentials
+osnpassword = os.getenv("OSN_PASSWORD")  # Website Credentials
 
-# Time between API refreshes
+# API Polling Rate
 # 900 = 15 mins, 1800 = 30 mins, 3600 = 1 hour
 # OpenSky-Networks IP bans for too many requests, check rate limit.
 # https://openskynetwork.github.io/opensky-api/rest.html#limitations
-sleep_time = 1800
-
-# Get WiFi details, ensure these are setup in settings.toml
-ssid = os.getenv("CIRCUITPY_WIFI_SSID")
-password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
-osnu = os.getenv("OSN_Username")
-osnp = os.getenv("OSN_Password")
+SLEEP_TIME = 1800
 
-osn_cred = str(osnu) + ":" + str(osnp)
-bytes_to_encode = b" " + str(osn_cred) + " "
-base64_string = base64.encodebytes(bytes_to_encode)
-base64cred = repr(base64_string)[2:-1]
-
-Debug_Auth = False  # STREAMER WARNING this will show your credentials!
-if Debug_Auth:
-    osn_cred = str(osnu) + ":" + str(osnp)
-    bytes_to_encode = b" " + str(osn_cred) + " "
-    print(repr(bytes_to_encode))
-    base64_string = base64.encodebytes(bytes_to_encode)
-    print(repr(base64_string)[2:-1])
-    base64cred = repr(base64_string)[2:-1]
-    print("Decoded Bytes:", str(base64cred))
+# Set debug to True for full JSON response.
+# WARNING: makes credentials visible
+DEBUG = False
+
+# Initalize Wifi, Socket Pool, Request Session
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
+requests = adafruit_requests.Session(pool, ssl_context)
 
 # Requests URL - icao24 is their endpoint required for a transponder
 # example https://opensky-network.org/api/states/all?icao24=a808c5
-# OSN private requires your username:password to be base64 encoded
-osn_header = {"Authorization": "Basic " + str(base64cred)}
-OPENSKY_SOURCE = "https://opensky-network.org/api/states/all?" + "icao24=" + transponder
+OPENSKY_SOURCE = "https://opensky-network.org/api/states/all?" + "icao24=" + TRANSPONDER
 
 
-# Converts seconds to human readable minutes/hours/days
-def time_calc(input_time):  # input_time in seconds
+def time_calc(input_time):
+    """Converts seconds to minutes/hours/days"""
     if input_time < 60:
-        sleep_int = input_time
-        time_output = f"{sleep_int:.0f} seconds"
-    elif 60 <= input_time < 3600:
-        sleep_int = input_time / 60
-        time_output = f"{sleep_int:.0f} minutes"
-    elif 3600 <= input_time < 86400:
-        sleep_int = input_time / 60 / 60
-        time_output = f"{sleep_int:.1f} hours"
-    else:
-        sleep_int = input_time / 60 / 60 / 24
-        time_output = f"{sleep_int:.1f} days"
-    return time_output
+        return f"{input_time:.0f} seconds"
+    if input_time < 3600:
+        return f"{input_time / 60:.0f} minutes"
+    if input_time < 86400:
+        return f"{input_time / 60 / 60:.0f} hours"
+    return f"{input_time / 60 / 60 / 24:.1f} days"
 
 
 def _format_datetime(datetime):
-    return "{:02}/{:02}/{} {:02}:{:02}:{:02}".format(
-        datetime.tm_mon,
-        datetime.tm_mday,
-        datetime.tm_year,
-        datetime.tm_hour,
-        datetime.tm_min,
-        datetime.tm_sec,
+    """F-String formatted struct time conversion"""
+    return (
+        f"{datetime.tm_mon:02}/"
+        + f"{datetime.tm_mday:02}/"
+        + f"{datetime.tm_year:02} "
+        + f"{datetime.tm_hour:02}:"
+        + f"{datetime.tm_min:02}:"
+        + f"{datetime.tm_sec:02}"
     )
 
 
-# Connect to Wi-Fi
-print("\n===============================")
-print("Connecting to WiFi...")
-request = adafruit_requests.Session(pool, ssl.create_default_context())
-while not wifi.radio.ipv4_address:
-    try:
-        wifi.radio.connect(ssid, password)
-    except ConnectionError as e:
-        print("Connection Error:", e)
-        print("Retrying in 10 seconds")
-    time.sleep(10)
-print("Connected!\n")
-
 while True:
-    # STREAMER WARNING this will show your credentials!
-    debug_request = False  # Set True to see full request
-    if debug_request:
-        print("Full API HEADER: ", str(osn_header))
-        print("Full API GET URL: ", OPENSKY_SOURCE)
-        print("===============================")
-
-    print("\nAttempting to GET OpenSky-Network Data!")
-    opensky_response = request.get(url=OPENSKY_SOURCE, headers=osn_header).json()
-
-    # Print Full JSON to Serial (doesn't show credentials)
-    debug_response = False  # Set True to see full response
-    if debug_response:
-        dump_object = json.dumps(opensky_response)
-        print("JSON Dump: ", dump_object)
-
-    # Key:Value Serial Debug (doesn't show credentials)
-    osn_debug_keys = True  # Set True to print Serial data
-    if osn_debug_keys:
+    # Connect to Wi-Fi
+    print("\nConnecting to WiFi...")
+    while not wifi.radio.ipv4_address:
         try:
-            osn_flight = opensky_response["time"]
-            print("Current Unix Time: ", osn_flight)
+            wifi.radio.connect(ssid, password)
+        except ConnectionError as e:
+            print("❌ Connection Error:", e)
+            print("Retrying in 10 seconds")
+    print("✅ Wifi!")
 
-            current_struct_time = time.localtime(osn_flight)
-            current_date = "{}".format(_format_datetime(current_struct_time))
-            print(f"Unix to Readable Time: {current_date}")
-
-            # Current flight data for single callsign (right now)
-            osn_single_flight_data = opensky_response["states"]
-
-            if osn_single_flight_data is not None:
-                print("Flight Data: ", osn_single_flight_data)
-                transponder = opensky_response["states"][0][0]
-                print("Transponder: ", transponder)
-                callsign = opensky_response["states"][0][1]
-                print("Callsign: ", callsign)
-                country = opensky_response["states"][0][2]
-                print("Flight Country: ", country)
+    try:
+        print(" | Attempting to GET OpenSky-Network Single Flight JSON!")
+        try:
+            opensky_response = requests.get(url=OPENSKY_SOURCE)
+            opensky_json = opensky_response.json()
+        except ConnectionError as e:
+            print("Connection Error:", e)
+            print("Retrying in 10 seconds")
+
+        print(" | ✅ OpenSky-Network JSON!")
+
+        if DEBUG:
+            print("Full API GET URL: ", OPENSKY_SOURCE)
+            print(opensky_json)
+
+        # ERROR MESSAGE RESPONSES
+        if "timestamp" in opensky_json:
+            osn_timestamp = opensky_json["timestamp"]
+            print(f"❌ Timestamp: {osn_timestamp}")
+
+        if "message" in opensky_json:
+            osn_message = opensky_json["message"]
+            print(f"❌ Message: {osn_message}")
+
+        if "error" in opensky_json:
+            osn_error = opensky_json["error"]
+            print(f"❌ Error: {osn_error}")
+
+        if "path" in opensky_json:
+            osn_path = opensky_json["path"]
+            print(f"❌ Path: {osn_path}")
+
+        if "status" in opensky_json:
+            osn_status = opensky_json["status"]
+            print(f"❌ Status: {osn_status}")
+
+        # Current flight data for single callsign (right now)
+        osn_single_flight_data = opensky_json["states"]
+
+        if osn_single_flight_data is not None:
+            if DEBUG:
+                print(f" |  | Single Flight Public Data: {osn_single_flight_data}")
+
+            last_contact = opensky_json["states"][0][4]
+            # print(f" |  | Last Contact Unix Time: {last_contact}")
+            lc_struct_time = time.localtime(last_contact)
+            lc_readable_time = f"{_format_datetime(lc_struct_time)}"
+            print(f" |  | Last Contact: {lc_readable_time}")
+
+            flight_transponder = opensky_json["states"][0][0]
+            print(f" |  | Transponder: {flight_transponder}")
+
+            callsign = opensky_json["states"][0][1]
+            print(f" |  | Callsign: {callsign}")
+
+            squawk = opensky_json["states"][0][14]
+            print(f" |  | Squawk: {squawk}")
+
+            country = opensky_json["states"][0][2]
+            print(f" |  | Origin: {country}")
+
+            longitude = opensky_json["states"][0][5]
+            print(f" |  | Longitude: {longitude}")
+
+            latitude = opensky_json["states"][0][6]
+            print(f" |  | Latitude: {latitude}")
+
+            # Return Air Flight data if not on ground
+            on_ground = opensky_json["states"][0][8]
+            if on_ground is True:
+                print(f" |  | On Ground: {on_ground}")
             else:
-                print("Flight has no active data or you're polling too fast.")
+                altitude = opensky_json["states"][0][7]
+                print(f" |  | Barometric Altitude: {altitude}")
+
+                velocity = opensky_json["states"][0][9]
+                if velocity != "null":
+                    print(f" |  | Velocity: {velocity}")
+
+                vertical_rate = opensky_json["states"][0][11]
+                if vertical_rate != "null":
+                    print(f" |  | Vertical Rate: {vertical_rate}")
+        else:
+            print("This flight has no active data or you're polling too fast.")
+            print("Public Limits: 10 second max poll & 400 weighted calls daily")
+
+        opensky_response.close()
+        print("✂️ Disconnected from OpenSky-Network API")
+
+        print("\nFinished!")
+        print(f"Board Uptime: {time_calc(time.monotonic())}")
+        print(f"Next Update: {time_calc(SLEEP_TIME)}")
+        print("===============================")
 
-            print("\nFinished!")
-            print("Board Uptime: ", time_calc(time.monotonic()))
-            print("Next Update: ", time_calc(sleep_time))
-            time.sleep(sleep_time)
-            print("===============================")
-
-        except (ConnectionError, ValueError, NameError) as e:
-            print("OSN Connection Error:", e)
-            print("Next Retry: ", time_calc(sleep_time))
-            time.sleep(sleep_time)
+    except (ValueError, RuntimeError) as e:
+        print(f"Failed to get data, retrying\n {e}")
+        time.sleep(60)
+        break
+    time.sleep(SLEEP_TIME)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_openskynetwork_private_area.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_openskynetwork_private.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,186 +1,193 @@
-# SPDX-FileCopyrightText: 2023 DJDevon3
+# SPDX-FileCopyrightText: 2024 DJDevon3
 # SPDX-License-Identifier: MIT
-# Coded for Circuit Python 8.1
-# DJDevon3 ESP32-S3 OpenSkyNetwork_Private_Area_API_Example
+# Coded for Circuit Python 8.2.x
+"""OpenSky-Network.org Single Flight Private API Example"""
 
-import json
+import binascii
 import os
-import ssl
 import time
 
-import circuitpython_base64 as base64
-import socketpool
+import adafruit_connection_manager
 import wifi
 
 import adafruit_requests
 
-# OpenSky-Network.org Website Login required for this API
+# OpenSky-Network.org Login required for this API
 # REST API: https://openskynetwork.github.io/opensky-api/rest.html
+# All active flights JSON: https://opensky-network.org/api/states/all  # PICK ONE! :)
+# JSON order: transponder, callsign, country
+# ACTIVE transpondes only, for multiple "c822af&icao24=cb3993&icao24=c63923"
+TRANSPONDER = "4b1812"
 
-# Retrieves all traffic within a geographic area (Orlando example)
-latmin = "27.22"  # east bounding box
-latmax = "28.8"  # west bounding box
-lonmin = "-81.46"  # north bounding box
-lonmax = "-80.40"  # south bounding box
-
-# Initialize WiFi Pool (There can be only 1 pool & top of script)
-pool = socketpool.SocketPool(wifi.radio)
+# Get WiFi details, ensure these are setup in settings.toml
+ssid = os.getenv("CIRCUITPY_WIFI_SSID")
+password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
+osnusername = os.getenv("OSN_USERNAME")  # Website Credentials
+osnpassword = os.getenv("OSN_PASSWORD")  # Website Credentials
 
-# Time between API refreshes
+# API Polling Rate
 # 900 = 15 mins, 1800 = 30 mins, 3600 = 1 hour
 # OpenSky-Networks IP bans for too many requests, check rate limit.
 # https://openskynetwork.github.io/opensky-api/rest.html#limitations
-sleep_time = 1800
+SLEEP_TIME = 1800
 
-# Get WiFi details, ensure these are setup in settings.toml
-ssid = os.getenv("CIRCUITPY_WIFI_SSID")
-password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
-# No token required, only website login
-osnu = os.getenv("OSN_Username")
-osnp = os.getenv("OSN_Password")
-
-osn_cred = str(osnu) + ":" + str(osnp)
-bytes_to_encode = b" " + str(osn_cred) + " "
-base64_string = base64.encodebytes(bytes_to_encode)
-base64cred = repr(base64_string)[2:-1]
-
-Debug_Auth = False  # STREAMER WARNING this will show your credentials!
-if Debug_Auth:
-    osn_cred = str(osnu) + ":" + str(osnp)
-    bytes_to_encode = b" " + str(osn_cred) + " "
-    print(repr(bytes_to_encode))
-    base64_string = base64.encodebytes(bytes_to_encode)
-    print(repr(base64_string)[2:-1])
-    base64cred = repr(base64_string)[2:-1]
-    print("Decoded Bytes:", str(base64cred))
-
-# OSN requires your username:password to be base64 encoded
-# so technically it's not transmitted in the clear but w/e
-osn_header = {"Authorization": "Basic " + str(base64cred)}
-
-# Example request of all traffic over Florida, geographic areas cost less per call.
-# https://opensky-network.org/api/states/all?lamin=25.21&lomin=-84.36&lamax=30.0&lomax=-78.40
-OPENSKY_SOURCE = (
-    "https://opensky-network.org/api/states/all?"
-    + "lamin="
-    + latmin
-    + "&lomin="
-    + lonmin
-    + "&lamax="
-    + latmax
-    + "&lomax="
-    + lonmax
-)
+# Set debug to True for full JSON response.
+# WARNING: makes credentials visible
+DEBUG = False
+
+# Initalize Wifi, Socket Pool, Request Session
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
+requests = adafruit_requests.Session(pool, ssl_context)
+
+# -- Base64 Conversion --
+OSN_CREDENTIALS = str(osnusername) + ":" + str(osnpassword)
+# base64 encode and strip appended \n from bytearray
+OSN_CREDENTIALS_B = binascii.b2a_base64(OSN_CREDENTIALS.encode()).strip()
+BASE64_STRING = OSN_CREDENTIALS_B.decode()  # bytearray
+
+
+if DEBUG:
+    print("Base64 ByteArray: ", BASE64_STRING)
 
+# Requests URL - icao24 is their endpoint required for a transponder
+# example https://opensky-network.org/api/states/all?icao24=a808c5
+# OSN private: requires your website username:password to be base64 encoded
+OPENSKY_HEADER = {"Authorization": "Basic " + BASE64_STRING}
+OPENSKY_SOURCE = "https://opensky-network.org/api/states/all?" + "icao24=" + TRANSPONDER
 
-# Converts seconds to human readable minutes/hours/days
-def time_calc(input_time):  # input_time in seconds
+
+def time_calc(input_time):
+    """Converts seconds to minutes/hours/days"""
     if input_time < 60:
-        sleep_int = input_time
-        time_output = f"{sleep_int:.0f} seconds"
-    elif 60 <= input_time < 3600:
-        sleep_int = input_time / 60
-        time_output = f"{sleep_int:.0f} minutes"
-    elif 3600 <= input_time < 86400:
-        sleep_int = input_time / 60 / 60
-        time_output = f"{sleep_int:.1f} hours"
-    else:
-        sleep_int = input_time / 60 / 60 / 24
-        time_output = f"{sleep_int:.1f} days"
-    return time_output
+        return f"{input_time:.0f} seconds"
+    if input_time < 3600:
+        return f"{input_time / 60:.0f} minutes"
+    if input_time < 86400:
+        return f"{input_time / 60 / 60:.0f} hours"
+    return f"{input_time / 60 / 60 / 24:.1f} days"
 
 
 def _format_datetime(datetime):
-    return "{:02}/{:02}/{} {:02}:{:02}:{:02}".format(
-        datetime.tm_mon,
-        datetime.tm_mday,
-        datetime.tm_year,
-        datetime.tm_hour,
-        datetime.tm_min,
-        datetime.tm_sec,
+    return (
+        f"{datetime.tm_mon:02}/"
+        + f"{datetime.tm_mday:02}/"
+        + f"{datetime.tm_year:02} "
+        + f"{datetime.tm_hour:02}:"
+        + f"{datetime.tm_min:02}:"
+        + f"{datetime.tm_sec:02}"
     )
 
 
-# Connect to Wi-Fi
-print("\n===============================")
-print("Connecting to WiFi...")
-request = adafruit_requests.Session(pool, ssl.create_default_context())
-while not wifi.radio.ipv4_address:
-    try:
-        wifi.radio.connect(ssid, password)
-    except ConnectionError as e:
-        print("Connection Error:", e)
-        print("Retrying in 10 seconds")
-    time.sleep(10)
-print("Connected!\n")
-
 while True:
-    # STREAMER WARNING this will show your credentials!
-    debug_request = False  # Set True to see full request
-    if debug_request:
-        print("Full API HEADER: ", str(osn_header))
-        print("Full API GET URL: ", OPENSKY_SOURCE)
-        print("===============================")
-
-    print("\nAttempting to GET OpenSky-Network Data!")
-    opensky_response = request.get(url=OPENSKY_SOURCE, headers=osn_header).json()
-
-    # Print Full JSON to Serial (doesn't show credentials)
-    debug_response = False  # Set True to see full response
-    if debug_response:
-        dump_object = json.dumps(opensky_response)
-        print("JSON Dump: ", dump_object)
-
-    # Key:Value Serial Debug (doesn't show credentials)
-    osn_debug_keys = True  # Set True to print Serial data
-    if osn_debug_keys:
+    # Connect to Wi-Fi
+    print("\nConnecting to WiFi...")
+    while not wifi.radio.ipv4_address:
         try:
-            osn_flight = opensky_response["time"]
-            print("Current Unix Time: ", osn_flight)
+            wifi.radio.connect(ssid, password)
+        except ConnectionError as e:
+            print("❌ Connection Error:", e)
+            print("Retrying in 10 seconds")
+    print("✅ Wifi!")
 
-            current_struct_time = time.localtime(osn_flight)
-            current_date = "{}".format(_format_datetime(current_struct_time))
-            print(f"Unix to Readable Time: {current_date}")
-
-            # Current flight data for single callsign (right now)
-            osn_all_flights = opensky_response["states"]
-
-            if osn_all_flights is not None:
-                # print("Flight Data: ", osn_all_flights)
-                for flights in osn_all_flights:
-                    osn_t = f"Trans:{flights[0]} "
-                    osn_c = f"Sign:{flights[1]} "
-                    osn_o = f"Origin:{flights[2]} "
-                    osn_tm = f"Time:{flights[3]} "
-                    osn_l = f"Last:{flights[4]} "
-                    osn_lo = f"Lon:{flights[5]} "
-                    osn_la = f"Lat:{flights[6]} "
-                    osn_ba = f"BaroAlt:{flights[7]} "
-                    osn_g = f"Ground:{flights[8]} "
-                    osn_v = f"Vel:{flights[9]} "
-                    osn_h = f"Head:{flights[10]} "
-                    osn_vr = f"VertRate:{flights[11]} "
-                    osn_s = f"Sens:{flights[12]} "
-                    osn_ga = f"GeoAlt:{flights[13]} "
-                    osn_sq = f"Squawk:{flights[14]} "
-                    osn_pr = f"Task:{flights[15]} "
-                    osn_ps = f"PosSys:{flights[16]} "
-                    osn_ca = f"Cat:{flights[16]} "
-                    # This is just because pylint complains about long lines
-                    string1 = f"{osn_t}{osn_c}{osn_o}{osn_tm}{osn_l}{osn_lo}"
-                    string2 = f"{osn_la}{osn_ba}{osn_g}{osn_v}{osn_h}{osn_vr}"
-                    string3 = f"{osn_s}{osn_ga}{osn_sq}{osn_pr}{osn_ps}{osn_ca}"
-                    print(f"{string1}{string2}{string3}")
+    try:
+        print(" | Attempting to GET OpenSky-Network Single Private Flight JSON!")
+        print(" | Website Credentials Required! Allows more daily calls than Public.")
+        try:
+            opensky_response = requests.get(url=OPENSKY_SOURCE, headers=OPENSKY_HEADER)
+            opensky_json = opensky_response.json()
+        except ConnectionError as e:
+            print("Connection Error:", e)
+            print("Retrying in 10 seconds")
+
+        print(" | ✅ OpenSky-Network JSON!")
+
+        if DEBUG:
+            print("Full API GET URL: ", OPENSKY_SOURCE)
+            print("Full API GET Header: ", OPENSKY_HEADER)
+            print(opensky_json)
+
+        # ERROR MESSAGE RESPONSES
+        if "timestamp" in opensky_json:
+            osn_timestamp = opensky_json["timestamp"]
+            print(f"❌ Timestamp: {osn_timestamp}")
+
+        if "message" in opensky_json:
+            osn_message = opensky_json["message"]
+            print(f"❌ Message: {osn_message}")
+
+        if "error" in opensky_json:
+            osn_error = opensky_json["error"]
+            print(f"❌ Error: {osn_error}")
+
+        if "path" in opensky_json:
+            osn_path = opensky_json["path"]
+            print(f"❌ Path: {osn_path}")
+
+        if "status" in opensky_json:
+            osn_status = opensky_json["status"]
+            print(f"❌ Status: {osn_status}")
+
+        # Current flight data for single callsign (right now)
+        osn_single_flight_data = opensky_json["states"]
+
+        if osn_single_flight_data is not None:
+            if DEBUG:
+                print(f" |  | Single Private Flight Data: {osn_single_flight_data}")
+
+            last_contact = opensky_json["states"][0][4]
+            # print(f" |  | Last Contact Unix Time: {last_contact}")
+            lc_struct_time = time.localtime(last_contact)
+            lc_readable_time = f"{_format_datetime(lc_struct_time)}"
+            print(f" |  | Last Contact: {lc_readable_time}")
+
+            flight_transponder = opensky_json["states"][0][0]
+            print(f" |  | Transponder: {flight_transponder}")
+
+            callsign = opensky_json["states"][0][1]
+            print(f" |  | Callsign: {callsign}")
+
+            squawk = opensky_json["states"][0][14]
+            print(f" |  | Squawk: {squawk}")
+
+            country = opensky_json["states"][0][2]
+            print(f" |  | Origin: {country}")
+
+            longitude = opensky_json["states"][0][5]
+            print(f" |  | Longitude: {longitude}")
+
+            latitude = opensky_json["states"][0][6]
+            print(f" |  | Latitude: {latitude}")
+
+            # Return Air Flight data if not on ground
+            on_ground = opensky_json["states"][0][8]
+            if on_ground is True:
+                print(f" |  | On Ground: {on_ground}")
             else:
-                print("Flight has no active data or you're polling too fast.")
+                altitude = opensky_json["states"][0][7]
+                print(f" |  | Barometric Altitude: {altitude}")
+
+                velocity = opensky_json["states"][0][9]
+                if velocity != "null":
+                    print(f" |  | Velocity: {velocity}")
+
+                vertical_rate = opensky_json["states"][0][11]
+                if vertical_rate != "null":
+                    print(f" |  | Vertical Rate: {vertical_rate}")
+
+        else:
+            print(" |  | ❌ Flight has no active data or you're polling too fast.")
+
+        opensky_response.close()
+        print("✂️ Disconnected from OpenSky-Network API")
+
+        print("\nFinished!")
+        print(f"Board Uptime: {time_calc(time.monotonic())}")
+        print(f"Next Update: {time_calc(SLEEP_TIME)}")
+        print("===============================")
 
-            print("\nFinished!")
-            print("Board Uptime: ", time_calc(time.monotonic()))
-            print("Next Update: ", time_calc(sleep_time))
-            time.sleep(sleep_time)
-            print("===============================")
-
-        except (ConnectionError, ValueError, NameError) as e:
-            print("OSN Connection Error:", e)
-            print("Next Retry: ", time_calc(sleep_time))
-            time.sleep(sleep_time)
+    except (ValueError, RuntimeError) as e:
+        print(f"Failed to get data, retrying\n {e}")
+        time.sleep(60)
+        break
+    time.sleep(SLEEP_TIME)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_premiereleague.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_premiereleague.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_rocketlaunch_live.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_steam.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_steam.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_twitch.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_twitch.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_api_youtube.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_api_youtube.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/expanded/requests_wifi_multiple_cookies.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/expanded/requests_wifi_multiple_cookies.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # SPDX-FileCopyrightText: 2022 Alec Delaney
 # SPDX-License-Identifier: MIT
-
-"""
-This example was written for the MagTag; changes may be needed
-for connecting to the internet depending on your device.
-"""
+# Coded for Circuit Python 9.0
+""" Multiple Cookies Example written for MagTag """
 
 import os
-import ssl
 
-import socketpool
+import adafruit_connection_manager
 import wifi
 
 import adafruit_requests
 
-COOKIE_TEST_URL = "https://www.adafruit.com"
-
 # Get WiFi details, ensure these are setup in settings.toml
 ssid = os.getenv("CIRCUITPY_WIFI_SSID")
 password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
 
-# Connect to the Wi-Fi network
-print("Connecting to %s" % ssid)
-wifi.radio.connect(ssid, password)
-
-# Set up the requests library
-pool = socketpool.SocketPool(wifi.radio)
-requests = adafruit_requests.Session(pool, ssl.create_default_context())
-
-# GET from the URL
-print("Fetching multiple cookies from", COOKIE_TEST_URL)
-response = requests.get(COOKIE_TEST_URL)
+COOKIE_TEST_URL = "https://www.adafruit.com"
+
+# Initalize Wifi, Socket Pool, Request Session
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
+requests = adafruit_requests.Session(pool, ssl_context)
+
+print(f"\nConnecting to {ssid}...")
+try:
+    # Connect to the Wi-Fi network
+    wifi.radio.connect(ssid, password)
+    # URL GET Request
+    response = requests.get(COOKIE_TEST_URL)
+except OSError as e:
+    print(f"❌ OSError: {e}")
+print("✅ Wifi!")
+
+print(f" | Fetching Cookies: {COOKIE_TEST_URL}")
 
 # Spilt up the cookies by ", "
 elements = response.headers["set-cookie"].split(", ")
 
 # NOTE: Some cookies use ", " when describing dates.  This code will iterate through
 # the previously split up 'set-cookie' header value and piece back together cookies
 # that were accidentally split up for this reason
@@ -45,14 +46,17 @@
     captured_day = [day for day in days_of_week if element.endswith(day)]
     if captured_day:
         cookie_list.append(element + ", " + next(elements_iter))
     else:
         cookie_list.append(element)
 
 # Pring the information about the cookies
-print("Number of cookies:", len(cookie_list))
-print("")
-print("Cookies received:")
-print("-" * 40)
+print(f" | Total Cookies: {len(cookie_list)}")
+print("-" * 80)
+
 for cookie in cookie_list:
-    print(cookie)
-    print("-" * 40)
+    print(f" | 🍪 {cookie}")
+    print("-" * 80)
+
+response.close()
+print(f"✂️ Disconnected from {COOKIE_TEST_URL}")
+print("Finished!")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/requests_wifi_advanced.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/requests_wifi_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wifi/requests_wifi_simpletest.py` & `adafruit-circuitpython-requests-3.2.4/examples/wiznet5k/requests_wiznet5k_simpletest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,32 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
-import os
-import ssl
-
-import socketpool
-import wifi
+import adafruit_connection_manager
+import board
+import busio
+from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
+from digitalio import DigitalInOut
 
 import adafruit_requests
 
-# Get WiFi details, ensure these are setup in settings.toml
-ssid = os.getenv("CIRCUITPY_WIFI_SSID")
-password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
-
-# Initialize WiFi Pool (There can be only 1 pool & top of script)
-radio = wifi.radio
-pool = socketpool.SocketPool(radio)
-
-print("Connecting to AP...")
-while not wifi.radio.ipv4_address:
-    try:
-        wifi.radio.connect(ssid, password)
-    except ConnectionError as e:
-        print("could not connect to AP, retrying: ", e)
-print("Connected to", str(radio.ap_info.ssid, "utf-8"), "\tRSSI:", radio.ap_info.rssi)
+cs = DigitalInOut(board.D10)
+spi_bus = busio.SPI(board.SCK, MOSI=board.MOSI, MISO=board.MISO)
+
+# Initialize ethernet interface with DHCP
+radio = WIZNET5K(spi_bus, cs)
 
 # Initialize a requests session
-ssl_context = ssl.create_default_context()
+pool = adafruit_connection_manager.get_radio_socketpool(radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(radio)
 requests = adafruit_requests.Session(pool, ssl_context)
 
 TEXT_URL = "http://wifitest.adafruit.com/testwifi/index.html"
-JSON_GET_URL = "https://httpbin.org/get"
-JSON_POST_URL = "https://httpbin.org/post"
+JSON_GET_URL = "http://httpbin.org/get"
+JSON_POST_URL = "http://httpbin.org/post"
 
 print("Fetching text from %s" % TEXT_URL)
 response = requests.get(TEXT_URL)
 print("-" * 40)
 
 print("Text Response: ", response.text)
 print("-" * 40)
```

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wiznet5k/requests_wiznet5k_advanced.py` & `adafruit-circuitpython-requests-3.2.4/examples/wiznet5k/requests_wiznet5k_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/examples/wiznet5k/requests_wiznet5k_simpletest.py` & `adafruit-circuitpython-requests-3.2.4/examples/wifi/requests_wifi_simpletest.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,70 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
+# Updated for Circuit Python 9.0
+""" WiFi Simpletest """
+
+import os
 
 import adafruit_connection_manager
-import board
-import busio
-from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
-from digitalio import DigitalInOut
+import wifi
 
 import adafruit_requests
 
-cs = DigitalInOut(board.D10)
-spi_bus = busio.SPI(board.SCK, MOSI=board.MOSI, MISO=board.MISO)
+# Get WiFi details, ensure these are setup in settings.toml
+ssid = os.getenv("CIRCUITPY_WIFI_SSID")
+password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
 
-# Initialize ethernet interface with DHCP
-radio = WIZNET5K(spi_bus, cs)
+TEXT_URL = "http://wifitest.adafruit.com/testwifi/index.html"
+JSON_GET_URL = "https://httpbin.org/get"
+JSON_POST_URL = "https://httpbin.org/post"
 
-# Initialize a requests session
-pool = adafruit_connection_manager.get_radio_socketpool(radio)
-ssl_context = adafruit_connection_manager.get_radio_ssl_context(radio)
+# Initalize Wifi, Socket Pool, Request Session
+pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
+ssl_context = adafruit_connection_manager.get_radio_ssl_context(wifi.radio)
 requests = adafruit_requests.Session(pool, ssl_context)
+rssi = wifi.radio.ap_info.rssi
 
-TEXT_URL = "http://wifitest.adafruit.com/testwifi/index.html"
-JSON_GET_URL = "http://httpbin.org/get"
-JSON_POST_URL = "http://httpbin.org/post"
+print(f"\nConnecting to {ssid}...")
+print(f"Signal Strength: {rssi}")
+try:
+    # Connect to the Wi-Fi network
+    wifi.radio.connect(ssid, password)
+except OSError as e:
+    print(f"❌ OSError: {e}")
+print("✅ Wifi!")
 
-print("Fetching text from %s" % TEXT_URL)
+print(f" | GET Text Test: {TEXT_URL}")
 response = requests.get(TEXT_URL)
-print("-" * 40)
-
-print("Text Response: ", response.text)
-print("-" * 40)
+print(f" | ✅ GET Response: {response.text}")
 response.close()
+print(f" | ✂️ Disconnected from {TEXT_URL}")
+print("-" * 80)
 
-print("Fetching JSON data from %s" % JSON_GET_URL)
+print(f" | GET Full Response Test: {JSON_GET_URL}")
 response = requests.get(JSON_GET_URL)
-print("-" * 40)
-
-print("JSON Response: ", response.json())
-print("-" * 40)
+print(f" | ✅ Unparsed Full JSON Response: {response.json()}")
 response.close()
+print(f" | ✂️ Disconnected from {JSON_GET_URL}")
+print("-" * 80)
 
-data = "31F"
-print("POSTing data to {0}: {1}".format(JSON_POST_URL, data))
-response = requests.post(JSON_POST_URL, data=data)
-print("-" * 40)
-
+DATA = "This is an example of a JSON value"
+print(f" | ✅ JSON 'value' POST Test: {JSON_POST_URL} {DATA}")
+response = requests.post(JSON_POST_URL, data=DATA)
 json_resp = response.json()
 # Parse out the 'data' key from json_resp dict.
-print("Data received from server:", json_resp["data"])
-print("-" * 40)
+print(f" | ✅ JSON 'value' Response: {json_resp['data']}")
 response.close()
+print(f" | ✂️ Disconnected from {JSON_POST_URL}")
+print("-" * 80)
 
-json_data = {"Date": "July 25, 2019"}
-print("POSTing data to {0}: {1}".format(JSON_POST_URL, json_data))
+json_data = {"Date": "January 1, 1970"}
+print(f" | ✅ JSON 'key':'value' POST Test: {JSON_POST_URL} {json_data}")
 response = requests.post(JSON_POST_URL, json=json_data)
-print("-" * 40)
-
 json_resp = response.json()
 # Parse out the 'json' key from json_resp dict.
-print("JSON Data received from server:", json_resp["json"])
-print("-" * 40)
+print(f" | ✅ JSON 'key':'value' Response: {json_resp['json']}")
 response.close()
+print(f" | ✂️ Disconnected from {JSON_POST_URL}")
+print("-" * 80)
+
+print("Finished!")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-requests-3.2.3/pyproject.toml` & `adafruit-circuitpython-requests-3.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-requests"
 description = "A requests-like library for web interfacing"
-version = "3.2.3"
+version = "3.2.4"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Requests"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-requests-3.2.3/tests/chunk_test.py` & `adafruit-circuitpython-requests-3.2.4/tests/chunk_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/tests/chunked_redirect_test.py` & `adafruit-circuitpython-requests-3.2.4/tests/chunked_redirect_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/tests/concurrent_test.py` & `adafruit-circuitpython-requests-3.2.4/tests/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/tests/conftest.py` & `adafruit-circuitpython-requests-3.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/tests/header_test.py` & `adafruit-circuitpython-requests-3.2.4/tests/header_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/tests/method_test.py` & `adafruit-circuitpython-requests-3.2.4/tests/method_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/tests/mocket.py` & `adafruit-circuitpython-requests-3.2.4/tests/mocket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/tests/parse_test.py` & `adafruit-circuitpython-requests-3.2.4/tests/parse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/tests/protocol_test.py` & `adafruit-circuitpython-requests-3.2.4/tests/protocol_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/tests/reuse_test.py` & `adafruit-circuitpython-requests-3.2.4/tests/reuse_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-3.2.3/tox.ini` & `adafruit-circuitpython-requests-3.2.4/tox.ini`

 * *Files identical despite different names*

