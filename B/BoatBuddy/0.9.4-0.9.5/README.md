# Comparing `tmp/boatbuddy-0.9.4.tar.gz` & `tmp/boatbuddy-0.9.5.tar.gz`

## Comparing `boatbuddy-0.9.4.tar` & `boatbuddy-0.9.5.tar`

### file list

```diff
@@ -1,2169 +1,2168 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/.DS_Store
--rw-r--r--   0        0        0    21502 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/CHANGELOG.md
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/change-log-builder.sh
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/requirements.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/.idea/BoatBuddy.iml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/.idea/misc.xml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/__init__.py
--rw-r--r--   0        0        0    13672 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/__main__.py
--rw-r--r--   0        0        0    12097 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/anchor_manager.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/clock_plugin.py
--rw-r--r--   0        0        0    17162 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/console_manager.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/database_manager.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/email_manager.py
--rw-r--r--   0        0        0    25830 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/flask_manager.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/generic_plugin.py
--rw-r--r--   0        0        0     7911 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/globals.py
--rw-r--r--   0        0        0    16087 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/gps_plugin.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/log_manager.py
--rw-r--r--   0        0        0    17339 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/mysql_wrapper.py
--rw-r--r--   0        0        0    23602 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/nmea_plugin.py
--rw-r--r--   0        0        0    27253 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/notifications_manager.py
--rw-r--r--   0        0        0    21434 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/plugin_manager.py
--rw-r--r--   0        0        0    16001 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/sample-config.json
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/sound_manager.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/telegram_manager.py
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/utils.py
--rw-r--r--   0        0        0    31209 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/victron_plugin.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/resources/.DS_Store
--rw-r--r--   0        0        0   132000 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/resources/alarm.mp3
--rw-r--r--   0        0        0    25984 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/resources/application_started.mp3
--rw-r--r--   0        0        0    20506 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/resources/session_ended.wav
--rw-r--r--   0        0        0   123715 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/resources/session_started.mp3
--rw-r--r--   0        0        0    61022 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/resources/warning.mp3
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/.DS_Store
--rw-r--r--   0        0        0    14417 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/CustomGaugeMeter.js
--rw-r--r--   0        0        0    13910 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/GaugeMeter.js
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/favicon.ico
--rw-r--r--   0        0        0    44733 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/gauge.min.js
--rw-r--r--   0        0        0    87532 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/jquery-3.7.1.min.js
--rw-r--r--   0        0        0   134767 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/jquery-3.7.1.min.map
--rw-r--r--   0        0        0    66082 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/logo.png
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/main.css
--rw-r--r--   0        0        0    20121 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/popper.min.js
--rw-r--r--   0        0        0   110046 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/popper.min.js.map
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/.DS_Store
--rw-r--r--   0        0        0    70329 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203178 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51795 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115987 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70403 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203182 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51870 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116064 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129327 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10126 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51369 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129342 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63943 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107823 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267491 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85352 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180381 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107691 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267432 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85281 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180217 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   280813 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   679011 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.css.map
--rw-r--r--   0        0        0   232948 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   589161 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280392 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   678856 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   233055 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   588695 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   207731 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444286 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80663 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   331886 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135747 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305152 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    74154 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222462 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145313 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0   306320 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.js.map
--rw-r--r--   0        0        0    60577 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   220350 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/.DS_Store
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/0-circle-fill.svg
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/0-circle.svg
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/0-square-fill.svg
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/0-square.svg
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/1-circle-fill.svg
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/1-circle.svg
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/1-square-fill.svg
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/1-square.svg
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/123.svg
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/2-circle-fill.svg
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/2-circle.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/2-square-fill.svg
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/2-square.svg
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/3-circle-fill.svg
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/3-circle.svg
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/3-square-fill.svg
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/3-square.svg
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/4-circle-fill.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/4-circle.svg
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/4-square-fill.svg
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/4-square.svg
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/5-circle-fill.svg
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/5-circle.svg
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/5-square-fill.svg
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/5-square.svg
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/6-circle-fill.svg
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/6-circle.svg
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/6-square-fill.svg
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/6-square.svg
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/7-circle-fill.svg
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/7-circle.svg
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/7-square-fill.svg
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/7-square.svg
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/8-circle-fill.svg
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/8-circle.svg
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/8-square-fill.svg
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/8-square.svg
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/9-circle-fill.svg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/9-circle.svg
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/9-square-fill.svg
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/9-square.svg
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/activity.svg
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/airplane-engines-fill.svg
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/airplane-engines.svg
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/airplane-fill.svg
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/airplane.svg
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/alarm-fill.svg
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/alarm.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/alexa.svg
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/align-bottom.svg
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/align-center.svg
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/align-end.svg
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/align-middle.svg
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/align-start.svg
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/align-top.svg
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/alipay.svg
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/alphabet-uppercase.svg
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/alphabet.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/alt.svg
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/amazon.svg
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/amd.svg
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/android.svg
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/android2.svg
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/app-indicator.svg
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/app.svg
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/apple.svg
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/archive-fill.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/archive.svg
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-90deg-down.svg
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-90deg-left.svg
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-90deg-right.svg
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-90deg-up.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-bar-down.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-bar-left.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-bar-right.svg
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-bar-up.svg
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-clockwise.svg
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-counterclockwise.svg
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-circle-fill.svg
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-circle.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-left-circle-fill.svg
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-left-circle.svg
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-left-square-fill.svg
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-left-square.svg
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-left.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-right-circle-fill.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-right-circle.svg
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-right-square-fill.svg
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-right-square.svg
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-right.svg
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-short.svg
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-square-fill.svg
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-square.svg
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down-up.svg
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-down.svg
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-left-circle-fill.svg
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-left-circle.svg
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-left-right.svg
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-left-short.svg
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-left-square-fill.svg
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-left-square.svg
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-left.svg
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-repeat.svg
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-return-left.svg
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-return-right.svg
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-right-circle-fill.svg
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-right-circle.svg
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-right-short.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-right-square-fill.svg
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-right-square.svg
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-right.svg
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-through-heart-fill.svg
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-through-heart.svg
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-circle-fill.svg
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-circle.svg
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-left-circle-fill.svg
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-left-circle.svg
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-left-square-fill.svg
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-left-square.svg
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-left.svg
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-right-circle-fill.svg
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-right-circle.svg
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-right-square-fill.svg
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-right-square.svg
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-right.svg
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-short.svg
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-square-fill.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up-square.svg
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-up.svg
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrows-angle-contract.svg
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrows-angle-expand.svg
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrows-collapse-vertical.svg
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrows-collapse.svg
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrows-expand-vertical.svg
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrows-expand.svg
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrows-fullscreen.svg
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrows-move.svg
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrows-vertical.svg
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrows.svg
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/aspect-ratio-fill.svg
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/aspect-ratio.svg
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/asterisk.svg
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/at.svg
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/award-fill.svg
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/award.svg
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/back.svg
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack-fill.svg
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack.svg
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack2-fill.svg
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack2.svg
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack3-fill.svg
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack3.svg
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack4-fill.svg
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack4.svg
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backspace-fill.svg
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backspace-reverse-fill.svg
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backspace-reverse.svg
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backspace.svg
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-3d-fill.svg
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-3d.svg
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-4k-fill.svg
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-4k.svg
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-8k-fill.svg
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-8k.svg
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-ad-fill.svg
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-ad.svg
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-ar-fill.svg
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-ar.svg
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-cc-fill.svg
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-cc.svg
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-hd-fill.svg
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-hd.svg
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-sd-fill.svg
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-sd.svg
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-tm-fill.svg
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-tm.svg
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-vo-fill.svg
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-vo.svg
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-vr-fill.svg
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-vr.svg
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-wc-fill.svg
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-wc.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag-check-fill.svg
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag-check.svg
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag-dash-fill.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag-dash.svg
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag-fill.svg
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag-heart-fill.svg
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag-heart.svg
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag-plus-fill.svg
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag-plus.svg
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag-x-fill.svg
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag-x.svg
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag.svg
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/balloon-fill.svg
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/balloon-heart-fill.svg
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/balloon-heart.svg
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/balloon.svg
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ban-fill.svg
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ban.svg
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bandaid-fill.svg
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bandaid.svg
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bank.svg
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bank2.svg
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bar-chart-fill.svg
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bar-chart-line-fill.svg
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bar-chart-line.svg
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bar-chart-steps.svg
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bar-chart.svg
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/basket-fill.svg
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/basket.svg
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/basket2-fill.svg
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/basket2.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/basket3-fill.svg
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/basket3.svg
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/battery-charging.svg
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/battery-full.svg
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/battery-half.svg
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/battery.svg
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/behance.svg
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bell-fill.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bell-slash-fill.svg
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bell-slash.svg
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bell.svg
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bezier.svg
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bezier2.svg
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bicycle.svg
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bing.svg
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/binoculars-fill.svg
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/binoculars.svg
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/blockquote-left.svg
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/blockquote-right.svg
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bluetooth.svg
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/body-text.svg
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/book-fill.svg
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/book-half.svg
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/book.svg
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-check-fill.svg
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-check.svg
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-dash-fill.svg
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-dash.svg
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-fill.svg
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-heart-fill.svg
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-heart.svg
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-plus-fill.svg
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-plus.svg
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-star-fill.svg
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-star.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-x-fill.svg
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-x.svg
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark.svg
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmarks-fill.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmarks.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookshelf.svg
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/boombox-fill.svg
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/boombox.svg
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-fill.svg
--rw-r--r--   0        0        0    98255 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-icons.css
--rw-r--r--   0        0        0    52358 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-icons.json
--rw-r--r--   0        0        0    85875 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-icons.min.css
--rw-r--r--   0        0        0    57755 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-icons.scss
--rw-r--r--   0        0        0  1149049 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-icons.svg
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-reboot.svg
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap.svg
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-all.svg
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-bottom.svg
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-center.svg
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-inner.svg
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-left.svg
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-middle.svg
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-outer.svg
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-right.svg
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-style.svg
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-top.svg
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-width.svg
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border.svg
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bounding-box-circles.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bounding-box.svg
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-down-left.svg
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-down-right.svg
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-down.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-down-left.svg
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-down-right.svg
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-down.svg
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-left.svg
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-right.svg
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-up-left.svg
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-up-right.svg
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-up.svg
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-left.svg
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-right.svg
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-up-left.svg
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-up-right.svg
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-up.svg
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-fill.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-seam-fill.svg
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-seam.svg
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box.svg
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box2-fill.svg
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box2-heart-fill.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box2-heart.svg
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box2.svg
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/boxes.svg
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/braces-asterisk.svg
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/braces.svg
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bricks.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/briefcase-fill.svg
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/briefcase.svg
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-alt-high-fill.svg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-alt-high.svg
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-alt-low-fill.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-alt-low.svg
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-high-fill.svg
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-high.svg
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-low-fill.svg
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-low.svg
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brilliance.svg
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/broadcast-pin.svg
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/broadcast.svg
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/browser-chrome.svg
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/browser-edge.svg
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/browser-firefox.svg
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/browser-safari.svg
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brush-fill.svg
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brush.svg
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bucket-fill.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bucket.svg
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bug-fill.svg
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bug.svg
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-add.svg
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-check.svg
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-dash.svg
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-down.svg
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-exclamation.svg
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-add.svg
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-check.svg
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-dash.svg
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-down.svg
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-exclamation.svg
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-gear.svg
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-lock.svg
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-slash.svg
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-up.svg
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-x.svg
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill.svg
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-gear.svg
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-lock.svg
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-slash.svg
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-up.svg
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-x.svg
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building.svg
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/buildings-fill.svg
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/buildings.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bullseye.svg
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bus-front-fill.svg
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bus-front.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/c-circle-fill.svg
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/c-circle.svg
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/c-square-fill.svg
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/c-square.svg
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cake-fill.svg
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cake.svg
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cake2-fill.svg
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cake2.svg
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calculator-fill.svg
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calculator.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-check-fill.svg
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-check.svg
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-date-fill.svg
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-date.svg
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-day-fill.svg
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-day.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-event-fill.svg
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-event.svg
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-fill.svg
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-heart-fill.svg
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-heart.svg
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-minus-fill.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-minus.svg
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-month-fill.svg
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-month.svg
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-plus-fill.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-plus.svg
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-range-fill.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-range.svg
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-week-fill.svg
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-week.svg
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-x-fill.svg
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-x.svg
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar.svg
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-check-fill.svg
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-check.svg
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-date-fill.svg
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-date.svg
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-day-fill.svg
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-day.svg
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-event-fill.svg
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-event.svg
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-fill.svg
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-heart-fill.svg
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-heart.svg
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-minus-fill.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-minus.svg
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-month-fill.svg
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-month.svg
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-plus-fill.svg
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-plus.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-range-fill.svg
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-range.svg
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-week-fill.svg
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-week.svg
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-x-fill.svg
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-x.svg
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2.svg
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar3-event-fill.svg
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar3-event.svg
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar3-fill.svg
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar3-range-fill.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar3-range.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar3-week-fill.svg
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar3-week.svg
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar3.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar4-event.svg
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar4-range.svg
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar4-week.svg
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar4.svg
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera-fill.svg
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera-reels-fill.svg
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera-reels.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera-video-fill.svg
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera-video-off-fill.svg
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera-video-off.svg
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera-video.svg
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera.svg
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera2.svg
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/capslock-fill.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/capslock.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/capsule-pill.svg
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/capsule.svg
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/car-front-fill.svg
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/car-front.svg
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/card-checklist.svg
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/card-heading.svg
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/card-image.svg
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/card-list.svg
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/card-text.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-down-fill.svg
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-down-square-fill.svg
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-down-square.svg
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-down.svg
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-left-fill.svg
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-left-square-fill.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-left-square.svg
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-left.svg
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-right-fill.svg
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-right-square-fill.svg
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-right-square.svg
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-right.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-up-fill.svg
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-up-square-fill.svg
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-up-square.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/caret-up.svg
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-check-fill.svg
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-check.svg
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-dash-fill.svg
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-dash.svg
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-fill.svg
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-plus-fill.svg
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-plus.svg
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-x-fill.svg
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-x.svg
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart.svg
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart2.svg
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart3.svg
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart4.svg
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cash-coin.svg
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cash-stack.svg
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cash.svg
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cassette-fill.svg
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cassette.svg
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cast.svg
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cc-circle-fill.svg
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cc-circle.svg
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cc-square-fill.svg
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cc-square.svg
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-dots-fill.svg
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-dots.svg
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-fill.svg
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-heart-fill.svg
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-heart.svg
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left-dots-fill.svg
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left-dots.svg
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left-fill.svg
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left-heart-fill.svg
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left-heart.svg
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left-quote-fill.svg
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left-quote.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left-text-fill.svg
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left-text.svg
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left.svg
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-quote-fill.svg
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-quote.svg
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right-dots-fill.svg
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right-dots.svg
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right-fill.svg
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right-heart-fill.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right-heart.svg
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right-quote-fill.svg
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right-quote.svg
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right-text-fill.svg
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right-text.svg
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right.svg
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-dots-fill.svg
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-dots.svg
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-fill.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-heart-fill.svg
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-heart.svg
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-quote-fill.svg
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-quote.svg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-text-fill.svg
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-text.svg
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-text-fill.svg
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-text.svg
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat.svg
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/check-all.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/check-circle-fill.svg
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/check-circle.svg
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/check-lg.svg
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/check-square-fill.svg
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/check-square.svg
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/check.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/check2-all.svg
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/check2-circle.svg
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/check2-square.svg
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/check2.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-bar-contract.svg
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-bar-down.svg
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-bar-expand.svg
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-bar-left.svg
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-bar-right.svg
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-bar-up.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-compact-down.svg
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-compact-left.svg
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-compact-right.svg
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-compact-up.svg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-contract.svg
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-double-down.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-double-left.svg
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-double-right.svg
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-double-up.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-down.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-expand.svg
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-left.svg
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-right.svg
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chevron-up.svg
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/circle-fill.svg
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/circle-half.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/circle-square.svg
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/circle.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-check-fill.svg
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-check.svg
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-data-fill.svg
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-data.svg
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-fill.svg
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-heart-fill.svg
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-heart.svg
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-minus-fill.svg
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-minus.svg
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-plus-fill.svg
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-plus.svg
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-pulse.svg
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-x-fill.svg
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-x.svg
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard.svg
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-check-fill.svg
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-check.svg
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-data-fill.svg
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-data.svg
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-fill.svg
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-heart-fill.svg
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-heart.svg
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-minus-fill.svg
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-minus.svg
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-plus-fill.svg
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-plus.svg
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-pulse-fill.svg
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-pulse.svg
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-x-fill.svg
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-x.svg
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2.svg
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clock-fill.svg
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clock-history.svg
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clock.svg
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-arrow-down-fill.svg
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-arrow-down.svg
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-arrow-up-fill.svg
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-arrow-up.svg
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-check-fill.svg
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-check.svg
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-download-fill.svg
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-download.svg
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-drizzle-fill.svg
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-drizzle.svg
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-fill.svg
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-fog-fill.svg
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-fog.svg
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-fog2-fill.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-fog2.svg
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-hail-fill.svg
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-hail.svg
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-haze-fill.svg
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-haze.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-haze2-fill.svg
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-haze2.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-lightning-fill.svg
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-lightning-rain-fill.svg
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-lightning-rain.svg
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-lightning.svg
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-minus-fill.svg
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-minus.svg
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-moon-fill.svg
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-moon.svg
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-plus-fill.svg
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-plus.svg
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-rain-fill.svg
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-rain-heavy-fill.svg
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-rain-heavy.svg
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-rain.svg
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-slash-fill.svg
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-slash.svg
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-sleet-fill.svg
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-sleet.svg
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-snow-fill.svg
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-snow.svg
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-sun-fill.svg
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-sun.svg
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-upload-fill.svg
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-upload.svg
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud.svg
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clouds-fill.svg
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clouds.svg
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloudy-fill.svg
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloudy.svg
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/code-slash.svg
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/code-square.svg
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/code.svg
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/coin.svg
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/collection-fill.svg
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/collection-play-fill.svg
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/collection-play.svg
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/collection.svg
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/columns-gap.svg
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/columns.svg
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/command.svg
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/compass-fill.svg
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/compass.svg
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cone-striped.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cone.svg
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/controller.svg
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cookie.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/copy.svg
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cpu-fill.svg
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cpu.svg
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/credit-card-2-back-fill.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/credit-card-2-back.svg
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/credit-card-2-front-fill.svg
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/credit-card-2-front.svg
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/credit-card-fill.svg
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/credit-card.svg
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/crop.svg
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/crosshair.svg
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/crosshair2.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cup-fill.svg
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cup-hot-fill.svg
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cup-hot.svg
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cup-straw.svg
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cup.svg
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/currency-bitcoin.svg
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/currency-dollar.svg
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/currency-euro.svg
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/currency-exchange.svg
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/currency-pound.svg
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/currency-rupee.svg
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/currency-yen.svg
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cursor-fill.svg
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cursor-text.svg
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cursor.svg
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dash-circle-dotted.svg
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dash-circle-fill.svg
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dash-circle.svg
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dash-lg.svg
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dash-square-dotted.svg
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dash-square-fill.svg
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dash-square.svg
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dash.svg
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-add.svg
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-check.svg
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-dash.svg
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-down.svg
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-exclamation.svg
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-add.svg
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-check.svg
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-dash.svg
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-down.svg
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-exclamation.svg
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-gear.svg
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-lock.svg
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-slash.svg
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-up.svg
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-x.svg
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill.svg
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-gear.svg
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-lock.svg
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-slash.svg
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-up.svg
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-x.svg
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database.svg
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/device-hdd-fill.svg
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/device-hdd.svg
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/device-ssd-fill.svg
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/device-ssd.svg
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/diagram-2-fill.svg
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/diagram-2.svg
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/diagram-3-fill.svg
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/diagram-3.svg
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/diamond-fill.svg
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/diamond-half.svg
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/diamond.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-1-fill.svg
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-1.svg
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-2-fill.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-2.svg
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-3-fill.svg
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-3.svg
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-4-fill.svg
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-4.svg
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-5-fill.svg
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-5.svg
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-6-fill.svg
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-6.svg
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/disc-fill.svg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/disc.svg
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/discord.svg
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/display-fill.svg
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/display.svg
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/displayport-fill.svg
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/displayport.svg
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/distribute-horizontal.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/distribute-vertical.svg
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/door-closed-fill.svg
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/door-closed.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/door-open-fill.svg
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/door-open.svg
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dot.svg
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/download.svg
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dpad-fill.svg
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dpad.svg
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dribbble.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dropbox.svg
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/droplet-fill.svg
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/droplet-half.svg
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/droplet.svg
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/duffle-fill.svg
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/duffle.svg
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ear-fill.svg
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ear.svg
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/earbuds.svg
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/easel-fill.svg
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/easel.svg
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/easel2-fill.svg
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/easel2.svg
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/easel3-fill.svg
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/easel3.svg
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/egg-fill.svg
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/egg-fried.svg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/egg.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eject-fill.svg
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eject.svg
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-angry-fill.svg
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-angry.svg
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-astonished-fill.svg
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-astonished.svg
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-dizzy-fill.svg
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-dizzy.svg
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-expressionless-fill.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-expressionless.svg
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-frown-fill.svg
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-frown.svg
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-grimace-fill.svg
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-grimace.svg
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-grin-fill.svg
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-grin.svg
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-heart-eyes-fill.svg
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-heart-eyes.svg
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-kiss-fill.svg
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-kiss.svg
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-laughing-fill.svg
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-laughing.svg
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-neutral-fill.svg
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-neutral.svg
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-smile-fill.svg
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-smile-upside-down-fill.svg
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-smile-upside-down.svg
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-smile.svg
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-sunglasses-fill.svg
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-sunglasses.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-surprise-fill.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-surprise.svg
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-tear-fill.svg
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-tear.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-wink-fill.svg
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-wink.svg
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-arrow-down-fill.svg
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-arrow-down.svg
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-arrow-up-fill.svg
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-arrow-up.svg
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-at-fill.svg
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-at.svg
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-check-fill.svg
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-check.svg
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-dash-fill.svg
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-dash.svg
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-exclamation-fill.svg
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-exclamation.svg
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-fill.svg
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-heart-fill.svg
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-heart.svg
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-open-fill.svg
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-open-heart-fill.svg
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-open-heart.svg
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-open.svg
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-paper-fill.svg
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-paper-heart-fill.svg
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-paper-heart.svg
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-paper.svg
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-plus-fill.svg
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-plus.svg
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-slash-fill.svg
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-slash.svg
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-x-fill.svg
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-x.svg
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope.svg
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eraser-fill.svg
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eraser.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/escape.svg
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ethernet.svg
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ev-front-fill.svg
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ev-front.svg
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ev-station-fill.svg
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ev-station.svg
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-circle-fill.svg
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-circle.svg
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-diamond-fill.svg
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-diamond.svg
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-lg.svg
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-octagon-fill.svg
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-octagon.svg
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-square-fill.svg
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-square.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-triangle-fill.svg
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-triangle.svg
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation.svg
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclude.svg
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/explicit-fill.svg
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/explicit.svg
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exposure.svg
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eye-fill.svg
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eye-slash-fill.svg
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eye-slash.svg
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eye.svg
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eyedropper.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eyeglasses.svg
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/facebook.svg
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fan.svg
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fast-forward-btn-fill.svg
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fast-forward-btn.svg
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fast-forward-circle-fill.svg
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fast-forward-circle.svg
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fast-forward-fill.svg
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fast-forward.svg
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/feather.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/feather2.svg
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-arrow-down-fill.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-arrow-down.svg
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-arrow-up-fill.svg
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-arrow-up.svg
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-bar-graph-fill.svg
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-bar-graph.svg
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-binary-fill.svg
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-binary.svg
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-break-fill.svg
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-break.svg
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-check-fill.svg
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-check.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-code-fill.svg
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-code.svg
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-diff-fill.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-diff.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-arrow-down-fill.svg
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-arrow-down.svg
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-arrow-up-fill.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-arrow-up.svg
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-bar-graph-fill.svg
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-bar-graph.svg
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-binary-fill.svg
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-binary.svg
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-break-fill.svg
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-break.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-check-fill.svg
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-check.svg
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-code-fill.svg
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-code.svg
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-diff-fill.svg
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-diff.svg
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-easel-fill.svg
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-easel.svg
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-excel-fill.svg
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-excel.svg
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-fill.svg
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-font-fill.svg
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-font.svg
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-image-fill.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-image.svg
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-lock-fill.svg
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-lock.svg
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-lock2-fill.svg
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-lock2.svg
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-medical-fill.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-medical.svg
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-minus-fill.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-minus.svg
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-music-fill.svg
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-music.svg
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-pdf-fill.svg
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-pdf.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-person-fill.svg
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-person.svg
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-play-fill.svg
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-play.svg
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-plus-fill.svg
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-plus.svg
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-post-fill.svg
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-post.svg
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-ppt-fill.svg
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-ppt.svg
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-richtext-fill.svg
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-richtext.svg
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-ruled-fill.svg
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-ruled.svg
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-slides-fill.svg
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-slides.svg
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-spreadsheet-fill.svg
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-spreadsheet.svg
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-text-fill.svg
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-text.svg
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-word-fill.svg
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-word.svg
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-x-fill.svg
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-x.svg
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-zip-fill.svg
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-zip.svg
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark.svg
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-easel-fill.svg
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-easel.svg
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-excel-fill.svg
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-excel.svg
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-fill.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-font-fill.svg
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-font.svg
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-image-fill.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-image.svg
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-lock-fill.svg
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-lock.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-lock2-fill.svg
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-lock2.svg
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-medical-fill.svg
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-medical.svg
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-minus-fill.svg
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-minus.svg
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-music-fill.svg
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-music.svg
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-pdf-fill.svg
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-pdf.svg
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-person-fill.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-person.svg
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-play-fill.svg
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-play.svg
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-plus-fill.svg
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-plus.svg
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-post-fill.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-post.svg
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-ppt-fill.svg
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-ppt.svg
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-richtext-fill.svg
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-richtext.svg
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-ruled-fill.svg
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-ruled.svg
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-slides-fill.svg
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-slides.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-spreadsheet-fill.svg
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-spreadsheet.svg
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-text-fill.svg
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-text.svg
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-word-fill.svg
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-word.svg
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-x-fill.svg
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-x.svg
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-zip-fill.svg
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-zip.svg
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file.svg
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/files-alt.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/files.svg
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-aac.svg
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-ai.svg
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-bmp.svg
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-cs.svg
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-css.svg
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-csv.svg
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-doc.svg
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-docx.svg
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-exe.svg
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-gif.svg
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-heic.svg
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-html.svg
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-java.svg
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-jpg.svg
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-js.svg
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-json.svg
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-jsx.svg
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-key.svg
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-m4p.svg
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-md.svg
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-mdx.svg
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-mov.svg
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-mp3.svg
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-mp4.svg
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-otf.svg
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-pdf.svg
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-php.svg
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-png.svg
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-ppt.svg
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-pptx.svg
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-psd.svg
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-py.svg
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-raw.svg
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-rb.svg
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-sass.svg
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-scss.svg
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-sh.svg
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-sql.svg
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-svg.svg
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-tiff.svg
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-tsx.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-ttf.svg
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-txt.svg
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-wav.svg
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-woff.svg
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-xls.svg
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-xlsx.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-xml.svg
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-yml.svg
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/film.svg
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filter-circle-fill.svg
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filter-circle.svg
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filter-left.svg
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filter-right.svg
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filter-square-fill.svg
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filter-square.svg
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filter.svg
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fingerprint.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fire.svg
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/flag-fill.svg
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/flag.svg
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/floppy-fill.svg
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/floppy.svg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/floppy2-fill.svg
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/floppy2.svg
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/flower1.svg
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/flower2.svg
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/flower3.svg
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-check.svg
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-fill.svg
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-minus.svg
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-plus.svg
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-symlink-fill.svg
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-symlink.svg
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-x.svg
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder.svg
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder2-open.svg
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder2.svg
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fonts.svg
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/forward-fill.svg
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/forward.svg
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/front.svg
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fuel-pump-diesel-fill.svg
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fuel-pump-diesel.svg
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fuel-pump-fill.svg
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fuel-pump.svg
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fullscreen-exit.svg
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fullscreen.svg
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/funnel-fill.svg
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/funnel.svg
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gear-fill.svg
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gear-wide-connected.svg
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gear-wide.svg
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gear.svg
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gem.svg
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gender-ambiguous.svg
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gender-female.svg
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gender-male.svg
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gender-neuter.svg
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gender-trans.svg
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/geo-alt-fill.svg
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/geo-alt.svg
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/geo-fill.svg
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/geo.svg
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gift-fill.svg
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gift.svg
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/git.svg
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/github.svg
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gitlab.svg
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/globe-americas.svg
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/globe-asia-australia.svg
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/globe-central-south-asia.svg
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/globe-europe-africa.svg
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/globe.svg
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/globe2.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/google-play.svg
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/google.svg
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gpu-card.svg
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/graph-down-arrow.svg
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/graph-down.svg
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/graph-up-arrow.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/graph-up.svg
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-1x2-fill.svg
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-1x2.svg
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-3x2-gap-fill.svg
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-3x2-gap.svg
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-3x2.svg
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-3x3-gap-fill.svg
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-3x3-gap.svg
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-3x3.svg
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-fill.svg
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid.svg
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grip-horizontal.svg
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grip-vertical.svg
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/h-circle-fill.svg
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/h-circle.svg
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/h-square-fill.svg
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/h-square.svg
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hammer.svg
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-index-fill.svg
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-index-thumb-fill.svg
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-index-thumb.svg
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-index.svg
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-thumbs-down-fill.svg
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-thumbs-down.svg
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-thumbs-up-fill.svg
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-thumbs-up.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/handbag-fill.svg
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/handbag.svg
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hash.svg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdd-fill.svg
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdd-network-fill.svg
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdd-network.svg
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdd-rack-fill.svg
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdd-rack.svg
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdd-stack-fill.svg
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdd-stack.svg
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdd.svg
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdmi-fill.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdmi.svg
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/headphones.svg
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/headset-vr.svg
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/headset.svg
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heart-arrow.svg
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heart-fill.svg
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heart-half.svg
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heart-pulse-fill.svg
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heart-pulse.svg
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heart.svg
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heartbreak-fill.svg
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heartbreak.svg
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hearts.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heptagon-fill.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heptagon-half.svg
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heptagon.svg
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hexagon-fill.svg
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hexagon-half.svg
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hexagon.svg
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/highlighter.svg
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/highlights.svg
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hospital-fill.svg
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hospital.svg
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hourglass-bottom.svg
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hourglass-split.svg
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hourglass-top.svg
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hourglass.svg
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-add-fill.svg
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-add.svg
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-check-fill.svg
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-check.svg
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-dash-fill.svg
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-dash.svg
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-door-fill.svg
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-door.svg
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-down-fill.svg
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-down.svg
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-exclamation-fill.svg
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-exclamation.svg
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-fill.svg
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-gear-fill.svg
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-gear.svg
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-heart-fill.svg
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-heart.svg
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-lock-fill.svg
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-lock.svg
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-slash-fill.svg
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-slash.svg
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-up-fill.svg
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-up.svg
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-x-fill.svg
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-x.svg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house.svg
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/houses-fill.svg
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/houses.svg
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hr.svg
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hurricane.svg
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hypnotize.svg
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/image-alt.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/image-fill.svg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/image.svg
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/images.svg
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/inbox-fill.svg
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/inbox.svg
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/inboxes-fill.svg
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/inboxes.svg
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/incognito.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/indent.svg
--rw-r--r--   0        0        0   153096 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/index.html
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/infinity.svg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/info-circle-fill.svg
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/info-circle.svg
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/info-lg.svg
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/info-square-fill.svg
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/info-square.svg
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/info.svg
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/input-cursor-text.svg
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/input-cursor.svg
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/instagram.svg
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/intersect.svg
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-album.svg
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-arrow-down.svg
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-arrow-up.svg
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-bookmark-fill.svg
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-bookmark.svg
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-check.svg
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-code.svg
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-medical.svg
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-minus.svg
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-plus.svg
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-richtext.svg
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-text.svg
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-x.svg
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal.svg
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journals.svg
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/joystick.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/justify-left.svg
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/justify-right.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/justify.svg
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/kanban-fill.svg
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/kanban.svg
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/key-fill.svg
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/key.svg
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/keyboard-fill.svg
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/keyboard.svg
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ladder.svg
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lamp-fill.svg
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lamp.svg
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/laptop-fill.svg
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/laptop.svg
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layer-backward.svg
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layer-forward.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layers-fill.svg
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layers-half.svg
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layers.svg
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-sidebar-inset-reverse.svg
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-sidebar-inset.svg
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-sidebar-reverse.svg
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-sidebar.svg
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-split.svg
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-text-sidebar-reverse.svg
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-text-sidebar.svg
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-text-window-reverse.svg
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-text-window.svg
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-three-columns.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-wtf.svg
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/life-preserver.svg
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lightbulb-fill.svg
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lightbulb-off-fill.svg
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lightbulb-off.svg
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lightbulb.svg
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lightning-charge-fill.svg
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lightning-charge.svg
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lightning-fill.svg
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lightning.svg
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/line.svg
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/link-45deg.svg
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/link.svg
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/linkedin.svg
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-check.svg
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-columns-reverse.svg
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-columns.svg
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-nested.svg
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-ol.svg
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-stars.svg
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-task.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-ul.svg
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list.svg
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lock-fill.svg
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lock.svg
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/luggage-fill.svg
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/luggage.svg
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lungs-fill.svg
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lungs.svg
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/magic.svg
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/magnet-fill.svg
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/magnet.svg
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mailbox-flag.svg
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mailbox.svg
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mailbox2-flag.svg
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mailbox2.svg
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/map-fill.svg
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/map.svg
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/markdown-fill.svg
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/markdown.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/marker-tip.svg
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mask.svg
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mastodon.svg
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/medium.svg
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/megaphone-fill.svg
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/megaphone.svg
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/memory.svg
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-app-fill.svg
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-app.svg
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-button-fill.svg
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-button-wide-fill.svg
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-button-wide.svg
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-button.svg
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-down.svg
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-up.svg
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/messenger.svg
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/meta.svg
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mic-fill.svg
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mic-mute-fill.svg
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mic-mute.svg
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mic.svg
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/microsoft-teams.svg
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/microsoft.svg
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/minecart-loaded.svg
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/minecart.svg
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/modem-fill.svg
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/modem.svg
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/moisture.svg
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/moon-fill.svg
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/moon-stars-fill.svg
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/moon-stars.svg
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/moon.svg
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mortarboard-fill.svg
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mortarboard.svg
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/motherboard-fill.svg
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/motherboard.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mouse-fill.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mouse.svg
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mouse2-fill.svg
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mouse2.svg
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mouse3-fill.svg
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mouse3.svg
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/music-note-beamed.svg
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/music-note-list.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/music-note.svg
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/music-player-fill.svg
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/music-player.svg
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/newspaper.svg
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/nintendo-switch.svg
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/node-minus-fill.svg
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/node-minus.svg
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/node-plus-fill.svg
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/node-plus.svg
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/noise-reduction.svg
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/nut-fill.svg
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/nut.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/nvidia.svg
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/nvme-fill.svg
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/nvme.svg
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/octagon-fill.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/octagon-half.svg
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/octagon.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/opencollective.svg
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/optical-audio-fill.svg
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/optical-audio.svg
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/option.svg
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/outlet.svg
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/p-circle-fill.svg
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/p-circle.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/p-square-fill.svg
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/p-square.svg
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/paint-bucket.svg
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/palette-fill.svg
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/palette.svg
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/palette2.svg
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/paperclip.svg
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/paragraph.svg
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pass-fill.svg
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pass.svg
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/passport-fill.svg
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/passport.svg
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-check-fill.svg
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-check.svg
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-exclamation-fill.svg
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-exclamation.svg
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-minus-fill.svg
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-minus.svg
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-plus-fill.svg
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-plus.svg
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-question-fill.svg
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-question.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pause-btn-fill.svg
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pause-btn.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pause-circle-fill.svg
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pause-circle.svg
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pause-fill.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pause.svg
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/paypal.svg
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pc-display-horizontal.svg
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pc-display.svg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pc-horizontal.svg
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pc.svg
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pci-card-network.svg
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pci-card-sound.svg
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pci-card.svg
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/peace-fill.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/peace.svg
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pen-fill.svg
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pen.svg
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pencil-fill.svg
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pencil-square.svg
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pencil.svg
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pentagon-fill.svg
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pentagon-half.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pentagon.svg
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/people-fill.svg
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/people.svg
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/percent.svg
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-add.svg
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-arms-up.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-badge-fill.svg
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-badge.svg
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-bounding-box.svg
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-check-fill.svg
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-check.svg
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-circle.svg
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-dash-fill.svg
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-dash.svg
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-down.svg
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-exclamation.svg
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill-add.svg
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill-check.svg
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill-dash.svg
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill-down.svg
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill-exclamation.svg
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill-gear.svg
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill-lock.svg
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill-slash.svg
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill-up.svg
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill-x.svg
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill.svg
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-gear.svg
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-heart.svg
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-hearts.svg
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-lines-fill.svg
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-lock.svg
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-plus-fill.svg
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-plus.svg
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-raised-hand.svg
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-rolodex.svg
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-slash.svg
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-square.svg
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-standing-dress.svg
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-standing.svg
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-up.svg
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-vcard-fill.svg
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-vcard.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-video.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-video2.svg
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-video3.svg
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-walking.svg
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-wheelchair.svg
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-workspace.svg
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-x-fill.svg
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-x.svg
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person.svg
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/phone-fill.svg
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/phone-flip.svg
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/phone-landscape-fill.svg
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/phone-landscape.svg
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/phone-vibrate-fill.svg
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/phone-vibrate.svg
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/phone.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pie-chart-fill.svg
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pie-chart.svg
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/piggy-bank-fill.svg
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/piggy-bank.svg
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pin-angle-fill.svg
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pin-angle.svg
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pin-fill.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pin-map-fill.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pin-map.svg
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pin.svg
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pinterest.svg
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pip-fill.svg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pip.svg
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/play-btn-fill.svg
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/play-btn.svg
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/play-circle-fill.svg
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/play-circle.svg
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/play-fill.svg
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/play.svg
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/playstation.svg
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plug-fill.svg
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plug.svg
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plugin.svg
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plus-circle-dotted.svg
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plus-circle-fill.svg
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plus-circle.svg
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plus-lg.svg
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plus-slash-minus.svg
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plus-square-dotted.svg
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plus-square-fill.svg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plus-square.svg
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plus.svg
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postage-fill.svg
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postage-heart-fill.svg
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postage-heart.svg
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postage.svg
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postcard-fill.svg
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postcard-heart-fill.svg
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postcard-heart.svg
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postcard.svg
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/power.svg
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/prescription.svg
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/prescription2.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/printer-fill.svg
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/printer.svg
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/projector-fill.svg
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/projector.svg
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/puzzle-fill.svg
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/puzzle.svg
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/qr-code-scan.svg
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/qr-code.svg
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-circle-fill.svg
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-circle.svg
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-diamond-fill.svg
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-diamond.svg
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-lg.svg
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-octagon-fill.svg
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-octagon.svg
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-square-fill.svg
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-square.svg
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question.svg
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/quora.svg
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/quote.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/r-circle-fill.svg
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/r-circle.svg
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/r-square-fill.svg
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/r-square.svg
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/radar.svg
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/radioactive.svg
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rainbow.svg
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/receipt-cutoff.svg
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/receipt.svg
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reception-0.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reception-1.svg
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reception-2.svg
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reception-3.svg
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reception-4.svg
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/record-btn-fill.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/record-btn.svg
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/record-circle-fill.svg
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/record-circle.svg
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/record-fill.svg
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/record.svg
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/record2-fill.svg
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/record2.svg
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/recycle.svg
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reddit.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/regex.svg
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/repeat-1.svg
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/repeat.svg
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reply-all-fill.svg
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reply-all.svg
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reply-fill.svg
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reply.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rewind-btn-fill.svg
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rewind-btn.svg
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rewind-circle-fill.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rewind-circle.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rewind-fill.svg
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rewind.svg
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/robot.svg
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rocket-fill.svg
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rocket-takeoff-fill.svg
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rocket-takeoff.svg
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rocket.svg
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/router-fill.svg
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/router.svg
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rss-fill.svg
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rss.svg
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rulers.svg
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/safe-fill.svg
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/safe.svg
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/safe2-fill.svg
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/safe2.svg
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/save-fill.svg
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/save.svg
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/save2-fill.svg
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/save2.svg
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/scissors.svg
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/scooter.svg
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/screwdriver.svg
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sd-card-fill.svg
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sd-card.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/search-heart-fill.svg
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/search-heart.svg
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/search.svg
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/segmented-nav.svg
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-arrow-down-fill.svg
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-arrow-down.svg
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-arrow-up-fill.svg
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-arrow-up.svg
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-check-fill.svg
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-check.svg
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-dash-fill.svg
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-dash.svg
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-exclamation-fill.svg
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-exclamation.svg
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-fill.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-plus-fill.svg
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-plus.svg
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-slash-fill.svg
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-slash.svg
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-x-fill.svg
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-x.svg
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send.svg
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/server.svg
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shadows.svg
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/share-fill.svg
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/share.svg
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-check.svg
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-exclamation.svg
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-fill-check.svg
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-fill-exclamation.svg
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-fill-minus.svg
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-fill-plus.svg
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-fill-x.svg
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-fill.svg
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-lock-fill.svg
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-lock.svg
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-minus.svg
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-plus.svg
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-shaded.svg
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-slash-fill.svg
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-slash.svg
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-x.svg
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield.svg
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shift-fill.svg
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shift.svg
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shop-window.svg
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shop.svg
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shuffle.svg
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-dead-end-fill.svg
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-dead-end.svg
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-do-not-enter-fill.svg
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-do-not-enter.svg
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-intersection-fill.svg
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-intersection-side-fill.svg
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-intersection-side.svg
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-intersection-t-fill.svg
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-intersection-t.svg
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-intersection-y-fill.svg
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-intersection-y.svg
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-intersection.svg
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-merge-left-fill.svg
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-merge-left.svg
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-merge-right-fill.svg
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-merge-right.svg
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-no-left-turn-fill.svg
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-no-left-turn.svg
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-no-parking-fill.svg
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-no-parking.svg
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-no-right-turn-fill.svg
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-no-right-turn.svg
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-railroad-fill.svg
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-railroad.svg
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-stop-fill.svg
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-stop-lights-fill.svg
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-stop-lights.svg
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-stop.svg
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-left-fill.svg
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-left.svg
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-right-fill.svg
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-right.svg
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-slight-left-fill.svg
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-slight-left.svg
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-slight-right-fill.svg
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-slight-right.svg
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-yield-fill.svg
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-yield.svg
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/signal.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/signpost-2-fill.svg
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/signpost-2.svg
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/signpost-fill.svg
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/signpost-split-fill.svg
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/signpost-split.svg
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/signpost.svg
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sim-fill.svg
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sim-slash-fill.svg
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sim-slash.svg
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sim.svg
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sina-weibo.svg
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-backward-btn-fill.svg
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-backward-btn.svg
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-backward-circle-fill.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-backward-circle.svg
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-backward-fill.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-backward.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-end-btn-fill.svg
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-end-btn.svg
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-end-circle-fill.svg
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-end-circle.svg
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-end-fill.svg
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-end.svg
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-forward-btn-fill.svg
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-forward-btn.svg
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-forward-circle-fill.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-forward-circle.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-forward-fill.svg
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-forward.svg
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-start-btn-fill.svg
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-start-btn.svg
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-start-circle-fill.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-start-circle.svg
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-start-fill.svg
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skip-start.svg
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skype.svg
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/slack.svg
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/slash-circle-fill.svg
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/slash-circle.svg
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/slash-lg.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/slash-square-fill.svg
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/slash-square.svg
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/slash.svg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sliders.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sliders2-vertical.svg
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sliders2.svg
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/smartwatch.svg
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/snapchat.svg
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/snow.svg
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/snow2.svg
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/snow3.svg
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-alpha-down-alt.svg
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-alpha-down.svg
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-alpha-up-alt.svg
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-alpha-up.svg
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-down-alt.svg
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-down.svg
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-numeric-down-alt.svg
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-numeric-down.svg
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-numeric-up-alt.svg
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-numeric-up.svg
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-up-alt.svg
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-up.svg
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/soundwave.svg
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sourceforge.svg
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/speaker-fill.svg
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/speaker.svg
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/speedometer.svg
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/speedometer2.svg
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/spellcheck.svg
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/spotify.svg
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/square-fill.svg
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/square-half.svg
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/square.svg
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stack-overflow.svg
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stack.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/star-fill.svg
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/star-half.svg
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/star.svg
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stars.svg
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/steam.svg
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stickies-fill.svg
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stickies.svg
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sticky-fill.svg
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sticky.svg
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stop-btn-fill.svg
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stop-btn.svg
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stop-circle-fill.svg
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stop-circle.svg
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stop-fill.svg
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stop.svg
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stoplights-fill.svg
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stoplights.svg
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stopwatch-fill.svg
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stopwatch.svg
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/strava.svg
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stripe.svg
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/subscript.svg
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/substack.svg
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/subtract.svg
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suit-club-fill.svg
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suit-club.svg
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suit-diamond-fill.svg
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suit-diamond.svg
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suit-heart-fill.svg
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suit-heart.svg
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suit-spade-fill.svg
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suit-spade.svg
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suitcase-fill.svg
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suitcase-lg-fill.svg
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suitcase-lg.svg
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suitcase.svg
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suitcase2-fill.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suitcase2.svg
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sun-fill.svg
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sun.svg
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sunglasses.svg
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sunrise-fill.svg
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sunrise.svg
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sunset-fill.svg
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sunset.svg
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/superscript.svg
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/symmetry-horizontal.svg
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/symmetry-vertical.svg
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/table.svg
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tablet-fill.svg
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tablet-landscape-fill.svg
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tablet-landscape.svg
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tablet.svg
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tag-fill.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tag.svg
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tags-fill.svg
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tags.svg
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/taxi-front-fill.svg
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/taxi-front.svg
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telegram.svg
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-fill.svg
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-forward-fill.svg
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-forward.svg
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-inbound-fill.svg
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-inbound.svg
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-minus-fill.svg
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-minus.svg
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-outbound-fill.svg
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-outbound.svg
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-plus-fill.svg
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-plus.svg
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-x-fill.svg
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-x.svg
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone.svg
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tencent-qq.svg
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/terminal-dash.svg
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/terminal-fill.svg
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/terminal-plus.svg
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/terminal-split.svg
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/terminal-x.svg
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/terminal.svg
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/text-center.svg
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/text-indent-left.svg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/text-indent-right.svg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/text-left.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/text-paragraph.svg
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/text-right.svg
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/text-wrap.svg
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/textarea-resize.svg
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/textarea-t.svg
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/textarea.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/thermometer-half.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/thermometer-high.svg
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/thermometer-low.svg
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/thermometer-snow.svg
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/thermometer-sun.svg
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/thermometer.svg
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/threads-fill.svg
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/threads.svg
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/three-dots-vertical.svg
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/three-dots.svg
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/thunderbolt-fill.svg
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/thunderbolt.svg
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ticket-detailed-fill.svg
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ticket-detailed.svg
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ticket-fill.svg
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ticket-perforated-fill.svg
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ticket-perforated.svg
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ticket.svg
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tiktok.svg
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/toggle-off.svg
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/toggle-on.svg
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/toggle2-off.svg
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/toggle2-on.svg
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/toggles.svg
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/toggles2.svg
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tools.svg
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tornado.svg
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/train-freight-front-fill.svg
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/train-freight-front.svg
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/train-front-fill.svg
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/train-front.svg
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/train-lightrail-front-fill.svg
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/train-lightrail-front.svg
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/translate.svg
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/transparency.svg
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trash-fill.svg
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trash.svg
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trash2-fill.svg
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trash2.svg
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trash3-fill.svg
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trash3.svg
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tree-fill.svg
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tree.svg
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trello.svg
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/triangle-fill.svg
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/triangle-half.svg
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/triangle.svg
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trophy-fill.svg
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trophy.svg
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tropical-storm.svg
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/truck-flatbed.svg
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/truck-front-fill.svg
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/truck-front.svg
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/truck.svg
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tsunami.svg
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tv-fill.svg
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tv.svg
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/twitch.svg
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/twitter-x.svg
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/twitter.svg
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-bold.svg
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-h1.svg
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-h2.svg
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-h3.svg
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-h4.svg
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-h5.svg
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-h6.svg
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-italic.svg
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-strikethrough.svg
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-underline.svg
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type.svg
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ubuntu.svg
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ui-checks-grid.svg
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ui-checks.svg
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ui-radios-grid.svg
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ui-radios.svg
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/umbrella-fill.svg
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/umbrella.svg
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/unindent.svg
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/union.svg
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/unity.svg
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/universal-access-circle.svg
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/universal-access.svg
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/unlock-fill.svg
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/unlock.svg
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/upc-scan.svg
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/upc.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/upload.svg
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-c-fill.svg
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-c.svg
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-drive-fill.svg
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-drive.svg
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-fill.svg
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-micro-fill.svg
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-micro.svg
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-mini-fill.svg
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-mini.svg
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-plug-fill.svg
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-plug.svg
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-symbol.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb.svg
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/valentine.svg
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/valentine2.svg
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/vector-pen.svg
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/view-list.svg
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/view-stacked.svg
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/vignette.svg
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/vimeo.svg
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/vinyl-fill.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/vinyl.svg
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/virus.svg
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/virus2.svg
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/voicemail.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/volume-down-fill.svg
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/volume-down.svg
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/volume-mute-fill.svg
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/volume-mute.svg
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/volume-off-fill.svg
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/volume-off.svg
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/volume-up-fill.svg
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/volume-up.svg
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/vr.svg
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wallet-fill.svg
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wallet.svg
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wallet2.svg
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/watch.svg
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/water.svg
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/webcam-fill.svg
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/webcam.svg
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wechat.svg
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/whatsapp.svg
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wifi-1.svg
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wifi-2.svg
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wifi-off.svg
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wifi.svg
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wikipedia.svg
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wind.svg
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-dash.svg
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-desktop.svg
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-dock.svg
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-fullscreen.svg
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-plus.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-sidebar.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-split.svg
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-stack.svg
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-x.svg
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window.svg
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/windows.svg
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wordpress.svg
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wrench-adjustable-circle-fill.svg
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wrench-adjustable-circle.svg
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wrench-adjustable.svg
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wrench.svg
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x-circle-fill.svg
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x-circle.svg
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x-diamond-fill.svg
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x-diamond.svg
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x-lg.svg
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x-octagon-fill.svg
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x-octagon.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x-square-fill.svg
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x-square.svg
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x.svg
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/xbox.svg
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/yelp.svg
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/yin-yang.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/youtube.svg
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/zoom-in.svg
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/zoom-out.svg
--rw-r--r--   0        0        0   176200 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   130608 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0   788921 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/ol/ol.js
--rw-r--r--   0        0        0  4438539 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/static/ol/ol.js.map
--rw-r--r--   0        0        0    10014 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/templates/base.html
--rw-r--r--   0        0        0    94148 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/BoatBuddy/templates/index.html
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/resources/.DS_Store
--rw-r--r--   0        0        0    66082 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/resources/logo/Boat Buddy - No Bg.png
--rw-r--r--   0        0        0    50830 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/resources/logo/Boat Buddy.png
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/resources/manuals/.DS_Store
--rw-r--r--   0        0        0    53569 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/resources/manuals/CCGX-Modbus-TCP-register-list-2.90.xlsx
--rw-r--r--   0        0        0   740435 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/resources/manuals/NMEA0183 Sentences Table.jpg
--rw-r--r--   0        0        0    60113 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/resources/manuals/NMEA0183.pdf
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/LICENSE
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/README.md
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 boatbuddy-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/.DS_Store
+-rw-r--r--   0        0        0    21572 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/CHANGELOG.md
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/change-log-builder.sh
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/requirements.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/.idea/BoatBuddy.iml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/.idea/misc.xml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/__init__.py
+-rw-r--r--   0        0        0    13672 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/__main__.py
+-rw-r--r--   0        0        0    12097 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/anchor_manager.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/clock_plugin.py
+-rw-r--r--   0        0        0    17162 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/console_manager.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/database_manager.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/email_manager.py
+-rw-r--r--   0        0        0    25830 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/flask_manager.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/generic_plugin.py
+-rw-r--r--   0        0        0     7911 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/globals.py
+-rw-r--r--   0        0        0    16087 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/gps_plugin.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/log_manager.py
+-rw-r--r--   0        0        0    17339 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/mysql_wrapper.py
+-rw-r--r--   0        0        0    23602 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/nmea_plugin.py
+-rw-r--r--   0        0        0    27253 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/notifications_manager.py
+-rw-r--r--   0        0        0    21434 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/plugin_manager.py
+-rw-r--r--   0        0        0    16001 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/sample-config.json
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/sound_manager.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/telegram_manager.py
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/utils.py
+-rw-r--r--   0        0        0    31209 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/victron_plugin.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/resources/.DS_Store
+-rw-r--r--   0        0        0   132000 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/resources/alarm.mp3
+-rw-r--r--   0        0        0    25984 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/resources/application_started.mp3
+-rw-r--r--   0        0        0    20506 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/resources/session_ended.wav
+-rw-r--r--   0        0        0   123715 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/resources/session_started.mp3
+-rw-r--r--   0        0        0    61022 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/resources/warning.mp3
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/.DS_Store
+-rw-r--r--   0        0        0    14782 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/GaugeMeter.js
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/favicon.ico
+-rw-r--r--   0        0        0    44733 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/gauge.min.js
+-rw-r--r--   0        0        0    87532 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/jquery-3.7.1.min.js
+-rw-r--r--   0        0        0   134767 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/jquery-3.7.1.min.map
+-rw-r--r--   0        0        0    66082 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/logo.png
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/main.css
+-rw-r--r--   0        0        0    20121 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/popper.min.js
+-rw-r--r--   0        0        0   110046 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/popper.min.js.map
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/.DS_Store
+-rw-r--r--   0        0        0    70329 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203178 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51795 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115987 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70403 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203182 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51870 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116064 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129327 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10126 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51369 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129342 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63943 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107823 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267491 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85352 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180381 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107691 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267432 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85281 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180217 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   280813 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   679011 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232948 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589161 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280392 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   678856 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   233055 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   588695 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   207731 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444286 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80663 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   331886 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135747 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305152 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    74154 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222462 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145313 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0   306320 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60577 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220350 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/.DS_Store
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/0-circle-fill.svg
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/0-circle.svg
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/0-square-fill.svg
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/0-square.svg
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/1-circle-fill.svg
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/1-circle.svg
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/1-square-fill.svg
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/1-square.svg
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/123.svg
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/2-circle-fill.svg
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/2-circle.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/2-square-fill.svg
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/2-square.svg
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/3-circle-fill.svg
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/3-circle.svg
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/3-square-fill.svg
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/3-square.svg
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/4-circle-fill.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/4-circle.svg
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/4-square-fill.svg
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/4-square.svg
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/5-circle-fill.svg
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/5-circle.svg
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/5-square-fill.svg
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/5-square.svg
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/6-circle-fill.svg
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/6-circle.svg
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/6-square-fill.svg
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/6-square.svg
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/7-circle-fill.svg
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/7-circle.svg
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/7-square-fill.svg
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/7-square.svg
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/8-circle-fill.svg
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/8-circle.svg
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/8-square-fill.svg
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/8-square.svg
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/9-circle-fill.svg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/9-circle.svg
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/9-square-fill.svg
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/9-square.svg
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/activity.svg
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/airplane-engines-fill.svg
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/airplane-engines.svg
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/airplane-fill.svg
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/airplane.svg
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/alarm-fill.svg
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/alarm.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/alexa.svg
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/align-bottom.svg
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/align-center.svg
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/align-end.svg
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/align-middle.svg
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/align-start.svg
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/align-top.svg
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/alipay.svg
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/alphabet-uppercase.svg
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/alphabet.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/alt.svg
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/amazon.svg
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/amd.svg
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/android.svg
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/android2.svg
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/app-indicator.svg
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/app.svg
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/apple.svg
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/archive-fill.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/archive.svg
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-90deg-down.svg
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-90deg-left.svg
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-90deg-right.svg
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-90deg-up.svg
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-bar-down.svg
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-bar-left.svg
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-bar-right.svg
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-bar-up.svg
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-clockwise.svg
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-counterclockwise.svg
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-circle-fill.svg
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-circle.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-left-circle-fill.svg
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-left-circle.svg
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-left-square-fill.svg
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-left-square.svg
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-left.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-right-circle-fill.svg
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-right-circle.svg
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-right-square-fill.svg
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-right-square.svg
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-right.svg
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-square-fill.svg
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-square.svg
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down-up.svg
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-down.svg
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-left-circle-fill.svg
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-left-circle.svg
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-left-right.svg
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-left-short.svg
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-left-square-fill.svg
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-left-square.svg
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-left.svg
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-repeat.svg
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-return-left.svg
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-return-right.svg
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-right-circle-fill.svg
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-right-circle.svg
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-right-short.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-right-square-fill.svg
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-right-square.svg
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-right.svg
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-through-heart-fill.svg
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-through-heart.svg
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-circle-fill.svg
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-circle.svg
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-left-circle-fill.svg
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-left-circle.svg
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-left-square-fill.svg
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-left-square.svg
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-left.svg
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-right-circle-fill.svg
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-right-circle.svg
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-right-square-fill.svg
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-right-square.svg
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-right.svg
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-short.svg
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-square-fill.svg
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up-square.svg
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-up.svg
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrows-angle-contract.svg
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrows-angle-expand.svg
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrows-collapse-vertical.svg
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrows-collapse.svg
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrows-expand-vertical.svg
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrows-expand.svg
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrows-fullscreen.svg
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrows-move.svg
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrows-vertical.svg
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrows.svg
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/aspect-ratio-fill.svg
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/aspect-ratio.svg
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/asterisk.svg
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/at.svg
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/award-fill.svg
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/award.svg
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/back.svg
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack-fill.svg
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack.svg
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack2-fill.svg
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack2.svg
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack3-fill.svg
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack3.svg
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack4-fill.svg
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack4.svg
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backspace-fill.svg
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backspace-reverse-fill.svg
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backspace-reverse.svg
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backspace.svg
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-3d-fill.svg
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-3d.svg
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-4k-fill.svg
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-4k.svg
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-8k-fill.svg
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-8k.svg
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-ad-fill.svg
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-ad.svg
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-ar-fill.svg
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-ar.svg
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-cc-fill.svg
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-cc.svg
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-hd-fill.svg
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-hd.svg
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-sd-fill.svg
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-sd.svg
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-tm-fill.svg
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-tm.svg
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-vo-fill.svg
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-vo.svg
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-vr-fill.svg
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-vr.svg
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-wc-fill.svg
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-wc.svg
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag-check-fill.svg
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag-check.svg
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag-dash-fill.svg
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag-dash.svg
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag-fill.svg
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag-heart-fill.svg
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag-heart.svg
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag-plus-fill.svg
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag-plus.svg
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag-x-fill.svg
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag-x.svg
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag.svg
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/balloon-fill.svg
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/balloon-heart-fill.svg
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/balloon-heart.svg
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/balloon.svg
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ban-fill.svg
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ban.svg
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bandaid-fill.svg
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bandaid.svg
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bank.svg
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bank2.svg
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bar-chart-fill.svg
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bar-chart-line-fill.svg
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bar-chart-line.svg
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bar-chart-steps.svg
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bar-chart.svg
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/basket-fill.svg
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/basket.svg
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/basket2-fill.svg
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/basket2.svg
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/basket3-fill.svg
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/basket3.svg
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/battery-charging.svg
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/battery-full.svg
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/battery-half.svg
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/battery.svg
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/behance.svg
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bell-fill.svg
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bell-slash-fill.svg
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bell-slash.svg
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bell.svg
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bezier.svg
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bezier2.svg
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bicycle.svg
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bing.svg
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/binoculars-fill.svg
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/binoculars.svg
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/blockquote-left.svg
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/blockquote-right.svg
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bluetooth.svg
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/body-text.svg
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/book-fill.svg
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/book-half.svg
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/book.svg
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-check-fill.svg
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-check.svg
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-dash-fill.svg
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-dash.svg
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-fill.svg
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-heart-fill.svg
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-heart.svg
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-plus-fill.svg
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-plus.svg
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-star-fill.svg
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-star.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-x-fill.svg
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-x.svg
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark.svg
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmarks-fill.svg
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmarks.svg
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookshelf.svg
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/boombox-fill.svg
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/boombox.svg
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-fill.svg
+-rw-r--r--   0        0        0    98255 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    52358 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-icons.json
+-rw-r--r--   0        0        0    85875 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-icons.min.css
+-rw-r--r--   0        0        0    57755 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0  1149049 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-icons.svg
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-reboot.svg
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap.svg
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-all.svg
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-bottom.svg
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-center.svg
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-inner.svg
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-left.svg
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-middle.svg
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-outer.svg
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-right.svg
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-style.svg
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-top.svg
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-width.svg
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border.svg
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bounding-box-circles.svg
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bounding-box.svg
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-down-left.svg
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-down-right.svg
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-down.svg
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-down-left.svg
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-down-right.svg
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-down.svg
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-left.svg
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-right.svg
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-up-left.svg
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-up-right.svg
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-up.svg
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-left.svg
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-right.svg
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-up-left.svg
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-up-right.svg
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-up.svg
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-fill.svg
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-seam-fill.svg
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-seam.svg
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box.svg
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box2-fill.svg
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box2-heart-fill.svg
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box2-heart.svg
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box2.svg
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/boxes.svg
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/braces-asterisk.svg
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/braces.svg
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bricks.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/briefcase-fill.svg
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/briefcase.svg
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-alt-high-fill.svg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-alt-high.svg
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-alt-low-fill.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-alt-low.svg
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-high-fill.svg
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-high.svg
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-low-fill.svg
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-low.svg
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brilliance.svg
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/broadcast-pin.svg
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/broadcast.svg
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/browser-chrome.svg
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/browser-edge.svg
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/browser-firefox.svg
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/browser-safari.svg
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brush-fill.svg
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brush.svg
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bucket-fill.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bucket.svg
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bug-fill.svg
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bug.svg
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-add.svg
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-check.svg
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-dash.svg
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-down.svg
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-exclamation.svg
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-add.svg
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-check.svg
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-dash.svg
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-down.svg
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-exclamation.svg
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-gear.svg
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-lock.svg
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-slash.svg
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-up.svg
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-x.svg
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill.svg
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-gear.svg
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-lock.svg
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-slash.svg
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-up.svg
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-x.svg
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building.svg
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/buildings-fill.svg
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/buildings.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bullseye.svg
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bus-front-fill.svg
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bus-front.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/c-circle-fill.svg
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/c-circle.svg
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/c-square-fill.svg
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/c-square.svg
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cake-fill.svg
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cake.svg
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cake2-fill.svg
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cake2.svg
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calculator-fill.svg
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calculator.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-check-fill.svg
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-check.svg
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-date-fill.svg
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-date.svg
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-day-fill.svg
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-day.svg
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-event-fill.svg
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-event.svg
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-fill.svg
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-heart-fill.svg
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-heart.svg
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-minus-fill.svg
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-minus.svg
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-month-fill.svg
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-month.svg
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-plus-fill.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-plus.svg
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-range-fill.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-range.svg
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-week-fill.svg
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-week.svg
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-x-fill.svg
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-x.svg
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar.svg
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-check-fill.svg
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-check.svg
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-date-fill.svg
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-date.svg
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-day-fill.svg
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-day.svg
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-event-fill.svg
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-event.svg
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-fill.svg
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-heart-fill.svg
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-heart.svg
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-minus-fill.svg
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-minus.svg
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-month-fill.svg
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-month.svg
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-plus-fill.svg
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-plus.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-range-fill.svg
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-range.svg
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-week-fill.svg
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-week.svg
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-x-fill.svg
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-x.svg
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2.svg
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar3-event-fill.svg
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar3-event.svg
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar3-fill.svg
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar3-range-fill.svg
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar3-range.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar3-week-fill.svg
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar3-week.svg
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar3.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar4-event.svg
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar4-range.svg
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar4-week.svg
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar4.svg
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera-fill.svg
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera-reels-fill.svg
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera-reels.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera-video-fill.svg
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera-video-off-fill.svg
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera-video-off.svg
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera-video.svg
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera.svg
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera2.svg
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/capslock-fill.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/capslock.svg
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/capsule-pill.svg
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/capsule.svg
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/car-front-fill.svg
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/car-front.svg
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/card-checklist.svg
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/card-heading.svg
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/card-image.svg
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/card-list.svg
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/card-text.svg
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-down-fill.svg
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-down-square-fill.svg
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-down-square.svg
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-down.svg
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-left-fill.svg
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-left-square-fill.svg
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-left-square.svg
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-left.svg
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-right-fill.svg
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-right-square-fill.svg
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-right-square.svg
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-right.svg
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-up-fill.svg
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-up-square-fill.svg
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-up-square.svg
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/caret-up.svg
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-check-fill.svg
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-check.svg
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-dash-fill.svg
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-dash.svg
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-fill.svg
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-plus-fill.svg
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-plus.svg
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-x-fill.svg
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-x.svg
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart.svg
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart2.svg
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart3.svg
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart4.svg
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cash-coin.svg
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cash-stack.svg
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cash.svg
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cassette-fill.svg
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cassette.svg
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cast.svg
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cc-circle-fill.svg
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cc-circle.svg
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cc-square-fill.svg
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cc-square.svg
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-dots-fill.svg
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-dots.svg
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-fill.svg
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-heart-fill.svg
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-heart.svg
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left-dots-fill.svg
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left-dots.svg
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left-fill.svg
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left-heart-fill.svg
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left-heart.svg
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left-quote-fill.svg
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left-quote.svg
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left-text-fill.svg
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left-text.svg
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left.svg
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-quote-fill.svg
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-quote.svg
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right-dots-fill.svg
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right-dots.svg
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right-fill.svg
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right-heart-fill.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right-heart.svg
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right-quote-fill.svg
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right-quote.svg
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right-text-fill.svg
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right-text.svg
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right.svg
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-dots-fill.svg
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-dots.svg
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-fill.svg
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-heart-fill.svg
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-heart.svg
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-quote-fill.svg
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-quote.svg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-text-fill.svg
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-text.svg
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-text-fill.svg
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-text.svg
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat.svg
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/check-all.svg
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/check-circle-fill.svg
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/check-circle.svg
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/check-lg.svg
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/check-square-fill.svg
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/check-square.svg
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/check.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/check2-all.svg
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/check2-circle.svg
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/check2-square.svg
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/check2.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-bar-contract.svg
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-bar-down.svg
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-bar-expand.svg
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-bar-left.svg
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-bar-right.svg
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-bar-up.svg
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-compact-down.svg
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-compact-left.svg
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-compact-right.svg
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-compact-up.svg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-contract.svg
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-double-down.svg
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-double-left.svg
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-double-right.svg
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-double-up.svg
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-down.svg
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-expand.svg
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-left.svg
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-right.svg
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chevron-up.svg
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/circle-fill.svg
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/circle-half.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/circle-square.svg
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/circle.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-check-fill.svg
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-check.svg
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-data-fill.svg
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-data.svg
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-fill.svg
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-heart-fill.svg
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-heart.svg
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-minus-fill.svg
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-minus.svg
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-plus-fill.svg
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-plus.svg
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-pulse.svg
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-x-fill.svg
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-x.svg
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard.svg
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-check-fill.svg
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-check.svg
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-data-fill.svg
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-data.svg
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-fill.svg
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-heart-fill.svg
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-heart.svg
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-minus-fill.svg
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-minus.svg
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-plus-fill.svg
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-plus.svg
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-pulse-fill.svg
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-pulse.svg
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-x-fill.svg
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-x.svg
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2.svg
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clock-fill.svg
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clock-history.svg
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clock.svg
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-arrow-down-fill.svg
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-arrow-down.svg
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-arrow-up-fill.svg
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-arrow-up.svg
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-check-fill.svg
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-check.svg
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-download-fill.svg
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-download.svg
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-drizzle-fill.svg
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-drizzle.svg
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-fill.svg
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-fog-fill.svg
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-fog.svg
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-fog2-fill.svg
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-fog2.svg
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-hail-fill.svg
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-hail.svg
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-haze-fill.svg
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-haze.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-haze2-fill.svg
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-haze2.svg
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-lightning-fill.svg
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-lightning-rain-fill.svg
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-lightning-rain.svg
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-lightning.svg
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-minus-fill.svg
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-minus.svg
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-moon-fill.svg
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-moon.svg
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-plus-fill.svg
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-plus.svg
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-rain-fill.svg
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-rain-heavy-fill.svg
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-rain-heavy.svg
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-rain.svg
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-slash-fill.svg
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-slash.svg
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-sleet-fill.svg
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-sleet.svg
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-snow-fill.svg
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-snow.svg
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-sun-fill.svg
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-sun.svg
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-upload-fill.svg
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-upload.svg
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud.svg
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clouds-fill.svg
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clouds.svg
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloudy-fill.svg
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloudy.svg
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/code-slash.svg
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/code-square.svg
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/code.svg
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/coin.svg
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/collection-fill.svg
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/collection-play-fill.svg
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/collection-play.svg
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/collection.svg
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/columns-gap.svg
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/columns.svg
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/command.svg
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/compass-fill.svg
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/compass.svg
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cone-striped.svg
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cone.svg
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/controller.svg
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cookie.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/copy.svg
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cpu-fill.svg
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cpu.svg
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/credit-card-2-back-fill.svg
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/credit-card-2-back.svg
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/credit-card-2-front-fill.svg
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/credit-card-2-front.svg
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/credit-card-fill.svg
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/credit-card.svg
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/crop.svg
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/crosshair.svg
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/crosshair2.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cup-fill.svg
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cup-hot-fill.svg
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cup-hot.svg
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cup-straw.svg
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cup.svg
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/currency-bitcoin.svg
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/currency-dollar.svg
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/currency-euro.svg
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/currency-exchange.svg
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/currency-pound.svg
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/currency-rupee.svg
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/currency-yen.svg
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cursor-fill.svg
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cursor-text.svg
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cursor.svg
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dash-circle-dotted.svg
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dash-circle-fill.svg
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dash-circle.svg
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dash-lg.svg
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dash-square-dotted.svg
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dash-square-fill.svg
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dash-square.svg
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dash.svg
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-add.svg
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-check.svg
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-dash.svg
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-down.svg
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-exclamation.svg
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-add.svg
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-check.svg
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-dash.svg
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-down.svg
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-exclamation.svg
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-gear.svg
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-lock.svg
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-slash.svg
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-up.svg
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-x.svg
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill.svg
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-gear.svg
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-lock.svg
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-slash.svg
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-up.svg
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-x.svg
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database.svg
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/device-hdd-fill.svg
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/device-hdd.svg
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/device-ssd-fill.svg
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/device-ssd.svg
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/diagram-2-fill.svg
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/diagram-2.svg
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/diagram-3-fill.svg
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/diagram-3.svg
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/diamond-fill.svg
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/diamond-half.svg
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/diamond.svg
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-1-fill.svg
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-1.svg
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-2-fill.svg
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-2.svg
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-3-fill.svg
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-3.svg
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-4-fill.svg
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-4.svg
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-5-fill.svg
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-5.svg
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-6-fill.svg
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-6.svg
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/disc-fill.svg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/disc.svg
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/discord.svg
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/display-fill.svg
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/display.svg
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/displayport-fill.svg
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/displayport.svg
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/distribute-horizontal.svg
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/distribute-vertical.svg
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/door-closed-fill.svg
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/door-closed.svg
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/door-open-fill.svg
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/door-open.svg
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dot.svg
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/download.svg
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dpad-fill.svg
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dpad.svg
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dribbble.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dropbox.svg
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/droplet-fill.svg
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/droplet-half.svg
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/droplet.svg
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/duffle-fill.svg
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/duffle.svg
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ear-fill.svg
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ear.svg
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/earbuds.svg
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/easel-fill.svg
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/easel.svg
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/easel2-fill.svg
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/easel2.svg
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/easel3-fill.svg
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/easel3.svg
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/egg-fill.svg
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/egg-fried.svg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/egg.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eject-fill.svg
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eject.svg
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-angry-fill.svg
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-angry.svg
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-astonished-fill.svg
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-astonished.svg
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-dizzy-fill.svg
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-dizzy.svg
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-expressionless-fill.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-expressionless.svg
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-frown-fill.svg
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-frown.svg
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-grimace-fill.svg
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-grimace.svg
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-grin-fill.svg
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-grin.svg
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-heart-eyes-fill.svg
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-heart-eyes.svg
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-kiss-fill.svg
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-kiss.svg
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-laughing-fill.svg
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-laughing.svg
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-neutral-fill.svg
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-neutral.svg
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-smile-fill.svg
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-smile-upside-down-fill.svg
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-smile-upside-down.svg
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-smile.svg
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-sunglasses-fill.svg
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-sunglasses.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-surprise-fill.svg
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-surprise.svg
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-tear-fill.svg
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-tear.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-wink-fill.svg
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-wink.svg
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-arrow-down-fill.svg
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-arrow-down.svg
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-arrow-up-fill.svg
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-arrow-up.svg
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-at-fill.svg
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-at.svg
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-check-fill.svg
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-check.svg
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-dash-fill.svg
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-dash.svg
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-exclamation-fill.svg
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-exclamation.svg
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-fill.svg
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-heart-fill.svg
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-heart.svg
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-open-fill.svg
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-open-heart-fill.svg
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-open-heart.svg
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-open.svg
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-paper-fill.svg
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-paper-heart-fill.svg
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-paper-heart.svg
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-paper.svg
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-plus-fill.svg
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-plus.svg
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-slash-fill.svg
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-slash.svg
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-x-fill.svg
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-x.svg
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope.svg
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eraser-fill.svg
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eraser.svg
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/escape.svg
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ethernet.svg
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ev-front-fill.svg
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ev-front.svg
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ev-station-fill.svg
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ev-station.svg
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-circle-fill.svg
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-circle.svg
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-diamond-fill.svg
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-diamond.svg
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-lg.svg
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-octagon-fill.svg
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-octagon.svg
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-square-fill.svg
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-square.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-triangle-fill.svg
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-triangle.svg
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation.svg
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclude.svg
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/explicit-fill.svg
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/explicit.svg
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exposure.svg
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eye-fill.svg
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eye-slash-fill.svg
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eye-slash.svg
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eye.svg
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eyedropper.svg
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eyeglasses.svg
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/facebook.svg
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fan.svg
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fast-forward-btn-fill.svg
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fast-forward-btn.svg
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fast-forward-circle-fill.svg
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fast-forward-circle.svg
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fast-forward-fill.svg
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fast-forward.svg
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/feather.svg
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/feather2.svg
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-arrow-down-fill.svg
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-arrow-down.svg
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-arrow-up-fill.svg
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-arrow-up.svg
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-bar-graph-fill.svg
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-bar-graph.svg
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-binary-fill.svg
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-binary.svg
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-break-fill.svg
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-break.svg
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-check-fill.svg
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-check.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-code-fill.svg
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-code.svg
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-diff-fill.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-diff.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-arrow-down-fill.svg
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-arrow-down.svg
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-arrow-up-fill.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-arrow-up.svg
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-bar-graph-fill.svg
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-bar-graph.svg
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-binary-fill.svg
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-binary.svg
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-break-fill.svg
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-break.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-check-fill.svg
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-check.svg
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-code-fill.svg
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-code.svg
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-diff-fill.svg
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-diff.svg
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-easel-fill.svg
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-easel.svg
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-excel-fill.svg
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-excel.svg
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-fill.svg
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-font-fill.svg
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-font.svg
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-image-fill.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-image.svg
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-lock-fill.svg
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-lock.svg
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-lock2-fill.svg
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-lock2.svg
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-medical-fill.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-medical.svg
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-minus-fill.svg
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-minus.svg
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-music-fill.svg
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-music.svg
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-pdf-fill.svg
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-pdf.svg
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-person-fill.svg
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-person.svg
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-play-fill.svg
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-play.svg
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-plus-fill.svg
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-plus.svg
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-post-fill.svg
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-post.svg
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-ppt-fill.svg
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-ppt.svg
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-richtext-fill.svg
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-richtext.svg
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-ruled-fill.svg
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-ruled.svg
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-slides-fill.svg
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-slides.svg
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-spreadsheet-fill.svg
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-spreadsheet.svg
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-text-fill.svg
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-text.svg
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-word-fill.svg
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-word.svg
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-x-fill.svg
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-x.svg
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-zip-fill.svg
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-zip.svg
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark.svg
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-easel-fill.svg
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-easel.svg
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-excel-fill.svg
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-excel.svg
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-fill.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-font-fill.svg
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-font.svg
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-image-fill.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-image.svg
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-lock-fill.svg
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-lock.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-lock2-fill.svg
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-lock2.svg
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-medical-fill.svg
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-medical.svg
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-minus-fill.svg
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-minus.svg
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-music-fill.svg
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-music.svg
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-pdf-fill.svg
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-pdf.svg
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-person-fill.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-person.svg
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-play-fill.svg
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-play.svg
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-plus-fill.svg
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-plus.svg
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-post-fill.svg
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-post.svg
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-ppt-fill.svg
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-ppt.svg
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-richtext-fill.svg
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-richtext.svg
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-ruled-fill.svg
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-ruled.svg
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-slides-fill.svg
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-slides.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-spreadsheet-fill.svg
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-spreadsheet.svg
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-text-fill.svg
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-text.svg
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-word-fill.svg
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-word.svg
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-x-fill.svg
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-x.svg
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-zip-fill.svg
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-zip.svg
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file.svg
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/files-alt.svg
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/files.svg
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-aac.svg
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-ai.svg
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-bmp.svg
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-cs.svg
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-css.svg
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-csv.svg
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-doc.svg
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-docx.svg
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-exe.svg
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-gif.svg
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-heic.svg
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-html.svg
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-java.svg
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-jpg.svg
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-js.svg
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-json.svg
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-jsx.svg
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-key.svg
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-m4p.svg
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-md.svg
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-mdx.svg
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-mov.svg
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-mp3.svg
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-mp4.svg
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-otf.svg
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-pdf.svg
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-php.svg
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-png.svg
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-ppt.svg
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-pptx.svg
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-psd.svg
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-py.svg
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-raw.svg
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-rb.svg
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-sass.svg
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-scss.svg
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-sh.svg
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-sql.svg
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-svg.svg
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-tiff.svg
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-tsx.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-ttf.svg
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-txt.svg
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-wav.svg
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-woff.svg
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-xls.svg
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-xlsx.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-xml.svg
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-yml.svg
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/film.svg
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filter-circle-fill.svg
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filter-circle.svg
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filter-left.svg
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filter-right.svg
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filter-square-fill.svg
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filter-square.svg
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filter.svg
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fingerprint.svg
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fire.svg
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/flag-fill.svg
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/flag.svg
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/floppy-fill.svg
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/floppy.svg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/floppy2-fill.svg
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/floppy2.svg
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/flower1.svg
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/flower2.svg
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/flower3.svg
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-check.svg
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-fill.svg
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-minus.svg
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-plus.svg
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-symlink-fill.svg
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-symlink.svg
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-x.svg
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder.svg
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder2-open.svg
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder2.svg
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fonts.svg
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/forward-fill.svg
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/forward.svg
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/front.svg
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fuel-pump-diesel-fill.svg
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fuel-pump-diesel.svg
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fuel-pump-fill.svg
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fuel-pump.svg
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fullscreen-exit.svg
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fullscreen.svg
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/funnel-fill.svg
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/funnel.svg
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gear-fill.svg
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gear-wide-connected.svg
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gear-wide.svg
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gear.svg
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gem.svg
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gender-ambiguous.svg
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gender-female.svg
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gender-male.svg
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gender-neuter.svg
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gender-trans.svg
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/geo-alt-fill.svg
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/geo-alt.svg
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/geo-fill.svg
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/geo.svg
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gift-fill.svg
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gift.svg
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/git.svg
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/github.svg
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gitlab.svg
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/globe-americas.svg
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/globe-asia-australia.svg
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/globe-central-south-asia.svg
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/globe-europe-africa.svg
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/globe.svg
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/globe2.svg
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/google-play.svg
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/google.svg
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gpu-card.svg
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/graph-down-arrow.svg
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/graph-down.svg
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/graph-up-arrow.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/graph-up.svg
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-1x2-fill.svg
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-1x2.svg
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-3x2-gap-fill.svg
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-3x2-gap.svg
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-3x2.svg
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-3x3-gap-fill.svg
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-3x3-gap.svg
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-3x3.svg
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-fill.svg
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid.svg
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grip-horizontal.svg
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grip-vertical.svg
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/h-circle-fill.svg
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/h-circle.svg
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/h-square-fill.svg
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/h-square.svg
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hammer.svg
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-index-fill.svg
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-index-thumb-fill.svg
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-index-thumb.svg
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-index.svg
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-thumbs-down-fill.svg
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-thumbs-down.svg
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-thumbs-up-fill.svg
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-thumbs-up.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/handbag-fill.svg
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/handbag.svg
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hash.svg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdd-fill.svg
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdd-network-fill.svg
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdd-network.svg
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdd-rack-fill.svg
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdd-rack.svg
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdd-stack-fill.svg
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdd-stack.svg
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdd.svg
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdmi-fill.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdmi.svg
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/headphones.svg
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/headset-vr.svg
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/headset.svg
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heart-arrow.svg
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heart-fill.svg
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heart-half.svg
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heart-pulse-fill.svg
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heart-pulse.svg
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heart.svg
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heartbreak-fill.svg
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heartbreak.svg
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hearts.svg
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heptagon-fill.svg
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heptagon-half.svg
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heptagon.svg
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hexagon-fill.svg
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hexagon-half.svg
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hexagon.svg
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/highlighter.svg
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/highlights.svg
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hospital-fill.svg
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hospital.svg
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hourglass-bottom.svg
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hourglass-split.svg
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hourglass-top.svg
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hourglass.svg
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-add-fill.svg
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-add.svg
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-check-fill.svg
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-check.svg
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-dash-fill.svg
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-dash.svg
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-door-fill.svg
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-door.svg
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-down-fill.svg
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-down.svg
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-exclamation-fill.svg
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-exclamation.svg
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-fill.svg
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-gear-fill.svg
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-gear.svg
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-heart-fill.svg
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-heart.svg
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-lock-fill.svg
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-lock.svg
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-slash-fill.svg
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-slash.svg
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-up-fill.svg
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-up.svg
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-x-fill.svg
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-x.svg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house.svg
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/houses-fill.svg
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/houses.svg
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hr.svg
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hurricane.svg
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hypnotize.svg
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/image-alt.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/image-fill.svg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/image.svg
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/images.svg
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/inbox-fill.svg
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/inbox.svg
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/inboxes-fill.svg
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/inboxes.svg
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/incognito.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/indent.svg
+-rw-r--r--   0        0        0   153096 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/index.html
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/infinity.svg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/info-circle-fill.svg
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/info-circle.svg
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/info-lg.svg
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/info-square-fill.svg
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/info-square.svg
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/info.svg
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/input-cursor-text.svg
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/input-cursor.svg
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/instagram.svg
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/intersect.svg
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-album.svg
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-arrow-down.svg
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-arrow-up.svg
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-bookmark-fill.svg
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-bookmark.svg
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-check.svg
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-code.svg
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-medical.svg
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-minus.svg
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-plus.svg
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-richtext.svg
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-text.svg
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-x.svg
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal.svg
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journals.svg
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/joystick.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/justify-left.svg
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/justify-right.svg
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/justify.svg
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/kanban-fill.svg
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/kanban.svg
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/key-fill.svg
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/key.svg
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/keyboard-fill.svg
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/keyboard.svg
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ladder.svg
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lamp-fill.svg
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lamp.svg
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/laptop-fill.svg
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/laptop.svg
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layer-backward.svg
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layer-forward.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layers-fill.svg
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layers-half.svg
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layers.svg
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-sidebar-inset-reverse.svg
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-sidebar-inset.svg
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-sidebar-reverse.svg
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-sidebar.svg
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-split.svg
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-text-sidebar-reverse.svg
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-text-sidebar.svg
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-text-window-reverse.svg
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-text-window.svg
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-three-columns.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-wtf.svg
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/life-preserver.svg
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lightbulb-fill.svg
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lightbulb-off-fill.svg
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lightbulb-off.svg
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lightbulb.svg
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lightning-charge-fill.svg
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lightning-charge.svg
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lightning-fill.svg
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lightning.svg
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/line.svg
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/link-45deg.svg
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/link.svg
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/linkedin.svg
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-check.svg
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-columns-reverse.svg
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-columns.svg
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-nested.svg
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-ol.svg
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-stars.svg
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-task.svg
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-ul.svg
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list.svg
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lock-fill.svg
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lock.svg
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/luggage-fill.svg
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/luggage.svg
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lungs-fill.svg
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lungs.svg
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/magic.svg
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/magnet-fill.svg
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/magnet.svg
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mailbox-flag.svg
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mailbox.svg
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mailbox2-flag.svg
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mailbox2.svg
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/map-fill.svg
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/map.svg
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/markdown-fill.svg
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/markdown.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/marker-tip.svg
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mask.svg
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mastodon.svg
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/medium.svg
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/megaphone-fill.svg
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/megaphone.svg
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/memory.svg
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-app-fill.svg
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-app.svg
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-button-fill.svg
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-button-wide-fill.svg
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-button-wide.svg
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-button.svg
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-down.svg
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-up.svg
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/messenger.svg
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/meta.svg
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mic-fill.svg
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mic-mute-fill.svg
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mic-mute.svg
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mic.svg
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/microsoft-teams.svg
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/microsoft.svg
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/minecart-loaded.svg
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/minecart.svg
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/modem-fill.svg
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/modem.svg
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/moisture.svg
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/moon-fill.svg
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/moon-stars-fill.svg
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/moon-stars.svg
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/moon.svg
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mortarboard-fill.svg
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mortarboard.svg
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/motherboard-fill.svg
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/motherboard.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mouse-fill.svg
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mouse.svg
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mouse2-fill.svg
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mouse2.svg
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mouse3-fill.svg
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mouse3.svg
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/music-note-beamed.svg
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/music-note-list.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/music-note.svg
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/music-player-fill.svg
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/music-player.svg
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/newspaper.svg
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/nintendo-switch.svg
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/node-minus-fill.svg
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/node-minus.svg
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/node-plus-fill.svg
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/node-plus.svg
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/noise-reduction.svg
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/nut-fill.svg
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/nut.svg
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/nvidia.svg
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/nvme-fill.svg
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/nvme.svg
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/octagon-fill.svg
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/octagon-half.svg
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/octagon.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/opencollective.svg
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/optical-audio-fill.svg
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/optical-audio.svg
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/option.svg
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/outlet.svg
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/p-circle-fill.svg
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/p-circle.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/p-square-fill.svg
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/p-square.svg
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/paint-bucket.svg
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/palette-fill.svg
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/palette.svg
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/palette2.svg
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/paperclip.svg
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/paragraph.svg
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pass-fill.svg
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pass.svg
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/passport-fill.svg
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/passport.svg
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-check-fill.svg
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-check.svg
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-exclamation-fill.svg
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-exclamation.svg
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-minus-fill.svg
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-minus.svg
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-plus-fill.svg
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-plus.svg
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-question-fill.svg
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-question.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pause-btn-fill.svg
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pause-btn.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pause-circle-fill.svg
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pause-circle.svg
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pause-fill.svg
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pause.svg
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/paypal.svg
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pc-display-horizontal.svg
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pc-display.svg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pc-horizontal.svg
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pc.svg
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pci-card-network.svg
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pci-card-sound.svg
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pci-card.svg
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/peace-fill.svg
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/peace.svg
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pen-fill.svg
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pen.svg
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pencil-fill.svg
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pencil-square.svg
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pencil.svg
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pentagon-fill.svg
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pentagon-half.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pentagon.svg
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/people-fill.svg
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/people.svg
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/percent.svg
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-add.svg
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-arms-up.svg
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-badge-fill.svg
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-badge.svg
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-bounding-box.svg
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-check-fill.svg
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-check.svg
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-circle.svg
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-dash-fill.svg
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-dash.svg
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-down.svg
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-exclamation.svg
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill-add.svg
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill-check.svg
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill-dash.svg
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill-down.svg
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill-exclamation.svg
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill-gear.svg
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill-lock.svg
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill-slash.svg
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill-up.svg
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill-x.svg
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill.svg
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-gear.svg
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-heart.svg
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-hearts.svg
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-lines-fill.svg
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-lock.svg
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-plus-fill.svg
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-plus.svg
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-raised-hand.svg
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-rolodex.svg
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-slash.svg
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-square.svg
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-standing-dress.svg
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-standing.svg
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-up.svg
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-vcard-fill.svg
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-vcard.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-video.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-video2.svg
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-video3.svg
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-walking.svg
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-wheelchair.svg
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-workspace.svg
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-x-fill.svg
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-x.svg
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person.svg
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/phone-fill.svg
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/phone-flip.svg
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/phone-landscape-fill.svg
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/phone-landscape.svg
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/phone-vibrate-fill.svg
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/phone-vibrate.svg
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/phone.svg
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pie-chart-fill.svg
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pie-chart.svg
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/piggy-bank-fill.svg
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/piggy-bank.svg
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pin-angle-fill.svg
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pin-angle.svg
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pin-fill.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pin-map-fill.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pin-map.svg
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pin.svg
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pinterest.svg
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pip-fill.svg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pip.svg
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/play-btn-fill.svg
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/play-btn.svg
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/play-circle-fill.svg
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/play-circle.svg
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/play-fill.svg
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/play.svg
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/playstation.svg
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plug-fill.svg
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plug.svg
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plugin.svg
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plus-circle-dotted.svg
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plus-circle-fill.svg
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plus-circle.svg
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plus-lg.svg
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plus-slash-minus.svg
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plus-square-dotted.svg
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plus-square-fill.svg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plus-square.svg
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plus.svg
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postage-fill.svg
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postage-heart-fill.svg
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postage-heart.svg
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postage.svg
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postcard-fill.svg
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postcard-heart-fill.svg
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postcard-heart.svg
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postcard.svg
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/power.svg
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/prescription.svg
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/prescription2.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/printer-fill.svg
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/printer.svg
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/projector-fill.svg
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/projector.svg
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/puzzle-fill.svg
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/puzzle.svg
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/qr-code-scan.svg
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/qr-code.svg
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-circle-fill.svg
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-circle.svg
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-diamond-fill.svg
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-diamond.svg
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-lg.svg
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-octagon-fill.svg
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-octagon.svg
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-square-fill.svg
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-square.svg
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question.svg
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/quora.svg
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/quote.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/r-circle-fill.svg
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/r-circle.svg
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/r-square-fill.svg
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/r-square.svg
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/radar.svg
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/radioactive.svg
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rainbow.svg
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/receipt-cutoff.svg
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/receipt.svg
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reception-0.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reception-1.svg
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reception-2.svg
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reception-3.svg
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reception-4.svg
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/record-btn-fill.svg
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/record-btn.svg
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/record-circle-fill.svg
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/record-circle.svg
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/record-fill.svg
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/record.svg
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/record2-fill.svg
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/record2.svg
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/recycle.svg
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reddit.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/regex.svg
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/repeat-1.svg
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/repeat.svg
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reply-all-fill.svg
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reply-all.svg
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reply-fill.svg
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reply.svg
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rewind-btn-fill.svg
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rewind-btn.svg
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rewind-circle-fill.svg
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rewind-circle.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rewind-fill.svg
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rewind.svg
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/robot.svg
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rocket-fill.svg
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rocket-takeoff-fill.svg
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rocket-takeoff.svg
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rocket.svg
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/router-fill.svg
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/router.svg
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rss-fill.svg
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rss.svg
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rulers.svg
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/safe-fill.svg
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/safe.svg
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/safe2-fill.svg
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/safe2.svg
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/save-fill.svg
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/save.svg
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/save2-fill.svg
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/save2.svg
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/scissors.svg
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/scooter.svg
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/screwdriver.svg
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sd-card-fill.svg
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sd-card.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/search-heart-fill.svg
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/search-heart.svg
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/search.svg
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/segmented-nav.svg
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-arrow-down-fill.svg
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-arrow-down.svg
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-arrow-up-fill.svg
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-arrow-up.svg
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-check-fill.svg
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-check.svg
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-dash-fill.svg
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-dash.svg
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-exclamation-fill.svg
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-exclamation.svg
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-fill.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-plus-fill.svg
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-plus.svg
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-slash-fill.svg
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-slash.svg
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-x-fill.svg
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-x.svg
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send.svg
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/server.svg
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shadows.svg
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/share-fill.svg
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/share.svg
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-check.svg
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-exclamation.svg
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-fill-check.svg
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-fill-exclamation.svg
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-fill-minus.svg
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-fill-plus.svg
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-fill-x.svg
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-fill.svg
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-lock-fill.svg
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-lock.svg
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-minus.svg
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-plus.svg
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-shaded.svg
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-slash-fill.svg
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-slash.svg
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-x.svg
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield.svg
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shift-fill.svg
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shift.svg
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shop-window.svg
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shop.svg
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shuffle.svg
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-dead-end-fill.svg
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-dead-end.svg
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-do-not-enter-fill.svg
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-do-not-enter.svg
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-intersection-fill.svg
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-intersection-side-fill.svg
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-intersection-side.svg
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-intersection-t-fill.svg
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-intersection-t.svg
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-intersection-y-fill.svg
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-intersection-y.svg
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-intersection.svg
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-merge-left-fill.svg
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-merge-left.svg
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-merge-right-fill.svg
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-merge-right.svg
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-no-left-turn-fill.svg
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-no-left-turn.svg
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-no-parking-fill.svg
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-no-parking.svg
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-no-right-turn-fill.svg
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-no-right-turn.svg
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-railroad-fill.svg
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-railroad.svg
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-stop-fill.svg
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-stop-lights-fill.svg
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-stop-lights.svg
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-stop.svg
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-left-fill.svg
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-left.svg
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-right-fill.svg
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-right.svg
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-slight-left-fill.svg
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-slight-left.svg
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-slight-right-fill.svg
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-slight-right.svg
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-yield-fill.svg
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-yield.svg
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/signal.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/signpost-2-fill.svg
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/signpost-2.svg
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/signpost-fill.svg
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/signpost-split-fill.svg
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/signpost-split.svg
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/signpost.svg
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sim-fill.svg
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sim-slash-fill.svg
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sim-slash.svg
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sim.svg
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sina-weibo.svg
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-backward-btn-fill.svg
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-backward-btn.svg
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-backward-circle-fill.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-backward-circle.svg
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-backward-fill.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-backward.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-end-btn-fill.svg
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-end-btn.svg
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-end-circle-fill.svg
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-end-circle.svg
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-end-fill.svg
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-end.svg
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-forward-btn-fill.svg
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-forward-btn.svg
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-forward-circle-fill.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-forward-circle.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-forward-fill.svg
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-forward.svg
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-start-btn-fill.svg
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-start-btn.svg
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-start-circle-fill.svg
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-start-circle.svg
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-start-fill.svg
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skip-start.svg
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skype.svg
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/slack.svg
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/slash-circle-fill.svg
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/slash-circle.svg
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/slash-lg.svg
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/slash-square-fill.svg
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/slash-square.svg
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/slash.svg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sliders.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sliders2-vertical.svg
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sliders2.svg
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/smartwatch.svg
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/snapchat.svg
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/snow.svg
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/snow2.svg
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/snow3.svg
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-alpha-down-alt.svg
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-alpha-down.svg
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-alpha-up-alt.svg
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-alpha-up.svg
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-down-alt.svg
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-down.svg
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-numeric-down-alt.svg
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-numeric-down.svg
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-numeric-up-alt.svg
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-numeric-up.svg
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-up-alt.svg
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-up.svg
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/soundwave.svg
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sourceforge.svg
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/speaker-fill.svg
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/speaker.svg
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/speedometer.svg
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/speedometer2.svg
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/spellcheck.svg
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/spotify.svg
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/square-fill.svg
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/square-half.svg
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/square.svg
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stack-overflow.svg
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stack.svg
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/star-fill.svg
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/star-half.svg
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/star.svg
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stars.svg
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/steam.svg
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stickies-fill.svg
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stickies.svg
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sticky-fill.svg
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sticky.svg
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stop-btn-fill.svg
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stop-btn.svg
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stop-circle-fill.svg
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stop-circle.svg
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stop-fill.svg
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stop.svg
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stoplights-fill.svg
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stoplights.svg
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stopwatch-fill.svg
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stopwatch.svg
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/strava.svg
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stripe.svg
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/subscript.svg
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/substack.svg
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/subtract.svg
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suit-club-fill.svg
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suit-club.svg
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suit-diamond-fill.svg
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suit-diamond.svg
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suit-heart-fill.svg
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suit-heart.svg
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suit-spade-fill.svg
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suit-spade.svg
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suitcase-fill.svg
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suitcase-lg-fill.svg
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suitcase-lg.svg
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suitcase.svg
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suitcase2-fill.svg
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suitcase2.svg
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sun-fill.svg
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sun.svg
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sunglasses.svg
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sunrise-fill.svg
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sunrise.svg
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sunset-fill.svg
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sunset.svg
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/superscript.svg
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/symmetry-horizontal.svg
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/symmetry-vertical.svg
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/table.svg
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tablet-fill.svg
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tablet-landscape-fill.svg
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tablet-landscape.svg
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tablet.svg
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tag-fill.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tag.svg
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tags-fill.svg
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tags.svg
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/taxi-front-fill.svg
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/taxi-front.svg
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telegram.svg
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-fill.svg
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-forward-fill.svg
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-forward.svg
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-inbound-fill.svg
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-inbound.svg
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-minus-fill.svg
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-minus.svg
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-outbound-fill.svg
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-outbound.svg
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-plus-fill.svg
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-plus.svg
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-x-fill.svg
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-x.svg
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone.svg
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tencent-qq.svg
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/terminal-dash.svg
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/terminal-fill.svg
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/terminal-plus.svg
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/terminal-split.svg
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/terminal-x.svg
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/terminal.svg
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/text-center.svg
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/text-indent-left.svg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/text-indent-right.svg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/text-left.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/text-paragraph.svg
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/text-right.svg
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/text-wrap.svg
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/textarea-resize.svg
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/textarea-t.svg
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/textarea.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/thermometer-half.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/thermometer-high.svg
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/thermometer-low.svg
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/thermometer-snow.svg
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/thermometer-sun.svg
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/thermometer.svg
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/threads-fill.svg
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/threads.svg
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/three-dots-vertical.svg
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/three-dots.svg
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/thunderbolt-fill.svg
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/thunderbolt.svg
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ticket-detailed-fill.svg
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ticket-detailed.svg
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ticket-fill.svg
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ticket-perforated-fill.svg
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ticket-perforated.svg
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ticket.svg
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tiktok.svg
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/toggle-off.svg
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/toggle-on.svg
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/toggle2-off.svg
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/toggle2-on.svg
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/toggles.svg
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/toggles2.svg
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tools.svg
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tornado.svg
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/train-freight-front-fill.svg
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/train-freight-front.svg
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/train-front-fill.svg
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/train-front.svg
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/train-lightrail-front-fill.svg
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/train-lightrail-front.svg
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/translate.svg
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/transparency.svg
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trash-fill.svg
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trash.svg
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trash2-fill.svg
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trash2.svg
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trash3-fill.svg
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trash3.svg
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tree-fill.svg
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tree.svg
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trello.svg
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/triangle-fill.svg
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/triangle-half.svg
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/triangle.svg
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trophy-fill.svg
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trophy.svg
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tropical-storm.svg
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/truck-flatbed.svg
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/truck-front-fill.svg
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/truck-front.svg
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/truck.svg
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tsunami.svg
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tv-fill.svg
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tv.svg
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/twitch.svg
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/twitter-x.svg
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/twitter.svg
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-bold.svg
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-h1.svg
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-h2.svg
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-h3.svg
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-h4.svg
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-h5.svg
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-h6.svg
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-italic.svg
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-strikethrough.svg
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-underline.svg
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type.svg
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ubuntu.svg
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ui-checks-grid.svg
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ui-checks.svg
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ui-radios-grid.svg
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ui-radios.svg
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/umbrella-fill.svg
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/umbrella.svg
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/unindent.svg
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/union.svg
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/unity.svg
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/universal-access-circle.svg
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/universal-access.svg
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/unlock-fill.svg
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/unlock.svg
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/upc-scan.svg
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/upc.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/upload.svg
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-c-fill.svg
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-c.svg
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-drive-fill.svg
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-drive.svg
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-fill.svg
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-micro-fill.svg
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-micro.svg
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-mini-fill.svg
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-mini.svg
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-plug-fill.svg
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-plug.svg
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-symbol.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb.svg
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/valentine.svg
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/valentine2.svg
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/vector-pen.svg
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/view-list.svg
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/view-stacked.svg
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/vignette.svg
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/vimeo.svg
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/vinyl-fill.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/vinyl.svg
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/virus.svg
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/virus2.svg
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/voicemail.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/volume-down-fill.svg
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/volume-down.svg
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/volume-mute-fill.svg
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/volume-mute.svg
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/volume-off-fill.svg
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/volume-off.svg
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/volume-up-fill.svg
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/volume-up.svg
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/vr.svg
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wallet-fill.svg
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wallet.svg
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wallet2.svg
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/watch.svg
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/water.svg
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/webcam-fill.svg
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/webcam.svg
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wechat.svg
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/whatsapp.svg
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wifi-1.svg
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wifi-2.svg
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wifi-off.svg
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wifi.svg
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wikipedia.svg
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wind.svg
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-dash.svg
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-desktop.svg
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-dock.svg
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-fullscreen.svg
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-plus.svg
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-sidebar.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-split.svg
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-stack.svg
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-x.svg
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window.svg
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/windows.svg
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wordpress.svg
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wrench-adjustable-circle-fill.svg
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wrench-adjustable-circle.svg
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wrench-adjustable.svg
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wrench.svg
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x-circle-fill.svg
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x-circle.svg
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x-diamond-fill.svg
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x-diamond.svg
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x-lg.svg
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x-octagon-fill.svg
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x-octagon.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x-square-fill.svg
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x-square.svg
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x.svg
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/xbox.svg
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/yelp.svg
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/yin-yang.svg
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/youtube.svg
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/zoom-in.svg
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/zoom-out.svg
+-rw-r--r--   0        0        0   176200 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   130608 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0   788921 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/ol/ol.js
+-rw-r--r--   0        0        0  4438539 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/static/ol/ol.js.map
+-rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/templates/base.html
+-rw-r--r--   0        0        0    94174 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/BoatBuddy/templates/index.html
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/resources/.DS_Store
+-rw-r--r--   0        0        0    66082 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/resources/logo/Boat Buddy - No Bg.png
+-rw-r--r--   0        0        0    50830 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/resources/logo/Boat Buddy.png
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/resources/manuals/.DS_Store
+-rw-r--r--   0        0        0    53569 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/resources/manuals/CCGX-Modbus-TCP-register-list-2.90.xlsx
+-rw-r--r--   0        0        0   740435 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/resources/manuals/NMEA0183 Sentences Table.jpg
+-rw-r--r--   0        0        0    60113 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/resources/manuals/NMEA0183.pdf
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/LICENSE
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/README.md
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 boatbuddy-0.9.5/PKG-INFO
```

### Comparing `boatbuddy-0.9.4/.DS_Store` & `boatbuddy-0.9.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/CHANGELOG.md` & `boatbuddy-0.9.5/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.9.5 (2023-12-03)
+
+* Layout improvements
+* Version bump to 0.9.5
+
 ## 0.9.4 (2023-12-02)
 
 * Layout improvements
 * Version bump to 0.9.4
 
 ## 0.9.3 (2023-11-29)
```

### Comparing `boatbuddy-0.9.4/requirements.txt` & `boatbuddy-0.9.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/.DS_Store` & `boatbuddy-0.9.5/BoatBuddy/.DS_Store`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/__main__.py` & `boatbuddy-0.9.5/BoatBuddy/__main__.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/anchor_manager.py` & `boatbuddy-0.9.5/BoatBuddy/anchor_manager.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/clock_plugin.py` & `boatbuddy-0.9.5/BoatBuddy/clock_plugin.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/console_manager.py` & `boatbuddy-0.9.5/BoatBuddy/console_manager.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/database_manager.py` & `boatbuddy-0.9.5/BoatBuddy/database_manager.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/email_manager.py` & `boatbuddy-0.9.5/BoatBuddy/email_manager.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/flask_manager.py` & `boatbuddy-0.9.5/BoatBuddy/flask_manager.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/generic_plugin.py` & `boatbuddy-0.9.5/BoatBuddy/generic_plugin.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/globals.py` & `boatbuddy-0.9.5/BoatBuddy/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 
 # General
 APPLICATION_NAME = 'Boat Buddy'
-APPLICATION_VERSION = '0.9.4'
+APPLICATION_VERSION = '0.9.5'
 LOG_FILENAME = 'BoatBuddy.log'
 LOG_FILE_SIZE = 1024 * 1024  # Log file size 1MB
 LOGGER_NAME = 'BoatBuddy'
 INITIAL_SNAPSHOT_INTERVAL = 1  # Time to wait for the first snapshot to be taken after the session starts in seconds
 EMPTY_METRIC_VALUE = "N/A"
 JSON_RESPONSE_FORMAT_VERSION = 6
```

### Comparing `boatbuddy-0.9.4/BoatBuddy/gps_plugin.py` & `boatbuddy-0.9.5/BoatBuddy/gps_plugin.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/log_manager.py` & `boatbuddy-0.9.5/BoatBuddy/log_manager.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/mysql_wrapper.py` & `boatbuddy-0.9.5/BoatBuddy/mysql_wrapper.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/nmea_plugin.py` & `boatbuddy-0.9.5/BoatBuddy/nmea_plugin.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/notifications_manager.py` & `boatbuddy-0.9.5/BoatBuddy/notifications_manager.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/plugin_manager.py` & `boatbuddy-0.9.5/BoatBuddy/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/sample-config.json` & `boatbuddy-0.9.5/BoatBuddy/sample-config.json`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/sound_manager.py` & `boatbuddy-0.9.5/BoatBuddy/sound_manager.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/telegram_manager.py` & `boatbuddy-0.9.5/BoatBuddy/telegram_manager.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/utils.py` & `boatbuddy-0.9.5/BoatBuddy/utils.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/victron_plugin.py` & `boatbuddy-0.9.5/BoatBuddy/victron_plugin.py`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/resources/.DS_Store` & `boatbuddy-0.9.5/BoatBuddy/resources/.DS_Store`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/resources/alarm.mp3` & `boatbuddy-0.9.5/BoatBuddy/resources/alarm.mp3`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/resources/application_started.mp3` & `boatbuddy-0.9.5/BoatBuddy/resources/application_started.mp3`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/resources/session_ended.wav` & `boatbuddy-0.9.5/BoatBuddy/resources/session_ended.wav`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/resources/session_started.mp3` & `boatbuddy-0.9.5/BoatBuddy/resources/session_started.mp3`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/resources/warning.mp3` & `boatbuddy-0.9.5/BoatBuddy/resources/warning.mp3`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/.DS_Store` & `boatbuddy-0.9.5/BoatBuddy/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/CustomGaugeMeter.js` & `boatbuddy-0.9.5/BoatBuddy/static/GaugeMeter.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
  *
  * This is a bug fixed and modified version of the AshAlom Gauge Meter.
  * Copyright 2023 Michael Wolf (Mictronics)
  * https://github.com/mictronics/GaugeMeter
  *
  */
 !(function($) {
-    $.fn.customGaugeMeter = function(t) {
+    $.fn.gaugeMeter = function(t) {
         var defaults = $.extend({
                 id: '',
                 percent: 0,
                 used: null,
                 min: null,
                 total: null,
                 size: 100,
@@ -32,15 +32,16 @@
                 animate_gauge_colors: false,
                 animate_text_colors: false,
                 label: '',
                 label_color: 'Black',
                 text: '',
                 text_size: 0.22,
                 fill: '',
-                showvalue: false
+                showvalue: false,
+                middle_value_format: false
             },
             t
         );
         return this.each(function() {
             function getThemeColor(e) {
                 var t = '#2C94E0';
                 return (
@@ -268,29 +269,37 @@
                 g.lineWidth = lw;
                 g.strokeStyle = option.back;
                 option.stripe > parseInt(0) ?
                     g.setLineDash([option.stripe], 1) :
                     (g.lineCap = 'round');
                 g.stroke();
 
-                // Draw a line from the center to the specified value
-                g.beginPath();
-                startAngle = 0;
-                endAngle = 0
-                if (a <= 0.5) {
-                    startAngle = P * a - I;
-                    endAngle = P * 0.5 - I;
+                if (option.middle_value_format) {
+                    // Draw a line from the center to the specified value
+                    g.beginPath();
+                    startAngle = 0;
+                    endAngle = 0
+                    if (a <= 0.5) {
+                        startAngle = P * a - I;
+                        endAngle = P * 0.5 - I;
+                    } else {
+                        startAngle = P * 0.5 - I;
+                        endAngle = P * a - I;
+                    }
+                    g.arc(m, v, x, startAngle, endAngle, !1);
+                    g.lineWidth = lw;
+                    g.strokeStyle = option.fgcolor;
+                    g.stroke();
                 } else {
-                    startAngle = P * 0.5 - I;
-                    endAngle = P * a - I;
+                    g.beginPath();
+                    g.arc(m, v, x, -I, P * a - I, !1);
+                    g.lineWidth = lw;
+                    g.strokeStyle = option.fgcolor;
+                    g.stroke();
                 }
-                g.arc(m, v, x, startAngle, endAngle, !1);
-                g.lineWidth = lw;
-                g.strokeStyle = option.fgcolor;
-                g.stroke();
 
                 // Highlight Circle
                 g.beginPath();
                 g.arc(m, v, x, P * a - I, P * a - I, !1);
                 g.lineWidth = lw + 5;
                 g.strokeStyle = option.fgcolor;
                 g.stroke();
@@ -328,15 +337,16 @@
                     'animate_gauge_colors',
                     'animate_text_colors',
                     'label',
                     'label_color',
                     'text',
                     'text_size',
                     'fill',
-                    'showvalue'
+                    'showvalue',
+                    'middle_value_format'
                 ],
                 option = {},
                 c = 0,
                 p = $(this),
                 s = false;
             p.addClass('gaugeMeter');
             getDataAttr(p);
```

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/favicon.ico` & `boatbuddy-0.9.5/BoatBuddy/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/gauge.min.js` & `boatbuddy-0.9.5/BoatBuddy/static/gauge.min.js`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/jquery-3.7.1.min.js` & `boatbuddy-0.9.5/BoatBuddy/static/jquery-3.7.1.min.js`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/jquery-3.7.1.min.map` & `boatbuddy-0.9.5/BoatBuddy/static/jquery-3.7.1.min.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/logo.png` & `boatbuddy-0.9.5/BoatBuddy/static/logo.png`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/main.css` & `boatbuddy-0.9.5/BoatBuddy/static/main.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/popper.min.js` & `boatbuddy-0.9.5/BoatBuddy/static/popper.min.js`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/popper.min.js.map` & `boatbuddy-0.9.5/BoatBuddy/static/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/.DS_Store` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/.DS_Store`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.min.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.min.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.min.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.min.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.min.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.min.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.min.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.min.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.min.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.min.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.min.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.rtl.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.rtl.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.rtl.min.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/css/bootstrap.rtl.min.css.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.bundle.js` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.bundle.js.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.bundle.min.js` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.bundle.min.js.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.esm.js` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.esm.js.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.esm.min.js` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.esm.min.js.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.js` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.js.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.min.js` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap/js/bootstrap.min.js.map` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/.DS_Store` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/0-square-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/0-square-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/0-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/0-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/123.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/123.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/2-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/2-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/3-circle-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/3-circle-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/3-circle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/3-circle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/3-square-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/3-square-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/3-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/3-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/5-circle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/5-circle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/5-square-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/5-square-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/5-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/5-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/6-circle-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/6-circle-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/6-circle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/6-circle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/6-square-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/6-square-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/6-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/6-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/8-circle-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/8-circle-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/8-circle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/8-circle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/8-square-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/8-square-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/8-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/8-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/9-circle-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/9-circle-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/9-circle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/9-circle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/9-square-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/9-square-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/9-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/9-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/airplane-engines-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/airplane-engines-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/airplane-engines.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/airplane-engines.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/airplane.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/airplane.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/alarm-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/alarm-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/alarm.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/alarm.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/alipay.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/alipay.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/alphabet-uppercase.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/alphabet-uppercase.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/alphabet.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/alphabet.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/amazon.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/amazon.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/android2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/android2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/apple.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/apple.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-repeat.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-repeat.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-through-heart-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-through-heart-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrow-through-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrow-through-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrows-fullscreen.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrows-fullscreen.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/arrows-move.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/at.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/at.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/award.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/award.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack2-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack2-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack3-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack3-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack3.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack3.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack4-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack4-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backpack4.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backpack4.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backspace-reverse.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backspace-reverse.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/backspace.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/backspace.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-3d-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-3d-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-3d.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-3d.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-4k-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-4k-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-4k.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-4k.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-8k-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-8k-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-8k.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-8k.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-ad-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-ad-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-ad.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-ad.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-ar-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-ar-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-ar.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-ar.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-cc-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-cc-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-cc.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-cc.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-hd.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-hd.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-sd-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-sd-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-sd.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-sd.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-vo-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-vo-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-vo.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-vo.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-vr-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-vr-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-vr.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-vr.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-wc-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-wc-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/badge-wc.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/badge-wc.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bag-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bag-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/balloon-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/balloon-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/balloon-heart-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/balloon-heart-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/balloon-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/balloon-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/balloon.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/balloon.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bandaid-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bandaid-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bandaid.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bandaid.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bar-chart-steps.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bar-chart-steps.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/basket-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/basket-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/basket.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/basket.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/basket2-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/basket2-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/basket2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/basket2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/battery-charging.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/battery-charging.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/behance.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/behance.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bell-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bell-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bell.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bell.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bezier.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bezier.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bezier2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bezier2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bicycle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bicycle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bing.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bing.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/binoculars-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/binoculars-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/binoculars.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/binoculars.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/blockquote-left.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/blockquote-left.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/blockquote-right.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/blockquote-right.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/body-text.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/body-text.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/book-half.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/book-half.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/book.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/book.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-star-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-star-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-star.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-star.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bookmark-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bookmark-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/boombox-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/boombox-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/boombox.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/boombox.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-icons.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-icons.json` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-icons.min.css` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-icons.scss` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-icons.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap-reboot.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap-reboot.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bootstrap.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bootstrap.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-bottom.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-bottom.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-center.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-center.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-inner.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-inner.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-left.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-left.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-middle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-middle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-outer.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-outer.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-right.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-right.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-style.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-style.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border-top.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border-top.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/border.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/border.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bounding-box-circles.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bounding-box-circles.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-down-left.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-down-left.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-down-right.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-down-right.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-down-left.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-down-left.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-down-right.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-down-right.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-left.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-left.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-right.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-right.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-up-left.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-up-left.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-up-right.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-up-right.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-in-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-in-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-left.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-left.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-right.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-right.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-up-left.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-up-left.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-up-right.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-up-right.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-arrow-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-seam-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-seam-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/box-seam.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/box-seam.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/boxes.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/boxes.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/braces-asterisk.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/braces-asterisk.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/braces.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/braces.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bricks.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bricks.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/briefcase.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/briefcase.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-alt-high-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-alt-high-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-alt-high.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-alt-high.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-high-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-high-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-high.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-high.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-low-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-low-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brightness-low.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brightness-low.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/broadcast-pin.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/broadcast-pin.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/broadcast.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/broadcast.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/browser-chrome.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/browser-chrome.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/browser-edge.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/browser-edge.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/browser-firefox.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/browser-firefox.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/browser-safari.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/browser-safari.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brush-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brush-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/brush.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/brush.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bug-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bug-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bug.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bug.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-add.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-add.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-dash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-dash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-exclamation.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-exclamation.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-add.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-add.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-dash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-dash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-exclamation.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-exclamation.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-gear.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-gear.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-lock.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-lock.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-gear.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-gear.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-lock.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-lock.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/building.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/building.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/buildings-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/buildings-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/buildings.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/buildings.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bus-front-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bus-front-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/bus-front.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/bus-front.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/c-circle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/c-circle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/c-square-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/c-square-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/c-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/c-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cake-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cake-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cake.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cake.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cake2-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cake2-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cake2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cake2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calculator-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calculator-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calculator.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calculator.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-date-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-date-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-date.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-date.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-day-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-day-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-day.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-day.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-month-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-month-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-month.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-month.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-week-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-week-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-week.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-week.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-check-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-check-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-date-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-date-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-date.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-date.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-day-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-day-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-day.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-day.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-event.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-event.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-minus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-minus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-month-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-month-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-month.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-month.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-range.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-range.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-week-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-week-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-week.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-week.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-x-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-x-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar2-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar2-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar3.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar3.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/calendar4-week.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/calendar4-week.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera-reels.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera-reels.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera-video-off.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera-video-off.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/camera2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/camera2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/car-front-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/car-front-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/car-front.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/car-front.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/card-checklist.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/card-checklist.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/card-heading.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/card-heading.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/card-list.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/card-list.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/card-text.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/card-text.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-check-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-check-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-dash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-dash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-plus-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-plus-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-x-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-x-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart3.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart3.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cart4.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cart4.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cash-coin.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cash-coin.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cassette.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cassette.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cc-circle-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cc-circle-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cc-circle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cc-circle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cc-square-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cc-square-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cc-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cc-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-dots.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-dots.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left-quote-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left-quote-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left-quote.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left-quote.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-left-text.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-left-text.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-quote-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-quote-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-quote.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-quote.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right-quote-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right-quote-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right-quote.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right-quote.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-right-text.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-right-text.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-dots.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-dots.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-quote-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-quote-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-quote.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-quote.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-square-text.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-square-text.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat-text.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat-text.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/chat.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/chat.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-check-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-check-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-data-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-data-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-data.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-data.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-heart-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-heart-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-minus-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-minus-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-minus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-minus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-plus-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-plus-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-pulse.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-pulse.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-x-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-x-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-check-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-check-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-data-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-data-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-data.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-data.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-heart-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-heart-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-minus-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-minus-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-minus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-minus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-plus-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-plus-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-pulse-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-pulse-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-pulse.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-pulse.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-x-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-x-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clipboard2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clipboard2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clock-history.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clock-history.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-arrow-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-arrow-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-arrow-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-download-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-download-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-download.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-download.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-drizzle-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-drizzle-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-drizzle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-drizzle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-hail-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-hail-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-hail.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-hail.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-haze.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-haze.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-lightning-rain-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-lightning-rain-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-lightning-rain.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-lightning-rain.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-lightning.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-lightning.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-minus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-minus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-moon-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-moon-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-moon.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-moon.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-rain-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-rain-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-rain-heavy-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-rain-heavy-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-rain-heavy.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-rain-heavy.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-rain.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-rain.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-sleet-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-sleet-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-sleet.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-sleet.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-snow-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-snow-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-snow.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-snow.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-sun-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-sun-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-sun.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-sun.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-upload-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-upload-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud-upload.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud-upload.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cloud.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cloud.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/clouds.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/clouds.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/code-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/code-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/coin.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/coin.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/collection-play.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/collection-play.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cone-striped.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cone-striped.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/controller.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/controller.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cookie.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cookie.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cpu-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cpu-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cpu.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cpu.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/credit-card-2-front-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/credit-card-2-front-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/credit-card-2-front.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/credit-card-2-front.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/crosshair.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/crosshair.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/crosshair2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/crosshair2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cup-hot-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cup-hot-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cup-hot.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cup-hot.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cup-straw.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cup-straw.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/currency-bitcoin.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/currency-bitcoin.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/currency-dollar.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/currency-dollar.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/currency-exchange.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/currency-exchange.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/currency-pound.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/currency-pound.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/cursor-text.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/cursor-text.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dash-circle-dotted.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dash-circle-dotted.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dash-square-dotted.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dash-square-dotted.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-add.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-add.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-dash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-dash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-exclamation.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-exclamation.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-add.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-add.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-dash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-dash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-exclamation.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-exclamation.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-gear.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-gear.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-lock.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-lock.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-gear.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-gear.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-lock.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-lock.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/database.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/database.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/device-hdd-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/device-hdd-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/device-hdd.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/device-hdd.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/device-ssd-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/device-ssd-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/device-ssd.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/device-ssd.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/diagram-2-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/diagram-2-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/diagram-2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/diagram-2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/diagram-3-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/diagram-3-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/diagram-3.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/diagram-3.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-5.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-5.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dice-6.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dice-6.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/discord.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/discord.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/display.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/display.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dpad-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dpad-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dpad.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dpad.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/dribbble.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/dribbble.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/droplet-half.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/droplet-half.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/droplet.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/droplet.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/duffle-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/duffle-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/duffle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/duffle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ear.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ear.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/earbuds.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/earbuds.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/egg-fried.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/egg-fried.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-angry-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-angry-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-angry.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-angry.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-astonished-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-astonished-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-astonished.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-astonished.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-dizzy-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-dizzy-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-dizzy.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-dizzy.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-frown.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-frown.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-grimace-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-grimace-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-grimace.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-grimace.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-grin-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-grin-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-grin.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-grin.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-heart-eyes-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-heart-eyes-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-heart-eyes.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-heart-eyes.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-kiss-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-kiss-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-kiss.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-kiss.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-laughing-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-laughing-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-smile-upside-down-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-smile-upside-down-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-smile-upside-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-smile-upside-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-smile.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-smile.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-sunglasses-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-sunglasses-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-sunglasses.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-sunglasses.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-tear-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-tear-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-tear.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-tear.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-wink-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-wink-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/emoji-wink.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/emoji-wink.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-arrow-down-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-arrow-down-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-arrow-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-arrow-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-arrow-up-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-arrow-up-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-arrow-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-at-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-at-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-at.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-at.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-check-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-check-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-dash-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-dash-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-dash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-dash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-exclamation-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-exclamation-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-exclamation.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-exclamation.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-heart-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-heart-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-open-heart-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-open-heart-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-open-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-open-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-open.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-open.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-paper-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-paper-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-paper-heart-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-paper-heart-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-paper-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-paper-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-paper.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-paper.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-plus-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-plus-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-slash-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-slash-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-x-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-x-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/envelope-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/envelope-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ethernet.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ethernet.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ev-front-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ev-front-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ev-front.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ev-front.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ev-station-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ev-station-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ev-station.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ev-station.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-diamond.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-diamond.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-octagon-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-octagon-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-octagon.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-octagon.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/exclamation-triangle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/exclamation-triangle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eye-slash-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eye-slash-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eye-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eye-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/eye.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/eye.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fan.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fan.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/feather.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/feather.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-bar-graph.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-bar-graph.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-binary-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-binary-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-binary.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-binary.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-bar-graph-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-bar-graph-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-bar-graph.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-bar-graph.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-binary-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-binary-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-binary.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-binary.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-code.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-code.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-easel-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-easel-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-easel.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-easel.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-font.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-font.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-image-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-image-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-lock-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-lock-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-lock.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-lock.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-medical-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-medical-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-medical.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-medical.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-music-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-music-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-music.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-music.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-pdf-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-pdf-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-pdf.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-pdf.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-richtext-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-richtext-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-richtext.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-richtext.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-slides-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-slides-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-slides.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-slides.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-zip-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-zip-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-earmark-zip.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-earmark-zip.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-easel-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-easel-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-easel.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-easel.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-lock-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-lock-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-lock.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-lock.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-medical.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-medical.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-music.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-music.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-pdf-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-pdf-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-pdf.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-richtext.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-richtext.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-slides-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-slides-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-slides.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-slides.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-word.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-word.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-zip-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-zip-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/file-zip.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-aac.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-aac.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-bmp.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-bmp.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-cs.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-cs.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-css.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-css.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-csv.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-csv.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-doc.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-doc.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-docx.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-docx.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-exe.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-exe.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-gif.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-gif.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-heic.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-heic.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-html.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-html.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-java.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-java.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-jpg.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-jpg.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-js.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-js.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-json.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-json.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-jsx.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-jsx.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-key.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-key.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-m4p.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-m4p.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-md.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-md.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-mdx.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-mdx.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-mov.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-mov.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-mp3.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-mp3.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-mp4.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-mp4.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-otf.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-otf.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-pdf.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-pdf.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-php.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-php.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-png.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-png.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-ppt.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-ppt.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-pptx.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-pptx.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-psd.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-psd.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-py.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-py.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-raw.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-raw.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-rb.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-rb.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-sass.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-sass.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-scss.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-scss.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-sh.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-sh.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-sql.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-sql.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-svg.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-svg.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-tiff.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-tiff.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-tsx.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-tsx.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-txt.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-txt.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-wav.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-wav.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-woff.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-woff.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-xls.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-xls.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-xlsx.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-xlsx.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-xml.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-xml.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/filetype-yml.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/filetype-yml.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fingerprint.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/flag-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/flag-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/flag.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/flag.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/floppy-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/floppy-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/floppy.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/floppy.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/floppy2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/floppy2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/flower1.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/flower1.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/flower2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/flower2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/flower3.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/flower3.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-minus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-minus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-symlink-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-symlink-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-symlink.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-symlink.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/folder2-open.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/folder2-open.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/forward.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/forward.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fuel-pump-diesel-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fuel-pump-diesel-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fuel-pump-diesel.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fuel-pump-diesel.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fuel-pump-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fuel-pump-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fuel-pump.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fuel-pump.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fullscreen-exit.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fullscreen-exit.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fullscreen.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fullscreen.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gear-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gear-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gear-wide-connected.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gear-wide-connected.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gear-wide.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gear-wide.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gear.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gear.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gem.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gem.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gender-trans.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gender-trans.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/geo-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/geo-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/geo.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/geo.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gift-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gift-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gift.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gift.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/git.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/git.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/github.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/github.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/globe-americas.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/globe-americas.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/globe-asia-australia.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/globe-asia-australia.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/globe-central-south-asia.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/globe-central-south-asia.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/globe-europe-africa.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/globe-europe-africa.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/globe.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/globe.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/globe2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/globe2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/google.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/google.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/gpu-card.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/gpu-card.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-3x2-gap-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-3x2-gap-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-3x2-gap.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-3x2-gap.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-3x3-gap-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-3x3-gap-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-3x3-gap.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-3x3-gap.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/grid.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/grid.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-index-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-index-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-index-thumb-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-index-thumb-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-index-thumb.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-index-thumb.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-index.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-index.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-thumbs-down-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-thumbs-down-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-thumbs-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-thumbs-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-thumbs-up-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-thumbs-up-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hand-thumbs-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hand-thumbs-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/handbag.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/handbag.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdd-network.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdd-network.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdd-rack.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdd-rack.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdd-stack.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdd-stack.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hdd.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hdd.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/headset-vr.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/headset-vr.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heart-pulse-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heart-pulse-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heart-pulse.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heart-pulse.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/heartbreak.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/heartbreak.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/highlighter.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/highlighter.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hospital-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hospital-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hospital.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hospital.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hourglass-bottom.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hourglass-bottom.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hourglass-split.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hourglass-split.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hourglass-top.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hourglass-top.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hourglass.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hourglass.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-add-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-add-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-add.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-add.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-check-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-check-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-dash-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-dash-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-down-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-down-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-exclamation-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-exclamation-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-exclamation.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-exclamation.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-gear-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-gear-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-gear.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-gear.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-lock-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-lock-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-lock.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-lock.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-slash-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-slash-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-up-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-up-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-x-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-x-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/house-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/house-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/houses-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/houses-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/houses.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/houses.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/hypnotize.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/hypnotize.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/images.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/images.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/inbox.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/inbox.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/inboxes-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/inboxes-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/inboxes.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/inboxes.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/incognito.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/incognito.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/index.html` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/index.html`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/info-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/info-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/input-cursor-text.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/input-cursor-text.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/instagram.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/instagram.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-album.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-album.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-arrow-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-arrow-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-arrow-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-bookmark-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-bookmark-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-bookmark.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-bookmark.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-code.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-code.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-medical.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-medical.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-minus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-minus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-richtext.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-richtext.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-text.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-text.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journal-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journal-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/journals.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/journals.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/joystick.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/joystick.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/kanban.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/kanban.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/key.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/key.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/keyboard-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/keyboard-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/keyboard.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/keyboard.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lamp-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lamp-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lamp.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lamp.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layer-backward.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layer-backward.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layer-forward.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layer-forward.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-text-sidebar-reverse.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-text-sidebar-reverse.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-text-sidebar.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-text-sidebar.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/layout-text-window-reverse.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/layout-text-window-reverse.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/life-preserver.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/life-preserver.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lightbulb-off-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lightbulb-off-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lightbulb-off.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lightbulb-off.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lightbulb.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lightbulb.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/line.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/line.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/link-45deg.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/link-45deg.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/linkedin.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/linkedin.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-columns-reverse.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-columns-reverse.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-columns.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-columns.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-ol.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-ol.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-stars.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-stars.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/list-task.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/list-task.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/luggage-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/luggage-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/luggage.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/luggage.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lungs-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lungs-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/lungs.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/lungs.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/magic.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/magic.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mailbox-flag.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mailbox-flag.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/markdown.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/markdown.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mastodon.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mastodon.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/megaphone-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/megaphone-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/megaphone.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/megaphone.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/memory.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/memory.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-app-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-app-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-app.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-app.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-button-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-button-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-button-wide-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-button-wide-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-button-wide.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-button-wide.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-button.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-button.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/menu-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/menu-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/messenger.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/messenger.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/meta.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/meta.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mic-mute-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mic-mute-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mic-mute.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mic-mute.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/microsoft-teams.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/microsoft-teams.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/minecart-loaded.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/minecart-loaded.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/modem.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/modem.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/moisture.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/moisture.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/moon-stars-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/moon-stars-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/moon-stars.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/moon-stars.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/moon.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/moon.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mortarboard-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mortarboard-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mortarboard.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mortarboard.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/motherboard-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/motherboard-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/motherboard.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/motherboard.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mouse3-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mouse3-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/mouse3.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/mouse3.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/music-note-list.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/music-note-list.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/newspaper.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/newspaper.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/nintendo-switch.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/nintendo-switch.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/noise-reduction.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/noise-reduction.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/nvidia.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/nvidia.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/nvme-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/nvme-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/nvme.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/nvme.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/optical-audio.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/optical-audio.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/outlet.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/outlet.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/paint-bucket.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/paint-bucket.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/palette.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/palette.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/palette2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/palette2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-check-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-check-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-exclamation-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-exclamation-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-exclamation.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-exclamation.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-minus-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-minus-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-minus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-minus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-plus-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-plus-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-question-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-question-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/patch-question.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/patch-question.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/paypal.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/paypal.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pc-display-horizontal.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pc-display-horizontal.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pc-display.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pc-display.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pci-card-network.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pci-card-network.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pci-card-sound.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pci-card-sound.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pen.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pen.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pencil-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pencil-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pencil-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pencil-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pencil.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pencil.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/people.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/people.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-add.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-add.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-arms-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-arms-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-bounding-box.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-bounding-box.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-dash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-dash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-exclamation.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-exclamation.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill-gear.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill-gear.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-fill-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-fill-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-gear.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-gear.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-lock.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-lock.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-rolodex.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-rolodex.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-vcard-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-vcard-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-vcard.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-vcard.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-walking.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-walking.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-wheelchair.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-wheelchair.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/person-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/person-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/phone-flip.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/phone-flip.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/phone-vibrate-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/phone-vibrate-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/phone-vibrate.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/phone-vibrate.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/piggy-bank-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/piggy-bank-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/piggy-bank.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/piggy-bank.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pin-angle-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pin-angle-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pin-angle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pin-angle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pin-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pin-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pin.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pin.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/pinterest.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/pinterest.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/playstation.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/playstation.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plug-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plug-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plug.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plug.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plugin.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plugin.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plus-circle-dotted.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plus-circle-dotted.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/plus-square-dotted.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/plus-square-dotted.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postage-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postage-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postage-heart-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postage-heart-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postage-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postage-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postage.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postage.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postcard-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postcard-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postcard-heart-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postcard-heart-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postcard-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postcard-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/postcard.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/postcard.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/prescription.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/prescription.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/printer.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/printer.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/puzzle-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/puzzle-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/puzzle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/puzzle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/qr-code-scan.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/qr-code-scan.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/qr-code.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/qr-code.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-circle-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-circle-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-circle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-circle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-diamond-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-diamond-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-diamond.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-diamond.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-lg.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-lg.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-octagon-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-octagon-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-octagon.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-octagon.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-square-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-square-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question-square.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question-square.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/question.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/question.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/quora.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/quora.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/quote.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/quote.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/radioactive.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/radioactive.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/receipt-cutoff.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/receipt-cutoff.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/receipt.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/receipt.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/recycle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/recycle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reddit.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reddit.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/regex.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/regex.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/repeat-1.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/repeat-1.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reply-all-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reply-all-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reply-all.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reply-all.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/reply.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/reply.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/robot.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/robot.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rocket-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rocket-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rocket-takeoff-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rocket-takeoff-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rocket-takeoff.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rocket-takeoff.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/rocket.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/rocket.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/router-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/router-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/router.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/router.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/safe-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/safe-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/safe.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/safe.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/safe2-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/safe2-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/safe2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/safe2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/screwdriver.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/screwdriver.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sd-card-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sd-card-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sd-card.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sd-card.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-arrow-down-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-arrow-down-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-arrow-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-arrow-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-arrow-up-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-arrow-up-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-arrow-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-check-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-check-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-dash-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-dash-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-exclamation-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-exclamation-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-exclamation.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-exclamation.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-plus-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-plus-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-slash-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-slash-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-x-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-x-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/send-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/send-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/server.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/server.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shadows.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shadows.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-exclamation.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-exclamation.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-fill-check.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-fill-check.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-fill-exclamation.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-fill-exclamation.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-fill-minus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-fill-minus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-fill-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-fill-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-fill-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-fill-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-lock-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-lock-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-lock.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-lock.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-minus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-minus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-shaded.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-shaded.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-slash-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-slash-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shield.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shield.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shop-window.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shop-window.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shop.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shop.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/shuffle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/shuffle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-dead-end-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-dead-end-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-dead-end.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-dead-end.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-do-not-enter-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-do-not-enter-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-do-not-enter.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-do-not-enter.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-intersection-y.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-intersection-y.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-intersection.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-intersection.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-merge-left-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-merge-left-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-merge-left.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-merge-left.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-merge-right-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-merge-right-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-merge-right.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-merge-right.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-no-left-turn.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-no-left-turn.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-no-right-turn.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-no-right-turn.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-railroad-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-railroad-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-railroad.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-railroad.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-stop-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-stop-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-stop-lights.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-stop-lights.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-stop.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-stop.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-left.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-left.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-right.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-right.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-slight-left-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-slight-left-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-slight-left.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-slight-left.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-slight-right-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-slight-right-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-turn-slight-right.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-turn-slight-right.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-yield-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-yield-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sign-yield.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sign-yield.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/signal.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/signal.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sim-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sim-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sim-slash-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sim-slash-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sim-slash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sim-slash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sim.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sim.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sina-weibo.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sina-weibo.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/skype.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/skype.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/slack.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/slack.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sliders2-vertical.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sliders2-vertical.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sliders2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sliders2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/smartwatch.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/smartwatch.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/snapchat.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/snapchat.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/snow.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/snow.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/snow2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/snow2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/snow3.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/snow3.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-alpha-down-alt.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-alpha-down-alt.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-alpha-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-alpha-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-alpha-up-alt.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-alpha-up-alt.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-alpha-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-alpha-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-numeric-down-alt.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-numeric-down-alt.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-numeric-down.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-numeric-down.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-numeric-up-alt.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-numeric-up-alt.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sort-numeric-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sort-numeric-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/soundwave.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/soundwave.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sourceforge.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sourceforge.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/speedometer.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/speedometer.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/speedometer2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/speedometer2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/spellcheck.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/spellcheck.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/spotify.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/spotify.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stack.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stack.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/star-half.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/star-half.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/star.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/star.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stars.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stars.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/steam.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/steam.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stickies.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stickies.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stoplights.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stoplights.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stopwatch.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stopwatch.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/stripe.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/stripe.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suit-club.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suit-club.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suit-heart.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suit-heart.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suit-spade.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suit-spade.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/suitcase.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/suitcase.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sun-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sun-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sun.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sun.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sunglasses.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sunglasses.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sunrise-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sunrise-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sunrise.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sunrise.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sunset-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sunset-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/sunset.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/sunset.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/taxi-front-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/taxi-front-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/taxi-front.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/taxi-front.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telegram.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telegram.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-forward-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-forward-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-forward.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-forward.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-inbound-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-inbound-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-inbound.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-inbound.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-minus-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-minus-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-minus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-minus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-outbound-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-outbound-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-outbound.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-outbound.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-plus-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-plus-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-x-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-x-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/telephone.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/telephone.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tencent-qq.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tencent-qq.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/terminal-dash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/terminal-dash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/terminal-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/terminal-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/terminal-split.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/terminal-split.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/terminal-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/terminal-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/text-indent-left.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/text-indent-left.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/textarea-resize.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/textarea-resize.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/textarea-t.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/textarea-t.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/thermometer-snow.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/thermometer-snow.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/thermometer-sun.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/thermometer-sun.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/threads-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/threads-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/threads.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/threads.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ticket-detailed-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ticket-detailed-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ticket-detailed.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ticket-detailed.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ticket-perforated-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ticket-perforated-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ticket-perforated.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ticket-perforated.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tools.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tools.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tornado.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tornado.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/train-freight-front-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/train-freight-front-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/train-freight-front.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/train-freight-front.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/train-front-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/train-front-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/train-front.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/train-front.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/train-lightrail-front-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/train-lightrail-front-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/train-lightrail-front.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/train-lightrail-front.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/translate.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/translate.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/transparency.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/transparency.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trash2-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trash2-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trash3-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trash3-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trash3.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trash3.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tree.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tree.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trello.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trello.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/triangle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/triangle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trophy-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trophy-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/trophy.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/trophy.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/truck-flatbed.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/truck-flatbed.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/truck-front-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/truck-front-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/truck-front.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/truck-front.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/truck.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/truck.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tsunami.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tsunami.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/tv.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/tv.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/twitter.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/twitter.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-h3.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-h3.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-h5.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-h5.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-h6.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-h6.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type-strikethrough.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/type.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/type.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ubuntu.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ubuntu.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ui-checks-grid.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ui-checks-grid.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ui-checks.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ui-checks.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/ui-radios.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/ui-radios.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/umbrella-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/umbrella-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/umbrella.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/umbrella.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/unity.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/unity.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/upc-scan.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/upc-scan.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-plug.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-plug.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/usb-symbol.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/usb-symbol.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/valentine.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/valentine.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/valentine2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/valentine2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/vector-pen.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/vector-pen.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/vignette.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/vignette.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/vimeo.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/vimeo.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/virus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/virus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/virus2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/virus2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/volume-mute.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/volume-mute.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/volume-up-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/volume-up-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/volume-up.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/volume-up.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wallet-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wallet-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/watch.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/watch.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/water.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/water.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/webcam-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/webcam-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/webcam.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/webcam.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wechat.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wechat.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/whatsapp.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/whatsapp.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wifi-1.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wifi-1.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wifi-2.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wifi-2.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wifi-off.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wifi-off.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wifi.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wifi.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wikipedia.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wikipedia.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-dash.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-dash.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-desktop.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-desktop.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-dock.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-dock.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-plus.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-plus.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-stack.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-stack.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/window-x.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/window-x.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wordpress.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wordpress.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wrench-adjustable-circle-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wrench-adjustable-circle-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wrench-adjustable-circle.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wrench-adjustable-circle.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wrench-adjustable.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wrench-adjustable.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/wrench.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/wrench.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x-diamond.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x-diamond.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x-octagon-fill.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x-octagon-fill.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/x-octagon.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/x-octagon.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/xbox.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/xbox.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/yelp.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/yelp.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/youtube.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/youtube.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/zoom-in.svg` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/zoom-in.svg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fonts/bootstrap-icons.woff` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/bootstrap-icons/fonts/bootstrap-icons.woff2` & `boatbuddy-0.9.5/BoatBuddy/static/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/ol/ol.js` & `boatbuddy-0.9.5/BoatBuddy/static/ol/ol.js`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/static/ol/ol.js.map` & `boatbuddy-0.9.5/BoatBuddy/static/ol/ol.js.map`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/BoatBuddy/templates/base.html` & `boatbuddy-0.9.5/BoatBuddy/templates/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     <link rel="stylesheet" href="/static/bootstrap/css/bootstrap.css">
     <link rel="stylesheet" href="/static/bootstrap-icons/bootstrap-icons.css">
     <script src="/static/jquery-3.7.1.min.js"></script>
     <script src="/static/popper.min.js"></script>
     <script src="/static/bootstrap/js/bootstrap.min.js"></script>
     <script src="/static/gauge.min.js"></script>
     <script src="/static/GaugeMeter.js"></script>
-    <script src="/static/CustomGaugeMeter.js"></script>
     <script src="/static/ol/ol.js"></script>
 
     <!-- Custom CSS -->
     <link rel="stylesheet" href="/static/main.css" type="text/css">
     <link rel="shortcut icon" href="/static/favicon.ico">
     <title>{{application_name}} v{{application_version}}</title>
 </head>
```

### Comparing `boatbuddy-0.9.4/BoatBuddy/templates/index.html` & `boatbuddy-0.9.5/BoatBuddy/templates/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -580,14 +580,15 @@
             } else if (currentItem['style'] == 'current_gauge') {
                 gaugeDiv.setAttribute("data-append", "A");
                 gaugeDiv.setAttribute("data-theme", "Red-Gold-Green");
                 gaugeDiv.setAttribute("data-width", "15");
                 gaugeDiv.setAttribute("data-style", "Arch");
                 gaugeDiv.setAttribute("data-text_size", "0.22");
                 gaugeDiv.setAttribute("data-showvalue", true);
+                gaugeDiv.setAttribute("data-middle_value_format", true);
             }
 
             col.appendChild(gaugeDiv)
 
             elementsList[currentItem['order']] = col;
         } else if (currentItem['type'] == 'list') {
             // Create a new col element
@@ -1473,15 +1474,15 @@
                 }
 
                 if (document.getElementById("water_tank_gauge") !== null) {
                     $("#water_tank_gauge").gaugeMeter({used:parseInt(data['water_tank'])});
                 }
 
                 if (document.getElementById("housing_battery_current_gauge") !== null) {
-                    $("#housing_battery_current_gauge").customGaugeMeter({used:parseFloat(data['housing_battery_current'])});
+                    $("#housing_battery_current_gauge").gaugeMeter({used:parseFloat(data['housing_battery_current'])});
                 }
 
                 if (document.getElementById('active_input_source') !== null) {
                     document.getElementById('active_input_source').innerHTML = data['active_input_source'];
                 }
 
                 if (document.getElementById('ve_bus_state') !== null) {
@@ -1779,15 +1780,14 @@
         }
     });
 }
 
 $(document).ready(function() {
     $('#loading_modal').modal('show');
     $(".GaugeMeter").gaugeMeter();
-    $(".GaugeMeter").customGaugeMeter();
     // Call the refreshData function every 1 seconds
     setInterval(refreshData, 1000);
     setInterval(refreshAnchorData, 1000);
     setInterval(refreshNMEAInstrumentsData, 1000);
     setInterval(getGPSPosition, 2000);
 });
```

### Comparing `boatbuddy-0.9.4/resources/.DS_Store` & `boatbuddy-0.9.5/resources/.DS_Store`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/resources/logo/Boat Buddy - No Bg.png` & `boatbuddy-0.9.5/resources/logo/Boat Buddy - No Bg.png`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/resources/logo/Boat Buddy.png` & `boatbuddy-0.9.5/resources/logo/Boat Buddy.png`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/resources/manuals/.DS_Store` & `boatbuddy-0.9.5/resources/manuals/.DS_Store`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/resources/manuals/CCGX-Modbus-TCP-register-list-2.90.xlsx` & `boatbuddy-0.9.5/resources/manuals/CCGX-Modbus-TCP-register-list-2.90.xlsx`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/resources/manuals/NMEA0183 Sentences Table.jpg` & `boatbuddy-0.9.5/resources/manuals/NMEA0183 Sentences Table.jpg`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/resources/manuals/NMEA0183.pdf` & `boatbuddy-0.9.5/resources/manuals/NMEA0183.pdf`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/.gitignore` & `boatbuddy-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/LICENSE` & `boatbuddy-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/README.md` & `boatbuddy-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `boatbuddy-0.9.4/pyproject.toml` & `boatbuddy-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "BoatBuddy"
-version = "0.9.4"
+version = "0.9.5"
 authors = [
     { name = "Joe Zeitouny", email = "joezeitouny@gmail.com" },
 ]
 description = "A suite of tools to help collecting NMEA0183 and other marine metrics in a digital logbook format"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `boatbuddy-0.9.4/PKG-INFO` & `boatbuddy-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BoatBuddy
-Version: 0.9.4
+Version: 0.9.5
 Summary: A suite of tools to help collecting NMEA0183 and other marine metrics in a digital logbook format
 Project-URL: Homepage, https://boatbuddy.site
 Project-URL: Bug Tracker, https://github.com/joezeitouny/BoatBuddy/issues
 Author-email: Joe Zeitouny <joezeitouny@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

