# Comparing `tmp/fuglu-1.4.0.tar.gz` & `tmp/fuglu-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuglu-1.4.0.tar", last modified: Fri Sep 15 03:25:00 2023, max compression
+gzip compressed data, was "fuglu-1.5.0.tar", last modified: Thu Apr 11 09:00:28 2024, max compression
```

## Comparing `fuglu-1.4.0.tar` & `fuglu-1.5.0.tar`

### file list

```diff
@@ -1,160 +1,164 @@
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.260799 fuglu-1.4.0/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      597 2023-01-04 08:05:48.000000 fuglu-1.4.0/LICENSE
--rw-r--r--   0 lukas     (1000) lukas     (1000)      171 2022-01-14 02:33:11.000000 fuglu-1.4.0/MANIFEST.in
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1909 2023-09-15 03:25:00.260799 fuglu-1.4.0/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)      869 2022-01-14 02:33:11.000000 fuglu-1.4.0/README.md
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3152 2023-01-04 08:05:48.000000 fuglu-1.4.0/compareconfig.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/conf/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      128 2022-01-14 02:33:11.000000 fuglu-1.4.0/conf/archive.regex.dist
--rw-r--r--   0 lukas     (1000) lukas     (1000)    13032 2023-09-15 03:16:48.000000 fuglu-1.4.0/conf/fuglu.conf.dist
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2090 2022-01-14 02:33:11.000000 fuglu-1.4.0/conf/fuglu_mrtg.cfg.dist
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1760 2022-01-14 02:33:11.000000 fuglu-1.4.0/conf/logging.conf.dist
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/conf/rules/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      627 2022-01-14 02:33:11.000000 fuglu-1.4.0/conf/rules/default-archivefiletypes.conf.dist
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1099 2022-01-14 02:33:11.000000 fuglu-1.4.0/conf/rules/default-archivenames.conf.dist
--rw-r--r--   0 lukas     (1000) lukas     (1000)     6694 2022-02-08 12:29:26.000000 fuglu-1.4.0/conf/rules/default-filenames.conf.dist
--rw-r--r--   0 lukas     (1000) lukas     (1000)      797 2022-01-14 02:33:11.000000 fuglu-1.4.0/conf/rules/default-filetypes.conf.dist
--rw-r--r--   0 lukas     (1000) lukas     (1000)      335 2022-01-14 02:33:11.000000 fuglu-1.4.0/conf/skipplugins.regex.dist
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/conf/templates/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      152 2022-01-14 02:33:11.000000 fuglu-1.4.0/conf/templates/blockedfile.tmpl.dist
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/doc/
--rw-r--r--   0 lukas     (1000) lukas     (1000)    27403 2023-09-15 03:22:12.000000 fuglu-1.4.0/doc/CHANGELOG
--rw-r--r--   0 lukas     (1000) lukas     (1000)      368 2022-01-14 02:33:11.000000 fuglu-1.4.0/doc/INSTALL
--rw-r--r--   0 lukas     (1000) lukas     (1000)       57 2022-01-14 02:33:11.000000 fuglu-1.4.0/pyproject.toml
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.252799 fuglu-1.4.0/scripts/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/scripts/mrtg/
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)       71 2022-01-14 02:33:11.000000 fuglu-1.4.0/scripts/mrtg/fuglu_mrtg.sh
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.252799 fuglu-1.4.0/scripts/startscripts/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/scripts/startscripts/arch/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      271 2022-01-14 02:33:11.000000 fuglu-1.4.0/scripts/startscripts/arch/fuglu.service
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.252799 fuglu-1.4.0/scripts/startscripts/centos_rhel/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/scripts/startscripts/centos_rhel/6/
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     1107 2022-01-14 02:33:11.000000 fuglu-1.4.0/scripts/startscripts/centos_rhel/6/fuglu
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/scripts/startscripts/centos_rhel/7/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      306 2022-01-14 02:33:11.000000 fuglu-1.4.0/scripts/startscripts/centos_rhel/7/fuglu.service
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.252799 fuglu-1.4.0/scripts/startscripts/debian/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/scripts/startscripts/debian/7/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1306 2022-01-14 02:33:11.000000 fuglu-1.4.0/scripts/startscripts/debian/7/fuglu
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/scripts/startscripts/debian/8/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      274 2022-01-14 02:33:11.000000 fuglu-1.4.0/scripts/startscripts/debian/8/fuglu.service
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.252799 fuglu-1.4.0/scripts/startscripts/suse/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/scripts/startscripts/suse/13/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1677 2022-01-14 02:33:11.000000 fuglu-1.4.0/scripts/startscripts/suse/13/fuglu
--rw-r--r--   0 lukas     (1000) lukas     (1000)      139 2023-09-15 03:25:00.260799 fuglu-1.4.0/setup.cfg
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2045 2022-01-14 02:33:11.000000 fuglu-1.4.0/setup.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.252799 fuglu-1.4.0/src/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/src/fuglu/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      849 2023-09-15 03:22:12.000000 fuglu-1.4.0/src/fuglu/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     6113 2023-04-14 12:12:09.000000 fuglu-1.4.0/src/fuglu/addrcheck.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    31187 2023-07-07 14:24:41.000000 fuglu-1.4.0/src/fuglu/asyncprocpool.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    12536 2023-01-27 10:16:08.000000 fuglu-1.4.0/src/fuglu/bounce.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    14153 2023-06-02 08:06:05.000000 fuglu-1.4.0/src/fuglu/caching.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/src/fuglu/connectors/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      117 2022-01-14 02:33:11.000000 fuglu-1.4.0/src/fuglu/connectors/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)   105552 2023-09-14 01:26:24.000000 fuglu-1.4.0/src/fuglu/connectors/asyncmilterconnector.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5772 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/connectors/check.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    16049 2023-05-16 15:34:42.000000 fuglu-1.4.0/src/fuglu/connectors/esmtpconnector.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    44632 2023-09-14 01:26:24.000000 fuglu-1.4.0/src/fuglu/connectors/milterconnector.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     8502 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/connectors/ncconnector.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    20142 2023-05-16 15:34:42.000000 fuglu-1.4.0/src/fuglu/connectors/smtpconnector.py
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)    73702 2023-07-18 14:36:25.000000 fuglu-1.4.0/src/fuglu/core.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5154 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/daemon.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    43229 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/debug.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/src/fuglu/extensions/
--rw-r--r--   0 lukas     (1000) lukas     (1000)       94 2022-01-14 02:33:11.000000 fuglu-1.4.0/src/fuglu/extensions/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    14437 2023-09-15 03:22:12.000000 fuglu-1.4.0/src/fuglu/extensions/aioredisext.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     6187 2023-06-19 13:28:56.000000 fuglu-1.4.0/src/fuglu/extensions/dnsquery.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2032 2023-06-19 13:28:56.000000 fuglu-1.4.0/src/fuglu/extensions/elastic.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    42326 2023-07-26 11:28:16.000000 fuglu-1.4.0/src/fuglu/extensions/filearchives.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5204 2023-06-19 13:28:56.000000 fuglu-1.4.0/src/fuglu/extensions/filetype.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2443 2023-06-19 13:28:56.000000 fuglu-1.4.0/src/fuglu/extensions/fuzzyhashlib.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     9436 2023-06-19 13:28:56.000000 fuglu-1.4.0/src/fuglu/extensions/redisext.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    29376 2023-05-30 18:25:59.000000 fuglu-1.4.0/src/fuglu/extensions/sql.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2306 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/funkyconsole.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/src/fuglu/lib/
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2022-01-14 02:33:11.000000 fuglu-1.4.0/src/fuglu/lib/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    22368 2022-12-20 14:48:46.000000 fuglu-1.4.0/src/fuglu/lib/patcheddkimlib.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/src/fuglu/lib/patchedemail/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      351 2023-02-22 15:54:48.000000 fuglu-1.4.0/src/fuglu/lib/patchedemail/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4608 2023-02-22 15:54:48.000000 fuglu-1.4.0/src/fuglu/lib/patchedemail/message.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    22782 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/lib/patchedlibmilter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    26750 2022-10-31 13:25:01.000000 fuglu-1.4.0/src/fuglu/lib/ppymilterbase.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1827 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/loghandlers.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    15186 2023-01-04 11:07:44.000000 fuglu-1.4.0/src/fuglu/logtools.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    63580 2023-07-13 18:06:15.000000 fuglu-1.4.0/src/fuglu/mailattach.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     8784 2023-06-02 08:06:05.000000 fuglu-1.4.0/src/fuglu/mixins.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/src/fuglu/mplugins/
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2022-01-14 02:33:11.000000 fuglu-1.4.0/src/fuglu/mplugins/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3455 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/mplugins/demo.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     8376 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/mshared.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.260799 fuglu-1.4.0/src/fuglu/plugins/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1025 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/plugins/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    52308 2023-09-14 01:25:46.000000 fuglu-1.4.0/src/fuglu/plugins/a_logging.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5827 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/plugins/a_statsd.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    54635 2023-08-24 13:11:49.000000 fuglu-1.4.0/src/fuglu/plugins/antivirus.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    37718 2023-01-27 08:33:23.000000 fuglu-1.4.0/src/fuglu/plugins/archive.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    86949 2023-07-12 14:51:15.000000 fuglu-1.4.0/src/fuglu/plugins/attachment.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4248 2023-04-27 06:04:04.000000 fuglu-1.4.0/src/fuglu/plugins/bacn.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)   106007 2023-09-01 05:50:16.000000 fuglu-1.4.0/src/fuglu/plugins/call_ahead.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    21498 2023-08-14 15:05:50.000000 fuglu-1.4.0/src/fuglu/plugins/clamav.py
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)    20824 2023-03-17 11:47:38.000000 fuglu-1.4.0/src/fuglu/plugins/dataprovider.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    19863 2023-07-18 06:58:08.000000 fuglu-1.4.0/src/fuglu/plugins/decision.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3081 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/plugins/delay.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5558 2023-09-14 09:19:59.000000 fuglu-1.4.0/src/fuglu/plugins/dnsdata.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)   124687 2023-05-31 09:46:02.000000 fuglu-1.4.0/src/fuglu/plugins/domainauth.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    26066 2023-07-26 18:42:23.000000 fuglu-1.4.0/src/fuglu/plugins/fuzor.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5868 2023-05-23 08:26:55.000000 fuglu-1.4.0/src/fuglu/plugins/geoip.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    14990 2023-04-13 12:13:13.000000 fuglu-1.4.0/src/fuglu/plugins/knownsubject.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    38405 2023-09-15 02:50:54.000000 fuglu-1.4.0/src/fuglu/plugins/mailcopy.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     6704 2023-05-30 18:25:59.000000 fuglu-1.4.0/src/fuglu/plugins/messagesize.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    13528 2023-02-17 09:22:32.000000 fuglu-1.4.0/src/fuglu/plugins/originpolicy.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    63618 2023-09-01 05:50:16.000000 fuglu-1.4.0/src/fuglu/plugins/outpolicy.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    85466 2023-09-01 01:53:54.000000 fuglu-1.4.0/src/fuglu/plugins/p_blwl.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3368 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/plugins/p_debug.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3340 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/plugins/p_fraction.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5071 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/plugins/p_skipper.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.260799 fuglu-1.4.0/src/fuglu/plugins/ratelimit/
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2022-01-14 02:33:11.000000 fuglu-1.4.0/src/fuglu/plugins/ratelimit/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     8018 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/plugins/ratelimit/dynfunction.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    17582 2023-07-27 14:05:41.000000 fuglu-1.4.0/src/fuglu/plugins/ratelimit/helperfuncs.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    42777 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/plugins/ratelimit/main.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.260799 fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1508 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1187 2023-06-15 06:24:39.000000 fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/always_hit.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1573 2023-06-15 06:24:39.000000 fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/backendint.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     7639 2023-06-15 06:24:39.000000 fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/fixed_ratelimit.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     6148 2023-06-15 06:24:39.000000 fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/sliding_log_ratelimit.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    15367 2023-06-15 06:24:39.000000 fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/sliding_window_ratelimit.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    43946 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/plugins/restrictions.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    13822 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/plugins/rspamd.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    46705 2023-08-24 13:11:49.000000 fuglu-1.4.0/src/fuglu/plugins/sa.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5858 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/plugins/script.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1320 2023-03-16 11:34:26.000000 fuglu-1.4.0/src/fuglu/plugins/taction.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    11561 2023-05-30 18:25:59.000000 fuglu-1.4.0/src/fuglu/plugins/tlspolicy.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    63498 2023-09-08 05:01:12.000000 fuglu-1.4.0/src/fuglu/plugins/uriextract.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    16389 2023-06-15 06:30:42.000000 fuglu-1.4.0/src/fuglu/plugins/vacation.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    17218 2023-01-04 11:07:44.000000 fuglu-1.4.0/src/fuglu/procpool.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     8364 2023-07-12 14:51:15.000000 fuglu-1.4.0/src/fuglu/protocolbase.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    34684 2023-03-16 11:34:26.000000 fuglu-1.4.0/src/fuglu/scansession.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)   122688 2023-07-26 18:42:23.000000 fuglu-1.4.0/src/fuglu/shared.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     7402 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/stats.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    11959 2023-01-06 15:27:20.000000 fuglu-1.4.0/src/fuglu/stringencode.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    12201 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/threadpool.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.260799 fuglu-1.4.0/src/fuglu/utils/
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2022-01-14 02:33:11.000000 fuglu-1.4.0/src/fuglu/utils/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4621 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/fuglu/utils/version.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.256799 fuglu-1.4.0/src/fuglu.egg-info/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1909 2023-09-15 03:25:00.000000 fuglu-1.4.0/src/fuglu.egg-info/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3883 2023-09-15 03:25:00.000000 fuglu-1.4.0/src/fuglu.egg-info/SOURCES.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2023-09-15 03:25:00.000000 fuglu-1.4.0/src/fuglu.egg-info/dependency_links.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)       16 2023-09-15 03:25:00.000000 fuglu-1.4.0/src/fuglu.egg-info/requires.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        6 2023-09-15 03:25:00.000000 fuglu-1.4.0/src/fuglu.egg-info/top_level.txt
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.260799 fuglu-1.4.0/src/startscript/
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)    20076 2023-09-14 01:26:24.000000 fuglu-1.4.0/src/startscript/fuglu
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-09-15 03:25:00.260799 fuglu-1.4.0/src/tools/
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     6829 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/tools/fuglu_client
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     9605 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/tools/fuglu_conf
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     5352 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/tools/fuglu_control
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     2080 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/tools/fuglu_debug
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     2846 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/tools/fuglu_healthcheck
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     3128 2023-01-04 08:05:48.000000 fuglu-1.4.0/src/tools/fuglu_suspectfilter
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.498570 fuglu-1.5.0/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      597 2024-02-29 06:02:05.000000 fuglu-1.5.0/LICENSE
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      171 2024-02-07 08:58:39.000000 fuglu-1.5.0/MANIFEST.in
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1761 2024-04-11 09:00:28.498570 fuglu-1.5.0/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      869 2024-02-07 08:58:39.000000 fuglu-1.5.0/README.md
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3152 2024-02-29 06:02:05.000000 fuglu-1.5.0/compareconfig.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/conf/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      128 2024-02-07 08:58:39.000000 fuglu-1.5.0/conf/archive.regex.dist
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    13420 2024-04-11 06:42:36.000000 fuglu-1.5.0/conf/fuglu.conf.dist
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2090 2024-02-07 08:58:39.000000 fuglu-1.5.0/conf/fuglu_mrtg.cfg.dist
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1760 2024-02-07 08:58:39.000000 fuglu-1.5.0/conf/logging.conf.dist
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/conf/rules/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      627 2024-02-07 08:58:39.000000 fuglu-1.5.0/conf/rules/default-archivefiletypes.conf.dist
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1099 2024-02-07 08:58:39.000000 fuglu-1.5.0/conf/rules/default-archivenames.conf.dist
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6694 2024-02-29 06:02:05.000000 fuglu-1.5.0/conf/rules/default-filenames.conf.dist
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      797 2024-02-07 08:58:39.000000 fuglu-1.5.0/conf/rules/default-filetypes.conf.dist
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      335 2024-02-07 08:58:39.000000 fuglu-1.5.0/conf/skipplugins.regex.dist
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/conf/templates/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      152 2024-02-07 08:58:39.000000 fuglu-1.5.0/conf/templates/blockedfile.tmpl.dist
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/doc/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    29137 2024-04-11 08:57:53.000000 fuglu-1.5.0/doc/CHANGELOG
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      368 2024-02-07 08:58:39.000000 fuglu-1.5.0/doc/INSTALL
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       57 2024-02-07 08:58:39.000000 fuglu-1.5.0/pyproject.toml
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/scripts/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/scripts/buildscripts/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      355 2024-03-26 08:37:57.000000 fuglu-1.5.0/scripts/buildscripts/README.md
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      246 2024-03-26 08:37:57.000000 fuglu-1.5.0/scripts/buildscripts/build-deb.sh
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/scripts/mrtg/
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)       71 2024-02-07 08:58:39.000000 fuglu-1.5.0/scripts/mrtg/fuglu_mrtg.sh
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/scripts/startscripts/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/scripts/startscripts/arch/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      283 2024-04-09 06:25:23.000000 fuglu-1.5.0/scripts/startscripts/arch/fuglu.service
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/scripts/startscripts/centos_rhel/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/scripts/startscripts/centos_rhel/6/
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     1118 2024-04-09 06:25:23.000000 fuglu-1.5.0/scripts/startscripts/centos_rhel/6/fuglu
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/scripts/startscripts/centos_rhel/7/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      318 2024-04-09 06:25:23.000000 fuglu-1.5.0/scripts/startscripts/centos_rhel/7/fuglu.service
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/scripts/startscripts/debian/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.494570 fuglu-1.5.0/scripts/startscripts/debian/7/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1311 2024-04-09 06:25:23.000000 fuglu-1.5.0/scripts/startscripts/debian/7/fuglu
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.494570 fuglu-1.5.0/scripts/startscripts/debian/8/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      279 2024-04-09 06:25:23.000000 fuglu-1.5.0/scripts/startscripts/debian/8/fuglu.service
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/scripts/startscripts/suse/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.494570 fuglu-1.5.0/scripts/startscripts/suse/13/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1680 2024-04-09 06:25:23.000000 fuglu-1.5.0/scripts/startscripts/suse/13/fuglu
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      140 2024-04-11 09:00:28.498570 fuglu-1.5.0/setup.cfg
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2180 2024-04-09 06:25:23.000000 fuglu-1.5.0/setup.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.490570 fuglu-1.5.0/src/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.494570 fuglu-1.5.0/src/fuglu/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      849 2024-04-11 08:58:20.000000 fuglu-1.5.0/src/fuglu/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    20062 2024-04-09 06:25:23.000000 fuglu-1.5.0/src/fuglu/__main__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6113 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/addrcheck.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    31187 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/asyncprocpool.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    13154 2024-03-26 08:39:18.000000 fuglu-1.5.0/src/fuglu/bounce.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    14153 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/caching.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.494570 fuglu-1.5.0/src/fuglu/connectors/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      117 2024-02-07 08:58:39.000000 fuglu-1.5.0/src/fuglu/connectors/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   107594 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/connectors/asyncmilterconnector.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     5340 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/connectors/check.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    15981 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/connectors/esmtpconnector.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    45216 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/connectors/milterconnector.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     8502 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/connectors/ncconnector.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    20608 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/connectors/smtpconnector.py
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)    74516 2024-03-26 08:39:18.000000 fuglu-1.5.0/src/fuglu/core.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     5154 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/daemon.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    43321 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/debug.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.494570 fuglu-1.5.0/src/fuglu/extensions/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       94 2024-02-07 08:58:39.000000 fuglu-1.5.0/src/fuglu/extensions/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    13836 2024-03-08 02:15:02.000000 fuglu-1.5.0/src/fuglu/extensions/aioredisext.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6187 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/extensions/dnsquery.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2189 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/extensions/elastic.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    42361 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/extensions/filearchives.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     5204 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/extensions/filetype.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2443 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/extensions/fuzzyhashlib.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2726 2023-11-29 10:17:01.000000 fuglu-1.5.0/src/fuglu/extensions/matrixchat.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6504 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/extensions/redisext.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    30895 2024-03-08 02:15:02.000000 fuglu-1.5.0/src/fuglu/extensions/sql.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2306 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/funkyconsole.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.494570 fuglu-1.5.0/src/fuglu/lib/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2024-02-07 08:58:39.000000 fuglu-1.5.0/src/fuglu/lib/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    22368 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/lib/patcheddkimlib.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.494570 fuglu-1.5.0/src/fuglu/lib/patchedemail/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      351 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/lib/patchedemail/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4608 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/lib/patchedemail/message.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    22782 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/lib/patchedlibmilter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    26750 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/lib/ppymilterbase.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4695 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/loghandlers.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    15467 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/logtools.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    66063 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/mailattach.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     8784 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/mixins.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.494570 fuglu-1.5.0/src/fuglu/mplugins/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2024-02-07 08:58:39.000000 fuglu-1.5.0/src/fuglu/mplugins/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3455 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/mplugins/demo.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     8376 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/mshared.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.498570 fuglu-1.5.0/src/fuglu/plugins/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1025 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    55748 2024-04-10 15:33:13.000000 fuglu-1.5.0/src/fuglu/plugins/a_logging.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     5827 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/a_statsd.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    54653 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/antivirus.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    45615 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/archive.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    86864 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/attachment.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4248 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/bacn.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   106927 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/call_ahead.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    21516 2024-03-26 08:38:40.000000 fuglu-1.5.0/src/fuglu/plugins/clamav.py
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)    20883 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/dataprovider.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    21234 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/decision.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3081 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/delay.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     5558 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/dnsdata.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   141870 2024-04-10 15:33:13.000000 fuglu-1.5.0/src/fuglu/plugins/domainauth.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    26420 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/fuzor.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6239 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/geoip.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    15066 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/knownsubject.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    38902 2024-04-10 16:35:16.000000 fuglu-1.5.0/src/fuglu/plugins/mailcopy.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6704 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/messagesize.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    13528 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/originpolicy.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    66533 2024-04-10 15:33:13.000000 fuglu-1.5.0/src/fuglu/plugins/outpolicy.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    86033 2024-04-10 15:33:13.000000 fuglu-1.5.0/src/fuglu/plugins/p_blwl.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3368 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/p_debug.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3340 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/p_fraction.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     5071 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/p_skipper.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.498570 fuglu-1.5.0/src/fuglu/plugins/ratelimit/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2024-02-07 08:58:39.000000 fuglu-1.5.0/src/fuglu/plugins/ratelimit/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     7969 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/ratelimit/dynfunction.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    18892 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/ratelimit/helperfuncs.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    42784 2024-03-26 08:37:57.000000 fuglu-1.5.0/src/fuglu/plugins/ratelimit/main.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.498570 fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1508 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1187 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/always_hit.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1593 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/backendint.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     7639 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/fixed_ratelimit.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6048 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/sliding_log_ratelimit.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    15737 2024-03-26 08:37:57.000000 fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/sliding_window_ratelimit.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    43954 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/restrictions.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    13822 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/rspamd.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    47191 2024-04-10 15:33:22.000000 fuglu-1.5.0/src/fuglu/plugins/sa.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     5858 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/script.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    25061 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/sigenc.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1320 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/taction.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    11561 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/tlspolicy.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    69573 2024-03-08 02:15:02.000000 fuglu-1.5.0/src/fuglu/plugins/uriextract.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    16358 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/plugins/vacation.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    17236 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/procpool.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     8604 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/protocolbase.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    34685 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/scansession.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   128103 2024-04-10 16:35:16.000000 fuglu-1.5.0/src/fuglu/shared.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     7402 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/stats.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    11959 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/stringencode.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    12201 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/threadpool.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.498570 fuglu-1.5.0/src/fuglu/utils/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2024-02-07 08:58:39.000000 fuglu-1.5.0/src/fuglu/utils/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4619 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/fuglu/utils/version.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.494570 fuglu-1.5.0/src/fuglu.egg-info/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1761 2024-04-11 09:00:28.000000 fuglu-1.5.0/src/fuglu.egg-info/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4011 2024-04-11 09:00:28.000000 fuglu-1.5.0/src/fuglu.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2024-04-11 09:00:28.000000 fuglu-1.5.0/src/fuglu.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       61 2024-04-11 09:00:28.000000 fuglu-1.5.0/src/fuglu.egg-info/requires.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        6 2024-04-11 09:00:28.000000 fuglu-1.5.0/src/fuglu.egg-info/top_level.txt
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2024-04-11 09:00:28.498570 fuglu-1.5.0/src/tools/
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     6829 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/tools/fuglu_client
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     9605 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/tools/fuglu_conf
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     5387 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/tools/fuglu_control
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     2080 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/tools/fuglu_debug
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     2846 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/tools/fuglu_healthcheck
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     3128 2024-02-29 06:02:05.000000 fuglu-1.5.0/src/tools/fuglu_suspectfilter
```

### Comparing `fuglu-1.4.0/LICENSE` & `fuglu-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/PKG-INFO` & `fuglu-1.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: fuglu
-Version: 1.4.0
+Version: 1.5.0
 Summary: FuGlu Mail Content Scanner
 Home-page: http://www.fuglu.org
+Download-URL: https://gitlab.com/fumail/fuglu/-/archive/master/fuglu-master.tar.gz
 Author: O. Schacher
 Author-email: oli@fuglu.org
 License: Apache Software License
-Download-URL: https://gitlab.com/fumail/fuglu/-/archive/master/fuglu-master.tar.gz
-Description: FuGlu is a modular pre-queue/after-queue content filter written in Python that
-        acts as the glue application between the MTA and SPAM, Virus, and other scanners.
-        It can be used to filter spam, viruses, unwanted attachments, and do other content filtering.
-        
-        FuGlu focuses on being solid, easy to manage, debug and monitor.
-        
-        Quick links:
-        
-         * `Overview and documentation <https://fumail.gitlab.io/fuglu/>`_
-         * `Download <https://pypi.python.org/pypi/fuglu/>`_
-         * `Issue Tracker <https://gitlab.com/fumail/fuglu/issues>`_
-         * `Extra Plugins Repository <https://gitlab.com/fumail/fuglu-extra-plugins/>`_
-        
-        .. image:: https://badge.fury.io/py/fuglu.svg
-            :target: https://pypi.python.org/pypi/fuglu/
-            :alt: Latest PyPI version
-        
-        .. image:: https://gitlab.com/fumail/fuglu/badges/master/build.svg
-            :target: https://gitlab.com/fumail/fuglu/pipelines
-            :alt: Build status
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Communications :: Email :: Filters
 Classifier: Topic :: Communications :: Email :: Mail Transport Agents
 Requires: domainmagic
 Requires-Python: >=3.6
+Provides-Extra: test
+License-File: LICENSE
+
+FuGlu is a modular pre-queue/after-queue content filter written in Python that
+acts as the glue application between the MTA and SPAM, Virus, and other scanners.
+It can be used to filter spam, viruses, unwanted attachments, and do other content filtering.
+
+FuGlu focuses on being solid, easy to manage, debug and monitor.
+
+Quick links:
+
+ * `Overview and documentation <https://fumail.gitlab.io/fuglu/>`_
+ * `Download <https://pypi.python.org/pypi/fuglu/>`_
+ * `Issue Tracker <https://gitlab.com/fumail/fuglu/issues>`_
+ * `Extra Plugins Repository <https://gitlab.com/fumail/fuglu-extra-plugins/>`_
+
+.. image:: https://badge.fury.io/py/fuglu.svg
+    :target: https://pypi.python.org/pypi/fuglu/
+    :alt: Latest PyPI version
+
+.. image:: https://gitlab.com/fumail/fuglu/badges/master/build.svg
+    :target: https://gitlab.com/fumail/fuglu/pipelines
+    :alt: Build status
```

### Comparing `fuglu-1.4.0/README.md` & `fuglu-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/compareconfig.py` & `fuglu-1.5.0/compareconfig.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/conf/fuglu.conf.dist` & `fuglu-1.5.0/conf/fuglu.conf.dist`

 * *Files 5% similar despite different names*

```diff
@@ -42,21 +42,32 @@
 #10888: debug port
 incomingport=10025,10099,10888
 
 #outgoing hostname/ip where postfix is listening for re-injects.
 #use ${injecthost} to connect back to the IP where the incoming connection came from
 outgoinghost=127.0.0.1
 
-#outgoing port  where postfix is listening for re-injects)
+#outgoing port where postfix is listening for re-injects)
 outgoingport=10026
 
-##outgoing helo we should use for re-injects
+#outgoing helo we should use for re-injects
 #leave empty to auto-detect current hostname
 outgoinghelo=
 
+#how many times should we try to re-inject before returning temporary error (after queue mode only)
+outgoingretry=1
+
+#outgoing hostname/ip where postfix is listening for bounces.
+#supports same template variables as outgoinghost. leave empty to use outgoinghost value.
+bouncehost=
+
+#outgoing port where postfix is listening for bounces.
+#leave empty to use outgoingport value.
+bounceport=
+
 #temp dir where fuglu can store messages while scanning
 tempdir=/tmp
 
 #String to prepend to added headers
 prependaddedheaders=X-Fuglu-
 
 #If a plugin decides to delete a message, save a copy here
```

### Comparing `fuglu-1.4.0/conf/fuglu_mrtg.cfg.dist` & `fuglu-1.5.0/conf/fuglu_mrtg.cfg.dist`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/conf/logging.conf.dist` & `fuglu-1.5.0/conf/logging.conf.dist`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/conf/rules/default-archivefiletypes.conf.dist` & `fuglu-1.5.0/conf/rules/default-archivefiletypes.conf.dist`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/conf/rules/default-archivenames.conf.dist` & `fuglu-1.5.0/conf/rules/default-archivenames.conf.dist`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/conf/rules/default-filenames.conf.dist` & `fuglu-1.5.0/conf/rules/default-filenames.conf.dist`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/conf/rules/default-filetypes.conf.dist` & `fuglu-1.5.0/conf/rules/default-filetypes.conf.dist`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/doc/CHANGELOG` & `fuglu-1.5.0/doc/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+-- Fuglu 1.5.0 2024-04-11 "Chou Dou Fu"
+Chou Dou Fu or smelly tofu is a fermented bean curd popular in Taiwan. Think of it as a kinf of vegan
+cheese. You will notice the sour smell of preparation from afar on any night market. Follow it to
+discover an fantastic tasting, healthy snack. It is crispy on the outside, melting soft on the inside
+and usually served with some pickled cabbage on the side.
+
+* minor code security improvements
+* add fluentd loghandler
+* continued to improve log output
+* send bounces via separate outbound system
+* ratelimit: expire redis values
+* split FilterDecision plugin into two components (FilterDecision and DeliverDecision)
+* new plugin to extract uris/emails from attached qr codes
+* new plugins in domainauth to strip dkim/arc headers and pass dkim header data between fuglu instances
+* domainauth: various fixes and improvements to arc and dkim signing. use org domain for dmarc checks.
+* archive plugin: new backends for S3 and WebDAV storage
+* fuzor: make hash algorithm configurable
+* call-ahead: better behaviour on misbehaving target server, fix command line client
+* logging plugin: use async elasticsearch
+* new plugin: sigenc: sign and encrypt outgoing mail. decrypt and verify incoming mail. load and learn certificates.
+* fuglu/src/startscript/fuglu is superseded by python -m fuglu
+
+Developers
+* rework core mail handling. make less use of python message/emailmessage objects,
+  instead work directly with source, e.g. when altering headers. this prevents unintended
+  changes of mail structure (e.g. mime-headers) which may break crytographic signatures.
+* removed python-redis 2.x compatibility and RedisKeepAlive, deprecate explicit password
+* improved python 3.12 compatibility
+
+
+
 -- Fuglu 1.4.0 2023-09-15 "Haggis"
 Haggis is Scotland's national dish. It consists of sheep stomach filled with sheep offal, onion, oats,
 and is heavily spiced with black pepper. Thus it "is not for the weak of constitution". Slainte!
 
 * Python 3.11 compatibility
 * Improve dependency requirements
 * Better dependency linting
```

### Comparing `fuglu-1.4.0/scripts/startscripts/centos_rhel/6/fuglu` & `fuglu-1.5.0/scripts/startscripts/centos_rhel/6/fuglu`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Source networking configuration.
 . /etc/sysconfig/network
 
 # See how we were called.
 case "$1" in
   start)
         echo -n "Starting FuGlu Mail Content Scanner: "
-        daemon /usr/bin/fuglu --pidfile=/var/run/fuglud.pid
+        daemon /usr/bin/python3 -m fuglu --pidfile=/var/run/fuglud.pid
         RETVAL=$?
         echo
         ;;
   stop)
         echo -n "Stopping FuGlu Mail Content Scanner: "
         killproc fuglu
         rm -f /var/run/fuglu.pid
```

### Comparing `fuglu-1.4.0/scripts/startscripts/debian/7/fuglu` & `fuglu-1.5.0/scripts/startscripts/debian/7/fuglu`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Default-Stop:      0 1 6
 # Short-Description: Fuglu is yet another mail scanner daemon written in python.
 # Description:       Installed as a postfix after-queue filter fuglu can be used to filter spam, viruses, unwanted attachments etc.
 ### END INIT INFO
 
 set -e
 
-FUGLU="/usr/local/bin/fuglu"
+FUGLU="/usr/bin/python3 -m fuglu"
 PIDFILE="/var/run/fuglu.pid"
 
 OPTIONS="--pidfile=/var/run/fuglud.pid"
 MODULES=""
 
 # Get lsb functions
 . /lib/lsb/init-functions
```

### Comparing `fuglu-1.4.0/scripts/startscripts/suse/13/fuglu` & `fuglu-1.5.0/scripts/startscripts/suse/13/fuglu`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ### END INIT INFO
 
 . /etc/rc.status
 
 # Reset status of this service
 rc_reset
 
-FUGLU_BIN=/usr/bin/fuglu
+FUGLU_BIN="python -m fuglu"
 FUGLU_PID=/var/run/fuglu.pid
 test -x $FUGLU_BIN || {
         echo "$FUGLU_BIN not installed";
         if [ "$1" = "stop" ] ; then
                 exit 0
         else
                 exit 5
```

### Comparing `fuglu-1.4.0/setup.py` & `fuglu-1.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,29 +30,37 @@
     include_package_data=True,
     data_files=[
         ('/etc/fuglu', glob.glob('conf/*.dist')),
         ('/etc/fuglu/templates', glob.glob('conf/templates/*.dist')),
         ('/etc/fuglu/rules', glob.glob('conf/rules/*.dist')),
     ],
     scripts=[
-        'src/startscript/fuglu',
         'src/tools/fuglu_debug',
         'src/tools/fuglu_control',
         'src/tools/fuglu_conf',
         'src/tools/fuglu_suspectfilter',
         'src/tools/fuglu_client',
         'src/tools/fuglu_healthcheck'
     ],
     python_requires='>=3.6',
     install_requires=[
         'packaging>=16.8',
     ],
     requires=[
         'domainmagic',
     ],
+    extras_require={
+        "test": [
+            "pytest",
+            "rarfile",
+            "dkimpy",
+            "pyspf",
+            "pycrypto",
+        ]
+    },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: No Input/Output (Daemon)',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX',
```

### Comparing `fuglu-1.4.0/src/fuglu/__init__.py` & `fuglu-1.5.0/src/fuglu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #
 from fuglu.utils.version import get_version, VERSION_ALPHA, VERSION_BETA, VERSION_RC, VERSION_FINAL
 
 
-FUGLU_VERSION = (1, 4, 0, VERSION_FINAL, 0)
+FUGLU_VERSION = (1, 5, 0, VERSION_FINAL, 0)
 
 __version__ = get_version().strip() if isinstance(get_version(), str) else get_version()
```

### Comparing `fuglu-1.4.0/src/fuglu/addrcheck.py` & `fuglu-1.5.0/src/fuglu/addrcheck.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/asyncprocpool.py` & `fuglu-1.5.0/src/fuglu/asyncprocpool.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/bounce.py` & `fuglu-1.5.0/src/fuglu/bounce.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 import logging
 import os
 import email
 import re
 import ssl
 import asyncio
 from email.utils import formatdate, make_msgid
-from email.header import Header
-from .shared import apply_template, FileList, extract_domain, get_outgoing_helo, deprecated
+import typing as tp
+from .shared import apply_template, FileList, extract_domain, get_outgoing_helo, deprecated, make_header, Suspect
 from .stringencode import force_bString, force_uString
 
 try:
     from aiosmtplib import SMTP as aioSMTP
     from aiosmtplib.errors import SMTPException
     HAVE_AIOSMTP = True
 except ImportError:
@@ -68,15 +68,15 @@
         self.lastserveranswer = response
         self.lastservercode = code
         queueid = queueid_from_postfixreply(response.decode())
         if queueid is not None:
             self.queueid = queueid
         return code, response
 
-    def xclient(self, xclient_args=None):
+    def xclient(self, xclient_args:tp.Dict[str,str]=None) -> tp.Tuple[int, bytes]:
         self.ehlo_or_helo_if_needed()
         if not 'xclient' in self.esmtp_features:
             raise smtplib.SMTPNotSupportedError("SMTP XCLIENT extension not supported by server.")
 
         if xclient_args:
             xclient_cmds = self.esmtp_features['xclient'].split()
             if 'ADDR' in xclient_args and ':' in xclient_args['ADDR'] and not xclient_args['ADDR'].startswith('IPV6:'):
@@ -85,15 +85,15 @@
             xclient_str = ' '.join(values)
             if xclient_str:
                 return self.docmd('XCLIENT', xclient_str)
 
 
 class FugluAioSMTPClient(aioSMTP):
     """
-    This class patches aioSMTPLib
+    This class patches aioSMTPLib but is considered deprecated
     improvements:
     - do not check certificates during starttls
     - support xclient
     """
     async def starttls(self, *args, **kwargs):
         if not kwargs.get('tls_context'):
             ctx = ssl.create_default_context()
@@ -132,61 +132,60 @@
         if self.nobounce is None:
             filepath = self.config.get('main', 'nobouncefile', fallback=None)
             if filepath and os.path.exists(filepath):
                 self.nobounce = FileList(filepath)
             elif filepath:
                 self.logger.warning(f'nobouncefile {filepath} not found')
 
-    def _add_required_headers(self, recipient, messagecontent):
+    def _add_required_headers(self, recipient:str, messagecontent:bytes):
         """add headers required for sending automated mail"""
 
         msgrep = email.message_from_bytes(force_bString(messagecontent))
         msgrep.set_charset("utf-8")  # define unicode because the messagecontent is unicode
 
         if not 'to' in msgrep:
-            msgrep['To'] = Header(f'<{recipient}>').encode()
+            msgrep['to'] = make_header('to', recipient)
 
-        if not 'From' in msgrep:
-            msgrep['from'] = Header(f'<MAILER-DAEMON@{get_outgoing_helo(self.config)}>').encode()
+        if not 'from' in msgrep:
+            msgrep['from'] = make_header('from', f'MAILER-DAEMON@{get_outgoing_helo(self.config)}')
 
         if not 'auto-submitted' in msgrep:
-            msgrep['auto-submitted'] = Header('auto-generated').encode()
+            msgrep['auto-submitted'] = 'auto-generated'
 
         if not 'date' in msgrep:
             msgrep['Date'] = formatdate(localtime=True)
 
         if not 'Message-id' in msgrep:
             msgrep['Message-ID'] = make_msgid()
 
         return msgrep.as_string()
 
-    def send_template_file(self, recipient, templatefile, suspect, values):
+    def send_template_file(self, recipient:str, templatefile:str, suspect:Suspect, values:tp.Dict[str,str]) -> tp.Optional[bool]:
         """Send a E-Mail Bounce Message
 
         Args:
             recipient    (str):  Message recipient (bla@bla.com)
             templatefile (str): Template to use
             suspect      (fuglu.shared.Suspect) suspect that caused the bounce
             values            :Values to apply to the template. ensure all values are of type <str>
 
         If the suspect has the 'nobounce' tag set, the message will not be sent. The same happens
         if the global configuration 'disablebounces' is set.
         """
-
         if not os.path.exists(templatefile):
             self.logger.error(f'{suspect.id} Template file does not exist: {templatefile}')
             return
 
         with open(templatefile) as fp:
             filecontent = fp.read()
 
         queueid = self.send_template_string(recipient, filecontent, suspect, values)
         return queueid
 
-    def send_template_string(self, recipient, templatecontent, suspect, values):
+    def send_template_string(self, recipient:str, templatecontent:str, suspect:Suspect, values:tp.Dict[str,str]) -> tp.Optional[str]:
         """Send a E-Mail Bounce Message
 
         If the suspect has the 'nobounce' tag set, the message will not be sent. The same happens
         if the global configuration 'disablebounces' is set.
 
         Args:
             recipient       (unicode or str) : Message recipient (bla@bla.com)
@@ -206,15 +205,17 @@
 
         self.logger.debug(f'{suspect.id} Sending bounce message to {recipient}')
         fromaddress = "<>"
         queueid = self.send(fromaddress, recipient, message)
         return queueid
 
     def _get_targethost(self):
-        targethost: str = self.config.get('main', 'outgoinghost')
+        targethost = self.config.get('main', 'bouncehost', fallback='')
+        if not targethost:
+            targethost = self.config.get('main', 'outgoinghost')
         if targethost == '${injecthost}':
             # fall back to bindaddress
             targethost = self.config.get('main', 'bindaddress')
             if targethost == "0.0.0.0":
                 raise ValueError(f"Bouncer: targethost can't be set to '${{injecthost}}' "
                                  f"if bindaddress is set to '0.0.0.0'")
         elif targethost.startswith("$"):
@@ -222,47 +223,55 @@
             env_targethost = os.environ[targethost[1:]]
             if not env_targethost:
                 raise ValueError(f"Bouncer: Could not extract outgoing host from environment var '{targethost}'")
             targethost = env_targethost
         if not targethost or (isinstance(targethost, str) and not targethost.strip()):
             raise ValueError("Bouncer: No targethost defined for Bouncer, please define valid outgoinghost in config!")
         return targethost
+    
+    def _get_targetport(self) -> int:
+        try:
+            targetport = self.config.getint('main', 'bounceport', fallback=0)
+        except (ValueError, TypeError):
+            targetport = 0
+        if targetport == 0:
+            targetport = self.config.getint('main', 'outgoingport')
+        return targetport
 
-    def _send_sync(self, fromaddress, toaddress, message):
+    def _send_sync(self, fromaddress:str, toaddress:str, message:str) -> str:
         """really send message"""
         targethost = self._get_targethost()
-        outgoingport = self.config.getint('main', 'outgoingport')
+        targetport = self._get_targetport()
         helostring = get_outgoing_helo(self.config)
         try:
-            smtp_server = FugluSMTPClient(host=targethost, port=outgoingport, local_hostname=helostring)
+            smtp_server = FugluSMTPClient(host=targethost, port=targetport, local_hostname=helostring)
             smtp_server.sendmail(fromaddress, toaddress, message)
         except (smtplib.SMTPException, OSError) as e:
-            self.logger.error(
-                f'failed to send mail from={fromaddress} to={toaddress} via={targethost} port={outgoingport} helo={helostring} due to {e.__class__.__name__} {str(e)}')
+            self.logger.error(f'failed to send mail from={fromaddress} to={toaddress} via={targethost} port={targetport} helo={helostring} due to {e.__class__.__name__} {str(e)}')
             raise
         smtp_server.quit()
         return smtp_server.queueid
 
     @deprecated
-    def _send_async(self, fromaddress, toaddress, message):
+    def _send_async(self, fromaddress:str, toaddress:str, message:str) -> str:
         targethost = self._get_targethost()
-        outgoingport = self.config.getint('main', 'outgoingport')
+        targetport = self._get_targetport()
         helostring = get_outgoing_helo(self.config)
         try:
-            smtp_server = FugluAioSMTPClient(hostname=targethost, port=outgoingport, source_address=helostring)
+            smtp_server = FugluAioSMTPClient(hostname=targethost, port=targetport, source_address=helostring)
             smtp_server.connect()
             send_resp = smtp_server.sendmail(fromaddress, toaddress, message)
         except SMTPException as e:
             self.logger.error(
-                f'failed to send mail from={fromaddress} to={toaddress} via={targethost} port={outgoingport} due to {e.__class__.__name__} {str(e)}')
+                f'failed to send mail from={fromaddress} to={toaddress} via={targethost} port={targetport} due to {e.__class__.__name__} {str(e)}')
             raise
         smtp_server.quit()
         return smtp_server.parse_postfixreply(send_resp[1])
 
-    def send(self, fromaddress, toaddress, message):
+    def send(self, fromaddress:str, toaddress:str, message:str) -> tp.Optional[str]:
         if (not fromaddress or fromaddress == '<>') and self.config.getboolean('main', 'disablebounces'):
             self.logger.info(f'Bounces are disabled in config - not sending message to {toaddress}')
             return
 
         self._init_nobounce()
         if self.nobounce and extract_domain(toaddress) in self.nobounce.get_list():
             self.logger.info(f'Bounces to this rcpt are disabled - not sending message to {toaddress}')
@@ -278,15 +287,15 @@
                     self.event_loop = asyncio.get_event_loop()
             queueid = self.event_loop.run_until_complete(self._send_async(fromaddress, toaddress, message))
         else:
             queueid = self._send_sync(fromaddress, toaddress, message)
         return queueid
 
     @deprecated
-    def _send(self, fromaddress, toaddress, message):
+    def _send(self, fromaddress:str, toaddress:str, message:str) -> None:
         """deprecated version of send()"""
         self.send(fromaddress, toaddress, message)
 
     def lint(self):
         from fuglu.funkyconsole import FunkyConsole
         fc = FunkyConsole()
```

### Comparing `fuglu-1.4.0/src/fuglu/caching.py` & `fuglu-1.5.0/src/fuglu/caching.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/connectors/asyncmilterconnector.py` & `fuglu-1.5.0/src/fuglu/connectors/asyncmilterconnector.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,36 +10,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #
-import datetime
 import logging
 import socket
 import tempfile
 import os
 import typing as tp
 import asyncio
 import traceback
 import time
 import functools
 import copy
-import weakref
-
-from email.header import Header
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from io import BytesIO
 from collections import deque
-
 from fuglu.protocolbase import ProtocolHandler
 from fuglu.stringencode import force_bString, force_uString
-from fuglu.shared import Suspect, DUNNO, REJECT, DELETE, DEFER, ACCEPT, string_to_actioncode, utcnow
+from fuglu.shared import Suspect, DUNNO, REJECT, DELETE, DEFER, ACCEPT, string_to_actioncode, utcnow, fold_header
 from fuglu.scansession import TrackTimings
 from configparser import ConfigParser
 from fuglu.logtools import createPIDinfo
 from fuglu.debug import CrashStore
 from fuglu.addrcheck import Addrcheck
 
 try:
@@ -189,50 +184,71 @@
         # Milter can keep the connection and handle several suspect in one session
         self.keep_connection = True
 
         if not LIMBMILTER_AVAILABLE:
             raise ImportError("libmilter not available, not possible to use MilterHandler")
 
         try:
-            configstring = config.get('milter', 'milter_mode')
+            milter_mode = Suspect.getlist_space_comma_separated(config.get('milter', 'milter_mode'))
         except Exception:
-            configstring = "tags"
+            milter_mode = ["tags"]
+
+        milter_mode = [entry.lower() for entry in milter_mode]
+
+        # check for unknown options
+        unknown = [mm for mm in milter_mode if mm not in ("auto", "readonly", "tags", "replace_demo", "manual", "autoheaders", "autofrom", "autoto")]
+        if unknown:
+            self.logger.warning(f"ignoring unknown milter option(s): {','.join(unknown)}")
+
+        # keep only known options
+        milter_mode = [mm for mm in milter_mode if mm in ("auto", "readonly", "tags", "replace_demo", "manual", "autoheaders", "autofrom", "autoto")]
+
+        if any((entry in ("autoheaders", "autofrom", "autoto") for entry in milter_mode)) and not all((entry in ("autoheaders", "autofrom", "autoto") for entry in milter_mode)):
+            self.logger.error(f"milter options: 'autoheaders', 'autofrom', 'autoto' can not becombined with other options -> resetting")
+            milter_mode = []
 
-        configstring = configstring.lower()
+        if len(milter_mode) > 1 and not all(entry in ("autoheaders", "autofrom", "autoto") for entry in milter_mode):
+            self.logger.error(f"only milter options: 'autoheaders', 'autofrom', 'autoto' can be combined -> resetting")
+            milter_mode = []
 
-        if not configstring:
+        if not milter_mode:
             self.log("milter_mode: setting to default value: 'tags'")
-            configstring = "tags"
+            milter_mode = ["tags"]
 
-        if configstring not in ["auto", "readonly", "tags", "replace_demo", "manual", "autoheaders"]:
-            self.logger.warning("milter_mode: '%s' not recognised, resetting to 'tags'" % configstring)
 
-        self.enable_mode_manual = ("manual" == configstring)
-        self.enable_mode_auto = ("auto" == configstring)
-        self.enable_mode_autoheaders = ("autoheaders" == configstring)
-        self.enable_mode_readonly = ("readonly" == configstring)
-        self.enable_mode_tags = ("tags" == configstring)
-        self.replace_demo = ("replace_demo" == configstring)
+        self.enable_mode_manual = "manual" in milter_mode
+        self.enable_mode_auto = "auto" in milter_mode
+        self.enable_mode_autoheaders = "autoheaders" in milter_mode
+        self.enable_mode_autofrom = "autofrom" in milter_mode
+        self.enable_mode_autoto = "autoto" in milter_mode
+        self.enable_mode_readonly = "readonly" in milter_mode
+        self.enable_mode_tags = "tags" in milter_mode
+        self.replace_demo = "replace_demo" in milter_mode
+
         
         self.sess_options = 0x00 if self.enable_mode_readonly else lm.SMFIF_ALLOPTS
 
         self.logger.debug(f"{createPIDinfo()}: new MilterHandler (asyncid: {asyncid})")
-        self.log(f"Milter mode: auto={self.enable_mode_auto}, autoheaders={self.enable_mode_autoheaders}"
+        self.log(f"Milter mode: auto={self.enable_mode_auto}, "
+                 f"autoheaders={self.enable_mode_autoheaders}"
+                 f"autofrom={self.enable_mode_autofrom}"
+                 f"autoto={self.enable_mode_autoto}"
                  f"readonly={self.enable_mode_readonly}, "
                  f"tags={self.enable_mode_tags}")
 
-        # options:
-        # -> for replace option: "all" "body" "headers" "from" "to"
-        # -> for autoheaders option: "prepend" "append"
+        # valid milter_mode_options depending on milter_mode:
+        # -> "manual" : "all" "body" "headers" "from" "to"
+        # -> "autoheaders": "prepend" "append"
 
         try:
             self.milter_mode_options = Suspect.getlist_space_comma_separated(config.get('milter', 'milter_mode_options'))
         except Exception:
             self.milter_mode_options = []
 
+
         self.log("Milter config fixed replacements: all=%s, body=%s, headers=%s, from=%s, to=%s" %
                  ("all" in self.milter_mode_options, "body" in self.milter_mode_options,
                   "headers" in self.milter_mode_options, "from" in self.milter_mode_options,
                   "to" in self.milter_mode_options))
         self.log(f"prependers: {self.prependers}")
         self.log(f"plugins: {self.plugins}")
         self.log(f"appenders: {self.appenders}")
@@ -783,15 +799,22 @@
 
     def _clean_address(self, address: tp.Optional[bytes]) -> tp.Optional[bytes]:
         address_cleaned = None
         # convert address to string
         if address is not None:
             addr_split = address.split(b'\0', maxsplit=1)
             address_cleaned = addr_split[0].strip(b'<>')
-            address_cleaned = address_cleaned.rstrip(b'.')  # remove trailing .
+            address_cleaned_stripped = address_cleaned.strip()
+            if address_cleaned != address_cleaned_stripped:
+                self.logger.info(f"{self.id} Stripped unnecessary spaces from from/to-address(position=1): '{address_cleaned}' -> '{address_cleaned_stripped}'")
+            address_cleaned = address_cleaned_stripped.rstrip(b'.')  # remove trailing .
+            address_cleaned_stripped = address_cleaned.strip()
+            if address_cleaned != address_cleaned_stripped:
+                self.logger.info(f"{self.id} Stripped unnecessary spaces from from/to-address (position=2): '{address_cleaned}' -> '{address_cleaned_stripped}'")
+                address_cleaned = address_cleaned_stripped
         return address_cleaned
 
     def get_cleaned_from_address(self) -> bytes:
         """Return from_address, without <> qualification or other MAIL FROM parameters"""
         # now already cleaned while setting
         return self.sender
 
@@ -2040,14 +2063,22 @@
                 if "from" in milter_replace_tag:
                     replace_from = True
                 if "to" in milter_replace_tag:
                     replace_from = True
                 self.logger.debug(f"{suspect.id} Mode tags -> replace headers:{replace_headers}, "
                                   f"body:{replace_body}, from:{replace_from}, to:{replace_to}")
 
+        if self.mhandler.enable_mode_autofrom:
+            replace_from = suspect.orig_from_address_changed()
+            self.logger.debug(f"{suspect.id} Mode autofrom -> replace_from:{replace_from}")
+
+        if self.mhandler.enable_mode_autoto:
+            replace_to = suspect.orig_recipients_changed()
+            self.logger.debug(f"{suspect.id} Mode autoto -> replace_to:{replace_to}")
+
         # ----------------------- #
         # replace data in message #
         # ----------------------- #
         if replace_from:
             self.logger.warning(f"{suspect.id} Set new envelope \"from address\": {suspect.from_address}")
             await self.change_from(suspect.from_address)
 
@@ -2065,15 +2096,15 @@
             # --
             # auto mod
             # --
             lvl = logging.WARNING if len(suspect.modified_headers) > 0 else logging.INFO
 
             self.logger.log(lvl, f"{suspect.id} Modify {len(suspect.modified_headers)} headers according to modification track in suspect")
             for key, val in iter(suspect.modified_headers.items()):
-                hdr = Header(val, header_name=key, continuation_ws=' ')
+                hdr = fold_header(key, val, value_only=True)
                 await self.changeheader(key, hdr.encode())
 
             # --
             # auto remove
             # --
             lvl = logging.WARNING if len(suspect.removed_headers) > 0 else logging.INFO
             self.logger.log(lvl, f"{suspect.id} Autoremove {len(suspect.removed_headers)} headers according to modification track in suspect")
@@ -2088,15 +2119,15 @@
                 autoadd = {k: v for k, v in suspect.added_headers.items() if v not in suspect.addheaders}
             except Exception as e:
                 self.logger.warning(f"{suspect.id} Problem creating autoadd dict ({type(e)}): {str(e)}")
                 autoadd = {}
             lvl = logging.WARNING if len(autoadd) > 0 else logging.INFO
             self.logger.log(lvl, f"{suspect.id} Autoadd {len(autoadd)} headers not in addheaders according to modification track in suspect")
             for key, val in autoadd.items():
-                hdr = Header(val, header_name=key, continuation_ws=' ')
+                hdr = fold_header(key, val, value_only=True)
                 self.logger.debug(f"{suspect.id} AutoAdd suspect header-> {key}: {val}")
                 await self.addheader(key, hdr.encode())
 
         elif (self.mhandler.enable_mode_autoheaders and "prepend" in self.mhandler.milter_mode_options) and not replace_headers:
             dont_add_more_headers = True
             # rewrite headers from tracking, but replace so they are prepended
             newheaders = copy.deepcopy(self.original_headers)
@@ -2113,16 +2144,16 @@
                 try:
                     key, value = header
                     skey = force_uString(key).strip().lower()
                     newval = modified_headers.get(skey, None)
                     if newval is not None:
                         sval = force_uString(value)
                         self.logger.debug(f"{suspect.id} AutoMod suspect header-> {skey}: {sval} -> {newval}")
-                        hdr = Header(newval, header_name=skey, continuation_ws=' ')
-                        value = force_bString(hdr.encode())
+                        hdr = fold_header(skey, newval, value_only=True)
+                        value = hdr.encode()
                         newheaders.append((key, value))
                         changes += 1
                     else:
                         newheaders.append(header)
                 except Exception as e:
                     self.logger.warning(f"{self.id} problem modifying header {header}: ({type(e)}) {str(e)}")
                     # if anything goes wrong, put old header again...
@@ -2164,15 +2195,15 @@
                 autoadd = {k: v for k, v in added_headers.items() if v not in addheaders}
             except Exception as e:
                 self.logger.warning(f"{suspect.id} Problem creating autoadd dict ({type(e)}): {str(e)}")
                 autoadd = {}
             lvl = logging.WARNING if len(autoadd) > 0 else logging.INFO
             self.logger.log(lvl, f"{suspect.id} Autoadd(prepend) {len(autoadd)} headers not in addheaders according to modification track in suspect")
             for key, val in autoadd.items():
-                hdr = Header(val, header_name=key, continuation_ws=' ')
+                hdr = fold_header(key, val, value_only=True)
                 self.loggerheaders.debug(f"{suspect.id} AutoAdd suspect header-> {key}: {val}")
                 # await self.addheader(key, hdr.encode())
                 newheaders.appendleft((force_bString(key), force_bString(hdr.encode())))
                 changes += 1
             if newheaders:
                 newheaders = list(newheaders) + origheaders
             else:
@@ -2183,16 +2214,16 @@
             # add
             # --
             origheaders = newheaders
             newheaders = deque()
             lvl = logging.WARNING if len(addheaders) > 0 else logging.INFO
             self.logger.log(lvl, f"{suspect.id} Add(prepend) {len(addheaders)} headers according to suspect")
             for key, val in addheaders.items():
-                hdr = Header(val, header_name=key, continuation_ws=' ')
-                self.loggerheaders.debug(f"{suspect.id} Add(prepend) suspect header-> {key}: {val}")
+                hdr = fold_header(key, val, value_only=True)
+                self.loggerheaders.info(f"{suspect.id} Add(prepend) suspect header-> {key}: {val}")
                 newheaders.appendleft((force_bString(key), force_bString(hdr.encode())))
                 changes += 1
             if newheaders:
                 newheaders = list(newheaders) + origheaders
             else:
                 newheaders = origheaders
 
@@ -2211,25 +2242,24 @@
             self.logger.warning(f"{suspect.id} Remove {len(self.original_headers)} original headers ")
             await self.remove_headers()
 
             msg = suspect.get_message_rep()
             self.logger.warning(f"{suspect.id} Add {len(msg)} headers from suspect mail")
             for key, val in iter(msg.items()):
                 self.loggerheaders.debug(f"{suspect.id} Add header from msg-> {key}: {val}")
-                if not isinstance(val, Header):
-                    val = Header(val, header_name=key, continuation_ws=' ')
+                hdr = fold_header(key, val, value_only=True)
                 await self.addheader(key, val.encode())
         # --
         # headers to add, same as for the other connectors
         # --
         if not dont_add_more_headers:
             lvl = logging.WARNING if len(suspect.addheaders) > 0 else logging.INFO
             self.logger.log(lvl, f"{suspect.id} Add {len(suspect.addheaders)} headers as defined in suspect")
             for key, val in iter(suspect.addheaders.items()):
-                hdr = Header(val, header_name=key, continuation_ws=' ')
+                hdr = fold_header(key, val, value_only=True)
                 self.loggerheaders.debug(f"{suspect.id} Add suspect header-> {key}: {val}")
                 await self.addheader(key, hdr.encode())
 
         if replace_body:
             self.logger.warning(f"{suspect.id} Replace message body")
             msg_string = suspect.get_message_rep().as_string()
             # just dump everything below the headers
```

### Comparing `fuglu-1.4.0/src/fuglu/connectors/check.py` & `fuglu-1.5.0/src/fuglu/connectors/check.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,18 +14,15 @@
 # limitations under the License.
 #
 #
 #
 import socket
 import random
 import logging
-
-from email.header import Header
-
-from fuglu.shared import Suspect
+from fuglu.shared import Suspect, fold_header
 from fuglu.stringencode import force_uString
 
 
 class HealthCheckSuspect(Suspect):
     def __init__(self, *args, **kwargs):
         # try to initialise original suspect but don't fail on any error
         try:
@@ -75,27 +72,16 @@
         add_headers.append(("X-DATA-PREPEND-END", prepend_identifier))
 
         headerlines = b""
         for key, value in add_headers:
             # convert inputs if needed
             u_key = str(key)
             u_value = str(value)
-
-            try:
-                hdr = Header(u_value, header_name=u_key, continuation_ws=' ')
-            except (UnicodeDecodeError, UnicodeEncodeError):
-                b_value = u_value.encode()
-                hdr = Header(b_value, charset='utf-8', header_name=u_key, continuation_ws=' ')
-
-            hdrline = "%s: %s\r\n" % (u_key, hdr.encode())
-
-            if headerlines:
-                headerlines += hdrline.encode()
-            else:
-                headerlines = hdrline.encode()
+            hdr = fold_header(u_key, u_value)
+            headerlines += hdr.encode()
 
         logger.debug("Send headerlines...")
         sockfile.write(headerlines)
         sockfile.flush()
         logger.debug("Sent, now disable writing to socket")
         try:
             s.shutdown(socket.SHUT_WR)
```

### Comparing `fuglu-1.4.0/src/fuglu/connectors/esmtpconnector.py` & `fuglu-1.5.0/src/fuglu/connectors/esmtpconnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,35 +15,34 @@
 #
 #
 import logging
 import socket
 import tempfile
 import os
 from fuglu.protocolbase import ProtocolHandler, BasicTCPServer
-from fuglu.shared import Suspect, apply_template
+from fuglu.shared import Suspect, apply_template, fold_header
 from fuglu.stringencode import force_bString, force_uString
 from fuglu.bounce import FugluSMTPClient
 from .smtpconnector import smtp_strip_address
-from email.header import Header
 import re
 
 
 def buildmsgsource(suspect):
     """Build the message source with fuglu headers prepended"""
     # we must prepend headers manually as we can't set a header order in email
     # objects
 
     # -> the original message source is bytes
     origmsgtxt = suspect.get_source()
     newheaders = ""
-
+    
     for key in suspect.addheaders:
         val = suspect.addheaders[key]
-        hdr = Header(val, header_name=key, continuation_ws=' ')
-        newheaders += f"{key}: {hdr.encode()}\r\n"
+        hdr = fold_header(key, val)
+        newheaders += hdr
 
     # the original message should be in bytes, make sure the header added
     # is an encoded string as well
     modifiedtext = force_bString(newheaders) + force_bString(origmsgtxt)
     return modifiedtext
```

### Comparing `fuglu-1.4.0/src/fuglu/connectors/milterconnector.py` & `fuglu-1.5.0/src/fuglu/connectors/milterconnector.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,19 @@
 import tempfile
 import os
 import time
 import typing as tp
 import copy
 
 from typing import Tuple, Union
-from email.header import Header
 from io import BytesIO
 
 from fuglu.protocolbase import ProtocolHandler, BasicTCPServer
 from fuglu.stringencode import force_bString, force_uString
-from fuglu.shared import Suspect
+from fuglu.shared import Suspect, fold_header
 from configparser import ConfigParser
 from .asyncmilterconnector import MILTERMACROS, MILTERMACRO_TYPES
 
 try:
     import libmilter as lm
 
     # overwrite debug logger if required
@@ -417,35 +416,35 @@
             for recipient in suspect.recipients:
                 self.add_rcpt(recipient)
 
         if (self.enable_mode_auto or self.enable_mode_autoheaders) and not replace_headers:
             lvl = logging.WARNING if len(suspect.modified_headers) > 0 else logging.INFO
             self.logger.log(lvl, f"{suspect.id} Modify {len(suspect.modified_headers)} headers according to modification track in suspect")
             for key, val in iter(suspect.modified_headers.items()):
-                hdr = Header(val, header_name=key, continuation_ws=' ')
+                hdr = fold_header(key, val, value_only=True)
                 self.changeheader(key, hdr.encode())
 
         if replace_headers:
             self.logger.warning(f"{suspect.id} Remove {len(self.sess.original_headers)} original headers ")
             self.remove_headers()
 
             msg = suspect.get_message_rep()
             self.logger.warning(f"{suspect.id} Add {len(msg)} headers from suspect mail")
             for key, val in iter(msg.items()):
                 self.loggerheaders.debug(f"{suspect.id} Add header from msg-> {key}: {val}")
-                hdr = Header(val, header_name=key, continuation_ws=' ')
+                hdr = fold_header(key, val, value_only=True)
                 self.addheader(key, hdr.encode())
         # --
         # headers to add, same as for the other connectors
         # --
         lvl = logging.WARNING if len(suspect.addheaders) > 0 else logging.INFO
         self.logger.log(lvl, f"{suspect.id} Add {len(suspect.addheaders)} headers as defined in suspect")
         for key, val in iter(suspect.addheaders.items()):
-            hdr = Header(val, header_name=key, continuation_ws=' ')
             self.loggerheaders.debug(f"{suspect.id} Add suspect header-> {key}: {val}")
+            hdr = fold_header(key, val, value_only=True)
             self.addheader(key, hdr.encode())
 
         if replace_body:
             self.logger.warning(f"{suspect.id} Replace message body")
             msg_string = suspect.get_message_rep().as_string()
             # just dump everything below the headers
 
@@ -695,15 +694,22 @@
 
     def _clean_address(self, address: tp.Optional[bytes]) -> tp.Optional[bytes]:
         address_cleaned = None
         # convert address to string
         if address is not None:
             addr_split = address.split(b'\0', maxsplit=1)
             address_cleaned = addr_split[0].strip(b'<>')
-            address_cleaned = address_cleaned.rstrip(b'.')  # remove trailing .
+            address_cleaned_stripped = address_cleaned.strip()
+            if address_cleaned != address_cleaned_stripped:
+                self.logger.info(f"{self.id} Stripped unnecessary spaces from from/to-address(position=1): '{address_cleaned}' -> '{address_cleaned_stripped}'")
+            address_cleaned = address_cleaned_stripped.rstrip(b'.')  # remove trailing .
+            address_cleaned_stripped = address_cleaned.strip()
+            if address_cleaned != address_cleaned_stripped:
+                self.logger.info(f"{self.id} Stripped unnecessary spaces from from/to-address(position=2): '{address_cleaned}' -> '{address_cleaned_stripped}'")
+                address_cleaned = address_cleaned_stripped
         return address_cleaned
 
     def get_cleaned_from_address(self) -> bytes:
         """Return from_address, without <> qualification or other MAIL FROM parameters"""
         # now already cleaned while setting
         return self.sender
```

### Comparing `fuglu-1.4.0/src/fuglu/connectors/ncconnector.py` & `fuglu-1.5.0/src/fuglu/connectors/ncconnector.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/connectors/smtpconnector.py` & `fuglu-1.5.0/src/fuglu/connectors/smtpconnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 
 import smtplib
 import logging
 import socket
 import tempfile
 import os
 import re
+import time
 import typing as tp
 
-from fuglu.shared import Suspect, apply_template, get_outgoing_helo
+from fuglu.shared import Suspect, apply_template, get_outgoing_helo, fold_header
 from fuglu.protocolbase import ProtocolHandler, BasicTCPServer
 from fuglu.connectors.check import HealthCheckSuspect
-from email.header import Header
 from fuglu.stringencode import force_bString, force_uString
 from fuglu.bounce import FugluSMTPClient
 
 
 mailregex = re.compile(r"^[^@<>]+<((?:\".*\"|[^\"<>@\s]+)@[^<>@\s]+)>(\s.*)?$",
                        flags=re.IGNORECASE)
 
@@ -85,16 +85,16 @@
 
     # -> the original message source is bytes
     origmsgtxt = suspect.get_source()
     newheaders = ""
 
     for key in suspect.addheaders:
         val = suspect.addheaders[key]
-        hdr = Header(val, header_name=key, continuation_ws=' ')
-        newheaders += f"{key}: {hdr.encode()}\r\n"
+        hdr = fold_header(key, val)
+        newheaders += hdr
 
     # the original message should be in bytes, make sure the header added
     # is an encoded string as well
     modifiedtext = force_bString(newheaders) + force_bString(origmsgtxt)
     return modifiedtext
 
 
@@ -224,14 +224,29 @@
             else:
                 toaddr = ''
             self.logger.error(f'failed to initialise suspect with from=<{fromaddr}> to=<{toaddr}> : {str(e)}')
             raise
         return suspect
 
     def commitback(self, suspect):
+        retries = self.config.getint('main', 'outgoingretry', fallback=1)
+        while retries>0:
+            try:
+                self._commitback(suspect)
+                break
+            except ConnectionError as e:
+                retries=retries-1
+                if retries == 0:
+                    raise
+                else:
+                    self.logger.warning(f'{suspect.id} {e.__class__.__name__} in commitback: {str(e)}')
+                    time.sleep(0.1)
+            
+    
+    def _commitback(self, suspect):
         injectcode, injectanswer, queueid = self.re_inject(suspect)
         suspect.set_tag("injectanswer", injectanswer)
         suspect.set_tag("injectqueueid", queueid)
 
         if injectcode == 250:
             values = dict(injectanswer=injectanswer)
             message = apply_template(
@@ -265,22 +280,22 @@
     ST_INIT = 0
     ST_HELO = 1
     ST_MAIL = 2
     ST_RCPT = 3
     ST_DATA = 4
     ST_QUIT = 5
 
-    def __init__(self, socket, config):
+    def __init__(self, sock, config):
         self.config = config
         self.from_address = None
         self.recipients = []
         self.helo = None
         self.dataAccum = None
 
-        self.socket = socket
+        self.socket = sock
         self.state = SMTPSession.ST_INIT
         self.logger = logging.getLogger("fuglu.smtpsession")
         self.tempfilename = None
         self.tempfile = None
         self.smtpoptions = set()
         self.ehlo_options = ["SMTPUTF8", "8BITMIME", "SIZE"]
         self.healthcheck = False
```

### Comparing `fuglu-1.4.0/src/fuglu/core.py` & `fuglu-1.5.0/src/fuglu/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,21 +241,39 @@
                 'section': 'main',
                 'description': "outgoing hostname/ip where postfix is listening for re-injects.\nuse ${injecthost} to connect back to the IP where the incoming connection came from",
                 'default': "127.0.0.1",
             },
 
             'outgoingport': {
                 'section': 'main',
-                'description': "outgoing port  where postfix is listening for re-injects)",
+                'description': "outgoing port where postfix is listening for re-injects)",
                 'default': "10026",
             },
 
             'outgoinghelo': {
                 'section': 'main',
-                'description': "#outgoing helo we should use for re-injects\nleave empty to auto-detect current hostname",
+                'description': "outgoing helo we should use for re-injects\nleave empty to auto-detect current hostname",
+                'default': "",
+            },
+            
+            'outgoingretry': {
+                'section': 'main',
+                'description': "how many times should we try to re-inject before returning temporary error (after queue mode only)",
+                'default': '1',
+            },
+            
+            'bouncehost': {
+                'section': 'main',
+                'description': "outgoing hostname/ip where postfix is listening for bounces.\nsupports same template variables as outgoinghost. leave empty to use outgoinghost value.",
+                'default': "",
+            },
+            
+            'bounceport': {
+                'section': 'main',
+                'description': "outgoing port where postfix is listening for bounces.\nleave empty to use outgoingport value.",
                 'default': "",
             },
 
             'tempdir': {
                 'section': 'main',
                 'description': "temp dir where fuglu can store messages while scanning",
                 'default': "/tmp",
```

### Comparing `fuglu-1.4.0/src/fuglu/daemon.py` & `fuglu-1.5.0/src/fuglu/daemon.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/debug.py` & `fuglu-1.5.0/src/fuglu/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import socket
 import logging
 import datetime
 import traceback
 import string
 import os
 import weakref
+import tempfile
 from fuglu.stringencode import force_bString, force_uString
 from fuglu.shared import utcnow
 
 try:
     import objgraph
     OBJGRAPH_EXTENSION_ENABLED = True
 except ImportError:
@@ -53,16 +54,15 @@
 
         if isinstance(port, int):
             porttype = "inet"
             self.logger = logging.getLogger("fuglu.control.%s" % port)
             self.logger.debug('Starting Control/Info server on port %s' % port)
         else:
             porttype = "unix"
-            self.logger = logging.getLogger(
-                "fuglu.control.%s" % os.path.basename(port))
+            self.logger = logging.getLogger("fuglu.control.%s" % os.path.basename(port))
             self.logger.debug('Starting Control/Info server on %s' % port)
 
         self.port = port
         self.controller = controller
         self.stayalive = 1
 
         try:
@@ -80,15 +80,15 @@
                     pass
                 self._socket = socket.socket(
                     socket.AF_UNIX, socket.SOCK_STREAM)
                 self._socket.bind(port)
 
             self._socket.listen(5)
         except Exception as e:
-            self.logger.error('Could not start control server: %s' % e)
+            self.logger.error(f'Could not start control server: {e.__class__.__name__}: {str(e)}')
             sys.exit(1)
 
     def shutdown(self):
         self.stayalive = False
         self.logger.info("Control Server on port %s shutting down" % self.port)
         try:
             self._socket.shutdown(socket.SHUT_RDWR)
@@ -954,17 +954,18 @@
 
             if "selector" in keys:
                 selector = force_uString(args.get("selector", defaults["selector"]))
                 outdict["selector"] = selector
                 res += "* selector: %s\n" % selector
 
             if "filename" in keys:
+                tempdir = tempfile.mkdtemp(prefix='fuglu-debug')
                 filename = force_uString(args.get("filename", defaults["filename"]))
                 if not filename and len(outdict.get("typelist", [])) > 0:
-                    filename = os.path.join("/tmp", ".".join(outdict["typelist"])+".png")
+                    filename = os.path.join(tempdir, ".".join(outdict["typelist"])+".png")
 
                 outdict["filename"] = filename
                 res += "* filename: %s\n" % filename
         except Exception as e:
             res += f"Exception: {e}\n"
             logging.getLogger("fuglu.ControlSession.prepare_objectraph_list_from_dict").exception(e)
```

### Comparing `fuglu-1.4.0/src/fuglu/extensions/aioredisext.py` & `fuglu-1.5.0/src/fuglu/extensions/aioredisext.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,53 @@
+# -*- coding: utf-8 -*-
+#   Copyright Fumail Project
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+#
 import logging
 import socket
 import datetime
 from typing import AsyncIterator, Optional, Dict, Awaitable, Union
 
 try:
     import asyncio
     import redis.asyncio as aioredis
 
     from redis import __version__ as redisversion
     STATUS = f"redis.asyncio installed, redis version: {redisversion}"
     ENABLED = True
+    RETRY_ON_EXCS = (aioredis.ConnectionError,
+                 aioredis.TimeoutError,
+                 asyncio.exceptions.CancelledError,
+                 asyncio.exceptions.TimeoutError,
+                 )
 except ImportError:
     STATUS = "redis.asyncio not installed"
     ENABLED = False
     aioredis = None
     redisversion = 'unkonwn'
+    RETRY_ON_EXCS = (ConnectionError, TimeoutError)
 
 
 AIOREDIS_TIMEOUT = 10.0
 AIOEDIS_MAXATTEMPTS = 3
 REDIS_POOL_TIMEOUT = 10
 REDIS_POOL_MAXCON = 200
 
-RETRY_ON_EXCS = (aioredis.ConnectionError,
-                 aioredis.TimeoutError,
-                 asyncio.exceptions.CancelledError,
-                 asyncio.exceptions.TimeoutError,
-                 )
-
 
 class AIORedisBaseBackend:
     def __init__(self, backendconfig: str):
         super().__init__()
         self._url = backendconfig
         self._pool = None
         self._redis = None
@@ -52,15 +68,15 @@
                 socket_keepalive_options = {}
             self._pool = aioredis.BlockingConnectionPool(timeout=REDIS_POOL_TIMEOUT,
                                                          max_connections=REDIS_POOL_MAXCON,
                                                          socket_timeout=2,
                                                          socket_keepalive=True,
                                                          socket_connect_timeout=2.0,
                                                          socket_keepalive_options=socket_keepalive_options,
-                                                         retry_on_timeout=True,
+                                                         retry_on_timeout=False,
                                                          ).from_url(url=self._url)
         if self._redis is None:
             self.logger.debug(f"New redis instance connecting to pool(url={self._url})")
             self._redis = await aioredis.StrictRedis(connection_pool=self._pool)
         return self._redis
 
     async def get_redis(self, timeout: Optional[float] = None, timeout_attempts: Optional[int] = None):
@@ -86,40 +102,40 @@
                         self.logger.warning(f"Connection error in 'get_redis' - retry ({typestring}: {str(e)})")
                         await asyncio.sleep(0.1)
                     else:
                         self.logger.error(f"Connection error in 'get_redis': ({typestring}: {str(e)})", exc_info=e)
 
         return self._redis
 
-    async def hgetall(self, key: bytes, timeout: Optional[float] = None, timeout_attempts: Optional[int] = None) -> Optional[bytes]:
+    async def hgetall(self, key: bytes, timeout: Optional[float] = None, timeout_attempts: Optional[int] = None) -> Optional[Dict[bytes,bytes]]:
         keydata = None
         timeout = timeout if timeout else AIOREDIS_TIMEOUT
         attempts = timeout_attempts if timeout_attempts else AIOEDIS_MAXATTEMPTS
         while attempts:
             attempts -= 1
             try:
                 r = await self._get_redis(timeout=timeout)
                 keydata = await asyncio.wait_for(r.hgetall(key), timeout=timeout)
                 attempts = 0  # no more attempts
             except RETRY_ON_EXCS as e:
                 typestring = str(type(e)).replace("<", "").replace(">", "")
                 self._redis = None
                 if attempts:
-                    self.logger.warning(f"Connection error in 'hgetall' - retry ({typestring}: {str(e)})")
+                    self.logger.warning(f"Connection error in 'hgetall' key={key} - retry ({typestring}: {str(e)})")
                     await asyncio.sleep(0.1)
                 else:
-                    self.logger.error(f"Connection error in 'hgetall' ({typestring}: {str(e)})")
+                    self.logger.error(f"Connection error in 'hgetall' key={key} ({typestring}: {str(e)})")
             except Exception as e:
                 typestring = str(type(e)).replace("<", "").replace(">", "")
                 self._redis = None
                 if attempts:
-                    self.logger.warning(f"Connection error in 'hgetall' - retry ({typestring}: {str(e)})")
+                    self.logger.warning(f"Connection error in 'hgetall' key={key} - retry ({typestring}: {str(e)})")
                     await asyncio.sleep(0.1)
                 else:
-                    self.logger.error(f"Connection error in 'hgetall': ({typestring}: {str(e)})", exc_info=e)
+                    self.logger.error(f"Connection error in 'hgetall' key={key} ({typestring}: {str(e)})", exc_info=e)
         return keydata
 
     async def scan_iter(self, match: str = "*", count: int = 250, timeout: Optional[float] = None, timeout_attempts: Optional[int] = None) -> Optional[AsyncIterator]:
         iterator = None
         timeout = timeout if timeout else AIOREDIS_TIMEOUT
         attempts = timeout_attempts if timeout_attempts else AIOEDIS_MAXATTEMPTS
         while attempts:
@@ -129,26 +145,26 @@
                 #iterator = await asyncio.wait_for(r.scan_iter(match=match, count=count), timeout=timeout)
                 iterator = r.scan_iter(match=match, count=count)
                 attempts = 0  # no more attempts
             except RETRY_ON_EXCS as e:
                 typestring = str(type(e)).replace("<", "").replace(">", "")
                 self._redis = None
                 if attempts:
-                    self.logger.warning(f"Connection error in 'scan_iter' - retry ({typestring}) {str(e)}")
+                    self.logger.warning(f"Connection error in 'scan_iter' match={match} - retry ({typestring}) {str(e)}")
                     await asyncio.sleep(0.1)
                 else:
-                    self.logger.error(f"Connection error in 'scan_iter' ({typestring}) {str(e)}")
+                    self.logger.error(f"Connection error in 'scan_iter' match={match} ({typestring}) {str(e)}")
             except Exception as e:
                 typestring = str(type(e)).replace("<", "").replace(">", "")
                 self._redis = None
                 if attempts:
-                    self.logger.warning(f"Connection error in 'scan_iter' - retry ({typestring}) {str(e)}")
+                    self.logger.warning(f"Connection error in 'scan_iter' match={match} - retry ({typestring}) {str(e)}")
                     await asyncio.sleep(0.1)
                 else:
-                    self.logger.error(f"Connection error in 'scan_iter' ({typestring}) {str(e)}", exc_info=e)
+                    self.logger.error(f"Connection error in 'scan_iter' match={match} ({typestring}) {str(e)}", exc_info=e)
         if iterator:
             yield iterator
 
     async def hset(self, key: bytes, mapping: Dict, timeout: Optional[float] = None, timeout_attempts: Optional[int] = None) -> Awaitable:
         outdata = None
         timeout = timeout if timeout else AIOREDIS_TIMEOUT
         attempts = timeout_attempts if timeout_attempts else AIOEDIS_MAXATTEMPTS
@@ -158,54 +174,26 @@
                 r = await self._get_redis(timeout=timeout)
                 outdata = await asyncio.wait_for(r.hset(key, mapping=mapping), timeout=timeout)
                 attempts = 0  # no more attempts
             except RETRY_ON_EXCS as e:
                 typestring = str(type(e)).replace("<", "").replace(">", "")
                 self._redis = None
                 if attempts:
-                    self.logger.warning(f"Connection error in 'hset' - retry ({typestring}) {str(e)}")
-                    await asyncio.sleep(0.1)
-                else:
-                    self.logger.error(f"Connection error in 'hset' ({typestring}) {str(e)}")
-            except Exception as e:
-                typestring = str(type(e)).replace("<", "").replace(">", "")
-                self._redis = None
-                if attempts:
-                    self.logger.warning(f"Connection error in 'hset' - retry ({typestring}) {str(e)}")
-                    await asyncio.sleep(0.1)
-                else:
-                    self.logger.error(f"Connection error in 'hset' ({typestring}) {str(e)}", exc_info=e)
-        return outdata
-
-    async def hmset(self, key: bytes, mapping: Dict, timeout: Optional[float] = None, timeout_attempts: Optional[int] = None) -> Awaitable:
-        outdata = None
-        timeout = timeout if timeout else AIOREDIS_TIMEOUT
-        attempts = timeout_attempts if timeout_attempts else AIOEDIS_MAXATTEMPTS
-        while attempts:
-            attempts -= 1
-            try:
-                r = await self._get_redis(timeout=timeout)
-                outdata = await asyncio.wait_for(r.hmset(key, mapping=mapping), timeout=timeout)
-                attempts = 0  # no more attempts
-            except RETRY_ON_EXCS as e:
-                typestring = str(type(e)).replace("<", "").replace(">", "")
-                self._redis = None
-                if attempts:
-                    self.logger.warning(f"Connection error in 'hmset' - retry ({typestring}) {str(e)}")
+                    self.logger.warning(f"Connection error in 'hset' key={key} - retry ({typestring}) {str(e)}")
                     await asyncio.sleep(0.1)
                 else:
-                    self.logger.error(f"Connection error in 'hmset' ({typestring}) {str(e)}")
+                    self.logger.error(f"Connection error in 'hset' key={key} ({typestring}) {str(e)}")
             except Exception as e:
                 typestring = str(type(e)).replace("<", "").replace(">", "")
                 self._redis = None
                 if attempts:
-                    self.logger.warning(f"Connection error in 'hmset' - retry ({typestring}) {str(e)}")
+                    self.logger.warning(f"Connection error in 'hset' key={key} - retry ({typestring}) {str(e)}")
                     await asyncio.sleep(0.1)
                 else:
-                    self.logger.error(f"Connection error in 'hmset' ({typestring}) {str(e)}", exc_info=e)
+                    self.logger.error(f"Connection error in 'hset' key={key} ({typestring}) {str(e)}", exc_info=e)
         return outdata
 
     async def hincrby(self, key: bytes, field: bytes, increment: Union[int, float] = 1, timeout: Optional[float] = None, timeout_attempts: Optional[int] = None) -> Awaitable:
         outdata = None
         timeout = timeout if timeout else AIOREDIS_TIMEOUT
         attempts = timeout_attempts if timeout_attempts else AIOEDIS_MAXATTEMPTS
         while attempts:
@@ -217,54 +205,54 @@
                 else:
                     outdata = await asyncio.wait_for(r.hincrbyfloat(key, field, amount=increment), timeout=timeout)
                 attempts = 0  # no more attempts
             except RETRY_ON_EXCS as e:
                 typestring = str(type(e)).replace("<", "").replace(">", "")
                 self._redis = None
                 if attempts:
-                    self.logger.warning(f"Connection error in 'hincrby' - retry ({typestring}) {str(e)}")
+                    self.logger.warning(f"Connection error in 'hincrby' key={key} - retry ({typestring}) {str(e)}")
                     await asyncio.sleep(0.1)
                 else:
-                    self.logger.error(f"Connection error in 'hincrby' ({typestring}) {str(e)}")
+                    self.logger.error(f"Connection error in 'hincrby' key={key} ({typestring}) {str(e)}")
             except Exception as e:
                 typestring = str(type(e)).replace("<", "").replace(">", "")
                 self._redis = None
                 if attempts:
-                    self.logger.warning(f"Connection error in 'hincrby' - retry ({typestring}) {str(e)}")
+                    self.logger.warning(f"Connection error in 'hincrby' key={key} - retry ({typestring}) {str(e)}")
                     await asyncio.sleep(0.1)
                 else:
-                    self.logger.error(f"Connection error in 'hincrby' ({typestring}) {str(e)}", exc_info=e)
+                    self.logger.error(f"Connection error in 'hincrby' key={key} ({typestring}) {str(e)}", exc_info=e)
         return outdata
 
-    async def expire(self, key: bytes, time: Union[int, datetime.datetime], timeout: Optional[float] = None, timeout_attempts: Optional[int] = None) -> Awaitable:
+    async def expire(self, key: Union[bytes,str], time: Union[int, datetime.datetime], timeout: Optional[float] = None, timeout_attempts: Optional[int] = None) -> Awaitable:
         outdata = None
         timeout = timeout if timeout else AIOREDIS_TIMEOUT
         attempts = timeout_attempts if timeout_attempts else AIOEDIS_MAXATTEMPTS
         while attempts:
             attempts -= 1
             try:
                 r = await self._get_redis(timeout=timeout)
                 outdata = await asyncio.wait_for(r.expire(key, time), timeout=timeout)
                 attempts = 0  # no more attempts
             except RETRY_ON_EXCS as e:
                 typestring = str(type(e)).replace("<", "").replace(">", "")
                 self._redis = None
                 if attempts:
-                    self.logger.warning(f"Connection error in 'expire' - retry ({typestring}) {str(e)}")
+                    self.logger.warning(f"Connection error in 'expire' key={key} - retry ({typestring}) {str(e)}")
                     await asyncio.sleep(0.1)
                 else:
-                    self.logger.error(f"Connection error in 'expire' ({typestring}) {str(e)}")
+                    self.logger.error(f"Connection error in 'expire' key={key} ({typestring}) {str(e)}")
             except Exception as e:
                 typestring = str(type(e)).replace("<", "").replace(">", "")
                 self._redis = None
                 if attempts:
-                    self.logger.warning(f"Connection error in 'expire' - retry ({typestring}) {str(e)}")
+                    self.logger.warning(f"Connection error in 'expire' key={key} - retry ({typestring}) {str(e)}")
                     await asyncio.sleep(0.1)
                 else:
-                    self.logger.error(f"Connection error in 'expire' ({typestring}) {str(e)}", exc_info=e)
+                    self.logger.error(f"Connection error in 'expire' key={key} ({typestring}) {str(e)}", exc_info=e)
         return outdata
 
     async def close(self, timeout: Optional[float] = None):
         """Close open connections and pools"""
         timeout = timeout if timeout else AIOREDIS_TIMEOUT
         if self._redis:
             for url, red in self._redis.items():
@@ -282,8 +270,8 @@
                 except Exception as e:
                     typestring = str(type(e)).replace("<", "").replace(">", "")
                     self.logger.warning(f"Problem closing redis pool: ({typestring}) {str(e)}")
             self._pool = None
 
     def __del__(self):
         """destructor - make sure connections are all closed"""
-        self.close(timeout=3.0)
+        self.close(timeout=3.0)
```

### Comparing `fuglu-1.4.0/src/fuglu/extensions/dnsquery.py` & `fuglu-1.5.0/src/fuglu/extensions/dnsquery.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/extensions/elastic.py` & `fuglu-1.5.0/src/fuglu/extensions/elastic.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,27 +20,30 @@
 DISTRO_OPEN = 2
 
 
 HAVE_ELASTICSEARCH = DISTRO_NONE
 try:
     import elasticsearch as elasticclientlib
     ElasticClient = elasticclientlib.Elasticsearch
+    AsyncElasticClient = elasticclientlib.AsyncElasticsearch
     ElasticException = elasticclientlib.exceptions.ElasticsearchException
     HAVE_ELASTICSEARCH = DISTRO_ELASTIC
     STATUS = f'available, using elasticsearch {elasticclientlib.__versionstr__}'
 except ImportError:
     try:
         import opensearchpy as elasticclientlib
         ElasticClient = elasticclientlib.OpenSearch
+        AsyncElasticClient = elasticclientlib.AsyncOpenSearch
         ElasticException = elasticclientlib.exceptions.OpenSearchException
         HAVE_ELASTICSEARCH = DISTRO_OPEN
         STATUS = f'available, using opensearch {elasticclientlib.__versionstr__}'
     except ImportError:
         elasticclientlib = None
         ElasticClient = None
+        AsyncElasticClient = None
         STATUS = f'elasticsearch not installed'
 
         class ElasticException(Exception):
             pass
         
 ENABLED = HAVE_ELASTICSEARCH != DISTRO_NONE
```

### Comparing `fuglu-1.4.0/src/fuglu/extensions/filearchives.py` & `fuglu-1.5.0/src/fuglu/extensions/filearchives.py`

 * *Files 1% similar despite different names*

```diff
@@ -678,16 +678,16 @@
 
         Returns:
             (list) Returns a list of file paths within the archive
         """
         try:
             # extract filename from archive header if present:
             genericfilename, size = self._read_gzip_info(self._handle)
-        except IOError as e:
-            self.logger.warning(f'failed to extract gz filename from file header due to {str(e)}')
+        except Exception as e:
+            self.logger.warning(f'failed to extract gz filename and size from file header due to {e.__class__.__name__}: {str(e)}')
             genericfilename = ''
 
         # try to create a name from the archive name
         # gzipping a file creates the archive name by appending ".gz"
         if not genericfilename:
             genericfilename = self._archivename
```

### Comparing `fuglu-1.4.0/src/fuglu/extensions/filetype.py` & `fuglu-1.5.0/src/fuglu/extensions/filetype.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/extensions/fuzzyhashlib.py` & `fuglu-1.5.0/src/fuglu/extensions/fuzzyhashlib.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/extensions/redisext.py` & `fuglu-1.5.0/src/fuglu/protocolbase.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-#   Copyright Fumail Project
+#   Copyright Oli Schacher, Fumail Project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,243 +11,205 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #
 #
 import logging
+import pickle
+import socket
 import threading
-import time
-
-try:
-    import redis
-    from redis import StrictRedis
-    from redis import __version__ as redisversion
-    STATUS = f"redis installed, version: {redisversion}"
-    ENABLED = True
-    REDIS2 = redisversion.startswith('2')
-    if REDIS2:
-        logging.warning('support for redis-py version 2.x is deprecated in fuglu, please upgrade')
+from fuglu.scansession import SessionHandler
+import traceback
+from multiprocessing.reduction import ForkingPickler
+import os
+import sys
+from io import BytesIO
+from fuglu.logtools import createPIDinfo
+import typing as tp
+
+
+def set_keepalive_linux(sock, after_idle_sec=1, interval_sec=3, max_fails=5):
+    """Set TCP keepalive on an open socket.
+
+    It activates after 1 second (after_idle_sec) of idleness,
+    then sends a keepalive ping once every 3 seconds (interval_sec),
+    and closes the connection after 5 failed ping (max_fails), or 15 seconds
+    """
     try:
-        redisversion = [int(x) for x in redisversion.split('.')]
-        REDIS33X = (redisversion[0] == 3 and redisversion[1] >= 3) or redisversion[0] > 3
-    except Exception:
-        REDIS33X = None
-except ImportError:
-    STATUS = "redis not installed"
-    ENABLED = False
-    StrictRedis = object
-    redis = None
-    redisversion = 'n/a'
-    REDIS2 = False
-    REDIS33X = None
+        sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+        sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPIDLE, after_idle_sec)
+        sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPINTVL, interval_sec)
+        sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPCNT, max_fails)
+    except Exception as e:
+        logging.getLogger("fuglu.set_keepalive_linux").debug(f"Problem setting keepalive options: {e.__class__.__name__} {str(e)}")
+
+
+class ProtocolHandler(object):
+    protoname = 'UNDEFINED'
+
+    def __init__(self, sock, config):
+        self.socket = sock
+        self.config = config
+        self.logger = logging.getLogger('fuglu.%s' % self.__class__.__name__)
+        self.sess = None
+
+        self._att_mgr_cachesize = config.getint('performance', 'att_mgr_cachesize', fallback=None)
+        self._att_defaultlimit = self.config.getint('performance', 'att_mgr_default_maxextract', fallback=None)
+        self._att_maxlimit = self.config.getint('performance', 'att_mgr_hard_maxextract', fallback=None)
+
+    def remove_tmpfile(self):
+        tmpfile = self.get_tmpfile()
+        if tmpfile is not None:
+            try:
+                os.remove(tmpfile)
+            except OSError:
+                pass
+
+    def get_tmpfile(self):
+        tmpfilename = None
+        if self.sess is not None:
+            try:
+                tmpfilename = self.sess.tempfilename
+            except AttributeError:
+                tmpfilename = None
+        return tmpfilename
 
+    def get_suspect(self, **kwargs):
+        return None
 
-class RedisKeepAlive(StrictRedis):
-    """
-    Wrap standard Redis client to include a thread that
-    will keep sending a ping to the server which will prevent
-    connection timeout due to "timeout" setting in "redis.conf"
+    def commitback(self, suspect):
+        pass
 
-    Issue on github:
-    https://github.com/andymccurdy/redis-py/issues/722
+    def defer(self, reason):
+        pass
 
-    this should no longer be necessary as newer version of redispy
-    bring their own health_check_interval parameter
-    """
+    def discard(self, reason):
+        pass
+
+    def reject(self, reason):
+        pass
 
-    def __init__(self, *args, **kwargs):
+    def healthcheck_reply(self):
+        pass
+
+
+class BasicTCPServer(object):
+
+    def __init__(self, controller, port:int=10125, address:str="127.0.0.1", protohandlerclass=None):
+        if protohandlerclass is None:
+            protohandlerclass = ProtocolHandler
+        self.protohandlerclass = protohandlerclass
+        self.logger = logging.getLogger(f"fuglu.incoming.{port}")
+        self.logger.debug(f'Starting incoming Server on Port {port}, protocol={self.protohandlerclass.protoname}')
+        self.logger.debug(f'Incoming server process info: {createPIDinfo()} logger id: {id(self)}')
+        self.port = port
+        self.controller = controller
+        self.stayalive = True
+
+        addr_f = socket.getaddrinfo(address, 0)[0][0]
+
+        try:
+            self._socket = socket.socket(addr_f, socket.SOCK_STREAM)
+            self._socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            if sys.platform == 'linux':
+                set_keepalive_linux(self._socket)
+            self._socket.bind((address, port))
+            self._socket.listen(5)
+        except Exception as e:
+            self.logger.error(f'Could not start incoming Server on port {port}: {e.__class__.__name__}: {str(e)}')
+            self.stayalive = False
+
+    def shutdown(self):
+        self.logger.info(f"TCP Server on port {self.port} closing")
+        self.stayalive = False
+        try:
+            self._socket.shutdown(1)
+            self._socket.close()
+        except Exception:
+            pass
+
+    def serve(self):
+        # Important:
+        # -> do NOT create local variables which are copies of member variables like
+        # controller = self.controller
+        # threadpool = self.controller.threadpool
+        # procpool = self.controller.procpool
+        # Since thes variables might change while in the stayalive loop the process would get stuck,
+        # example: when sending SIGHUP which might recreate the processor pool or threads pool
+        #          which would then still point to the wrong (old) memory location and is therefore not served anymore
 
-        # check if pinginterval is given in kwargs
-        self._pinginterval = kwargs.pop("pinginterval", 0)
-        self._noisy = False
-        self.pingthread = None
+        threading.current_thread().name = f'{self.protohandlerclass.protoname} Server on Port {self.port}'
+        self.logger.info(f'{self.protohandlerclass.protoname} Server running on port {self.port}')
 
-        if self._pinginterval:
+        while self.stayalive:
             try:
-                # since redis 3.3.x there should be a variable "healtch_check_interval" which is doing exactly
-                # the pinginterval manually implemented before...
-                super(RedisKeepAlive, self).__init__(*args, **kwargs, health_check_interval=self._pinginterval)
-                logging.getLogger("fuglu.RedisKeepAlive").debug(f"Set ping interval {self._pinginterval} "
-                                                                f"for redis {redisversion} using "
-                                                                f"parameter health_check_interval")
+                self.logger.debug('Waiting for connection...')
+                nsd = self._socket.accept()
+                sock, addr = nsd
+                if not self.stayalive:
+                    break
+                handler_classname = self.protohandlerclass.__name__
+                handler_modulename = self.protohandlerclass.__module__
+                self.logger.debug(f'({createPIDinfo()}) Incoming connection [incoming server port: {self.port}, prot: {self.protohandlerclass.protoname}]')
+                if self.controller.threadpool:
+                    # this will block if queue is full
+                    self.controller.threadpool.add_task_from_socket(sock, handler_modulename, handler_classname, self.port)
+                elif self.controller.procpool:
+                    self.controller.procpool.add_task_from_socket(sock, handler_modulename, handler_classname, self.port)
+                elif self.controller.asyncprocpool:
+                    self.controller.asyncprocpool.add_task_from_socket(sock, handler_modulename, handler_classname, self.port)
+                else:
+                    ph = self.protohandlerclass(sock, self.controller.config)
+                    engine = SessionHandler(ph, self.controller.config, self.controller.prependers,
+                                            self.controller.plugins, self.controller.appenders, self.port,
+                                            self.controller.milterdict)
+                    engine.handlesession()
+            except ConnectionAbortedError:
+                if self.stayalive:
+                    self.logger.warning('Connection aborted - break and setting stayalive to False')
+                    self.stayalive = False
+                break
             except Exception as e:
-                if REDIS33X:
-                    logging.getLogger("fuglu.RedisKeepAlive").error(f"Setting ping interval {self._pinginterval} "
-                                                                    f"for redis {redisversion}: {e.__class__.__name__} {str(e)}")
-                super(RedisKeepAlive, self).__init__(*args, **kwargs)
-
-                # start a thread which will ping the server to keep
-                self.pingthread = threading.Thread(target=self.ping_and_wait)
-                self.pingthread.daemon = True
-                self.pingthread.start()
-        else:
-            # no ping interval, nothing special to do...
-            super(RedisKeepAlive, self).__init__(*args, **kwargs)
-
-    def ping_and_wait(self):
-        """Send a ping to the Redis server to keep connection alive"""
-        while True:
-            if self._noisy:
-                import logging
-                logging.getLogger("fuglu.RedisKeepAlive").debug("Sending ping to Redis Server")
-            self.ping()
-            time.sleep(self._pinginterval)
-
-
-class RedisPooledConn(object):
-    def __init__(self, redis_url: str = None, **args):
-        self.logger = logging.getLogger('fuglu.RedisPooledConn')
-        if 'password' in args.keys() and args['password']:
-            self.logger.warning(f'deprecated redis password config - include it in redis_conn URL')
-        elif 'password' in args.keys() and not args['password']:
-            del args['password']
-        self._pinginterval = args.pop("pinginterval", 0)
-
-        if 'retry_on_timeout' not in args.keys():
-            args['retry_on_timeout'] = True
-        if 'socket_keepalive' not in args.keys():
-            args['socket_keepalive'] = True
-        if 'health_check_interval' not in args.keys():
-            args['health_check_interval'] = 10
-        if 'socket_connect_timeout' not in args.keys():
-            args['socket_connect_timeout'] = 5
-        if 'client_name' not in args.keys():
-            args['client_name'] = f'fuglu'
-
-        if not redis_url:
-            self.pool = None
-        elif redis is None:
-            self.pool = None
-            self.logger.error('Redis python module not installed')
-        elif '://' in redis_url:
-            self.pool = redis.ConnectionPool(**args)
-            self.pool = self.pool.from_url(redis_url, retry_on_timeout=True)
-        else:
-            self.logger.warning(f'deprecated redis connection string {redis_url}')
-            host, port, db = redis_url.split(':')
-            self.pool = redis.ConnectionPool(host=host, port=port, db=int(db), **args)
-
-    def get_conn(self) -> StrictRedis:
-        if REDIS2 and self._pinginterval > 0:
-            args = {}
-            args['pinginterval'] = self._pinginterval
-            return RedisKeepAlive(connection_pool=self.pool, **args)
-        else:
-            return StrictRedis(connection_pool=self.pool)
-
-    def check_connection(self) -> bool:
-        if self.pool is None:
-            return False
-        else:
-            redisconn = self.get_conn()
-            return redisconn.ping()
-
-
-class ExpiringCounter(object):
-
-    def __init__(self, redis_pool: RedisPooledConn = None, ttl: int = 0, maxcount: int = 0):
-        self.redis_pool = redis_pool or RedisPooledConn()
-        self.ttl = ttl
-        self.maxcount = maxcount
-
-    def _to_int(self, value, default: int = 0) -> int:
-        """
-        Convert to integer if possible
-
-        Args:
-            value (str,unicode,bytes): string containing integer
-        Keyword Args:
-            default (int): value to be returned for conversion errors
+                exc = traceback.format_exc()
+                self.logger.error(f'Exception in serve(): {e.__class__.__name__}: {str(e)} - {exc}')
 
-        Returns:
-            (int) value from string or default value
 
-        """
-        try:
-            value = int(value)
-        except (ValueError, TypeError):
-            value = default
-        return value
-
-    def increase(self, key: str, value: int = 1):
-        """
-        Given the identifier, create a new entry for current time with given value.
-        Args:
-            key (str): identifier
-            value (int): value to set (increase) for current key and timestamp
-
-        Returns:
-            (int): return the increased counter value
-
-        """
-        redisconn = self.redis_pool.get_conn()
-        if self.maxcount > 0:
-            try:  # only increase if value is not already very high
-                values = redisconn.hgetall(key)
-                if len(values) > self.maxcount:
-                    return len(values)
-            except redis.exceptions.TimeoutError:
-                return 0
+def compress_task(sock:socket.socket, handler_modulename:str, handler_classname:str, port:int) -> tp.Tuple[bytes, str, str, int]:
+    """
+    Compress all the inputs required for a task into a tuple
+    Args:
+        sock (socket): Receiving socket
+        handler_modulename (str): Modulename of the handler to be used
+        handler_classname (str): Classname of the handler to be used
+        port (int):  incoming port
 
-        try:
-            ts = int(time.time()) + self.ttl
-            pipe = redisconn.pipeline()
-            # increase the value of 'ts' by 'value' for hash 'key'
-            pipe.hincrby(key, str(ts), value)  # returns the value of redis[key][ts], usually same as param value
-            pipe.expire(key, self.ttl)  # returns None, this is a safety measure to avoid stale keys
-            result = pipe.execute()
-            return result[0]
-        except redis.exceptions.TimeoutError:
-            return 0
-
-    def get_count(self, key: str, cleanup: bool = True) -> int:
-        """
-        Get value. This is the sum of the count values within the ttl value stored in the class.
-        Args:
-            key (str): identifier
-            cleanup (bool): Remove stale keys
-
-        Returns:
-            (int) aggregated value
-        """
-        count = 0
-        delkeys = []
-        redisconn = self.redis_pool.get_conn()
-        values = redisconn.hgetall(key)
-        ts = int(time.time())
-        for k, v in values.items():
-            if self._to_int(k) > ts:  # only count current keys
-                count += self._to_int(v)
-            elif cleanup:  # mark stale keys for cleanup
-                delkeys.append(k)
-
-        if delkeys and len(delkeys) == len(values):
-            # all keys are stale
-            redisconn.delete(key)
-        elif delkeys:
-            redisconn.hdel(key, *delkeys)
-
-        return count
-
-    def cleanup(self) -> None:
-        """
-        Remove stale entries from redis database
-        """
-        ts = int(time.time())
-        redisconn = self.redis_pool.get_conn()
-        for key in redisconn.scan_iter(match='*'):
-            delete = False
-            values = redisconn.hgetall(key)
-            if not values:
-                delete = True
-            else:
-                delkeys = []
-                for k, v in values.items():
-                    if self._to_int(k) <= ts:
-                        delkeys.append(k)
-                if delkeys and len(delkeys) == len(values):
-                    delete = True
-                elif delkeys:
-                    redisconn.hdel(key, *delkeys)
-            if delete:
-                redisconn.delete(key)
+    Returns:
+        tuple: All information suitable to put as a task in a queue
+
+    """
+    """ Pickle a socket This is required to pass the socket in multiprocessing"""
+    buf = BytesIO()
+    ForkingPickler(buf).dump(sock)
+    pickled_socket = buf.getvalue()
+
+    task = pickled_socket, handler_modulename, handler_classname, port
+    return task
+
+
+def uncompress_task(task:tp.Tuple[bytes, str, str, int]) -> tp.Optional[tp.Tuple[socket.socket,str,str,int]]:
+    """
+    Uncompress a task (which was created by "compress_task")
+
+    Args:
+        task (tuple): Tuple containing task information
+
+    Returns:
+        tuple: Tuple with uncompressed task objects
+
+    """
+    if task is None:
+        return None
+
+    pickled_socket, handler_modulename, handler_classname, port = task
+    sock = pickle.loads(pickled_socket) # nosemgrep python.lang.security.deserialization.pickle.avoid-pickle
+    return sock, handler_modulename, handler_classname, port
```

### Comparing `fuglu-1.4.0/src/fuglu/extensions/sql.py` & `fuglu-1.5.0/src/fuglu/extensions/sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,21 @@
 import json
 from io import StringIO
 import logging
 import traceback
 import weakref
 from fuglu.shared import default_template_values, FuConfigParser, Suspect, deprecated, get_default_cache
 from fuglu.utils.version import get_main_version
+from fuglu.stringencode import force_uString, force_bString
 import typing as tp
 import time
 import os
+import ssl
+import urllib.request
+import urllib.error
 
 modlogger = logging.getLogger('fuglu.extensions.sql')
 STATUS = "not loaded"
 try:
     from sqlalchemy import create_engine, text
     from sqlalchemy.orm import scoped_session, sessionmaker, declarative_base
     DeclarativeBase = declarative_base()
@@ -44,21 +48,14 @@
 
     def text(string):
         return string
 
 ENABLED = SQL_EXTENSION_ENABLED  # fuglu compatibility
 
 try:
-    import requests
-    requests.packages.urllib3.disable_warnings()
-    REQUESTS_AVAILABLE = True
-except ImportError:
-    REQUESTS_AVAILABLE = False
-
-try:
     import yaml
     YAML_AVAILABLE = True
 except ImportError:
     YAML_AVAILABLE = False
 
 
 _sessmaker = None
@@ -140,101 +137,124 @@
     def __init__(self, config: FuConfigParser, suspectid: str = '<unknown>'):
         self.logger = logging.getLogger('fuglu.sql.restconfig')
         self.config = config
         self.suspectid = suspectid
 
     _re_title = re.compile('<title>(.{1,1000})</title>', re.I)
 
-    def _get_errormsg(self, reply):
-        errmsg = reply.text
+    def _get_errormsg(self, errmsg:str) -> str:
         rgxtitle = self._re_title.search(errmsg)
         if rgxtitle:
             errmsg = rgxtitle.groups()[0]
         return errmsg
-
-    def _http_request(self, reqtype, jsondata, uri, headers, verify, timeout, retry=3):
-        req = getattr(requests, reqtype.lower())
-        reply = req(uri, headers=headers, json=jsondata, verify=verify, timeout=timeout)
-        if reply.status_code != 200:
+    
+    def _get_ssl_context(self) -> ssl.SSLContext:
+        """
+        create SSL context that accepts invalid or self-signed SSL certificates
+        :return: ssl context
+        """
+        ctx = ssl.create_default_context()
+        ctx.check_hostname = False
+        ctx.verify_mode = ssl.CERT_NONE
+        return ctx
+
+    def _http_request(self, reqtype:str, jsondata:tp.Optional[bytes], uri:str, headers:dict, verify:bool, timeout:float, retry:int=3) -> tp.Tuple[bytes, int]:
+        context = None
+        if not verify:
+            context = self._get_ssl_context()
+        req = urllib.request.Request(url=uri, data=jsondata, method=reqtype)
+        if not req.type in ['https', 'http']:
+            self.logger.error(f'{self.suspectid} not an http(s) URI: {uri}')
+            return b'', -1
+        for hdr in headers:
+            req.add_header(hdr, headers[hdr])
+        try:
+            with urllib.request.urlopen(req, timeout=timeout, context=context) as urlinfo: # nosemgrep CWE-939
+                status = urlinfo.status
+                content = urlinfo.read()
+                if status != 200:
+                    self.logger.warning(f'{self.suspectid} got unexpected status code {status} {self._get_errormsg(force_uString(content))} from {uri} for method {reqtype} and content {force_uString(jsondata)}')
+        except urllib.error.HTTPError as e:
             sleeptime = 0.1
-            if reply.status_code == 503:
+            if e.status == 503:
                 sleeptime = 2
             if retry > 0:
-                time.sleep(sleeptime * (4-retry))
-                self.logger.debug(f'{self.suspectid} got unexpected status code {reply.status_code} from {uri} retry {retry}')
-                reply = self._http_request(reqtype, jsondata, uri, headers, verify, timeout, retry=retry-1)
-            else:
-                self.logger.warning(f'{self.suspectid} got unexpected status code {reply.status_code} {self._get_errormsg(reply)} from {uri}')
-        return reply
+                time.sleep(sleeptime * (4 - retry))
+                try:
+                    errdoc = force_uString(e.fp.read())
+                    self.logger.debug(f'{self.suspectid} got unexpected status code {status} from {uri} retry {retry} error {errdoc}')
+                except Exception as e:
+                    self.logger.debug(f'{self.suspectid} got unexpected status code {status} from {uri} retry {retry} error getting error {e.__class__.__name__}: {str(e)}')
+                content, status = self._http_request(reqtype, jsondata, uri, headers, verify, timeout, retry=retry - 1)
+        return content, status
 
-    def _call(self, reqtype, jsondata, restapi_uri, headers, restapi_verify, timeout):
+    def call(self, reqtype:str, jsondata:tp.Optional[bytes], restapi_uri:str, headers:dict, restapi_verify:bool, timeout:float) -> tp.Any:
         try:
-            reply = self._http_request(reqtype, jsondata, restapi_uri, headers, restapi_verify, timeout)
-            if reply.status_code != 200:
+            body, status = self._http_request(reqtype, jsondata, restapi_uri, headers, restapi_verify, timeout)
+            if status != 200:
                 try:
-                    err = reply.json()
+                    err = json.loads(body)
                     errmsg = err['errorMessage']
                 except (KeyError, json.JSONDecodeError):
-                    errmsg = self._get_errormsg(reply)
+                    errmsg = self._get_errormsg(force_uString(body))
                 raise RESTAPIError(errmsg)
-            content = reply.json()
+            content = json.loads(body)
         except Exception as e:
+            self.logger.debug(f'{self.suspectid} got {e.__class__.__name__}: {str(e)} from {restapi_uri} with method {reqtype} and content {force_uString(jsondata)}')
             raise RESTAPIError(f'{e.__class__.__name__}: {str(e)}')
         return content
 
-    def get_headers(self):
+    def get_headers(self) -> tp.Dict[str,str]:
         restapi_headers = self.config.getlist('databaseconfig', 'restapi_headers', resolve_env=True)
         headers = {
             'User-Agent': f'Fuglu/{get_main_version().strip()}',
             'accept': 'application/json',
+            'content-type': 'application/json',
         }
         for item in restapi_headers:
             if not ':' in item:
                 self.logger.warning(f'{self.suspectid} invalid header definition {item}')
             else:
                 hdr, value = item.split(':', 1)
                 headers[hdr] = value
         return headers
 
     def get(self, endpoint: str, timeout: int = 0):
-        if not REQUESTS_AVAILABLE:
-            return []
         if not endpoint:
             return []
 
         restapi_uri = self.config.get('databaseconfig', 'restapi_uri', resolve_env=True)
         restapi_verify = self.config.getboolean('databaseconfig', 'restapi_verify', fallback=False)
         restapi_timeout = timeout or self.config.getfloat('databaseconfig', 'restapi_timeout', fallback=10)
 
         headers = self.get_headers()
 
         if not restapi_uri.endswith('/'):
             restapi_uri = f'{restapi_uri}/'
         restapi_uri = f'{restapi_uri}{endpoint}'
 
-        content = self._call('GET', None, restapi_uri, headers, restapi_verify, restapi_timeout)
+        content = self.call('GET', None, restapi_uri, headers, restapi_verify, restapi_timeout)
         return content
 
     def put(self, endpoint: str, jsondata, timeout: int = 0):
-        if not REQUESTS_AVAILABLE:
-            raise RESTAPIError('Requests unavailable')
         if not endpoint:
             raise RESTAPIError('no endpoint specified')
 
         restapi_uri = self.config.get('databaseconfig', 'restapi_uri', resolve_env=True)
         restapi_verify = self.config.getboolean('databaseconfig', 'restapi_verify', fallback=False)
         restapi_timeout = timeout or self.config.getfloat('databaseconfig', 'restapi_timeout', fallback=10)
 
         headers = self.get_headers()
 
         if not restapi_uri.endswith('/'):
             restapi_uri = f'{restapi_uri}/'
         restapi_uri = f'{restapi_uri}{endpoint}'
-
-        content = self._call('PUT', jsondata, restapi_uri, headers, restapi_verify, restapi_timeout)
+        
+        jsondata = force_bString(json.dumps(jsondata))
+        content = self.call('PUT', jsondata, restapi_uri, headers, restapi_verify, restapi_timeout)
         return content
 
 
 class SectionCacheRow(object):
     def __init__(self, config, scope, option, value):
         optionfield = config.get('databaseconfig', 'option_field', fallback='option')
         scopefield = config.get('databaseconfig', 'scope_field', fallback='scope')
@@ -311,15 +331,15 @@
                     result = session.execute(text(query), sqlvalues).fetchall()
                     self.sectioncache[section] = result
                 except Exception:
                     trb = traceback.format_exc()
                     self.logger.error(f'Error getting database config override section data: {trb}')
                 loaded = True
 
-        if REQUESTS_AVAILABLE and self.has_section('databaseconfig') \
+        if self.has_section('databaseconfig') \
                 and self.has_option('databaseconfig', 'restapi_uri') \
                 and self.has_option('databaseconfig', 'restapi_headers') \
                 and self.parentget('databaseconfig', 'restapi_uri'):
             content = self._get_rest(section, None)[0]
             cachable_sectiondata = []
             for scope in content:
                 scopedata = content[scope]
@@ -480,15 +500,15 @@
         else:
             self.cache.put_cache(self._mkcachekey(False, suspect.to_address, section, option), True, cache_ttl)
             self.cache.put_cache(self._mkcachekey(False, f'%{suspect.to_domain}', section, option), True, cache_ttl)
             self.cache.put_cache(self._mkcachekey(False, globalscope or '$GLOBAL', section, option), True, cache_ttl)
             return None, False
 
     def _get_rest(self, section: str, option: tp.Optional[str], **kwargs) -> tp.Tuple[tp.Any, bool]:
-        if (not REQUESTS_AVAILABLE) or (not self.has_section('databaseconfig')) \
+        if (not self.has_section('databaseconfig')) \
                 or (not self.has_option('databaseconfig', 'restapi_uri')) \
                 or (not self.has_option('databaseconfig', 'restapi_headers')):
             try:
                 return self.parentget(section, option, **kwargs), False
             except (configparser.NoSectionError, configparser.NoOptionError):
                 return None, False
 
@@ -533,15 +553,15 @@
 
         content = None
         if restapi_cachettl > 0:
             content = self.cache.get_cache(f'rest-{restapi_uri}')
         if content is None:
             restapi = RESTAPIConfig(config=FuConfigParser(), suspectid=suspect.id)
             # returns data for all scopes from this endpoint
-            content = restapi._call('GET', None, restapi_uri, headers, restapi_verify, restapi_timeout)
+            content = restapi.call('GET', None, restapi_uri, headers, restapi_verify, restapi_timeout)
             self.logger.debug(f'{suspect.id} fetched restapi data')
             if restapi_cachettl > 0:
                 self.cache.put_cache(f'rest-{restapi_uri}', content, restapi_cachettl)
         else:
             self.logger.debug(f'{suspect.id} using cached restapi data for section={section} option={option}')
 
         alldata = {}
@@ -594,16 +614,20 @@
             self.logger.warning(f'{suspect.id} no yaml file {yaml_filepath}')
             try:
                 return self.parentget(section, option, **kwargs), False
             except (configparser.NoSectionError, configparser.NoOptionError):
                 return None, False
 
         if not yaml_filepath in self.yamldata:
-            with open(yaml_filepath, 'r') as fp:
-                self.yamldata[yaml_filepath] = yaml.load(fp, Loader=yaml.FullLoader)
+            with open(yaml_filepath, 'r', encoding='utf-8') as fp:
+                try:
+                    configdict = yaml.full_load(fp)
+                except AttributeError:
+                    configdict = yaml.safe_load(fp)
+            self.yamldata[yaml_filepath] = configdict
             self.logger.debug(f'{suspect.id} loaded yaml file {yaml_filepath}')
 
         if option is None:
             alldata = {}
             sectiondata = self.yamldata[yaml_filepath].get(section, {})
             for o in sectiondata:
                 optiondata = sectiondata[o]
```

### Comparing `fuglu-1.4.0/src/fuglu/funkyconsole.py` & `fuglu-1.5.0/src/fuglu/funkyconsole.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/lib/patcheddkimlib.py` & `fuglu-1.5.0/src/fuglu/lib/patcheddkimlib.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/lib/patchedemail/message.py` & `fuglu-1.5.0/src/fuglu/lib/patchedemail/message.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/lib/patchedlibmilter.py` & `fuglu-1.5.0/src/fuglu/lib/patchedlibmilter.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/lib/ppymilterbase.py` & `fuglu-1.5.0/src/fuglu/lib/ppymilterbase.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/logtools.py` & `fuglu-1.5.0/src/fuglu/logtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #
 #
+import \
+    contextlib
 import logging
 import logging.handlers
 import logging.config
 import os
 import multiprocessing
 import signal
 import sys
@@ -371,7 +373,17 @@
     def __exit__(self, et, ev, tb):
         if self.level is not None:
             self.logger.setLevel(self.old_level)
         if self.handler:
             self.logger.removeHandler(self.handler)
         if self.handler and self.close:
             self.handler.close()
+
+
+@contextlib.contextmanager
+def get_context_logger(*args, **kwargs):
+    """Get a logger which is closed and removed at the end of the context"""
+    logger = logging.getLogger(*args, **kwargs)
+    try:
+        yield logger
+    finally:
+        del logger
```

### Comparing `fuglu-1.4.0/src/fuglu/mailattach.py` & `fuglu-1.5.0/src/fuglu/mailattach.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     HASHENC_HEX = 'hex'
     HASHENC_B64 = 'b64'
     HASHENC_B32 = 'b32'
 
     def __init__(self, buffer, filename, mgr, fugluid, filesize=None, in_obj=None, contenttype_mime=None,
                  maintype_mime=None, subtype_mime=None, ismultipart_mime=None, content_charset_mime=None,
                  is_attachment=False, is_inline=False, defects=None, filename_generated=False,
-                 archive_passwords = None):
+                 archive_passwords=None):
         """
         Constructor
 
         Args:
             fugluid (str): fuglu id
             buffer (bytes): buffer containing attachment source
             filename (str): filename of current attachment object
@@ -157,18 +157,25 @@
         self.defects = defects if defects else []  # make an empty list for None
         self.filename_generated = filename_generated
         self.archive_passwords = archive_passwords
         self.logger = logging.getLogger(f"fuglu.{self.__class__.__name__}")
 
         # use weak reference to avoid cyclic dependency
         self.in_obj = weakref.ref(in_obj) if in_obj is not None else None
-
+        
+        if not contenttype_mime and maintype_mime and subtype_mime:
+            contenttype_mime = f'{maintype_mime}/{subtype_mime}'
         self.contenttype_mime = contenttype_mime
+        if contenttype_mime and not maintype_mime:
+            maintype_mime = contenttype_mime.split('/',1)[0]
         self.maintype_mime = maintype_mime
+        if contenttype_mime and not subtype_mime:
+            subtype_mime = contenttype_mime.rsplit('/',1)[-1]
         self.subtype_mime = subtype_mime
+        
         self.ismultipart_mime = ismultipart_mime
         self.content_charset_mime = content_charset_mime
         self.is_attachment = is_attachment
         self.is_inline = is_inline
 
         # use weak reference to avoid cyclic dependency
         self._mgr = weakref.ref(mgr) if mgr is not None else None  # keep only weak reference
@@ -943,14 +950,15 @@
             cachelimit (int): cachelimit for keeping attachments during Suspect lifetime
             default_filelimit (int): default maximum filelimit to extract files if not defined otherwise
             max_filelimit (int): maximum filelimit to extract files, limiting all other limits
             default_numfilelimit (int): default maximum number of files extracted from a single archive
             max_numfilelimit (int): maximum number of files extracted from a single archive, limiting all other limits
         """
         self._msgrep = msgrep
+        self._manually_added = []  # List of manually added Mailattachments
         self.fugluid = fugluid
         if section is None:
             self.section = self.__class__.__name__
         else:
             self.section = section
         self.logger = logging.getLogger(f"fuglu.{self.__class__.__name__}")
 
@@ -1114,15 +1122,15 @@
                                                            is_attachment=isattachment, is_inline=isinline,
                                                            defects=defects, filename_generated=att_name_generated)
             else:
                 # No caching of the object
                 newatt_file_dict[counter] = None
         return newatt_file_dict
 
-    def get_mailatt_generator(self, archives_passwords:tp.Optional[tp.List[str]]):
+    def get_mailatt_generator(self, archives_passwords: tp.Optional[tp.List[str]]):
         """
         Dictionary storing attachments in mail. Key is filename, value is list of
         Mailattachment objects for given name.
 
         Internal member dependencies:
             - _msgrep (email.message.Message): Email message
 
@@ -1340,16 +1348,16 @@
 
         return (att_name, buffer, attsize,
                 contenttype_mime, maintype_mime,
                 subtype_mime, ismultipart_mime,
                 content_charset_mime, isattachment,
                 isinline, defects, att_name_generated)
 
-    @smart_cached_memberfunc(inputs=['att_file_dict'])
-    def get_fileslist(self, level: int = 0,
+    @smart_cached_memberfunc(inputs=['att_file_dict', '_manually_added'])
+    def get_fileslist(self, level: int | None = 0,
                       maxsize_extract: tp.Optional[int] = None,
                       maxfiles_extract: tp.Optional[int] = None,
                       archives_passwords: tp.Optional[tp.List[str]] = None):
         """
         (Cached Member Function)
 
         Get list of all filenames attached to message. For given recursion level attached
@@ -1369,14 +1377,18 @@
         file_list = []
         for att_obj in self.get_mailatt_generator(archives_passwords):
             file_list.extend(att_obj.get_fileslist(0, level,
                                                    self.get_maxsize_extract(maxsize_extract),
                                                    self.get_maxfilenum_extract(maxfiles_extract)
                                                    )
                              )
+
+        # add manually added attachment filenames
+        file_list.extend(obj.filename for obj in self._manually_added)
+
         return file_list
 
     def get_objectlist(self, level: int = 0,
                        maxsize_extract: tp.Optional[int] = None,
                        noextractinfo: tp.Optional[NoExtractInfo] = None,
                        include_parents: bool = False,
                        maxfiles_extract: tp.Optional[int] = None,
@@ -1403,14 +1415,17 @@
         g = self.get_mailatt_generator(archives_passwords)
 
         for att_obj in g:
             obj_list.extend(att_obj.get_objectlist(0, level,
                                                    self.get_maxsize_extract(maxsize_extract),
                                                    self.get_maxfilenum_extract(maxfiles_extract),
                                                    noextractinfo=noextractinfo, include_parents=include_parents))
+        # add manually added mailattachments
+        obj_list.extend(self._manually_added)
+
         return obj_list
 
     def get_fileslist_checksum(self, level: int = 0,
                                maxsize_extract: tp.Optional[int] = None,
                                methods: tp.Tuple = (),
                                noextractinfo: tp.Optional[NoExtractInfo] = None,
                                maxfiles_extract: tp.Optional[int] = None,
@@ -1430,11 +1445,34 @@
         obj_list = []
         for att_obj in self.get_mailatt_generator(archives_passwords):
             obj_list.extend(att_obj.get_objectlist(0, level,
                                                    self.get_maxsize_extract(maxsize_extract),
                                                    self.get_maxfilenum_extract(maxfiles_extract),
                                                    noextractinfo=noextractinfo))
 
+        # add manually added mailattachments
+        obj_list.extend(self._manually_added)
+
         checksumlist = []
         for obj in obj_list:
             checksumlist.append((obj.filename, obj.get_checksumdict(methods=methods)))
         return checksumlist
+
+    def manual_add(self, buffer: bytes, filename: str, filesize: int | None = None, contenttype_mime=None,
+                   maintype_mime=None, subtype_mime=None, ismultipart_mime=None, content_charset_mime=None):
+        """Manually add mailattachment to list independent of python message object linked...
+
+        Args:
+            buffer (bytes): buffer containing attachment source
+            filename (str): filename of current attachment object
+            filesize (int): file size in bytes (set to length of buffer if unset)
+            contenttype_mime (str): The contenttype as defined in the mail attachment, only available for direct mail attachments
+            maintype_mime (str): The main contenttype as defined in the mail attachment, only available for direct mail attachments
+            subtype_mime (str): The sub-contenttype as defined in the mail attachment, only available for direct mail attachments
+            ismultipart_mime (str): multipart as defined in the mail attachment, only available for direct mail attachments
+            content_charset_mime (str): The characterset as defined in the mail attachment, only available for direct mail attachments
+        """
+
+        m = Mailattachment(buffer, filename if filename else "unknown", self, fugluid=self.fugluid, filesize=filesize if isinstance(filesize, int) else len(buffer), contenttype_mime=contenttype_mime,
+                           maintype_mime=maintype_mime, subtype_mime=subtype_mime, ismultipart_mime=ismultipart_mime, content_charset_mime=content_charset_mime,
+                           is_attachment=True, is_inline=False, filename_generated=bool(filename))
+        self._manually_added.append(m)
```

### Comparing `fuglu-1.4.0/src/fuglu/mixins.py` & `fuglu-1.5.0/src/fuglu/mixins.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/mplugins/demo.py` & `fuglu-1.5.0/src/fuglu/mplugins/demo.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/mshared.py` & `fuglu-1.5.0/src/fuglu/mshared.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/__init__.py` & `fuglu-1.5.0/src/fuglu/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/a_logging.py` & `fuglu-1.5.0/src/fuglu/plugins/a_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 #
 #
 from fuglu.shared import AppenderPlugin, apply_template, get_outgoing_helo, FileList, actioncode_to_string, FuConfigParser, Suspect
 from fuglu.stringencode import force_uString, force_bString
 from fuglu.mailattach import NoExtractInfo
 from fuglu.caching import smart_cached_memberfunc
 from fuglu.plugins.uriextract import EXCLUDE_DOMAIN, EXCLUDE_FQDN
-from fuglu.extensions.elastic import ElasticClient, ElasticException, lint_elastic
+from fuglu.extensions.elastic import ElasticClient, AsyncElasticClient, ElasticException, lint_elastic
 from fuglu.extensions.dnsquery import revlookup
 from email.header import Header
 import datetime
 import time
 import re
 import os
 import json
 import logging
 import urllib
 import urllib.parse
 import hashlib
 import copy
+import asyncio
 import typing as tp
 try:
     from domainmagic import extractor, tld
     from domainmagic.mailaddr import strip_batv, decode_srs, domain_from_mail, split_mail
     from domainmagic.validators import is_email, is_url_tldcheck
     HAVE_DOMAINMAGIC = True
 except ImportError:
@@ -213,15 +214,15 @@
                 'src': emails.get(addr, 'unknown')
             }
             urilist.append(logitem)
         return urilist
 
 
 SKIP_ARCHIVE_RE = [
-    re.compile('^LOG/[0-9]{1,20}\.DLF$') # found in .idab
+    re.compile(r'^LOG/[0-9]{1,20}\.DLF$') # found in .idab
 ]
 class AttLogger(object):
     def __init__(self, config, section):
         self.logger = logging.getLogger(f'fuglu.plugins.logging.{self.__class__.__name__}')
         self.config = config
         self.section = section
 
@@ -276,39 +277,35 @@
                 'in_archive': attObj.in_archive,
                 'is_archive_pw': attObj.is_protected_archive,
             }
             for hashtype in hashes:
                 logitem[hashtype] = attObj.get_checksum(hashtype)
             attachments.append(logitem)
             count += 1
+        self.logger.debug(f'{suspect.id} got {len(attachments)} attachments')
         return attachments
 
 
 class ElasticBackend(object):
     def __init__(self, config, section):
         self.config = config
         self.section = section
         self.logger = logging.getLogger(f'fuglu.logging.{self.__class__.__name__}')
-        self.elastic_connection = {}
         self.mapping_file = None
 
-    def get_elastic_connection(self, reload:bool=False) -> ElasticClient:
+    def get_elastic_connection(self, use_async:bool=False) -> tp.Union[ElasticClient, AsyncElasticClient]:
         es = None
         elastic_uris = self.config.getlist(self.section, 'elastic_uris', resolve_env=True)
         if elastic_uris:
-            elastic_uri_string = ','.join(elastic_uris)
-            try:
-                if reload:
-                    del self.elastic_connection[elastic_uri_string]
-                es = self.elastic_connection[elastic_uri_string]
-            except KeyError:
-                verify_certs = self.config.getboolean(self.section, 'elastic_verify_certs')
-                timeout = self.config.getfloat(self.section, 'elastic_timeout')
+            verify_certs = self.config.getboolean(self.section, 'elastic_verify_certs')
+            timeout = self.config.getfloat(self.section, 'elastic_timeout', fallback=30)
+            if use_async:
+                es = AsyncElasticClient(hosts=elastic_uris, verify_certs=verify_certs, ssl_show_warn=False, timeout=timeout)
+            else:
                 es = ElasticClient(hosts=elastic_uris, verify_certs=verify_certs, ssl_show_warn=False, timeout=timeout)
-                self.elastic_connection[elastic_uri_string] = es
         return es
 
     def get_elastic_index(self, suspect: Suspect) -> str:
         indextmpl = self.config.get(self.section, 'elastic_index')
         tagindexlist = [item.rsplit(':', 1) for item in self.config.getlist(self.section, 'elastic_index_by_tags')]
         for tag, itmpl in tagindexlist:
             if suspect.get_tag(tag):
@@ -341,16 +338,20 @@
             properties = current_mapping.get(indexname, {}).get('mappings', {}).get('properties', {})
 
             mapping_file = self.config.get(self.section, 'elastic_mapping_file', fallback='')
             new_mapping = self._get_mapping(mapping_file)
 
             try:
                 for key in new_mapping['properties']:
+                    proptype = properties.get(key, {}).get('type')
                     if not new_mapping['properties'][key]['type'] == properties.get(key, {}).get('type'):
                         need_put = True
+                        self.logger.debug(f"mapping update required due to property of key '{key}'\n:"
+                                          f"new: {json.dumps(new_mapping['properties'][key]['type'], indent=4)}\n\n"
+                                          f"current: {json.dumps(proptype, indent=4)}")
                         break
             except KeyError as e:
                 need_put = False
                 if mapping_file:
                     self.logger.error(f'failed to load mapping file {mapping_file}: {e.__class__.__name__}: {str(e)}')
                 else:
                     self.logger.error(f'invalid mapping: {e.__class__.__name__}: {str(e)}')
@@ -359,49 +360,68 @@
                 try:
                     r = es.indices.put_mapping(body=LOG_MAPPING, index=indexname)
                 except ElasticException as e:
                     r = {'exc': e.__class__.__name__, 'msg': str(e)}
                 if r.get('acknowledged'):
                     self.logger.info(f'put new mapping to elastic index {indexname}')
                 else:
-                    self.logger.info(f'error putting new mapping to elastic index {indexname} : {str(r)}')
+                    self.logger.info(f'error putting new mapping to elastic index {indexname} : {str(r)}\n'
+                                     f'Input data body ways:\n'
+                                     f'{json.dumps(LOG_MAPPING, indent=4)}')
             else:
                 self.logger.debug(f'no need to update mapping of elastic index {indexname}')
         else:
             try:
                 log_mapping = {'mappings': LOG_MAPPING}
+                replicas = self.config.get(self.section, 'elastic_replicas', resolve_env=True)
+                try:
+                    replicas = int(replicas)
+                except (TypeError, ValueError):
+                    self.logger.debug('not setting replicas')
+                    replicas = None
+                if replicas is not None:
+                    log_mapping['settings'] = {'index': {'number_of_replicas': replicas}}
                 r = es.indices.create(indexname, body=log_mapping)
             except ElasticException as e:
                 r = {'exc': e.__class__.__name__, 'msg': str(e)}
             if r.get('acknowledged'):
                 self.logger.info(f'created new elastic index {indexname}')
             else:
                 self.logger.info(f'error creating new elastic index {indexname} : {str(r)}')
+            try:
+                self.logger.debug(f"body to create elastic index was:\n{json.dumps(log_mapping, indent=4)}")
+            except Exception:
+                # don't let logging break code
+                self.logger.exception(e)
+                pass
 
-    def log_to_elastic(self, suspect: Suspect, logdata: tp.Dict[str, tp.Any], rcpt_id: int, reload=False, retry: int = 3) -> tp.Dict[str, str]:
-        result = {}
+    async def log_to_elastic(self, suspect: Suspect, logdata: tp.Dict[str, tp.Any], rcpt_id: int, retry: int = 3) -> tp.Dict[str, str]:
+        result = {'rcpt_id': rcpt_id}
         try:
             logdata['timestamp'] = datetime.datetime.utcfromtimestamp(suspect.timestamp).isoformat()
-            es = self.get_elastic_connection(reload)
+            es = self.get_elastic_connection(use_async=True)
             indexname = self.get_elastic_index(suspect)
             self._set_index_mapping(indexname)
             documentid = f'{suspect.id}_{rcpt_id}'
-            timeout = self.config.getfloat(self.section, 'elastic_timeout')
-            r = es.index(index=indexname, id=documentid, body=logdata, request_timeout=timeout)
+            timeout = self.config.getfloat(self.section, 'elastic_timeout', fallback=30)
+            try:
+                r = await es.index(index=indexname, id=documentid, body=logdata, request_timeout=timeout)
+            finally:
+                await es.close()
             for key in ['_id', 'result']:
                 try:
                     result[key] = r[key]
                 except KeyError:
                     self.logger.warning(f'{suspect.id} key {key} not found in result {r}')
             self.logger.debug(f'{suspect.id} indexed in elastic {indexname}: {dict2str(r)}')
         except Exception as e:
             if retry > 0:
                 self.logger.debug(f'{suspect.id} failed to index in elastic, retry={retry} reason={e.__class__.__name__}: {str(e)}')
                 time.sleep(0.2*(4-retry))
-                result = self.log_to_elastic(suspect, logdata, rcpt_id, reload=True, retry=retry-1)
+                result = await self.log_to_elastic(suspect, logdata, rcpt_id, retry=retry-1)
             else:
                 raise
         return result
 
 
 class ElasticLogger(AppenderPlugin):
     """
@@ -422,28 +442,36 @@
                 'default': 'True',
                 'description': 'verify server\'s SSL certificates',
             },
             'elastic_timeout': {
                 'default': '30',
                 'description': 'set elastic connection timeout to this value',
             },
+            'elastic_retry': {
+                'default': '3',
+                'description': 'how many retries on elastic logging errors (e.g. timeouts)',
+            },
             'elastic_index': {
                 'default': 'fuglulog-${date}',
                 'description': 'Name of ElasticSearch index in which document will be stored. Template vars (e.g. ${to_domain} or ${date}) can be used.',
             },
             'elastic_mapping_file': {
                 'default': '',
                 'description': 'read elastic mapping from json file. leave empty to use default mapping.',
             },
+            'elastic_replicas': {
+                'default': '',
+                'description': 'override number of replicas. leave empty for default.',
+            },
             'elastic_index_by_tags': {
                 'default': '',
                 'description': 'Comma separated list of tuples of SuspectTag:IndexName of ElasticSearch index in which document will be stored. Template vars (e.g. ${to_domain} or ${date}) can be used for index name. SuspectTag value must evaluate to True. First hit wins.',
             },
             'log_headers': {
-                'default': 'from:addr,to:pseudo:md5,reply-to:addr,subject,subject:decode,subject:hash:md5,message-id:low',
+                'default': 'from:addr,from:namedecode,to:pseudo:md5,reply-to:addr,subject,subject:decode,subject:hash:md5,message-id:low',
                 'description:': """
                     Name of message headers to log and extract.
                     Address headers (e.g. To, From, Reply-To) support tags such as :addr (address only), :pseudo:algo (address only, with hashed localpart), :name (name label only), :namedecode (name label only, decoded).
                     All header support tag hash:algo - algo must be one of hashlibs supported hash algorithms
                     All headers support tag decode - try decode encoded headers
                     All header support tag low - lowercase value
                     All header names will be prefixed hdr_ in elastic document, - and : will be converted to _
@@ -746,16 +774,18 @@
                 logdata[key] = value
         return logdata
 
     def _get_raw_headers(self, suspect: Suspect, header_names: tp.List[str]) -> tp.List[tp.Dict[str, str]]:
         allhdr = header_names[0] == 'all'
         headerdata = []
         hdrline = 0
+        add_headers = list(suspect.addheaders.items())
         msgrep = suspect.get_message_rep()
-        headers = msgrep.items()
+        msg_headers = msgrep.items()
+        headers = add_headers + msg_headers
         hdrlines = len(headers)
         for hdr_name, hdr_content in headers:
             hdr_name_low = hdr_name.lower()
             if not (allhdr or hdr_name_low in header_names):
                 continue
             hdrline += 1
             hdrdata = {}
@@ -973,39 +1003,53 @@
             self.logger.warning(f'{suspect.id} not logging: cannot get elastic connection')
             return
         
         timeout = self.config.getint(self.section, 'timeout')
         suspect.stimeout_set_timer(self.section, timeout)
         self._add_tags(suspect, decision)
         core_logdata = self._get_log_coredata(suspect)
+        asyncio.run(self._async_process(suspect, core_logdata))
+        
+        
+    async def _async_process(self, suspect, core_logdata):
         rcpt_id = 0
         rcpt_count = len(suspect.recipients)
+        tasks = []
+        all_logdata = {}
+        retry = self.config.getint(self.section, 'elastic_retry')
         for recipient in suspect.recipients:
             #self.logger.debug(f'{suspect.id} preparing log data for recipient={recipient} with rcpt_id={rcpt_id}')
             recipient = recipient.lower()
             suspect.set_tag('to_address', recipient)
             suspect.set_tag('to_domain', domain_from_mail(recipient))
             suspect.set_tag('to_localpart', split_mail(recipient)[0])
             suspect.set_tag('recipient_id', rcpt_id)
             suspect.set_tag('insidemail', suspect.get_tag('log.sender_domain') == suspect.get_tag('to_domain'))
             logdata = self._get_log_userdata(suspect, copy.deepcopy(core_logdata))
-            self.logger.debug(f'{suspect.id} sending approximately {len(str(logdata))}b to elasticsearch')
-            starttime = time.time()
-            try:
-                result = self.elasticbackend.log_to_elastic(suspect, logdata, rcpt_id)
-                processtime = time.time()-starttime
-                self.logger.info(f'{suspect.id} processed with result {dict2str(result)} in {processtime:.2f}s')
-            except Exception as e:
-                processtime = time.time()-starttime
-                self.logger.error(f'{suspect.id} failed to index in elastic in {processtime:.2f}s due to {e.__class__.__name__} {str(e)}')
-                self._log_to_file(suspect, logdata, rcpt_id)
+            all_logdata[rcpt_id] = logdata
+            if retry >= 0: # disable elastic and dump straight to json file if retry is negative
+                future = self.elasticbackend.log_to_elastic(suspect, logdata, rcpt_id, retry=retry)
+                tasks.append(future)
+            else:
+                self.logger.warning(f'{suspect.id} retry={retry} not writing to elastic')
             rcpt_id += 1
             if not suspect.stimeout_continue(self.section) and rcpt_id<rcpt_count:
                 self.logger.error(f'{suspect.id} exceeded elastic data aggregation timeout after {rcpt_id} / {rcpt_count} recipients')
-                break
+                self._log_to_file(suspect, logdata, rcpt_id)
+                
+        results = await asyncio.gather(*tasks, return_exceptions=True)
+        for result in results:
+            if isinstance(result, Exception):
+                self.logger.error(f'{suspect.id} failed to index in elastic due to {result.__class__.__name__} {str(result)}')
+            else:
+                rcpt_id = result['rcpt_id']
+                self.logger.info(f'{suspect.id} processed {len(str(all_logdata[rcpt_id]))}b with result {dict2str(result)}')
+                del all_logdata[rcpt_id]
+        for rcpt_id in all_logdata:
+            self._log_to_file(suspect, all_logdata[rcpt_id], rcpt_id)
         
         if suspect.get_tag('loggererror') is True:
             self._write_eml(suspect)
 
     def lint(self):
         if not HAVE_DOMAINMAGIC:
             print('ERROR: domainmagic library missing, this plugin will do nothing')
@@ -1041,14 +1085,29 @@
             for key in new_mapping['properties']:
                 if not new_mapping['properties'][key]['type']:
                     print(f'empty value in key {key}')
                     return False
         except KeyError as e:
             print(str(e))
             return False
+        
+        retry = self.config.getint(self.section, 'elastic_retry')
+        if retry < 0:
+            print(f'WARNING: retry={retry} not writing to elastic')
+        
+        replicas = self.config.get(self.section, 'elastic_replicas', resolve_env=True)
+        try:
+            replicas = int(replicas)
+        except (TypeError, ValueError):
+            replicas = None
+
+        if replicas is not None:
+            print(f'INFO: setting to {replicas} replicas when creating indices')
+        else:
+            print(f'INFO: not overriding number of replicas...')
 
         return True
 
 
 class ElasticImport(object):
     def __init__(self, configfile):
         self.config = FuConfigParser()
@@ -1060,15 +1119,15 @@
         self.section = 'ElasticLogger'
         self.backend = ElasticBackend(self.config, 'ElasticLogger')
 
     def _log_to_elastic(self, indexname, suspectid, logdata):
         es = self.backend.get_elastic_connection()
         self.backend._set_index_mapping(indexname)
         success = True
-        timeout = self.config.getfloat(self.section, 'elastic_timeout')
+        timeout = self.config.getfloat(self.section, 'elastic_timeout', fallback=30)
         r = es.index(index=indexname, id=suspectid, body=logdata, request_timeout=timeout)
         if not '_id' in r:
             print(f'{suspectid} key _id not found in result {r}')
             success = False
         print(f'{suspectid} indexed in elastic {indexname}: {dict2str(r)}')
         return success
 
@@ -1083,14 +1142,19 @@
                 for filename in filenames:
                     if filename.endswith('.json'):
                         suspectid = filename.rsplit('.')[0]
                         filepath = os.path.join(dirpath, indexname, filename)
                         with open(filepath) as fp:
                             filecontent = json.load(fp)
                         try:
+                            if re.match(r'^[0-9]+\.[0-9]+$', filecontent['timestamp']):
+                                ts = float(filecontent['timestamp'])
+                                dt = datetime.datetime.utcfromtimestamp(ts).isoformat()
+                                filecontent['timestamp'] = dt
+                                print(f'WARNING: found timestamp as {ts} converted to {dt}')
                             success = self._log_to_elastic(indexname, suspectid, filecontent)
                             if success and cleanup:
                                 os.remove(filepath)
                         except Exception as e:
                             print(f'failed to import {filepath} due to {e.__class__.__name__}: {str(e)}')
             if cleanup:
                 self._cleanup_dirs(dirpath)
@@ -1123,8 +1187,12 @@
         sys.exit(1)
     elif args.mapping:
         print('Logger indices mapping:')
         print(json.dumps(LOG_MAPPING))
         sys.exit(0)
     elif importconfig:
         elimp = ElasticImport(importconfig)
-        elimp.load_files(not args.keepfiles)
+        try:
+            elimp.load_files(not args.keepfiles)
+        except KeyboardInterrupt:
+            print('aborted by user')
+            sys.exit(0)
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/a_statsd.py` & `fuglu-1.5.0/src/fuglu/plugins/a_statsd.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/antivirus.py` & `fuglu-1.5.0/src/fuglu/plugins/antivirus.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
             s = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
             s.settimeout(self.config.getfloat(self.section, 'timeout'))
             try:
                 s.connect(sock)
             except socket.error:
                 raise Exception('Could not reach SSSP server using unix socket %s' % sock)
         else:
-            host = self.config.get(self.section, 'host')
+            host = self.config.get(self.section, 'host', resolve_env=True)
             port = self.config.getint(self.section, 'port')
             timeout = self.config.getfloat(self.section, 'timeout')
             try:
                 s = socket.create_connection((host, port), timeout)
             except socket.error:
                 raise Exception('Could not reach SSSP server using network (%s, %s)' % (host, port))
             set_keepalive_linux(s)
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/archive.py` & `fuglu-1.5.0/src/fuglu/plugins/archive.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,62 +14,82 @@
 # limitations under the License.
 #
 #
 from fuglu.shared import ScannerPlugin, DUNNO, SuspectFilter, apply_template, get_outgoing_helo, Suspect
 from fuglu.stringencode import force_uString, force_bString
 from fuglu.extensions.elastic import ElasticClient, lint_elastic, ElasticException
 from fuglu.caching import smart_cached_memberfunc
+from fuglu.utils.version import get_main_version
 import os
 import shutil
 import pwd
 import grp
 import logging
 import time
 import smtplib
 import socket
 import datetime
 from collections import OrderedDict
 from base64 import b64encode
+from urllib.parse import urljoin
+import urllib.request
+import typing as tp
 
 try:
     from cassandra.cluster import Cluster
     from cassandra.policies import RoundRobinPolicy
     from cassandra import __version__ as cassandraversion
     HAVE_CASSANDRA = True
 except ImportError:
     HAVE_CASSANDRA = False
 
+try:
+    import boto3
+    from botocore.exceptions import ClientError as S3ClientError
+    from botocore.client import Config as S3Config
+    HAVE_S3 = True
+except ImportError:
+    HAVE_S3 = False
+
 
 LOG_MAPPING = {
     "properties": {
         "blob": {
             "type": "binary"
         }
     }
 }
 
+class ArchiveException(Exception):
+    pass
 
 class AbstractBackend(object):
     requiredvars = {}
 
     def __init__(self, config, section):
         self.config = config
         self.section = section
-        self.logger = logging.getLogger('fuglu.archive.backend.%s' % self.__class__.__name__)
+        self.logger = logging.getLogger(f'{__package__}.backend.{self.__class__.__name__}')
 
     def __str__(self):
         return self.__class__.__name__
 
-    def archive(self, suspect, fugluid_override=None):
+    def archive(self, suspect: Suspect, fugluid_override: str=None) -> tp.Dict[str,str]:
+        """
+        writes to actual archive. raise exception if archiving failed
+        :param suspect: the suspect object
+        :param fugluid_override: an alternative fuglu/suspect id to be logged instead of suspect.id
+        :return: dict with result data
+        """
         raise NotImplementedError
 
     def lint(self):
         raise NotImplementedError
 
-    def _get_msg_source(self, suspect, original=True):
+    def _get_msg_source(self, suspect: Suspect, original:bool=True) -> bytes:
         if original:
             content = suspect.get_original_source()
         else:
             content = suspect.get_source()
         return content
 
 
@@ -163,15 +183,15 @@
     def lint(self):
         archivedir = self.config.get(self.section, 'local_archivedir')
         if archivedir == "":
             print('Archivedir is not specified')
             return False
 
         if not os.path.isdir(archivedir):
-            print("Archivedir '%s' does not exist or is not a directory" % archivedir)
+            print(f"Archivedir {archivedir} does not exist or is not a directory")
             return False
 
         return True
 
     def _setperms(self, filename, chmod, chgrp, chown, fugluid):
         """Set file permissions and ownership
         :param filename The target file
@@ -234,15 +254,15 @@
             except Exception as e:
                 self.logger.error(f'{fugluid} Could not change user/group of file {filename} : {e.__class__.__name__}: {str(e)}')
 
 
 class ElasticBackend(AbstractBackend):
     """
     This backend stores mail in ElasticSearch.
-    Status: experimental
+    Status: Mature (using opensearch)
     """
     requiredvars = {
         'elastic_uris': {
             'default': '',
             'description': 'comma separated list of ElasticSearch host definition (hostname, hostname:port, https://user:pass@hostname:port/)',
         },
         'elastic_verify_certs': {
@@ -253,14 +273,18 @@
             'default': '30',
             'description': 'set elastic connection timeout to this value',
         },
         'elastic_index': {
             'default': 'fugluquar-${date}',
             'description': 'Name of ElasticSearch index in which document will be stored. Template vars (e.g. ${to_domain} or ${date}) can be used.',
         },
+        'elastic_replicas': {
+            'default': '',
+            'description': 'override number of replicas. leave empty for default.',
+        },
         'elastic_extrafields': {
             'default': '',
             'description': 'comma separated list of additional fields to be added to document. Any fuglu Suspect variable is permitted (e.g. to_address)',
         },
         'elastic_useoriginal': {
             'default': 'True',
             'description': """should we store the original message as retreived from postfix or store the
@@ -302,14 +326,15 @@
 
             new_mapping = LOG_MAPPING
 
             try:
                 for key in new_mapping['properties']:
                     if not new_mapping['properties'][key]['type'] == properties.get(key, {}).get('type'):
                         need_put = True
+                        self.logger.debug(f"mapping update required due to property of key '{key}'")
                         break
             except KeyError as e:
                 need_put = False
                 self.logger.error(f'invalid mapping: {e.__class__.__name__}: {str(e)}')
 
             if need_put:
                 try:
@@ -321,14 +346,22 @@
                 else:
                     self.logger.info(f'error putting new mapping to elastic index {indexname} : {str(r)}')
             else:
                 self.logger.debug(f'no need to update mapping of elastic index {indexname}')
         else:
             try:
                 log_mapping = {'mappings': LOG_MAPPING}
+                replicas = self.config.get(self.section, 'elastic_replicas', resolve_env=True)
+                try:
+                    replicas = int(replicas)
+                except (TypeError, ValueError):
+                    self.logger.debug('not setting replicas')
+                    replicas = None
+                if replicas is not None:
+                    log_mapping['settings'] = {'index': {'number_of_replicas': replicas}}
                 r = es.indices.create(indexname, body=log_mapping)
             except ElasticException as e:
                 r = {'exc': e.__class__.__name__, 'msg': str(e)}
             if r.get('acknowledged'):
                 self.logger.info(f'created new elastic index {indexname}')
             else:
                 self.logger.info(f'error creating new elastic index {indexname} : {str(r)}')
@@ -366,17 +399,17 @@
                 indexname = self._get_elastic_index(suspect)
                 self._set_index_mapping(indexname)
                 r = es.index(index=indexname, id=suspect.id, body=doc, request_timeout=30)
                 for key in ['_id', 'result']:
                     try:
                         result[key] = r[key]
                     except KeyError:
-                        self.logger.error('%s key %s not found in result %s' % (suspect.id, key, r))
+                        self.logger.error(f'{suspect.id} key {key} not found in result {r}')
 
-                self.logger.info('%s indexed in elastic: %s' % (suspect.id, r))
+                self.logger.info(f'{suspect.id} indexed in elastic: {r}')
                 retry = 0  # stop while loop
             except Exception as e:
                 if retry > 0:
                     self.logger.debug(f'{suspect.id} failed to index in elastic, retry={retry} reason={e.__class__.__name__}: {str(e)}')
                     time.sleep(0.2*(4-retry))
                     reload = True
                     #result = self.archive(suspect, fugluid_override, reload=True, retry=retry-1)
@@ -392,14 +425,25 @@
         if es is None:
             print('WARNING: elastic_uris not defined, this backend will do nothing')
             return False
         if not es.ping():
             elastic_uris = self.config.getlist(self.section, 'elastic_uris', resolve_env=True)
             print(f'ERROR: failed to connect to elasticsearch {", ".join(elastic_uris)}, connection info: {str(es)}')
             return False
+        
+        replicas = self.config.get(self.section, 'elastic_replicas', resolve_env=True)
+        try:
+            replicas = int(replicas)
+        except (TypeError, ValueError):
+            replicas = None
+
+        if replicas is not None:
+            print(f'INFO: setting to {replicas} replicas when creating indices')
+        else:
+            print(f'INFO: not overriding number of replicas...')
 
         return True
 
 
 class CassandraBackend(AbstractBackend):
     """
     This backend stores mail in an Apache Cassandra database cluster.
@@ -449,40 +493,201 @@
         content = self._get_msg_source(suspect, original)
         try:
             session = self.get_cassandra_session()
             fugluid = fugluid_override or suspect.id
             session.execute(self.cass_prep_quarantine, (fugluid, bytearray(content), ttl), timeout=20)
         except Exception as e:
             if retry > 0:
-                self.logger.info('%s failed to write to cassandra. try %s/3. error was: %s' % (suspect.id, retry, str(e)))
+                self.logger.info(f'{suspect.id} failed to write to cassandra. try {retry}/3. error was: {e.__class__.__name__}: {str(e)}')
                 time.sleep(0.1)
                 self._cassandra_store(suspect, fugluid_override, retry-1)
             else:
                 raise
 
     def archive(self, suspect, fugluid_override=None):
         result = {}
         self._cassandra_store(suspect, fugluid_override)
-        self.logger.info('%s stored in cassandra' % suspect.id)
+        self.logger.info(f'{suspect.id} stored in cassandra')
         result['success'] = True
         return result
 
     def lint(self):
         if not HAVE_CASSANDRA:
             print('ERROR: cassandra driver not available')
             return False
 
-        print("INFO: Cassandra Driver Version: %s" % cassandraversion)
+        print(f"INFO: Cassandra Driver Version: {cassandraversion}")
 
         try:
             self.get_cassandra_session().execute("SELECT * FROM quarantine WHERE fugluid='dummy'")
         except Exception as e:
-            print("ERROR: cassandra connection failed: %s" % str(e))
+            print(f"ERROR: cassandra connection failed: {e.__class__.__name__}: {str(e)}")
+            return False
+
+        return True
+
+
+class S3Backend(AbstractBackend):
+    """
+    This backend stores mail in S3 (or compatible) storage
+    Status: experimental
+    """
+    requiredvars = {
+        's3_uri': {
+            'default': '',
+            'description': "s3 uri",
+        },
+        's3_bucket': {
+            'default': 'fugluquar',
+            'description': "quarantine s3 bucket name",
+        },
+        's3_access_id': {
+            'default': '',
+            'description': "s3 access id",
+        },
+        's3_access_key': {
+            'default': '',
+            'description': "s3 access secret key",
+        },
+        's3_ttl': {
+            'default': str(14*24*3600),
+            'description': "ttl for quarantined files in seconds",
+        },
+    }
+    
+    
+    def _get_s3_connection(self):
+        s3_uri = self.config.get(self.section, 's3_uri')
+        s3_access_id = self.config.get(self.section, 's3_access_id')
+        s3_access_key = self.config.get(self.section, 's3_access_key')
+        
+        config = S3Config(
+           signature_version = 's3v4'
+        )
+        s3 = boto3.resource('s3',
+                    endpoint_url=s3_uri,
+                    aws_access_key_id=s3_access_id,
+                    aws_secret_access_key=s3_access_key,
+                    config=config)
+        return s3
+    
+    def archive(self, suspect, fugluid_override=None):
+        result = {'success': False}
+        if not HAVE_S3:
+            return result
+        
+        s3 = self._get_s3_connection()
+        
+        bucketname = self.config.get(self.section, 's3_bucket')
+        ttl = self.config.getint(self.section, 's3_ttl')
+        exp = datetime.datetime.now() + datetime.timedelta(seconds=ttl)
+        filename = f'{fugluid_override or suspect.id}.eml'
+        try:
+            s3.create_bucket(bucketname)
+            s3obj = s3.Object(bucket_name=bucketname, key=filename)
+            s3obj.put(
+                Body=suspect.get_source(),
+                ContentType='message/rfc822',
+                Expires=exp,
+            )
+            result['success'] = True
+        except S3ClientError as e:
+            raise ArchiveException(f'{suspect.id} failed to write data to bucket {bucketname} as {filename} due to {str(e)}')
+        return result
+
+    def lint(self):
+        if not HAVE_S3:
+            print('ERROR: s3 library (boto3) not available')
             return False
+        else:
+            s3 = self._get_s3_connection()
+            bucketname = self.config.get(self.section, 's3_bucket')
+            try:
+                s3.meta.client.head_bucket(Bucket=bucketname)
+            except S3ClientError as e:
+                s3_uri = self.config.get(self.section, 's3_uri')
+                print(f'ERROR: failed to access {bucketname} on {s3_uri} due to {str(e)}')
+
+        return True
+
 
+
+class WebDavBackend(AbstractBackend):
+    """
+    This backend stores mail in webdav storage
+    Status: experimental
+    """
+    requiredvars = {
+        'webdav_uri': {
+            'default': '',
+            'description': "webdav base uri (e.g. https://webdav.example.com/path/to/quar)",
+        },
+        'webdav_username': {
+            'default': '',
+            'description': "webdav username",
+        },
+        'webdav_password': {
+            'default': '',
+            'description': "webdav password",
+        },
+    }
+    
+    def _install_passman(self, webdav_uri):
+        username = self.config.get(self.section, 'webdav_username')
+        password = self.config.get(self.section, 'webdav_password')
+        
+        passman = urllib.request.HTTPPasswordMgrWithDefaultRealm()
+        passman.add_password(None, webdav_uri, username, password)
+        authhandler = urllib.request.HTTPBasicAuthHandler(passman)
+        opener = urllib.request.build_opener(authhandler)
+        urllib.request.install_opener(opener)
+    
+    def archive(self, suspect, fugluid_override=None):
+        result = {'success': False}
+        webdav_uri = self.config.get(self.section, 'webdav_uri')
+        self._install_passman(webdav_uri)
+        
+        filename = f'{fugluid_override or suspect.id}.eml'
+        uri = urljoin(webdav_uri, filename)
+        
+        try:
+            req = urllib.request.Request(url=uri, data=suspect.get_source(), method='PUT')
+            if not req.type in ['https', 'http']:
+                self.logger.error(f'{suspect.id} not an http(s) URI: {webdav_uri}')
+                return result
+            req.add_header('User-Agent', f'Fuglu/{get_main_version().strip()}')
+            with urllib.request.urlopen(req) as f: # nosemgrep CWE-939
+                pass
+            if 200 <= f.status <= 299: # put ok can be 201
+                result['success'] = True
+                result['archiveuri'] = uri
+                self.logger.info(f'{suspect.id} successful upload to {uri}')
+            else:
+                self.logger.error(f'{suspect.id} failed to upload to {uri} due to {f.status} {f.reason}')
+        except Exception as e:
+            raise ArchiveException(f'{suspect.id} failed to upload to {uri} due to {e.__class__.__name__}: {str(e)}')
+        return result
+
+    def lint(self):
+        webdav_uri = self.config.get(self.section, 'webdav_uri')
+        self._install_passman(webdav_uri)
+        try:
+            req = urllib.request.Request(url=webdav_uri, method='HEAD')
+            if not req.type in ['https', 'http']:
+                print(f'ERROR: not an http(s) URI: {webdav_uri}')
+                return False
+            req.add_header('User-Agent', f'Fuglu/{get_main_version().strip()}')
+            with urllib.request.urlopen(req) as f: # nosemgrep CWE-939
+                pass
+            if 200 <= f.status <= 299:
+                print(f'ERROR: failed to check {webdav_uri} due to {f.status} {f.reason}')
+                return False
+        except Exception as e:
+            print(f'ERROR: failed to check {webdav_uri} due to {e.__class__.__name__}: {str(e)}')
+            return False
         return True
 
 
 dovecot_username_chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ01234567890.-_@'
 
 
 def dovecot_username(username):
@@ -597,25 +802,25 @@
         lmtp_hosts = self.config.getlist(self.section, 'lmtp_hosts')
 
         s = None
         if not lmtp_hosts:
             return None
         elif lmtp_hosts[0].startswith('/'):  # unix socket
             if not os.path.exists(lmtp_hosts[0]):
-                raise Exception('unix socket %s not found' % lmtp_hosts)
+                raise ArchiveException(f'unix socket {lmtp_hosts} not found')
             s = MyLMTP(lmtp_hosts)
         else:
             hosttuples = [self._parse_host_port(h, defaultport=MyLMTP.LMTP_PORT) for h in lmtp_hosts]
             for host, port in hosttuples:
                 try:
                     s = MyLMTP(host, port, timeout=30)
                 except (socket.error, ConnectionRefusedError):
                     continue
             if s is None and hosttuples:
-                raise Exception('no LMTP server is reachable')
+                raise ArchiveException('no LMTP server is reachable')
         return s
 
     def __auth(self, lmtp):
         user = self.config.get(self.section, 'lmtp_user')
         password = self.config.get(self.section, 'lmtp_password')
         if user and password:
             lmtp.login(user, password)
@@ -636,22 +841,21 @@
             # sendmail_address will make sure address type is correct for Py2/3, unicode/str/bytes
             # force_bString is bytes because we don't want the internal algorithm to play with
             # the message and try to encode it...
             rcpt = dovecot_username(suspect.to_address)
             senderrs, resp = lmtp.sendmail(force_uString(lmtpfrom), force_uString(rcpt), force_bString(content))
             lmtp.quit()
             if rcpt in senderrs:
-                raise Exception('%s LMTP delivery error to %s on %s' % (suspect.id, rcpt, host))
+                raise ArchiveException(f'{suspect.id} LMTP delivery error to {rcpt} on {host}')
             else:
                 lmtp_id = self._lmtp_queueid(resp)
-                self.logger.info('%s message delivered to LMTP server %s with LMTP ID %s' % (suspect.id, host, lmtp_id))
+                self.logger.info(f'{suspect.id} message delivered to LMTP server {host} with LMTP ID {lmtp_id}')
         except Exception as e:
             if retry > 0:
-                self.logger.debug(
-                    '%s LMTP delivery failed. try %s/3 on %s. error was: %s' % (suspect.id, retry, host, str(e)))
+                self.logger.debug(f'{suspect.id} LMTP delivery failed. try {retry}/3 on {host}. error was: {e.__class__.__name__}: {str(e)}')
                 time.sleep(0.1)
                 self.__do_quarantine(suspect, content, retry - 1)
             else:
                 raise
 
         return host, lmtp_id
 
@@ -698,30 +902,32 @@
         try:
             lmtp = self.__init_socket()
             if lmtp is None:
                 print('ERROR: no LMTP connection defined')
                 return False
             helo = lmtp.docmd('LHLO', get_outgoing_helo(self.config))
             helostr = helo[1].decode('utf-8')
-            print('LMTP server sez: %s %s' % (helo[0], helostr))
+            print(f'LMTP server sez: {helo[0]} {helostr}')
             self.__auth(lmtp)
             lmtp.quit()
             success = True
         except Exception as e:
-            print('ERROR: LMTP connection error: %s' % str(e))
+            print(f'ERROR: LMTP connection error: {e.__class__.__name__}: {str(e)}')
             success = False
 
         return success
 
 
 ARCHIVE_BACKENDS = OrderedDict()
 ARCHIVE_BACKENDS['localdir'] = LocalDirBackend
 ARCHIVE_BACKENDS['lmtp'] = LMTPBackend
 ARCHIVE_BACKENDS['elastic'] = ElasticBackend
 ARCHIVE_BACKENDS['cassandra'] = CassandraBackend
+ARCHIVE_BACKENDS['s3'] = S3Backend
+ARCHIVE_BACKENDS['webdav'] = WebDavBackend
 
 
 class ArchivePlugin(ScannerPlugin):
     r"""
 This plugin stores a copy of the message if it matches certain criteria (Suspect Filter).
 You can use this if you want message archives for your domains, need a quarantine or to debug problems occuring only for certain recipients.
 The architecture allows to store data in various backends (databases), either simultaneously or using one backend as main and others as fallback in case the main backend is unavailable.
@@ -859,15 +1065,15 @@
         suspect.set_tag('archived', False)
         self.logger.debug(f"{suspect.id} archive -> loading rules")
         archiverules = self.config.get(self.section, 'archiverules')
         if archiverules is None or archiverules == "":
             return DUNNO
 
         if not os.path.exists(archiverules):
-            self.logger.error('%s Archive Rules file does not exist: %s' % (suspect.id, archiverules))
+            self.logger.error(f'{suspect.id} Archive Rules file does not exist: {archiverules}')
             return DUNNO
 
         self.logger.debug(f"{suspect.id} archive -> setup SuspectFilter with arhive rules")
         if self.filter is None:
             self.filter = SuspectFilter(archiverules)
 
         self.logger.debug(f"{suspect.id} archive -> set_archive_tags")
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/attachment.py` & `fuglu-1.5.0/src/fuglu/plugins/attachment.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 from threading import Lock
 try:
     from domainmagic.rbl import RBLLookup
     DOMAINMAGIC_AVAILABLE = True
 except ImportError:
     DOMAINMAGIC_AVAILABLE = False
 try:
+    import six
+    import sys
+    if sys.version_info >= (3, 12, 0): # https://github.com/dpkp/kafka-python/issues/2401#issuecomment-1760208950
+        sys.modules['kafka.vendor.six.moves'] = six.moves
     import kafka
     KAFKA_AVAILABLE = True
 except ImportError:
     KAFKA_AVAILABLE = False
 
 
 FUATT_NAMESCONFENDING = "-filenames.conf"
@@ -840,15 +844,15 @@
     def _get_body_words(self, suspect: Suspect):
         maxwordcount = self.config.getint(self.section, 'archive_passwords_maxbodywords')
         words = set()
         if maxwordcount > 0:
             minwordlength = self.config.getint(self.section, 'archive_passwords_minwordlength')
             maxtextpartlength = self.config.getint(self.section, 'archive_passwords_maxtextpartlength')
             
-            textparts = [suspect.get_header('subject', '')]
+            textparts = [force_uString(suspect.get_header('subject', ''))]
             sf = SuspectFilter()
             textparts.extend(sf.get_decoded_textparts(suspect, attachment=False))
             for textpart in textparts:
                 words.update({w for w in textpart[:maxtextpartlength].split() if len(w)>=minwordlength})
         return list(words)[:maxwordcount]
         
     
@@ -1256,18 +1260,14 @@
         self.logger = self._logger()
 
         self.requiredvars = {
             'redis_conn': {
                 'default': '',
                 'description': 'redis backend database connection: redis://host:port/dbid',
             },
-            'pinginterval': {
-                'default': '0',
-                'description': 'ping redis interval to prevent disconnect (0: don\'t ping)'
-            },
             'timeout': {
                 'default': '2',
                 'description': 'redis/kafka timeout in seconds'
             },
             'hashtype': {
                 'default': 'MD5',
                 'description': 'the hashing algorithm to be used',
@@ -1473,22 +1473,21 @@
             print('WARNING: extensions list is empty')
 
         return success
 
     def _init_redis(self):
         """
         initializes Redis on first call and returns the Redis connection object. Aborts the program if redis configuration is malformed.
-        :return: (RedisKeepAlive)
+        :return: (StrictRedis)
         """
         if self.redis_pool is None:
             redis_conn = self.config.get(self.section, 'redis_conn')
             if redis_conn:
                 timeout = self.config.getint(self.section, 'timeout'),
-                pinginterval = self.config.getint(self.section, 'pinginterval')
-                self.redis_pool = RedisPooledConn(redis_conn, socket_keepalive=True, socket_timeout=timeout, pinginterval=pinginterval)
+                self.redis_pool = RedisPooledConn(redis_conn, socket_timeout=timeout)
 
     def _check_hash(self, suspect, myhash):
         virusname = None
         self._init_redis()
 
         if self.redis_pool is not None:
             attempts = 2
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/bacn.py` & `fuglu-1.5.0/src/fuglu/plugins/bacn.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/call_ahead.py` & `fuglu-1.5.0/src/fuglu/plugins/call_ahead.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 import fuglu.connectors.asyncmilterconnector as asm
 import fuglu.connectors.milterconnector as sm
 from fuglu.mshared import BMPRCPTMixin, BasicMilterPlugin
 from fuglu.shared import _SuspectTemplate, Cache, FuConfigParser, FileList, get_outgoing_helo, utcnow
 from fuglu.stringencode import force_uString
 from fuglu.extensions.sql import SQL_EXTENSION_ENABLED, get_session, DBConfig, RESTAPIError, text
 from fuglu.extensions.dnsquery import lookup, DNSQUERY_EXTENSION_ENABLED, mxlookup
-from fuglu.extensions.redisext import RedisPooledConn, ENABLED as REDIS_ENABLED, REDIS2
+from fuglu.extensions.redisext import RedisPooledConn, ENABLED as REDIS_ENABLED
 from fuglu.scansession import TrackTimings
 
 
 def get_config(fugluconfigfile=None, dconfdir=None):
     newconfig = FuConfigParser()
     logger = logging.getLogger('%s.shared' % __package__ if __package__ else "fuglu")
 
@@ -528,14 +528,19 @@
         if not SQL_EXTENSION_ENABLED and (cache_storage=='sql' or backend=='sql'):
             print("ERROR: sqlalchemy is not installed")
             return False
         
         if not REDIS_ENABLED and (cache_storage=='redis' or backend=='redis'):
             print("ERROR: redis library is not installed")
             return False
+        
+        if cache_storage=='redis' or backend=='redis':
+            password = self.config.get(self.section, 'redis_password', fallback=None) or None
+            if password is not None:
+                print('deprecatioin warning: obsolete redis_password configured, set via redis_conn')
 
         if not HAVE_DOMAINMAGIC:
             print('WARNING: domainmagic is not installed - some functionality will not be available')
 
         if not self.check_config():
             return False
 
@@ -802,29 +807,30 @@
             for stage in [SMTPTestResult.STAGE_PRECONNECT, SMTPTestResult.STAGE_RESOLVE, SMTPTestResult.STAGE_CONNECT,
                           SMTPTestResult.STAGE_HELO, SMTPTestResult.STAGE_MAIL_FROM, SMTPTestResult.STAGE_RCPT_TO]:
                 if result.stage == stage:
                     stageaction, messagetmpl, interval = self._get_stage_config(stage, test, domain, domainconfig,
                                                                                 sessid=sess.id)
                     if messagetmpl is None:
                         messagetmpl = ''
-                        self.logger.warning(f'{sess.id} message template for stage {stage} not defined')
+                        self.logger.debug(f'{sess.id} message template for stage {stage} not defined')
 
                     template = _SuspectTemplate(messagetmpl)
                     templ_dict = sess.get_templ_dict()
                     templ_dict['relay'] = relay
                     templ_dict['stage'] = stage
                     templ_dict['errormessage'] = result.errormessage
                     message = template.safe_substitute(templ_dict)
 
                     if stageaction is not None:
                         action = stageaction
                     if interval is not None:
                         servercachetime = min(servercachetime, interval)
-
-            if relay is not None:
+            
+            # skiplist if we tested a relay AND testaddress was either not necessary to test or confirmed to be accepted
+            if relay is not None and (testaddress not in result.rcptoreplies or result.rcptoreplies[testaddress][0] == SMTPTestResult.ADDRESS_OK):
                 try:
                     self.cache.skiplist(domain, relay, servercachetime, result.stage, result.errormessage, sess.id)
                     self.logger.warning(
                         f'{sess.id} problem testing recipient verification support on server {relay} in stage {result.stage}: {result.errormessage}. putting on skiplist.')
                 except Exception as e:
                     self.logger.warning(f'{sess.id} failed to add skiplist entry for {domain} due to {e.__class__.__name__}: {str(e)}')
             timetracker.tracktime("SMTPTestResult.Test_OK-fail")
@@ -836,21 +842,22 @@
             addrstate, code, msg = result.rcptoreplies[testaddress]
             recverificationsupport = None
             if addrstate == SMTPTestResult.ADDRESS_OK:
                 blreason = 'accepts any recipient'
                 recverificationsupport = False
             elif addrstate == SMTPTestResult.ADDRESS_TEMPFAIL:
                 blreason = f'temporary failure: {code} {msg}'
-                recverificationsupport = False
+                self.logger.error(f'{sess.id} could not determine rcpt filter state: {testaddress} {code} {msg}')
             elif addrstate == SMTPTestResult.ADDRESS_DOES_NOT_EXIST:
                 recverificationsupport = True
-            try:
-                self.cache.put_address(testaddress, servercachetime, not recverificationsupport, msg, sess.id)
-            except Exception as e:
-                self.logger.warning(f'{sess.id} failed to add recipient {testaddress} in cache due to {e.__class__.__name__}: {str(e)}')
+            if recverificationsupport is not None:
+                try:
+                    self.cache.put_address(testaddress, servercachetime, not recverificationsupport, msg, sess.id)
+                except Exception as e:
+                    self.logger.warning(f'{sess.id} failed to add recipient {testaddress} to cache due to {e.__class__.__name__}: {str(e)}')
             timetracker.tracktime("need_server_test")
         else:
             recverificationsupport = True
 
         # override: ignore recipient verification fail
         if self.config.getboolean(self.section, 'always_assume_rec_verification_support'):
             recverificationsupport = True
@@ -1107,15 +1114,15 @@
         self.config = config
         self.section = section
         self.relaycache = relaycache
         self.logger = logging.getLogger('%s.smtptest' % __package__ if __package__ else "fuglu")
         if section is None:
             self.be_verbose = False
         else:
-            self.be_verbose = self.config.getboolean(self.section, 'verbose')
+            self.be_verbose = self.config.getboolean(self.section, 'verbose', fallback=False)
         self.miltersession = miltersession
 
     def is_ip(self, value):
         try:
             ipaddress.ip_address(value)
             return True
         except ValueError:
@@ -1319,17 +1326,16 @@
 
                     certfile = self.config.get('ca_default', 'ssl_cert_file', fallback='') or None
                     keyfile = self.config.get('ca_default', 'ssl_key_file', fallback='') or None
                     keypass = self.config.get('ca_default', 'ssl_key_pass', fallback='') or None
                     if certfile and os.path.exists(certfile) and keyfile and os.path.exists(keyfile):
                         try:
                             context.load_cert_chain(certfile, keyfile, keypass)
-                        except ssl.SSLError as e:
-                            self.logger.warning(
-                                f'{self.miltersession.id} could not load cert {certfile} with key {keyfile} due to {e.__class__.__name__}: {str(e)}')
+                        except (ssl.SSLError, PermissionError) as e:
+                            self.logger.warning(f'{self.miltersession.id} could not load cert {certfile} with key {keyfile} due to {e.__class__.__name__}: {str(e)}')
 
                     if not smtp._host:
                         smtp._host = relay
 
                     code, msg = smtp.starttls(context=context)
                     if 199 < code < 300:
                         code, msg = smtp.ehlo()
@@ -1379,15 +1385,15 @@
         result.stage = SMTPTestResult.STAGE_RCPT_TO
         try:
             addrstate = SMTPTestResult.ADDRESS_UNKNOWNSTATE
             for addr in addrlist:
                 if addrstate == SMTPTestResult.ADDRESS_DOES_NOT_EXIST and self.is_testaddress(addr):
                     # we can skip test address check if real rcpt addr does not exist
                     result.rcptoreplies[addr] = (addrstate, code, 'skipped test address check')
-                    self.logger.warning(f'{self.miltersession.id} skipped test addres check for {addr}')
+                    self.logger.debug(f'{self.miltersession.id} skipped test addres check for {addr} - rcpt filter already confirmed')
                     continue
 
                 code, msg = smtp.rcpt(addr)
                 if 199 < code < 300:
                     addrstate = SMTPTestResult.ADDRESS_OK
                 elif 399 > code < 500:
                     addrstate = SMTPTestResult.ADDRESS_TEMPFAIL
@@ -1661,30 +1667,29 @@
     def __init__(self, config, section):
         super().__init__(config, section)
         self.logger = logging.getLogger("fuglu.call-ahead.RedisCache")
 
         redis_url = config.get(self.section, 'redis_conn')
         timeout = self.config.getint(self.section, 'redis_timeout', fallback=3)
         password = self.config.get(self.section, 'redis_password', fallback=None) or None
-        self.redis_pool = RedisPooledConn(redis_url, password=password, socket_keepalive=True, socket_timeout=timeout)
+        if password is not None:
+            self.logger.warning('deprecatioin warning: obsolete redis_password configured, set via redis_conn')
+        self.redis_pool = RedisPooledConn(redis_url, password=password, socket_timeout=timeout)
 
     def _update(self, name, values, ttl):
         """atomic update of hash value and ttl in redis"""
         redisconn = self.redis_pool.get_conn()
         pipe = redisconn.pipeline()
-        if REDIS2:
-            pipe.hmset(name, values)
-        else:
-            nobools = {}
-            for k, v in values.items():
-                if isinstance(v, bool):
-                    nobools[k] = str(v)
-                else:
-                    nobools[k] = v
-            pipe.hset(name, mapping=nobools)
+        nobools = {}
+        for k, v in values.items():
+            if isinstance(v, bool):
+                nobools[k] = str(v)
+            else:
+                nobools[k] = v
+        pipe.hset(name, mapping=nobools)
         pipe.expire(name, ttl)
         pipe.execute()
 
     def _multiget(self, names, keys):
         """atomically gets multiple hashes from redis"""
         redisconn = self.redis_pool.get_conn()
         pipe = redisconn.pipeline()
@@ -2171,14 +2176,17 @@
             if key.startswith('$'):
                 template = _SuspectTemplate(key)
                 key = template.safe_substitute({'recipient': self.recipient, 'domain': self.domain})
             value = value.get(key, {})
         return value
 
 
+class MockSession:
+    id = 'cmd'
+
 class SMTPTestCommandLineInterface(BackendMixin):
     def __init__(self):
         super().__init__()
         self.section = 'AddressCheck'
 
         self.commandlist = {
             'put-address': self.put_address,
@@ -2266,15 +2274,15 @@
 
     def test_dry(self, *args):
         if len(args) < 2:
             print("usage: test-dry <server> <address> [...<address>]")
             sys.exit(1)
         server = args[0]
         addrs = args[1:]
-        test = SMTPTest()
+        test = SMTPTest(section=self.section, miltersession=MockSession()) # config is passed later
 
         domain = sm.MilterSession.extract_domain(addrs[0])
         try:
             config = get_config()
             test.config = config
             self._init_config_backend(addrs[0], config, self.section)
             domainconfig = self.config_backend.get_domain_config_all()
@@ -2320,15 +2328,15 @@
             etp = "negative"
             if positive:
                 etp = "positive"
             print(f"We have {etp} cache entry for {address}: {message}")
         else:
             print(f"No cache entry for {address}")
 
-        test = SMTPTest(config, self.section)
+        test = SMTPTest(config, self.section, miltersession=MockSession())
         relays = test.get_relays(domain, domainconfig)  # type: list
         if relays is None:
             print(f"No relay for domain {domain} found!")
             sys.exit(1)
         print(f"Relays for domain {domain} are {', '.join(relays)}")
         for relay in relays:
             print(f"Testing relay {relay}")
@@ -2481,15 +2489,15 @@
         domain = sm.MilterSession.extract_domain(address)
 
         config = get_config()
         self._init_cache(config, self.section)
         self._init_config_backend(address, config, self.section)
         domainconfig = self.config_backend.get_domain_config_all()
 
-        test = SMTPTest(config)
+        test = SMTPTest(config, self.section, miltersession=MockSession())
         relays = test.get_relays(domain, domainconfig)
         if relays is None:
             print(f"No relay for domain {domain} found!")
             sys.exit(1)
         print(f"Relays for domain {domain} are {relays}")
 
         relay = relays[0]
@@ -2548,16 +2556,16 @@
             self.cache.put_address(address, cachetime, positive, msg, 'cmdline-update-add')
             neg = ""
             if not positive:
                 neg = "negative"
             print(f"{neg} cached {address} for {cachetime} seconds")
         else:
             print("Server accepts any recipient")
-            if config.getboolean('AddressCheck', 'always_assume_rec_verification_support'):
-                print("skiplistings disabled in config- not skiplisting")
+            if config.getboolean('AddressCheck', 'always_assume_rec_verification_support', fallback=True):
+                print("skiplistings disabled in config - not skiplisting")
             else:
                 self.cache.skiplist(domain, relay, servercachetime, result.stage, 'accepts any recipient')
                 print("Server skiplisted")
 
 
 # Usage for checks/debugging (you might have to change location of plugin
 # for your installation
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/clamav.py` & `fuglu-1.5.0/src/fuglu/plugins/clamav.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from fuglu.stringencode import force_bString, force_uString
 from fuglu.protocolbase import set_keepalive_linux
 import socket
 import os
 import struct
 import threading
 import errno
-import subprocess
+import subprocess # nosemgrep CWE-78
 import time
 import math
 
 threadLocal = threading.local()
 # it's probably a good idea to re-establish the connection occasionally
 MAX_SCANS_PER_SOCKET = 5000
 
@@ -243,15 +243,15 @@
         clamscan = self.config.get(self.section, 'clamscan')
         timeout = self.config.getint(self.section, 'clamscantimeout')
 
         if not os.path.exists(clamscan):
             raise Exception(f'could not find clamscan executable in {clamscan}')
 
         try:
-            process = subprocess.Popen([clamscan, u'-'], stdin=subprocess.PIPE, stdout=subprocess.PIPE)  # file data by pipe
+            process = subprocess.Popen([clamscan, '-'], stdin=subprocess.PIPE, stdout=subprocess.PIPE)  # file data by pipe
             def kill_proc(p): return p.kill()
             timer = threading.Timer(timeout, kill_proc, [process])
             timer.start()
             stdout = process.communicate(force_bString(content))[0]
             process.stdin.close()
             exitcode = process.wait()
             timer.cancel()
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/dataprovider.py` & `fuglu-1.5.0/src/fuglu/plugins/dataprovider.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,16 @@
         for host, port in targets:
             for uri, source in uris:
                 data = self._format_data(suspect, uri, source)
                 if logonly:
                     self.logger.info(f"{suspect.id} LOGONLY: data={data}")
                 else:
                     self.sock.sendto(force_bString(data), (host, port))
-                    self.logger.debug(f"{suspect.id} SENT: data={data} to {host}:{port}")
+                    logdata = data.replace('\n', '\\n')
+                    self.logger.debug(f"{suspect.id} SENT: data={logdata} to {host}:{port}")
 
     def _get_uris(self, suspect, tags):
         uris = []
         for tag in tags:
             uris.extend(suspect.get_tag(tag, []))
 
         exclude_re = self.config.get(self.section, 'filter_regex').strip()
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/decision.py` & `fuglu-1.5.0/src/fuglu/plugins/decision.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 #
 from fuglu.shared import ScannerPlugin, DUNNO, DELETE, string_to_actioncode, SuspectFilter, \
-    Suspect, apply_template, REJECT, _SuspectTemplate
+    Suspect, apply_template, REJECT, _SuspectTemplate, actioncode_to_string
 from fuglu.extensions.sql import DBConfig
 from fuglu.stringencode import force_uString
 import os
 import re
 
 try:
     from domainmagic.validators import is_email
@@ -61,37 +61,35 @@
  * archive/quarantine status
  * block/welcomelist or filter settings
  * filtersettings tags, set e.g. by p_blwl FilterSettings backend
 and performs the following actions:
  * add headers or subject tags according to filter result
  * decide if mail should be delivered or deleted
  * wrap mail and send as .eml-attachment
+ * change the recipient
+Because this plugin may change subject (or body when wrapping) it's recommended
+to run it before signing plugins such as DKIMSignPlugin or ARCSignPlugin.
+This plugin will always return DUNNO, use DeliverDecision as last plugin to issue DELETE if needed.
     """
 
     def __init__(self, config, section=None):
         super().__init__(config, section)
         self.logger = self._logger()
         self.requiredvars = {
-            'testmode': {
-                'default': 'False',
-                'description': 'will not delete any mail if set to True',
-            },
             'wrap_template_file': {
                 'default': '',
                 'description': 'path to template file used as body for wrapped spam',
             },
         }
 
     def __str__(self):
         return "Filter Decision"
 
     def lint(self):
         allok = self.check_config()
-        if self.config.get(self.section, 'testmode'):
-            print('WARNING: testmode active, will not delete any mail. may forward untagged spam or malware!')
         if allok:
             wrap_template_file = self.config.get(self.section, 'wrap_template_file')
             if wrap_template_file and not os.path.exists(wrap_template_file):
                 print(f'ERROR: wrap_template_file {wrap_template_file} does not exist')
                 allok = False
         return allok
 
@@ -160,14 +158,15 @@
         elif suspect.is_highspam():
             suspect.add_header(f'{prependaddedheaders}HighSpam', 'yes')
             if not self._add_subject_tag_status(suspect, 'subject_tag_highspam'):
                 self._add_subject_tag_status(suspect, 'subject_tag_spam')
         elif suspect.is_spam():
             suspect.add_header(f'{prependaddedheaders}Spam', 'yes')
             self._add_subject_tag_status(suspect, 'subject_tag_spam')
+        suspect.set_tag('filterdecision.tagged', True)
 
     def _check_deliver_spam(self, suspect):
         deliver = True
         if suspect.is_virus():
             deliver = False
         elif suspect.is_blocklisted():
             deliver = False
@@ -181,43 +180,37 @@
                 self.logger.debug(f'{suspect.id} is highspam, but delivering due to filtersetting')
                 deliver = True
         elif suspect.is_spam():
             deliver = False
             if self._get_filtersetting(suspect, 'deliver_spam', False):
                 self.logger.debug(f'{suspect.id} is spam, but delivering due to filtersetting')
                 deliver = True
-
-        if not deliver and not suspect.is_ham() and not suspect.get_tag('archived', False):
-            self.logger.debug(f'{suspect.id} is ham={suspect.is_ham()}, but delivering because archived={suspect.get_tag("archived")}')
-            deliver = True
-
+        
         if deliver and not suspect.is_ham():
             spam_recipient = self._get_filtersetting(suspect, 'spam_recipient')
-            if spam_recipient:
+            if spam_recipient and is_email(spam_recipient):
                 self.logger.debug(f'{suspect.id} delivering to spam rcpt {spam_recipient}')
                 suspect.to_address = spam_recipient
+            elif spam_recipient and not is_email(spam_recipient):
+                self.logger.warning(f'{suspect.id} ignoring invalid spam rcpt {spam_recipient}')
         return deliver
 
     def examine(self, suspect):
         deliver = self._check_deliver_spam(suspect)
         if not deliver:
-            if self.config.getboolean(self.section, 'testmode'):
-                self.logger.info(f'{suspect.id} testmode enabled. else would be deleting due to filterdecision')
-                return DUNNO
-            else:
-                self.logger.info(f'{suspect.id} deleting due to filterdecision')
-                return DELETE
+            suspect.set_tag('filterdecision.action', actioncode_to_string(DELETE))
+            self.logger.info(f'{suspect.id} recommend DELETE due to filterdecision')
 
         orig_subject = suspect.get_header('subject')
 
-        if not suspect.is_ham():
+        if deliver and not suspect.is_ham():
             self._add_status_markers(suspect)
         self._add_subject_tag_ext(suspect)
 
-        if self._get_filtersetting(suspect, 'wrap_spam', False) and suspect.is_spam() \
+        if deliver and self._get_filtersetting(suspect, 'wrap_spam', False) and suspect.is_spam() \
                 or self._get_filtersetting(suspect, 'wrap_highspam', False) and suspect.is_highspam() \
                 or self._get_filtersetting(suspect, 'wrap_virus', False) and suspect.is_virus():
 
             wrap_template_file = self.config.get(self.section, 'wrap_template_file')
             if not wrap_template_file:
                 self.logger.error(f'{suspect.id} cannot wrap because wrap_template file not defined')
             elif not os.path.exists(wrap_template_file):
@@ -229,14 +222,48 @@
                 msg = suspect.wrap(suspect.from_address, suspect.to_address, orig_subject, body, 'original_mail.eml', self.config)
                 suspect.set_source(msg.as_bytes())
                 self.logger.debug(f'{suspect.id} wrapped')
 
         return DUNNO
 
 
+class DeliverDecision(FilterDecision):
+    def __init__(self, config, section=None):
+        super().__init__(config, section)
+        self.logger = self._logger()
+        self.requiredvars.update({
+            'testmode': {
+                'default': 'False',
+                'description': 'will not delete any mail if set to True',
+            },
+        })
+    
+    def lint(self):
+        allok = self.check_config()
+        if self.config.get(self.section, 'testmode'):
+            print('WARNING: testmode active, will not delete any mail. may forward untagged spam or malware!')
+        return allok
+    
+    def examine(self, suspect):
+        action = DUNNO
+        decision = suspect.get_tag('filterdecision.action')
+        if decision is not None:
+            action = string_to_actioncode(decision)
+            # message was not archived, we do not want to just discard it
+            if action == DELETE and not suspect.is_ham() and not suspect.get_tag('archived', False):
+                self.logger.debug(f'{suspect.id} is ham={suspect.is_ham()}, but delivering because archived={suspect.get_tag("archived")}')
+                action = DUNNO
+                if not suspect.get_tag('filterdecision.tagged'):
+                    self._add_status_markers(suspect)
+            if action == DELETE and self.config.getboolean(self.section, 'testmode'):
+                self.logger.info(f'{suspect.id} testmode enabled. else would be deleting due to filterdecision')
+                action = DUNNO
+        return action
+
+
 class ActionOverridePlugin(ScannerPlugin):
 
     """
 Override actions based on a Suspect Filter file.
 For example, delete all messages from a specific sender domain.
     """
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/delay.py` & `fuglu-1.5.0/src/fuglu/plugins/delay.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/dnsdata.py` & `fuglu-1.5.0/src/fuglu/plugins/dnsdata.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/domainauth.py` & `fuglu-1.5.0/src/fuglu/plugins/domainauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,34 +18,35 @@
 
 requires: dkimpy (not pydkim!!)
 requires: pyspf
 requires: pydns (or alternatively dnspython if only dkim is used)
 requires: pysrs
 requires: pynacl (rare dependeny of dkimpy)
 requires: dmarc
+requires: authres (for arc signing)
 """
 import ipaddress
 import logging
 import os
 import re
 import time
 import traceback
 import typing as tp
 import fnmatch
 import socket
-import copy
 import email
+import email.policy
 import operator
+from hashlib import md5
 from email.header import Header
-from email.errors import HeaderParseError
 import fuglu.connectors.asyncmilterconnector as asm
 import fuglu.connectors.milterconnector as sm
 
 from fuglu.shared import ScannerPlugin, apply_template, DUNNO, FileList, string_to_actioncode, get_default_cache, \
-    extract_domain, Suspect, Cache, actioncode_to_string, deprecated, get_outgoing_helo, ACCEPT
+    extract_domain, Suspect, Cache, actioncode_to_string, deprecated, get_outgoing_helo, ACCEPT, SuspectFilter
 from fuglu.mshared import BMPMailFromMixin, BMPRCPTMixin, BMPEOBMixin, BasicMilterPlugin, EOM, retcode2milter
 from fuglu.extensions.sql import get_session, SQL_EXTENSION_ENABLED, get_domain_setting, text
 from fuglu.extensions.dnsquery import DNSQUERY_EXTENSION_ENABLED, lookup, QTYPE_TXT, DNS_TIMEOUT, revlookup, FuSERVFAIL
 from fuglu.stringencode import force_bString, force_uString
 from fuglu.logtools import PrependLoggerMsg
 from fuglu.lib.patchedemail import PatchedMessage
 
@@ -139,47 +140,45 @@
 DMARC_RECORDFAIL = 'recordfail'
 SPF_SKIP = 'skip'
 
 
 _re_at = re.compile(r"(?<=[@＠])[\w.-]+")
 
 
-def extract_from_domains(suspect, header='From', get_display_part=False):
+def extract_from_domains(suspect:Suspect, header:str='From', get_display_part:bool=False) -> tp.Optional[tp.List[str]]:
     """
     Returns a list of all domains found in From header
     :param suspect: Suspect
     :param header: name of header to extract, defaults to From
     :param get_display_part: set to True to search and extract domains found in display part, not the actual addresses
     :return: list of domain names or None in case of errors
     """
 
     # checking display part there's no need checking for the validity of the associated
     # mail address
     from_addresses = suspect.parse_from_type_header(header=header, validate_mail=(not get_display_part))
     if len(from_addresses) < 1:
         return None
-
-    from_doms = []
+    
+    from_doms = set()
     for item in from_addresses:
         if get_display_part:
             domain_match = _re_at.search(item[0])
             if domain_match is None:
                 continue
-            from_doms.append(domain_match.group())
-        else:
+            from_doms.add(domain_match.group())
+        elif len(item)>1 and item[1] and '@' in item[1]:
             try:
-                from_doms.append(extract_domain(item[1]))
-            except Exception as e:
-                logging.getLogger("fuglu.extract_from_domains").exception(e)
-
-    from_addrs = list(set(from_doms))
-    return from_addrs
+                from_doms.add(extract_domain(item[1]))
+            except Exception:
+                logging.getLogger("fuglu.extract_from_domains").debug(f'{suspect.id} {traceback.format_exc()}')
+    return list(from_doms)
 
 
-def extract_from_domain(suspect, header='From', get_display_part=False):
+def extract_from_domain(suspect:Suspect, header:str='From', get_display_part:bool=False) -> tp.Optional[str]:
     """
     Returns the most significant domain found in From header.
     Usually this means the last domain that can be found.
     :param suspect: Suspect object
     :param header: name of header to extract, defaults to From
     :param get_display_part: set to True to search and extract domains found in display part, not the actual addresses
     :return: string with domain name or None if nothing found
@@ -213,15 +212,15 @@
         except FuSERVFAIL:
             return 'temperror'
         except Exception:
             return 'permerror'
     return None
 
 
-def check_skip_on_tag(suspect, taglist):
+def check_skip_on_tag(suspect: Suspect, taglist:tp.Iterable[str]) -> tp.Optional[str]:
     for tag in taglist:
         if '==' in tag:
             tagname, tagvalue = tag.split('==',1)
             op = operator.eq
         elif '!=' in tag:
             tagname, tagvalue = tag.split('!=',1)
             op = operator.ne
@@ -230,14 +229,29 @@
             tagvalue = True
             op = operator.eq
         if op(suspect.get_tag(tagname, False), tagvalue):
             return tagname
     return None
 
 
+def parse_received_xxx(hdrvalue:str) -> tp.Tuple[tp.Optional[str], tp.Dict[str,str], tp.Optional[str]]:
+    status = None
+    expl = None
+    fieldmap = {}
+    if hdrvalue:
+        fields = hdrvalue.replace('\r','').replace('\n', '').split(';')
+        if fields and fields[0]:
+            status, _, expl = fields[0].split(None,2)
+            expl = expl.rsplit(')',1)[0]
+            firstfield = fields[0].rsplit(None,1)[-1]
+            fields[0] = firstfield
+            fieldmap = {v[0].lower().strip():v[1].strip() for v in [f.split('=',1) for f in fields if '=' in f]}
+    return status, fieldmap, expl
+
+
 class ARCVerifyPlugin(ScannerPlugin):
     """
 This plugin checks the ARC signature of the message and sets tags.
 Tags set:
  * ARCVerify.skipreason set if the verification has been skipped
  * ARCVerify.cv chain validation result
  * ARCVerify.message ARC validation message
@@ -281,15 +295,15 @@
                 result_header = self.config.get(self.section, 'result_header')
                 if result_header:
                     suspect.add_header(result_header, DKIM_NONE)
                 suspect.debug(f"{suspect.id} ARC signature header {hdrname} not found")
                 return DUNNO
 
         timeout = self.config.getfloat(self.section, 'max_lookup_time')
-        source = suspect.get_source()
+        source = suspect.get_source(newline=b'\r\n')
         try:
             cv = 'none'
             message = 'Message validation error'
             # use the local logger of the plugin but prepend the fuglu id
             d = ARC(source, logger=PrependLoggerMsg(self.logger, prepend=suspect.id, maxlevel=logging.INFO), timeout=timeout)
             try:
                 if self.dkim_dns_func is not None:
@@ -334,14 +348,79 @@
         if not DNSQUERY_EXTENSION_ENABLED:
             print("Missing dependency: no supported DNS libary found: pydns or dnspython")
             all_ok = False
 
         return all_ok
 
 
+class ARCStripPlugin(ScannerPlugin):
+    """
+    This plugin removes previous ARC headers if ARC validation failed.
+    """
+    def __init__(self, config, section=None):
+        super().__init__(config, section)
+        self.logger = self._logger()
+        self.requiredvars = {
+            'arcstrip_filter': {
+                'default': '${confdir}/arcstrip_filter.regex',
+                'description': 'filterfile containing suspectfilter rules to strip broken arc signatures',
+            },
+        }
+        self.arcstrip_filter = None
+
+    def _init_arcstrip_filter(self):
+        """checks if there is a bacn filter file and initializes it. """
+        if self.arcstrip_filter is None:
+            filename = self.config.get(self.section, 'arcstrip_filter')
+            if filename and os.path.exists(filename):
+                self.arcstrip_filter = SuspectFilter(filename)
+    
+    
+    def __str__(self):
+        return "ARC Strip"
+    
+    
+    def examine(self, suspect):
+        if suspect.get_tag("ARCVerify.cv") != DKIM_FAIL:
+            return DUNNO
+        
+        self._init_arcstrip_filter()
+        if self.arcstrip_filter is None:
+            return DUNNO
+        
+        match, arg = self.arcstrip_filter.matches(suspect)
+        if match:
+            authres_hdr = suspect.get_header('Authentication-Results')
+            if authres_hdr:
+                suspect.set_tag('authres', authres_hdr) # keep for use in ARCSignPlugin._reuse_authres_header
+                self.logger.debug(f'{suspect.id} stored previous authres header {authres_hdr}')
+            
+            delhdrs = {'ARC-Seal', 'ARC-Message-Signature', 'ARC-Authentication-Results', 'Authentication-Results'}
+            stripped = suspect.remove_headers_from_source(delhdrs)
+            if stripped:
+                self.logger.info(f'{suspect.id} removed previous arc headers')
+            else:
+                self.logger.debug(f'{suspect.id} no arc headers found')
+            suspect.set_tag('ARCStrip', stripped)
+        return DUNNO
+    
+    
+    def lint(self):
+        ok = self.check_config()
+        if ok:
+            filename = self.config.get(self.section, 'arcstrip_filter')
+            if not filename:
+                ok = False
+                print('WARNING: no arcstrip_filter file specified. this plugin will do nothing.')
+            if filename and not os.path.exists(filename):
+                ok = False
+                print(f'ERROR: arcstrip_filter file {filename} not found. this plugin will do nothing.')
+        return ok
+
+
 class ARCSignPlugin(ScannerPlugin):
     """
 This plugin creates the ARC signature headers of the message.
 Special attention is given if message is from outlook.com, which adds broken authentication results headers.
 This plugin will add 4 new headers:
  * Authentication-Results
  * ARC-Authentication-Results
@@ -358,129 +437,158 @@
             'privatekeyfile': {
                 'default': "${confdir}/dkim/${header_from_domain}.key",
                 'description': "Location of the private key file. supports standard template variables plus additional ${header_from_domain} which extracts the domain name from the From: -Header and ${auth_host} which defaults to fuglu's helo",
             },
 
             'selector': {
                 'default': 'default',
-                'description': 'selector to use when signing, supports templates',
+                'description': 'selector to use when signing, supports templates and additional variables (see privatekeyfile)',
             },
 
             'signheaders': {
                 'default': 'From,Reply-To,Subject,Date,To,CC,Resent-Date,Resent-From,Resent-To,Resent-CC,In-Reply-To,References,List-Id,List-Help,List-Unsubscribe,List-Subscribe,List-Post,List-Owner,List-Archive',
                 'description': 'comma separated list of headers to sign. empty string=sign all headers',
             },
 
             'signdomain': {
                 'default': 'header:From',
                 'description': 'which domain to use in signature? use header:headername or static:example.com or tmpl:${template_var} (tmpl supports additional vars header_from_domain and auth_host)',
             },
+            
+            'get_authres_tag': {
+                'default': '',
+                'description': 'name of suspect tag providing authentication-results header'
+            },
 
             'trust_authres_rgx': {
                 'default': '',
                 'description': 'do not create own but use authentication-results header of previous host if ptr matches given regex'
             },
 
             'reuse_authres_tag': {
                 'default': '',
-                'description': 'name of suspect tag that must be set to True to enable authenetication-results header reuse (as per trust_authres_rgx). if empty no tag is checked.'
+                'description': 'name of suspect tag that must be set to True to enable authenetication-results header reuse (as per trust_authres_rgx). if empty no tag is checked and trust_authres_rgx is always checked.'
             },
 
-            'header_immediate': {
-                'default': 'False',
-                'description': 'write headers immediately (for use by other plugins).'
+            'debug_domains': {
+                'default': '',
+                'description': 'list of recipient domains for which to print additional debug output (potentially noisy)'
+            },
+            
+            'debugdumpdir': {
+                'default': '',
+                'description': 'define a directory where to dump sources on errors'
             },
         }
 
     def __str__(self):
         return "ARC Sign"
 
-    def _get_source(self, suspect: Suspect, authres_hdr: str) -> bytes:
+    def _get_source(self, suspect: Suspect, authres_hdr: str, debug_headers: tp.List[str]) -> bytes:
         """
         get source and patch/remove invalid authres headers (e.g. from microsoft)
         :param suspect: Suspect
         :return: message source as bytes
         """
         clientinfo = suspect.get_client_info(self.config)
         helo = clientinfo[0].lower() if clientinfo and clientinfo[0] else None
         ptr = clientinfo[2].lower() if clientinfo and clientinfo[2] else None
-        msgrep = copy.deepcopy(suspect.get_message_rep())  # ensure we work with a copy and not a reference of the original message
+        tempsuspect = Suspect(suspect.from_address, suspect.to_address, '/dev/null', id=suspect.id)
+        tempsuspect.set_source(suspect.get_source())
+        msgrep = tempsuspect.get_message_rep()
         authres_hdrs = msgrep.get_all('Authentication-Results', [])
         ok_hdrs = []
         if authres_hdrs:
             for hdr in authres_hdrs:
                 hdr = hdr.strip(';')
                 try:
                     try:
                         authres.AuthenticationResultsHeader.parse(f'Authentication-Results: {hdr}')
                         ok_hdrs.append(hdr)
                     except authres.core.SyntaxError:
-                        if helo and ptr and ptr.endswith('.outlook.com'):
+                        if helo and ptr and ptr.endswith(('.outlook.com', '.mx.microsoft')):
                             helohdr = f'{helo}; {hdr}'
                             authres.AuthenticationResultsHeader.parse(f'Authentication-Results: {helohdr}')
                             ok_hdrs.append(helohdr)
                             self.logger.debug(f'{suspect.id} patching invalid authres header {hdr}')
                         else:
                             self.logger.debug(f'{suspect.id} not patching invalid authres header from {helo}')
                             raise
                 except authres.core.SyntaxError:
                     self.logger.warning(f'{suspect.id} dropping invalid authres header {hdr}')
-            del msgrep['Authentication-Results']
+            tempsuspect.remove_headers_from_source({'Authentication-Results'})
         if authres_hdr:
             ok_hdrs.append(authres_hdr)
         for hdr in ok_hdrs:
-            msgrep.add_header('Authentication-Results', hdr)
+            hdr = hdr.replace('\r', '').replace('\n', '')
+            tempsuspect.add_header('Authentication-Results', hdr, immediate=True)
         self.logger.debug(f'{suspect.id} using {len(ok_hdrs)} authres headers')
-        return msgrep.as_bytes()
+        for header in debug_headers:
+            header = force_uString(header)
+            value = msgrep.get(header)
+            if value:
+                myhash = md5(force_bString(value)).hexdigest() # nosemgrep CWE-327
+                self.logger.debug(f'{suspect.id} source header {myhash} {header}: {value}')
+        return tempsuspect.get_source()
 
-    def _authres_insert_arcpass(self, authres_hdr:str) -> str:
+    def _authres_insert_arcpass(self, suspect:Suspect, authres_hdr:str) -> str:
         fields = authres_hdr.split(';')
         has_arc = False
         for field in fields:
             if field.strip().startswith('arc='):
                 has_arc = True
                 break
         if not has_arc:  # previous arc sig found but not mentioned in authres header
-            fields.append('arc=pass')
+            if suspect.get_tag('ARCStrip') is True:
+                # ARC was stripped, we spoof pass status. maybe need to set to None
+                arcstatus = DKIM_PASS
+            else:
+                arcstatus = suspect.get_tag('ARCVerify.cv')
+                if arcstatus == DKIM_SKIP: # no arc check performed
+                    arcstatus = None
+            if arcstatus: # only set if we have a reasonable status
+                fields.append(f'arc={arcstatus}')
         return ';'.join(fields)
 
     def _reuse_authres_header(self, suspect: Suspect, authhost: str) -> tp.Optional[str]:
         hdr = None
         ptrrgx = self.config.get(self.section, 'trust_authres_rgx')
         tag = self.config.get(self.section, 'reuse_authres_tag')
         reuse_tag = suspect.get_tag(tag, False) if tag else True
         if ptrrgx and reuse_tag == True:
             self.logger.debug(f'{suspect.id} ptrrgx is set and tag {tag} is {suspect.get_tag(tag)}')
             clientinfo = suspect.get_client_info(self.config)
             ptr = clientinfo[2].lower() if clientinfo and clientinfo[2] else None
             if ptr and re.search(ptrrgx, ptr):
                 msgrep = suspect.get_message_rep()
                 hdr = msgrep.get('Authentication-Results')
+                if hdr is None:
+                    hdr = suspect.get_tag('authres')
                 if hdr is not None:
                     hdr = hdr.strip(';')
                     try:
                         authres.AuthenticationResultsHeader.parse(f'Authentication-Results: {hdr}')
                     except authres.core.SyntaxError:
                         hdr = f'{authhost}; {hdr}'
                     else:
                         fields = hdr.split(';')
                         fields[0] = authhost
                         hdr = ';'.join(fields)
                     if msgrep.get('ARC-Seal'):  # previous arc sig found. we trust it passed. used for m365
-                        hdr = self._authres_insert_arcpass(hdr)
+                        hdr = self._authres_insert_arcpass(suspect, hdr)
                     self.logger.debug(f'{suspect.id} using previous authres header {hdr}')
                 else:
                     self.logger.debug(f'{suspect.id} no previous authres header found')
             else:
                 self.logger.debug(f'{suspect.id} ptr {ptr} does not match regex {ptrrgx}')
         else:
             self.logger.debug(f'{suspect.id} ptrrgx is empty or tag {tag} is not True')
         return hdr
 
-    def _create_authres_header(self, suspect: Suspect, authhost: str) -> str:
+    def _create_authres_header(self, suspect: Suspect, authhost: str, hdrfrom: str) -> str:
         """
         create authentication result header value as per rfc8601
         :param suspect: Suspect object
         :param authhost: name of authentication host (first field of authres header)
         :return: bytes string of authentication header, at least host.example.com;none
         """
         values = [authhost, ]
@@ -492,27 +600,34 @@
             dkimtag = f'dkim={dkimstate}'
             dkimdomain = suspect.get_tag("DKIMVerify.dkimdomain")
             if dkimdomain:
                 dkimtag = f'{dkimtag} header.d={dkimdomain}'
             dkimdomaini = suspect.get_tag("DKIMVerify.dkimdomaini")
             if dkimdomaini:
                 dkimtag = f'{dkimtag} header.i={dkimdomaini}'
+            selector = suspect.get_tag("DKIMVerify.selector")
+            if selector:
+                dkimtag = f'{dkimtag} header.s={selector}'
             values.append(dkimtag)
         dmarcstate = suspect.get_tag('dmarc.result')
-        if dmarcstate and dmarcstate != DMARC_SKIP:
-            values.append(f'dmarc={dmarcstate}')
+        if dmarcstate and dmarcstate not in [DMARC_SKIP, DMARC_NONE]:
+            dmarctag = f'dmarc={dmarcstate}'
+            if hdrfrom:
+                dmarctag = f'{dmarctag} header.from={hdrfrom}'
+            values.append(dmarctag)
         #arcstate = suspect.get_tag('ARCVerify.cv')
         #if arcstate:
         #    values.append(f'arc={arcstate}')  # not part of rfc
         iprev = check_iprev(suspect, self.config)
         if iprev:
             values.append(f'iprev={iprev}')
         if len(values) == 1:
             values.append('none')
         hdr = ';'.join(values)
+        self.logger.debug(f'{suspect.id} using generated authres header {hdr}')
         return hdr
 
     def _get_sign_domain(self, suspect: Suspect, headerfromdomain: str) -> str:
         domain = None
         sigkey = self.config.get(self.section, 'signdomain')
         if ':' in sigkey:
             key, value = sigkey.split(':', 1)
@@ -527,58 +642,93 @@
         return domain
 
     def examine(self, suspect):
         if not ARCSIGN_AVAILABLE:
             suspect.debug("dkimpy or authres not available, can not sign ARC")
             self.logger.debug(f"{suspect.id} ARC signing skipped - missing dkimpy or authres library")
             return DUNNO
-
-        authhost = get_outgoing_helo(self.config)
+        
+        if not suspect.get_header('received'):
+            self.logger.warning(f'{suspect.id} no received header found, cannot add ARC signature')
+            return DUNNO
+        
         headerfromdomain = extract_from_domain(suspect)
+        authhost = get_outgoing_helo(self.config)
         domain = self._get_sign_domain(suspect, headerfromdomain)
         selector = apply_template(self.config.get(self.section, 'selector'), suspect, dict(header_from_domain=headerfromdomain, auth_host=authhost))
 
         if domain is None:
-            self.logger.debug(f"{suspect.id} Failed to extract From-header domain for ARC signing")
+            self.logger.warning(f"{suspect.id} Failed to extract From-header domain for ARC signing")
             return DUNNO
 
         privkeyfile = apply_template(self.config.get(self.section, 'privatekeyfile'), suspect, dict(header_from_domain=headerfromdomain, auth_host=authhost))
         if not os.path.isfile(privkeyfile):
-            self.logger.debug(f"{suspect.id} ARC signing failed for domain {headerfromdomain} private key not found: {privkeyfile}")
+            self.logger.warning(f"{suspect.id} ARC signing failed for domain {headerfromdomain} private key not found: {privkeyfile}")
             return DUNNO
 
         with open(privkeyfile, 'br') as f:
             privkeycontent = f.read()
 
         headerconfig = self.config.get(self.section, 'signheaders')
         if headerconfig is None or headerconfig.strip() == '':
             inc_headers = None
         else:
             inc_headers = [force_bString(h.strip().lower()) for h in headerconfig.split(',')]
 
-        authres_hdr = self._reuse_authres_header(suspect, authhost)
+        authres_hdr = None
+        get_authres_tag = self.config.get(self.section, 'get_authres_tag')
+        if get_authres_tag:
+            # get authres header from tag. no checks applied.
+            authres_hdr = suspect.get_tag(get_authres_tag)
+            if authres_hdr:
+                self.logger.debug(f'{suspect.id} using authres header from tag {get_authres_tag}: {authres_hdr}')
+        if authres_hdr is None:
+            authres_hdr = self._reuse_authres_header(suspect, authhost)
         if authres_hdr is None:  # if empty string we use hdr from previous host but none was set
-            authres_hdr = self._create_authres_header(suspect, authhost)
+            authres_hdr = self._create_authres_header(suspect, authhost, headerfromdomain)
+        
+        debug_headers = []
+        debug_domains = self.config.getlist(self.section, 'debug_domains')
+        if debug_domains and suspect.to_domain in debug_domains:
+            debug_headers = inc_headers[:]
+            debug_headers.append('authentication-results')
 
         try:
-            source = self._get_source(suspect, authres_hdr)
+            source = self._get_source(suspect, authres_hdr, debug_headers)
             d = ARC(source, logger=PrependLoggerMsg(self.logger, prepend=suspect.id, maxlevel=logging.INFO))
             arc_set = d.sign(force_bString(selector), force_bString(domain), privkeycontent, force_bString(authhost), include_headers=inc_headers)
             if not arc_set:
                 self.logger.warning(f'{suspect.id} empty ARC signature set')
+                debugdumpdir = self.config.get(self.section, 'debugdumpdir')
+                if debugdumpdir:
+                    filename = os.path.join(debugdumpdir, f'{suspect.id}.eml')
+                    with open(filename, 'wb') as f:
+                        f.write(suspect.get_source())
+                    self.logger.warning(f'{suspect.id} ARC sealing failed, dumped original source to {filename}')
+                    
+                    filename = os.path.join(debugdumpdir, f'{suspect.id}.arcsource.eml')
+                    with open(filename, 'wb') as f:
+                        f.write(source)
+                    self.logger.warning(f'{suspect.id} ARC sealing failed, dumped ARC source to {filename}')
+                
             else:
-                immediate = self.config.getboolean(self.section, 'header_immediate')
-                suspect.add_header('Authentication-Results', authres_hdr, immediate=immediate)
                 arc_set.reverse()
                 for item in arc_set:
                     hdr, val = item.split(b':', 1)
-                    suspect.add_header(force_uString(hdr.strip()), force_uString(val.strip()), immediate=immediate)
+                    # dkim.ARC provides properly folded headers. we trust they're valid.
+                    suspect.add_header(force_uString(hdr.strip()), force_uString(val), immediate=True, raw=True)
+                # This header should be on top
+                authres_hdr = authres_hdr.replace('\r', '').replace('\n', '')
+                suspect.add_header('Authentication-Results', authres_hdr, immediate=True)
         except Exception as de:
-            self.logger.warning(f"{suspect.id} ARC signing failed: {de.__class__.__name__}: {str(de)}")
-            self.logger.debug(traceback.format_exc())
+            if suspect.get_tag("ARCVerify.cv") == DKIM_NONE and suspect.get_header('ARC-Seal') == '0':
+                self.logger.debug(f"{suspect.id} ARC signing of ARC-Seal:0 message failed: {de.__class__.__name__}: {str(de)}")
+            else:
+                self.logger.warning(f"{suspect.id} ARC signing failed: {de.__class__.__name__}: {str(de)}")
+                self.logger.debug(f"{suspect.id} ARC signing failed: {de.__class__.__name__}: {str(de)}", exc_info=de)
 
         return DUNNO
 
     def lint(self):
         all_ok = self.check_config()
 
         if not DKIMPY_AVAILABLE:
@@ -661,51 +811,87 @@
             'result_header': {
                 'default': '',
                 'description': 'write result to header of name specified here. leave empty to not write any header.'
             },
             'skip_on_tag': {
                 'default': '',
                 'description': 'skip DKIM evaluation if tag is present and has specified value (examples: x,y==z,a!=b -> x must be True, y must be "z" and a must not be "b")'
-            }
+            },
+            'create_received_dkim': {
+                'default': 'False',
+                'description': 'create Received-DKIM header'
+            },
+            'debugdumpdir': {
+                'default': '',
+                'description': 'define a directory where to dump sources on errors'
+            },
         }
         self.rgx_cache = {}
     
     def __str__(self):
         return "DKIM Verify"
     
     def _get_source(self, suspect:Suspect) -> bytes:
         """
         get message source from suspect and "patch" subject by applying strip_subject_rgx
         :param suspect: the suspect object
         :return: bytes representation of original message source (possibly with modified subject)
         """
-        source = suspect.get_source()
+        source = suspect.get_source(newline=b'\r\n')
         strip_subject_rgx = self.config.get(self.section, 'strip_subject_rgx')
         if strip_subject_rgx:
-            msgrep = email.message_from_bytes(source, _class=PatchedMessage)
+            msgrep = email.message_from_bytes(source, _class=PatchedMessage, policy=email.policy.SMTP)
             oldsubject = msgrep.get('subject')
             if oldsubject:
                 oldsubject = force_uString(suspect.decode_msg_header(oldsubject))
             if oldsubject:
                 rgx = self.rgx_cache.get(strip_subject_rgx)
                 if rgx is None:
                     rgx = re.compile(strip_subject_rgx, re.I)
                     self.rgx_cache = {strip_subject_rgx:rgx}
                 newsubject = rgx.sub('', oldsubject).strip()
                 if oldsubject.strip() != newsubject:
                     self.logger.debug(f'{suspect.id} updating subject to {newsubject}')
-                    msgrep.replace_header('subject', newsubject)
-                    source = msgrep.as_bytes()
+                    tmpsuspect = Suspect(from_address=suspect.from_address, recipients=suspect.recipients, tempfile=None, inbuffer=source)
+                    tmpsuspect.set_header('subject', newsubject)
+                    source = tmpsuspect.get_source()
                 else:
                     self.logger.debug(f'{suspect.id} not updating subject')
             else:
                 self.logger.debug(f'{suspect.id} not subject found')
         return source
     
+    def _create_received_dkim(self, valid:bool, dkimval: str, dkimdomain: str, dkimdomaini: str, selector: str) -> str:
+        """
+        create received-dkim header based on current dkim check result
+        """
+        myname = get_outgoing_helo(self.config)
+        fields = [f'receiver={myname}']
+        if selector:
+            fields.append(f'selector={selector}')
+        if dkimdomain:
+            fields.append(f'dkimdomain={dkimdomain}')
+        if dkimdomaini:
+            fields.append(f'dkimdomaini={dkimdomaini}')
+        headervalue = f'{dkimval} ({myname}: {valid}) {"; ".join(fields)}'
+        return headervalue
+    
+    
+    def _get_dkim_hdr_tags(self, header:tp.Union[str, bytes, email.header.Header]) -> tp.Dict[bytes, bytes]:
+        hdrval = Suspect.decode_msg_header(header)
+        # wants bytes, returns dict of bytes
+        tags = dkim.util.parse_tag_value(force_bString(hdrval))
+        return tags
+        
+    
     def examine(self, suspect:Suspect):
+        if suspect.get_tag("DKIMVerify.result") is not None:
+            suspect.debug(f"{suspect.id} DKIM already validated, skip further processing")
+            return DUNNO
+        
         suspect.set_tag("DKIMVerify.result", DKIM_SKIP)
         if not DKIMPY_AVAILABLE:
             suspect.debug(f"{suspect.id} dkimpy not available, can not check DKIM")
             suspect.set_tag('DKIMVerify.skipreason', 'dkimpy library not available')
             return DUNNO
 
         hdr_from_domain = extract_from_domain(suspect)
@@ -745,72 +931,89 @@
         dkimdomain = ''
         record_domaini = ''
         selector = ''
         is_authordomain = False
         is_senderdomain = False
         dkimval = DKIM_NEUTRAL
         saval = None
+        keysize = 0
         
         source = self._get_source(suspect)
         env_from_domain = suspect.from_domain.lower()
         timeout = self.config.getfloat(self.section, 'max_lookup_time')
         try:
             # use the local logger of the plugin but prepend the fuglu id
-            d = self.DKIM(source, logger=PrependLoggerMsg(self.logger, prepend=suspect.id, maxlevel=logging.INFO), timeout=timeout)
-            try:
-                # one dkim header has to be valid
-                # trust priority: d=hdr_from, d=env_from, d=3rdparty
-                for i in range(0, len(dkimhdrs)):
-                    tags = dkim.util.parse_tag_value(force_bString(dkimhdrs[i]))
-                    # wants bytes, returns dict of bytes
-                    record_domain = tags.get(b'd', b'').decode().lower()
-                    record_domaini = tags.get(b'i', b'').decode().lower()
-                    record_selector = tags.get(b's', b'').decode().lower()
+            dkimcheck = self.DKIM(source, logger=PrependLoggerMsg(self.logger, prepend=suspect.id, maxlevel=logging.INFO), timeout=timeout)
+            # one dkim header has to be valid
+            # trust priority: d=hdr_from, d=env_from, d=3rdparty
+            dkimexc = False
+            for i in range(0, len(dkimhdrs)):
+                tags = self._get_dkim_hdr_tags(dkimhdrs[i])
+                record_domain = tags.get(b'd', b'').decode().lower()
+                record_domaini = tags.get(b'i', b'').decode().lower()
+                record_selector = tags.get(b's', b'').decode().lower()
+                try:
                     if self.dkim_dns_func is not None:
-                        record_valid = d.verify(idx=i, dnsfunc=self.dkim_dns_func)  # in unit tests as dkim module cannot be patched with mock
+                        record_valid = dkimcheck.verify(idx=i, dnsfunc=self.dkim_dns_func)  # in unit tests as dkim module cannot be patched with mock
                     else:
-                        record_valid = d.verify(idx=i)
+                        record_valid = dkimcheck.verify(idx=i)
                     if record_valid:
                         valid = True
                         if record_domain == hdr_from_domain or record_domain.endswith(f'.{hdr_from_domain}'):
                             is_authordomain = True
                             dkimval = DKIM_PASS
                             saval = DKIM_PASS_AUTHOR
                             dkimdomain = record_domain
                             selector = record_selector
                             break  # highest level of trust, finish evaluation
                         elif not is_authordomain and suspect.from_domain and \
-                                (record_domain == env_from_domain or record_domain.endswith(f'.{env_from_domain}')
-                                 ):
+                                (record_domain == env_from_domain or record_domain.endswith(f'.{env_from_domain}')):
                             is_senderdomain = True
                             dkimval = DKIM_PASS
                             saval = DKIM_PASS_SENDER
                             dkimdomain = record_domain
                             selector = record_selector
                         elif not is_authordomain and not is_senderdomain:
                             dkimval = DKIM_PASS
                             dkimdomain = record_domain
                             selector = record_selector
                     elif not valid:
+                        keysize = dkimcheck.keysize
                         dkimval = DKIM_FAIL
                         dkimdomain = record_domain
                         selector = record_selector
-                    self.logger.debug(
-                        f"{suspect.id}: DKIM idx={i} valid={valid} domain={record_domain} selector={record_selector} authordomain={is_authordomain} senderdomain={is_senderdomain}")
-            except dkim.DKIMException as de:
-                self.logger.warning(f'{suspect.id} DKIM validation failed: {str(de)}')
+                    self.logger.debug(f"{suspect.id}: DKIM idx={i} valid={valid} domain={record_domain} selector={record_selector} authordomain={is_authordomain} senderdomain={is_senderdomain} keysize={keysize}")
+                except dkim.DKIMException as de:
+                    self.logger.warning(f'{suspect.id} DKIM validation failed idx={i} domain={record_domain} selector={record_selector}: {str(de)}', exc_info=de)
+                    dkimexc = True
+                    if not dkimdomain and record_domain:
+                        dkimdomain = record_domain
+            
+            if dkimexc:
+                debugdumpdir = self.config.get(self.section, 'debugdumpdir')
+                if debugdumpdir:
+                    filename = os.path.join(debugdumpdir, f'{suspect.id}.eml')
+                    with open(filename, 'wb') as f:
+                        f.write(suspect.get_source())
+                    self.logger.warning(f'{suspect.id} DKIM validation failed, dumped original source to {filename}')
+
+                    filename = os.path.join(debugdumpdir, f'{suspect.id}.dkimsource.eml')
+                    with open(filename, 'wb') as f:
+                        f.write(source)
+                    self.logger.warning(f'{suspect.id} DKIM validation failed, dumped DKIM source to {filename}')
+
                 dkimval = DKIM_PERMFAIL
         except dkim.MessageFormatError as e:
             dkimval = DKIM_NEUTRAL
             self.logger.warning(f'{suspect.id} DKIM validation failed: Message format error: {str(e)}')
-            suspect.set_tag('DKIMVerify.skipreason', 'plugin error')
+            suspect.set_tag('DKIMVerify.skipreason', 'message error')
         except (TimeoutError, DNS_TIMEOUT) as e:
             dkimval = DKIM_TEMPFAIL
             self.logger.warning(f'{suspect.id} DKIM validation failed due to: {str(e)}')
-            suspect.set_tag('DKIMVerify.skipreason', 'plugin error')
+            suspect.set_tag('DKIMVerify.skipreason', 'dns error')
         except NameError as e:
             self.logger.warning(f'{suspect.id} DKIM validation failed due to missing dependency: {str(e)}')
             suspect.set_tag('DKIMVerify.skipreason', 'plugin error')
         except Exception as e:
             self.logger.warning(f'{suspect.id} DKIM validation failed: {e.__class__.__name__}: {str(e)}')
             import traceback
             self.logger.debug(f'{suspect.id} {traceback.format_exc()}')
@@ -824,15 +1027,18 @@
         suspect.set_tag("DKIMVerify.selector", selector)
         suspect.set_tag("DKIMVerify.sigvalidauthor", is_authordomain)
         suspect.set_tag("DKIMVerify.sigvalidsender", is_senderdomain)
         suspect.write_sa_temp_header(SAHEADER_DKIM, saval or dkimval)
         result_header = self.config.get(self.section, 'result_header')
         if result_header:
             suspect.add_header(result_header, saval or dkimval)
-        self.logger.debug(f'{suspect.id} DKIM validation complete: valid={valid} domain={dkimdomain} selector={selector} result={saval}')
+        if self.config.getboolean(self.section, 'create_received_dkim'):
+            rcvdspfhdr = self._create_received_dkim(valid, saval or dkimval, dkimdomain, record_domaini, selector)
+            suspect.add_header('Received-DKIM', rcvdspfhdr, immediate=True)
+        self.logger.debug(f'{suspect.id} DKIM validation complete: valid={valid} domain={dkimdomain} selector={selector} keysize={keysize} result={saval}')
         return DUNNO
 
     def lint(self):
         all_ok = self.check_config()
 
         if not DKIMPY_AVAILABLE:
             print("Missing dependency: dkimpy https://launchpad.net/dkimpy")
@@ -856,14 +1062,73 @@
 # test:
 # plugdummy.py -p ...  domainauth.DKIMSignPlugin -s <sender> -o canonicalizeheaders:relaxed -o canonicalizebody:simple -o signbodylength:False
 # cat /tmp/fuglu_dummy_message_out.eml | swaks -f <sender>  -s <server>
 # -au <username> -ap <password> -4 -p 587 -tls -d -  -t
 # <someuser>@gmail.com
 
 
+class DKIMRcvdPlugin(ScannerPlugin):
+    """
+If DKIMVerify plugin is not run in this instance of Fuglu, use this plugin to extract a
+"Received-DKIM" header (a custom header in the style of Received-SPF but for DKIM verification)
+created by a Fuglu/Spam filter running on a previous system.
+Set create_received_dkim in DKIMVerify plugin config to write such a header. It'll write a header such as:
+Received-DKIM: pass (firsthost.fuglu.org: True) key1=value1;key2=value2
+To enable reading set received_dkim_header_receiver in DKIMRcvdPlugin config to the hostname/domain of the
+server writing the header, e.g. in this case firsthost.fuglu.org or .fuglu.org.
+The hostname is always read recursively, e.g. .fuglu.org would also match otherhost.fuglu.org
+    """
+    def __init__(self, config, section=None):
+        super().__init__(config, section)
+        self.logger = self._logger()
+        self.requiredvars = {
+            'received_dkim_header_receiver': {
+                'default': '',
+                'description': 'if dkim verify plugin is not run locally, use received-dkim header with receiver field value in given domain name. leave empty to not parse received-dkim header'
+            },
+        }
+    
+    
+    def examine(self, suspect):
+        rcvddkimreceiver = self.config.get(self.section, 'received_dkim_header_receiver')
+        if not rcvddkimreceiver:
+            self.logger.debug(f'{suspect.id} received_dkim_header_receiver not defined')
+            return DUNNO
+        
+        msgrep = suspect.get_message_rep()
+        rcvddkim_all = msgrep.get_all('Received-DKIM', [])
+        for rcvddkim in rcvddkim_all:
+            try:
+                rcvddkim = Suspect.decode_msg_header(rcvddkim)
+                rcvddkimstatus, fields, expl = parse_received_xxx(rcvddkim)
+                receiver = fields.get('receiver')
+                if rcvddkimstatus and receiver and receiver.lower().endswith(rcvddkimreceiver.lower()):
+                    rcvddkimstatus = rcvddkimstatus.lower()
+                    if rcvddkimstatus in [DKIM_PASS_SENDER, DKIM_PASS_AUTHOR]:
+                        self.logger.debug(f'{suspect.id} rewriting DKIM status from {rcvddkimstatus} to {DKIM_PASS}')
+                        dkimval = DKIM_PASS
+                    else:
+                        dkimval = rcvddkimstatus
+                    
+                    suspect.set_tag("DKIMVerify.sigvalid", expl and expl.lower()=='true')
+                    suspect.set_tag("DKIMVerify.result", dkimval)
+                    suspect.set_tag("DKIMVerify.dkimdomain", fields.get('dkimdomain'))
+                    suspect.set_tag("DKIMVerify.dkimdomaini", fields.get('dkimdomaini'))
+                    suspect.set_tag("DKIMVerify.selector", fields.get('selector'))
+                    suspect.write_sa_temp_header(SAHEADER_DKIM, rcvddkimstatus)
+                    break
+                elif rcvddkim:
+                    self.logger.debug(f'{suspect.id} failed to get status from received-dkim header. status={rcvddkimstatus} receiver={receiver} received-dkim={rcvddkim}')
+                elif not rcvddkim:
+                    self.logger.debug(f'{suspect.id} no received-dkim header')
+            except Exception as e:
+                self.logger.error(f'{suspect.id} failed to parse received-dkim header "{rcvddkim}" due to {e.__class__.__name__}: {str(e)}')
+        return DUNNO
+
+
 class DKIMSignPlugin(ScannerPlugin):
     """
 Add DKIM Signature to outgoing mails
 
 Setting up your keys:
 
 ::
@@ -921,15 +1186,15 @@
 
     def examine(self, suspect):
         if not DKIMPY_AVAILABLE:
             suspect.debug("dkimpy not available, can not sign DKIM")
             self.logger.error(f'{suspect.id} DKIM signing skipped - missing dkimpy library')
             return DUNNO
 
-        message = suspect.get_source()
+        message = suspect.get_source(newline=b'\r\n')
         header_from_domain = extract_from_domain(suspect)
         if header_from_domain is None:
             self.logger.debug(f"{suspect.id} Failed to extract From-header domain for DKIM signing")
             return DUNNO
 
         addvalues = dict(header_from_domain=header_from_domain)
         selector = apply_template(self.config.get(self.section, 'selector'), suspect, addvalues)
@@ -957,16 +1222,16 @@
         blength = self.config.getboolean(self.section, 'signbodylength')
 
         dkimhdr = dkim.sign(message, force_bString(selector), force_bString(header_from_domain), privkeycontent,
                             canonicalize=canon, include_headers=inc_headers, length=blength,
                             logger=suspect.get_tag('debugfile'))
         if dkimhdr.startswith(b'DKIM-Signature: '):
             dkimhdr = dkimhdr[16:]
-
-        suspect.add_header('DKIM-Signature', force_uString(dkimhdr), immediate=True)
+        # dkim.sign provides a properly folded header. we trust it's valid.
+        suspect.add_header('DKIM-Signature', force_uString(dkimhdr), immediate=True, raw=True)
         return DUNNO
 
     def lint(self):
         all_ok = self.check_config()
 
         if not DKIMPY_AVAILABLE:
             print("Missing dependency: dkimpy https://launchpad.net/dkimpy")
@@ -980,14 +1245,94 @@
         if '{' not in privkeytemplate and not os.path.exists(privkeytemplate):
             print("Private key file %s not found" % privkeytemplate)
             all_ok = False
 
         return all_ok
 
 
+class DKIMStripPlugin(ScannerPlugin):
+    """
+    This plugin removes previous DKIM headers if subject was changed
+    """
+    
+    def __init__(self, config, section=None):
+        super().__init__(config, section)
+        self.logger = self._logger()
+        self.requiredvars = {
+            'senderdomains': {
+                'default': '',
+                'description': 'only strip specific header sender domains. list comma separated.',
+            },
+            'recipientdomains': {
+                'default': '',
+                'description': 'only strip specific envelope recipient domains. list comma separated.',
+            },
+            'verbose': {
+                'default': 'False',
+                'description': 'be extra verbose'
+            }
+        }
+    
+    
+    def __str__(self):
+        return "DKIM Strip"
+    
+    
+    def examine(self, suspect):
+        verbose = self.config.getboolean(self.section, 'verbose')
+        origsubj = suspect.get_tag('origsubj')
+        if origsubj is None:
+            if verbose:
+                self.logger.debug(f'{suspect.id} subject unaltered (no origsubj tag)')
+            return DUNNO
+        
+        hdr_from_domain = None
+        hdr_from_address = suspect.parse_from_type_header(header='From', validate_mail=True)
+        if hdr_from_address and hdr_from_address[0] and hdr_from_address[0][1]:
+            hdr_from_domain = domain_from_mail(hdr_from_address[0][1])
+        if not hdr_from_domain:
+            self.logger.debug(f'{suspect.id} No From header address found')
+            return DUNNO
+        
+        recipientdomains = self.config.getlist(self.section, 'recipientdomains')
+        if suspect.to_domain not in recipientdomains:
+            if verbose:
+                self.logger.debug(f'{suspect.id} {suspect.to_domain} not in {recipientdomains}')
+            return DUNNO
+        
+        senderdomains = self.config.getlist(self.section, 'senderdomains')
+        if hdr_from_domain.lower() not in senderdomains:
+            if verbose:
+                self.logger.debug(f'{suspect.id} {hdr_from_domain} not in {senderdomains}')
+            return DUNNO
+            
+        subject = suspect.get_header('subject')
+        if origsubj != subject:
+            rm = suspect.remove_headers_from_source({'DKIM-Signature'})
+            if rm:
+                self.logger.info(f'{suspect.id} removed dkim headers')
+            elif verbose:
+                self.logger.debug(f'{suspect.id} no dkim headers')
+        elif verbose:
+            self.logger.debug(f'{suspect.id} subject unaltered: origsubj={origsubj} subject={subject}')
+        return DUNNO
+    
+    
+    def lint(self):
+        ok = self.check_config()
+        if ok:
+            recipientdomains = self.config.getlist(self.section, 'recipientdomains')
+            if not recipientdomains:
+                print('WARNING: no recipient domains specified. this plugin will do nothing.')
+            senderdomains = self.config.getlist(self.section, 'senderdomains')
+            if not senderdomains:
+                print('WARNING: no sender domains specified. this plugin will do nothing.')
+        return ok
+
+
 class NetworkList(FileList):
     def _parse_lines(self, lines):
         lines = super()._parse_lines(lines)
         return [ipaddress.ip_network(x, False) for x in lines]
 
     def is_listed(self, addr):
         try:
@@ -1043,16 +1388,16 @@
       - set a domain selective_spf_file and list the domains to be tested for hard fail
       - set selective_softfail to False
       - set on_fail to REJECT and on_softfail to DUNNO
 
     ==========================
     = NON-Milter stage (EOM) =
     ==========================
-    This plugin checks the SPF status and sets tag 'SPF.status' to one of the official states 'pass', 'fail', 'neutral',
-    'softfail, 'permerror', 'temperror', or 'skipped' if the SPF check could not be peformed.
+    This plugin checks the SPF status and sets tag 'SPF.status' to one of the official states 'none', 'pass', 'fail',
+    'softfail, 'neutral', 'permerror', 'temperror', or 'skipped' if the SPF check could not be peformed.
     Tag 'SPF.explanation' contains a human-readable explanation of the result.
     Additional information to be used by SA plugin is added
 
     The plugin does not take any action based on the SPF test result since. Other plugins might use the SPF result
     in combination with other factors to take action (for example a "DMARC" plugin could use this information)
 
     However, if mark_milter_check=True then the message is marked as spam if the milter stage
@@ -1127,15 +1472,15 @@
                 'description': 'maximum time per DNS lookup (RFC defaults to 20 seconds)',
             },
             'strict_level': {
                 'default': '1',
                 'description': 'strictness of SPF lookup: 0: relaxed, 1: strict, 2: harsh',
             },
             'hoster_mx_exception': {
-                'default': '.google.com .protection.outlook.com',
+                'default': '.google.com .protection.outlook.com .mx.microsoft',
                 'description': 'always consider pass if mail is sent from server with PTR ending in name specified, MX points to this server, and SPF record contains MX directive',
             },
             'hoster_include_exception': {
                 'default': '', # '.protection.outlook.com' is a hot candidate
                 'description': 'always consider pass if mail is sent from servers with PTR ending in name specified and SPF record contains include directive ending with name specified',
             },
             'state': {
@@ -1408,14 +1753,15 @@
         query = spf.query(client_address, sender, helo_name, strict=strict_level)
         try:
             retries = self.config.getint(self.section, 'temperror_retries')
             maxlookups = self.config.getint(self.section, 'max_lookups')
             spf.MAX_LOOKUP = maxlookups
             maxlookuptime = self.config.getint(self.section, 'max_lookup_time')
             spf.MAX_PER_LOOKUP_TIME = maxlookuptime
+            spf.query.timeout = maxlookuptime
             if is_ipv6(client_address):
                 # ugly hack, but only very few hosts have aaaa records and result in too many permerrors
                 spf.MAX_VOID_LOOKUPS = maxlookups
             if client_address and sender:
                 result, explanation, spfrecord = self._spf_lookup(sessid, query, retries=retries)
                 self.logger.debug(f"{sessid} lookup result={result}")
             elif sender:
@@ -1483,24 +1829,18 @@
             explanation = 'unknown'
         elif explanation and ('\n' in explanation or '\r' in explanation):
             explanation = explanation.replace('\n', '<NEWLINE>').replace('\r', '<LINEBREAK>')
 
         if result not in result_map:
             self.logger.error(f"{suspect.id} -> spf result '{result}' not in result_map")
         headervalue = f'{result_map.get(result)} ({myname}: {explanation}) {"; ".join(fields)}'
-        try:
-            header = Header(headervalue)
-            header.encode()
-        except HeaderParseError as e:
-            self.logger.debug(f'{suspect.id} received-spf header requires encoding: {str(e)}')
-            headervalue = Header(explanation, charset='utf-8').encode()
         return headervalue
     
     def _get_from_address(self, suspect:Suspect) -> str:
-        env_hdr = self.config.getlist(self.section, 'use_header_as_env_sender')
+        env_hdr = self.config.getlist(self.section, 'use_header_as_env_sender', resolve_env=True)
         for hdrname in env_hdr:
             value = suspect.get_header(hdrname)
             if value and is_email(value):
                 self.logger.debug(f'{suspect.id} using address {value} from header {hdrname} as envelope sender override')
                 return value
         return suspect.from_address
     
@@ -1850,17 +2190,14 @@
                 'default': '',
                 'description': 'override envelope sender with value from one of these headers (if set - first occurrence wins)'
             },
         }
 
     def _query_dmarc(self, domain):
         records = []
-        if self.tldmagic is not None:
-            domain = self.tldmagic.get_domain(domain)
-
         timeout = self.config.getfloat(self.section, 'max_lookup_time')
         hostname = f'_dmarc.{domain}'
         result = lookup(hostname, QTYPE_TXT, timeout=timeout)
         if result is None:
             return records
 
         for item in result:
@@ -1892,38 +2229,26 @@
         else:
             dkim_domain = suspect.get_tag("DKIMVerify.dkimdomain")
             dkim_selector = suspect.get_tag("DKIMVerify.selector")
 
         self.logger.debug(f'{suspect.id} dkim result={dkim_result} status={value} domain={dkim_domain} selector={dkim_selector}')
         return dkim_result, dkim_domain, dkim_selector
     
-    def _parse_received_spf(self, rcvdspf):
-        status = None
-        receiver = None
-        if rcvdspf:
-            fields = rcvdspf.split(';')
-            if fields and fields[0]:
-                status = fields[0].split(None,1)[0]
-                firstfield = fields[0].rsplit(None,1)[-1]
-                fields[0] = firstfield
-                fieldmap = {v[0].lower():v[1] for v in [f.split('=',1) for f in fields if '=' in f]}
-                receiver = fieldmap.get('receiver')
-        return status, receiver
-    
     def _get_spf_result(self, suspect):
         status = suspect.get_tag('SPF.status', None)
         if status is None:
             rcvdspfreceiver = self.config.get(self.section, 'received_spf_header_receiver')
             if rcvdspfreceiver:
                 msgrep = suspect.get_message_rep()
                 rcvdspf_all = msgrep.get_all('Received-SPF', [])
                 for rcvdspf in rcvdspf_all:
                     try:
                         rcvdspf = Suspect.decode_msg_header(rcvdspf)
-                        rcvdspfstatus, receiver = self._parse_received_spf(rcvdspf)
+                        rcvdspfstatus, fields, expl = parse_received_xxx(rcvdspf)
+                        receiver = fields.get('receiver')
                         if rcvdspfstatus and receiver and receiver.lower().endswith(rcvdspfreceiver.lower()):
                             status = rcvdspfstatus.lower()
                             suspect.set_tag('SPF.status', status)
                             break
                         elif rcvdspf:
                             self.logger.debug(f'{suspect.id} failed to get status from received-spf header. status={rcvdspfstatus} receiver={receiver} received-spf={rcvdspf}')
                         elif not rcvdspf:
@@ -1945,15 +2270,15 @@
         }
         spf_result = spf_value_map.get(status)
         self.logger.debug(f'{suspect.id} spf result={spf_result} status={status}')
         return spf_result
 
     def _mk_aspf(self, suspect, spf_result):
         from_domain = suspect.from_domain
-        env_headers = self.config.getlist(self.section, 'use_header_as_env_sender')
+        env_headers = self.config.getlist(self.section, 'use_header_as_env_sender', resolve_env=True)
         if env_headers:
             for header in env_headers:
                 value = suspect.get_header(header)
                 if value and '@' in value:
                     from_domain = domain_from_mail(value)
                     self.logger.debug(f'{suspect.id} SPF override env domain={from_domain} from header {header}')
     
@@ -1968,20 +2293,20 @@
     def _mk_adkim(self, dkim_domain, dkim_result, dkim_selector):
         if dkim_result is None:
             adkim = None
         else:
             adkim = dmarc.DKIM(domain=dkim_domain, result=dkim_result, selector=dkim_selector)
         return adkim
 
-    def _do_dmarc_check(self, dmarc_record, header_from_domain, aspf, adkim, suspectid):
+    def _do_dmarc_check(self, dmarc_record, header_from_domain, aspf, adkim, suspectid, org_domain):
         result = None
         dispo = None
         try:
             d = dmarc.DMARC()
-            p = d.parse_record(record=dmarc_record, domain=header_from_domain)
+            p = d.parse_record(record=dmarc_record, domain=header_from_domain, org_domain=org_domain)
             r = d.get_result(p, spf=aspf, dkim=adkim)
             result = r.result
             dispo = r.disposition
         except dmarc.RecordSyntaxError as e:
             self.logger.info(f'{suspectid} invalid DMARC record for {header_from_domain}: "{dmarc_record}" error: {str(e)}')
         except ValueError:
             if aspf is not None:
@@ -2017,31 +2342,41 @@
 
         header_from_domain = extract_from_domain(suspect)
         if not header_from_domain:
             self._write_result(suspect, DMARC_SKIP)
             self.logger.debug(f'{suspect.id} no valid domain found in From header')
             return DUNNO
 
+        org_domain = None
         dmarc_records = self._query_dmarc(header_from_domain)
         dmarc_records_len = len(dmarc_records)
+        if dmarc_records_len == 0 or dmarc_records_len > 1:
+            # No valid records found, try Organizational Domain
+            if self.tldmagic is not None:
+                domain = self.tldmagic.get_domain(header_from_domain)
+                if domain and domain != header_from_domain:
+                    org_domain = domain
+                    dmarc_records = self._query_dmarc(org_domain)
+                    dmarc_records_len = len(dmarc_records)
+        
         if dmarc_records_len == 0:
-            self._write_result(suspect, DMARC_SKIP)
+            self._write_result(suspect, DMARC_NONE)
             self.logger.debug(f'{suspect.id} no DMARC record found for domain {header_from_domain}')
             return DUNNO
         elif dmarc_records_len > 1:
             self._write_result(suspect, DMARC_RECORDFAIL)
             self.logger.debug(f'{suspect.id} DMARC check failed. too many records count={dmarc_records_len}')
             return DUNNO
 
         spf_result = self._get_spf_result(suspect)
         dkim_result, dkim_domain, dkim_selector = self._get_dkim_result(suspect)
 
         aspf = self._mk_aspf(suspect, spf_result)
         adkim = self._mk_adkim(dkim_domain, dkim_result, dkim_selector)
-        result, dispo = self._do_dmarc_check(dmarc_records[0], header_from_domain, aspf, adkim, suspect.id)
+        result, dispo = self._do_dmarc_check(dmarc_records[0], header_from_domain, aspf, adkim, suspect.id, org_domain)
         self.logger.debug(f'{suspect.id} dmarc eval for {header_from_domain} with result={result} and dispo={dispo} input spf={spf_result} dkim_result={dkim_result} dkim_domain={dkim_domain} dkim_selector={dkim_selector}')
 
         if result is None:
             self._write_result(suspect, DMARC_RECORDFAIL)
         elif result == dmarc.POLICY_PASS:
             self._write_result(suspect, DMARC_PASS)
         elif result == dmarc.POLICY_FAIL:
@@ -2417,14 +2752,19 @@
                 'description': 'SRS token separator',
             },
 
             'rewrite_header_to': {
                 'default': 'True',
                 'description': 'set True to rewrite address in To: header in bounce messages (reverse/decrypt mode)',
             },
+            
+            'spf_only': {
+                'default': 'False',
+                'description': 'only rewrite if sender domain is spf protected (requires SPFPlugin to run first)',
+            }
         }
 
     def get_sql_setting(self, domain, dbconnection, sqlquery, cache, cachename, default_value=None, logger=None):
         if logger is None:
             logger = logging.getLogger('fuglu.plugins.domainauth.SenderRewriteScheme.sql')
 
         cachekey = '%s-%s' % (cachename, domain)
@@ -2490,14 +2830,18 @@
         else:
             new_hdr = f'<{to_address}>'
         suspect.set_header('To', new_hdr)
 
     def examine(self, suspect):
         if not SRS_AVAILABLE:
             return DUNNO
+        
+        if self.config.getboolean(self.section, 'spf_only') and suspect.get_tag("SPF.status") == 'none':
+            self.logger.info(f'{suspect.id} ignoring mail from {suspect.from_domain} without spf')
+            return DUNNO
 
         if not self.should_we_rewrite_this_domain(suspect):
             self.logger.info(f'{suspect.id} ignoring mail to {suspect.to_address}')
             return DUNNO
 
         if not suspect.from_address:
             self.logger.info(f'{suspect.id} ignoring bounce message')
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/fuzor.py` & `fuglu-1.5.0/src/fuglu/plugins/fuzor.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 from fuglu.stringencode import force_bString
 
 CONN_EXC = []
 if REDIS_ENABLED:
     CONN_EXC.append(redis.exceptions.ConnectionError)
 
 try:
+    import six
+    import sys
+    if sys.version_info >= (3, 12, 0): # https://github.com/dpkp/kafka-python/issues/2401#issuecomment-1760208950
+        sys.modules['kafka.vendor.six.moves'] = six.moves
     # requires kafka-python
     import kafka
     CONN_EXC.append(kafka.errors.KafkaError)
     KAFKA_AVAILABLE = True
 except ImportError:
     KAFKA_AVAILABLE = False
 CONN_EXC = tuple(CONN_EXC)
@@ -43,14 +47,18 @@
 
 class FuzorMixin(object):
     requiredvars = {
         'backend': {
             'default': 'redis',
             'description': 'storage backend to be used. currently supported: redis (check/report), kafka (report only)'
         },
+        'hash_algo': {
+            'default': 'sha1',
+            'description': f'hash algorithm to be used, specify any hash supported by hashlib: {",".join(hashlib.algorithms_available)}'
+        },
 
         'redis_conn': {
             'default': 'redis://localhost:6379/0',
             'description': 'redis config: redis://host:port/db',
         },
         'redis_password': {
             'default': '',
@@ -113,15 +121,15 @@
 
     def _init_backend_redis(self):
         if self.backend is not None:
             return
         redis_url = self.config.get(self.section, 'redis_conn')
         password = self.config.get(self.section, 'redis_password') or None
         timeout = self.config.getint(self.section, 'timeout')
-        redis_pool = RedisPooledConn(redis_url, password=password, timeout=timeout)
+        redis_pool = RedisPooledConn(redis_url, password=password, socket_timeout=timeout)
         self.backend = RedisBackend(redis_pool)
         self.backend.ttl = self.config.getint(self.section, 'redis_ttl')
 
     def _init_backend_kafka(self):
         if self.backend is not None:
             return
         hosts = self.config.get(self.section, 'kafkahosts').split()
@@ -134,14 +142,19 @@
     def lint(self):
         if not self.check_config():
             return False
 
         if self.config.getboolean(self.section, 'stripoversize'):
             maxsize = self.config.getint(self.section, 'maxsize')
             print("Stripping oversize messages (size > %u) to calculate a fuzor hash..." % maxsize)
+        
+        hash_algo = self.config.get(self.section, 'hash_algo')
+        if not hash_algo in hashlib.algorithms_available:
+            print(f'ERROR: invalid hash algorithm {hash_algo} - use one of {",".join(hashlib.algorithms_available)}')
+            return False
 
         backend = self.config.get(self.section, 'backend').lower()
         if backend == 'redis':
             ok = self._lint_redis()
             print('INFO: using redis backend')
         elif backend == 'kafka':
             ok = self._lint_kafka()
@@ -152,34 +165,19 @@
         return ok
 
     def _lint_redis(self):
         ok = True
         if not REDIS_ENABLED:
             print('ERROR: redis extension not available. This plugin will do nothing.')
             return False
-
-        # check redis version
-        # 2.10.a has a bug which can make the connections stuck with python3
-        py3minversion = [2, 10, 2]
-        try:
-            redisversion = [int(i) for i in redis.__version__.split('.')]
-            print("Redis version found %s" % ".".join([str(i) for i in redisversion]))
-        except Exception:
-            print("Could not extract package version.")
-            print("Make sure you have minimum %s installed" % ".".join([str(i) for i in py3minversion]))
-        else:
-            for minv, avail in zip(py3minversion, redisversion):
-                if avail < minv:
-                    ok = False
-                elif avail > minv:
-                    ok = True
-                    break
-            if not ok:
-                print("WARNING: Please update. Minimum version %s" % ".".join([str(i) for i in py3minversion]))
-
+        
+        password = self.config.get(self.section, 'redis_password', fallback=None) or None
+        if password is not None:
+            print('deprecatioin warning: obsolete redis_password configured, set via redis_conn')
+            
         if ok:
             try:
                 self._init_backend()
                 reply = self.backend.redis_pool.check_connection()
                 if reply:
                     print('OK: redis server replied to ping')
                 else:
@@ -222,16 +220,17 @@
                     _class=PatchedMessage
                 )
             else:
                 self.logger.debug(f'{suspect.id} message too big, {suspect.size} > {maxsize}')
                 return digest, count
         else:
             msgrep = suspect.get_message_rep()
-
-        fuhash = FuzorDigest(msgrep)
+            
+        hash_algo = self.config.get(self.section, 'hash_algo')
+        fuhash = FuzorDigest(msgrep, hash_algo)
 
         try:
             self.logger.debug(f"{suspect.id} to={suspect.to_address} hash={fuhash.digest} usable_body={fuhash.bodytext_size} predigest={fuhash.predigest[:50]} subject={msgrep.get('Subject')}")
         except Exception:
             pass
 
         if fuhash.digest is not None:
@@ -371,16 +370,17 @@
             else:
                 suspect.debug('Fuzor: message too big, not digesting')
                 self.logger.debug(f'{suspect.id} message too big, {suspect.size} > {maxsize}')
                 # self.logger.info("%s: FUZOR END (SIZE SKIP)"%suspect.id)
                 return DUNNO
         else:
             msgrep = suspect.get_message_rep()
+        hash_algo = self.config.get(self.section, 'hash_algo')
         # self.logger.info("%s: FUZOR PRE-HASH"%suspect.id)
-        fuhash = FuzorDigest(msgrep)
+        fuhash = FuzorDigest(msgrep, hash_algo)
         digest = fuhash.digest
         # self.logger.info("%s: FUZOR POST-HASH"%suspect.id)
         if digest is not None:
             suspect.debug(f'Fuzor digest {digest}')
 
             self._init_ignorelist()
             if self.ignorelist is not None:
@@ -468,27 +468,28 @@
     """Just print out the fuzor hash (for debugging) """
 
     def __init__(self, config, section=None):
         super().__init__(config, section)
         self.logger = self._logger()
 
     def examine(self, suspect):
+        hash_algo = self.config.get(self.section, 'hash_algo')
         msg = suspect.get_message_rep()
-        fuhash = FuzorDigest(msg)
+        fuhash = FuzorDigest(msg, hash_algo)
         if fuhash.digest is not None:
             self.logger.info(f'{suspect.id} Predigest: {fuhash.predigest}')
             self.logger.info(f'{suspect.id} hash {fuhash.digest}')
         else:
             self.logger.info(f'{suspect.id} does not produce enough data for a unique hash')
 
         return DUNNO
 
 
 class FuzorDigest(object):
-    def __init__(self, msg):
+    def __init__(self, msg, hash_algo):
         self.debug = []
         self.digest = None
         self.predigest = None
         self.bodytext_size = 0
         self.filter = SuspectFilter(None)
         self.logger = logging.getLogger('fuglu.plugins.fuzor.Digest')
 
@@ -506,15 +507,16 @@
         self.MINIMUM_BODYTEXT_SIZE = 27  # if the body text content is smaller than this, ignore this message
         self.STRIP_WHITESPACE = True  # remove all whitespace from the pre-digest
         self.STRIP_HTML_MARKUP = True  # remove html tags (but keep content)
         self.REMOVE_HTML_TAGS = [
             'script',
             'style',
         ]  # strip tags (including content)
-
+        
+        self.hasher = getattr(hashlib, hash_algo)
         self.predigest = self._make_predigest(msg)
         self.digest = self._make_hash(self.predigest)
     
     _re_hex = re.compile(r'\[[A-Z0-9:]+]')
     def _make_hash(self, predigest):
         if self.bodytext_size < self.MINIMUM_BODYTEXT_SIZE:
             return None
@@ -522,15 +524,15 @@
         if len(predigest) < self.MINIMUM_PREDIGEST_SIZE:
             return None
         unmodified = self._re_hex.sub('', predigest)
         if len(unmodified) < self.MINIMUM_UNMODIFIED_CONTENT:
             return None
 
         predigest = predigest.encode('utf-8', errors='ignore')
-        return hashlib.sha1(predigest).hexdigest()
+        return self.hasher(predigest).hexdigest()
     
     _re_email = re.compile(r'\S{1,50}@\S{1,30}')
     _re_uri = re.compile(r'[a-z]+:\S{1,100}')
     _re_ws = re.compile(r'\s')
     def _handle_text_part(self, part):
         payload = part.get_payload(decode=True)
         charset = part.get_content_charset()
@@ -579,15 +581,15 @@
                     predigest += normalized_text_part
                     self.bodytext_size += len(normalized_text_part)
                 except Exception as e:
                     self.logger.warning(e)
             else:
                 attachment_count += 1
                 if self.INCLUDE_ATTACHMENT_CONTENT:
-                    predigest += f"[ATTH:{hashlib.sha1(part.get_payload()).hexdigest()}]"
+                    predigest += f"[ATTH:{self.hasher(part.get_payload()).hexdigest()}]"
 
         if self.INCLUDE_ATTACHMENT_COUNT and attachment_count:
             predigest += f"[ATTC:{attachment_count}]"
 
         if self.STRIP_WHITESPACE:
             predigest = self._re_ws.sub('', predigest)
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/geoip.py` & `fuglu-1.5.0/src/fuglu/plugins/geoip.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,18 @@
                 'default': 'geoip.countrycode',
                 'description': 'list of tag name',
             },
             'database': {
                 'default': '',
                 'description': 'path to geoip database',
             },
+            'debug': {
+                'default': 'False',
+                'description': 'enable additional debugging output',
+            },
         }
         self.geoip = None
 
     def _init_geoip(self):
         filename = self.config.get(self.section, 'database')
         if self.geoip is None and filename:
             if os.path.exists(filename):
@@ -75,29 +79,30 @@
         return cc, None
 
     def _run(self, suspect: Suspect):
         if not HAVE_GEOIP2:
             return DUNNO
 
         self._init_geoip()
-
+        debug = self.config.getboolean(self.section, 'debug')
+        
         if self.geoip is not None:
             clientip = self._get_clientip(suspect)
             if clientip is not None:
                 values = self._get_geodata(clientip, suspect.id)
-                self.logger.debug(f'{suspect.id} clientip {clientip} has values {values}')
+                debug and self.logger.debug(f'{suspect.id} clientip {clientip} has values {values}')
                 if values[0] is not None:
                     headernames = self.config.getlist(self.section, 'headernames')
                     for hn, val in zip(headernames, values):
                         suspect.write_sa_temp_header(hn, val)
-                        self.logger.debug(f'{suspect.id} set sa temp header {hn} with value {val}')
+                        debug and self.logger.debug(f'{suspect.id} set sa temp header {hn} with value {val}')
                     tagnames = self.config.getlist(self.section, 'tagnames')
                     for tn, val in zip(tagnames, values):
                         suspect.set_tag(tn, val)
-                        self.logger.debug(f'{suspect.id} set tag {tn} with value {val}')
+                        debug and self.logger.debug(f'{suspect.id} set tag {tn} with value {val}')
         else:
             self.logger.debug(f'{suspect.id} no clientip found')
         return DUNNO
 
     def examine(self, suspect):
         return self._run(suspect)
 
@@ -117,15 +122,18 @@
     def lint(self):
         if not HAVE_GEOIP2:
             print('ERROR: geoip2 module not found. this plugin will do nothing')
 
         ok = self.check_config()
         if ok:
             filename = self.config.get(self.section, 'database')
-            if not os.path.exists(filename):
+            if not filename:
+                print(f'ERROR: geoip database file name not defined')
+                ok = False
+            elif not os.path.exists(filename):
                 print(f'ERROR: Could not find geoip database {filename}')
                 ok = False
             else:
                 self._init_geoip()
                 if self.geoip is None:
                     print('ERROR: geoip not initialized')
                     ok = False
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/knownsubject.py` & `fuglu-1.5.0/src/fuglu/plugins/knownsubject.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     DOMAINMAGIC_AVAILABLE = True
 except ImportError:
     DOMAINMAGIC_AVAILABLE = False
 
     def unconfuse(value):
         return value
 try:
+    import six
+    import sys
+    if sys.version_info >= (3, 12, 0): # https://github.com/dpkp/kafka-python/issues/2401#issuecomment-1760208950
+        sys.modules['kafka.vendor.six.moves'] = six.moves
     import kafka
     KAFKA_AVAILABLE = True
 except ImportError:
     KAFKA_AVAILABLE = False
 
 
 class KnownSubjectMixin(object):
@@ -99,16 +103,15 @@
         """
         if self.backend_redis is not None:
             return
         redis_conn = self.config.get(self.section, 'redis_conn')
         if redis_conn and REDIS_AVAILABLE:
             ttl = self.config.getint(self.section, 'ttl')
             socket_timeout = self.config.getint(self.section, 'timeout'),
-            pinginterval = self.config.getint(self.section, 'pinginterval')
-            redis_pool = RedisPooledConn(redis_conn, socket_keepalive=True, socket_timeout=socket_timeout, pinginterval=pinginterval)
+            redis_pool = RedisPooledConn(redis_conn, socket_timeout=socket_timeout)
             self.backend_redis = ExpiringCounter(redis_pool, ttl)
 
     def _insert_redis(self, suspect, subject):
         self._init_backend_redis()
         if self.backend_redis:
             multiplicator = self.config.getint(self.section, 'multiplicator')
             try:
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/mailcopy.py` & `fuglu-1.5.0/src/fuglu/plugins/mailcopy.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,24 +95,25 @@
                 self.logger.warning(f'{suspect.id} imapcopy rule issued DELETE, ignoring in appender plugin (original decision={actioncode_to_string(decision)})')
         except Exception as e:
             self.logger.error(f'{suspect.id} failed to copy to imap server due to {e.__class__.__name__}: {str(e)}')
 
     def _run(self, suspect: Suspect):
         imapcopyrules = self.config.get(self.section, 'imapcopyrules')
         if imapcopyrules is None or imapcopyrules == "":
+            self.logger.warning(f'{suspect.id} not IMAP copy rules file defined')
             return DUNNO
 
         if not os.path.exists(imapcopyrules):
-            self._logger().error(f'{suspect.id} IMAP copy rules file does not exist: {imapcopyrules}')
+            self.logger.error(f'{suspect.id} IMAP copy rules file does not exist: {imapcopyrules}')
             return DUNNO
 
         if self.filter is None:
             self.filter = SuspectFilter(imapcopyrules)
 
-        (match, info) = self.filter.matches(suspect, extended=True)
+        match, info = self.filter.matches(suspect, extended=True)
         if match:
             delete = False
             field, matchedvalue, arg, regex = info
             if arg is not None and arg.lower() == 'no':
                 suspect.debug("Suspect matches imap copy exception rule")
                 self.logger.info(f"{suspect.id} Header {field} matches imap copy exception rule '{regex}'")
             else:
@@ -124,26 +125,28 @@
                     if suspect.get_tag('debug'):
                         suspect.debug("Suspect matches imap copy rule (I would copy it if we weren't in debug mode)")
                     else:
                         if ' ' not in arg:
                             if arg.upper() != 'DELETE':
                                 self.storeimap(suspect, arg)
                             else:
+                                self.logger.debug(f'{suspect.id} cannot store. arg={arg}')
                                 return DUNNO
                         else:
                             for value in arg.split():
                                 if value.upper() == 'DELETE':
                                     self.logger.info(f"{suspect.id} imap copy rule '{regex}' action DELETE")
                                     delete = True
                                     continue
                                 self.storeimap(suspect, value)
                     if delete:
                         return DELETE
         else:
-            suspect.debug(f"{suspect.id} No imap copy rule/exception rule applies to this message")
+            suspect.debug("No imap copy rule/exception rule applies to this message")
+            self.logger.debug(f"{suspect.id} No imap copy rule/exception rule applies to this message")
         return DUNNO
 
     def imapconnect(self, imapurl: str, lintmode: bool = False, fugluid='n/a'):
         p = urlparse(imapurl)
         scheme = p.scheme.lower()
         host = p.hostname
         port = p.port
@@ -232,26 +235,31 @@
         if self.config.getboolean(self.section, 'storeoriginal'):
             src = suspect.get_original_source()
         else:
             src = suspect.get_source()
 
         mtype, data = imap.append(folder, None, None, src)
         if mtype != 'OK':
-            self.logger.error(f'{suspect.id} Could put store in IMAP. APPEND command failed: {data}')
+            self.logger.error(f'{suspect.id} Could put store in IMAP {imapurl}. APPEND command failed: {data}')
+        else:
+            self.logger.debug(f'{suspect.id} stored in {imapurl} as {data}')
         imap.logout()
 
     def lint(self):
         allok = (self.check_config() and self.lint_imap())
         return allok
 
     def lint_imap(self):
         # read file, check for all imap accounts
         imapcopyrules = self.config.get(self.section, 'imapcopyrules')
         if imapcopyrules != '' and not os.path.exists(imapcopyrules):
-            print(f'Imap copy rules file does not exist : {imapcopyrules}')
+            print(f'ERROR: Imap copy rules file does not exist : {imapcopyrules}')
+            return False
+        elif not imapcopyrules:
+            print(f'ERROR: Imap copy rules file not defined')
             return False
         sfilter = SuspectFilter(imapcopyrules)
 
         accounts = []
         for tup in sfilter.get_list():
             headername, pattern, arg = tup
             if arg not in accounts:
@@ -506,15 +514,15 @@
                     return
             logger = getattr(self.logger, level)
             logger(logmessage)
         else:
             self.logger.error(logmessage)
 
     def _get_content(self, suspect: Suspect) -> bytes:
-        msg_buffer = suspect.get_original_source()
+        msg_buffer = suspect.get_source(newline=b'\r\n')
         # prepend header with original sender
         original_sender_header = self.config.get(self.section, 'original_sender_header')
         if original_sender_header:
             msg_buffer = Suspect.prepend_header_to_source(original_sender_header, suspect.from_address, msg_buffer)
         # prepend header with original recipient
         original_recipient_header = self.config.get(self.section, 'original_recipient_header')
         if original_recipient_header:
@@ -571,15 +579,15 @@
                 self._log_response(f'{suspect.id} sent quit to {target_host}', quit_resp, level=LOGLEVEL_EXTREME)
             except Exception as e:
                 self.logger.debug(f'{suspect.id} error sending quit to {target_host}: {e.__class__.__name__}: {str(e)}')
         except Exception as e:
             #self.logger.error('%s failed to forward to %s due to %s' % (suspect.id, target_host, str(e)))
             errcode = self._get_errcode_from_exc(e, to_address)
             if retry > 0 and not (500 < errcode < 599):
-                time.sleep((4-retry)/2)
+                time.sleep(abs(4-retry)/2)
                 fails = self._send_sync(suspect, target_host, target_args, from_address, to_address, retry=retry-1)
             else:
                 fails = {to_address: f'{e.__class__.__name__}: {str(e)}'}
         return fails
 
     @deprecated
     async def _send_async(self, suspect: Suspect, target_host: str, target_args: dict, from_address: str, to_address: str, retry: int = 3):
@@ -621,15 +629,15 @@
             except Exception as e:
                 self.logger.debug('%s error sending quit to %s: %s' % (suspect.id, target_host, str(e)))
         except Exception as e:
             import traceback
             self.logger.error('%s failed to forward to %s due to %s' % (suspect.id, target_host, str(e)))
             self.logger.error(traceback.format_exc())
             if retry > 0:
-                time.sleep((4-retry)/2)
+                time.sleep(abs(4-retry)/2)
                 fails = await self._send_async(suspect, target_host, target_args, from_address, to_address, retry=retry-1)
             else:
                 fails = {to_address: str(e)}
         return fails
 
     def _send_mail(self, target_host: str, target_args: dict, suspect: Suspect):
         exceptions = target_args.get('exc', [])
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/messagesize.py` & `fuglu-1.5.0/src/fuglu/plugins/messagesize.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/originpolicy.py` & `fuglu-1.5.0/src/fuglu/plugins/originpolicy.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/outpolicy.py` & `fuglu-1.5.0/src/fuglu/plugins/outpolicy.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,19 @@
 import socket
 import os
 import logging
 import threading
 import time
 import typing as tp
 from string import Template
-import random
 import re
 import datetime
 from email import message_from_bytes
-from fuglu.shared import strip_address, extract_domain, FileList, ScannerPlugin, DUNNO, apply_template, \
-    string_to_actioncode, actioncode_to_string, get_outgoing_helo
+from fuglu.shared import strip_address, extract_domain, FileList, ScannerPlugin, DUNNO, REJECT, \
+    apply_template, string_to_actioncode, actioncode_to_string, get_outgoing_helo
 from fuglu.bounce import Bounce
 from fuglu.stringencode import force_uString, force_bString
 from fuglu.extensions.sql import get_session, text, SQL_EXTENSION_ENABLED
 from fuglu.extensions.redisext import RedisPooledConn, redis, ENABLED as REDIS_ENABLED
 from fuglu.mshared import BMPRCPTMixin, BasicMilterPlugin
 from fuglu.lib.patchedemail import PatchedMessage
 import fuglu.connectors.asyncmilterconnector as asm
@@ -155,19 +154,19 @@
                     attempts = 0
                 except Exception as e:
                     try:
                         conn.close()
                     except Exception:
                         pass
                     if attempts:
-                        waitfor = random.random()
-                        self.logger.warning(f'Exception while reloading (retry in {waitfor}s): {str(e)}')
+                        waitfor = abs(4-attempts)/4
+                        self.logger.warning(f'Exception while reloading (retry in {waitfor}s): {e.__class__.__name__}: {str(e)}')
                         time.sleep(waitfor)
                     else:
-                        self.logger.error(f'Exception for {createPIDinfo()} while reloading: {str(e)}', exc_info=e)
+                        self.logger.error(f'Exception for {createPIDinfo()} while reloading: {e.__class__.__name__}: {str(e)}', exc_info=e)
             finally:
                 self.lock.release()
 
     def can_spoof(self, relay_account):
         value = self.spoofing_cache.get(relay_account)
         self.logger.debug(f'sasl_user: {relay_account} spoofing: {value}')
         return value
@@ -382,15 +381,15 @@
                 'description': 'list of mx hosts to which bounces will be disallowed (requires DNSData mx lookup on recipient)'
             },
             'rejectmessage': {
                 'default': '${to_domain} does not accept bounces',
                 'description': 'reject message template for policy violators'
             },
             'rejectmessage_mx': {
-                'default': '${to_domain}\'s MX {mx} does not accept bounces',
+                'default': '${to_domain}\'s MX ${mx} does not accept bounces',
                 'description': 'reject message template for policy violators due to uncooperative mx'
             },
             'state': {
                 'default': asm.RCPT,
                 'description': f'comma/space separated list states this plugin should be '
                                f'applied ({",".join(BasicMilterPlugin.ALL_STATES.keys())})'
             }
@@ -902,15 +901,15 @@
         else:
             self.logger.warning(f'{suspect.id} tried to block {suspect.from_address} but more than one record was updated in sql db')
             return False
 
     def _get_redis_conn(self, redis_url):
         if self.redis_pool.get(redis_url) is None:
             timeout = self.config.getint(self.section, 'redis_timeout', fallback=3)
-            self.redis_pool[redis_url] = RedisPooledConn(redis_url, timeout=timeout)
+            self.redis_pool[redis_url] = RedisPooledConn(redis_url, socket_timeout=timeout)
         redis_pool = self.redis_pool[redis_url]
         redisconn = redis_pool.get_conn()
         return redisconn
 
     def _block_sender_redis(self, suspect, culprit, message, redis_url):
         """
         call-ahead style redis backend
@@ -1156,16 +1155,17 @@
                         suspect.source_stripped_attachments(maxsize=maxsize), _class=PatchedMessage
                     )
                 else:
                     self.logger.debug('%s Fuzor: message too big (%u > %u), skipping' % (suspect.id, suspect.size, maxsize))
                     return DUNNO
             else:
                 msgrep = suspect.get_message_rep()
-
-            digest = FuzorDigest(msgrep).digest
+            
+            hash_algo = self.config.get(self.section, 'hash_algo')
+            digest = FuzorDigest(msgrep, hash_algo).digest
             if digest is None and self.config.getboolean(self.section, 'rate_limit_none_digest'):
                 digest = '00000000000000000000000000000000'
             self.logger.debug(f'{suspect.id} digest is {digest if digest else "<none>"}')
 
             if digest is not None:
                 try:
                     self._init_backend()
@@ -1458,7 +1458,75 @@
                     self.logger.error(msg)
 
         if queue_dom > maxqueue_dom * active_queue_factor or queue_user > maxqueue_user * active_queue_factor:
             self.logger.info(f'{sess.id} current queue for {from_domain} is {queue_dom} and {from_address} is {queue_user}')
             return sm.TEMPFAIL, 'sender queue limit exceeded - try again later'
 
         return sm.CONTINUE
+
+
+
+class ToCCLimit(ScannerPlugin):
+    """
+    Limit number of recipients in To and CC header
+    """
+
+    def __init__(self, config, section=None):
+        super().__init__(config, section)
+        self.logger = self._logger()
+        self.requiredvars = {
+            'max_to': {
+                'default': '0',
+                'description': 'maximum number of recipients in To: header. set to 0 for no limit.',
+            },
+            'max_cc': {
+                'default': '0',
+                'description': 'maximum number of recipients in CC: header. set to 0 for no limit.',
+            },
+            'max_rcpt': {
+                'default': '0',
+                'description': 'maximum number of recipients in To: and CC: headers combined. set to 0 for no limit.',
+            },
+            'rejectmessage': {
+                'default': 'maximum number of recipients in header ${header} exceeded (${count}>${max_hdr})',
+                'description': 'reject message template for policy violators'
+            },
+        }
+
+    def examine(self, suspect):
+        hdrs = {'to':0, 'cc':0}
+        
+        for hdr in hdrs:
+            value = suspect.parse_from_type_header(hdr)
+            option = f'max_{hdr}'
+            max_hdr = suspect.get_tag('filtersettings', {}).get(option, self.config.getint(self.section, option))
+            count = len(value)
+            hdrs[hdr] = count
+            if 0 < max_hdr < count:
+                valdict = {'header': hdr, 'count': count, 'max_hdr': max_hdr}
+                message = apply_template(self.config.get(self.section, 'rejectmessage'), suspect, valdict)
+                return REJECT, message
+        
+        total_rcpt = sum(hdrs.values())
+        max_rcpt = suspect.get_tag('filtersettings', {}).get('max_rcpt', self.config.getint(self.section, 'max_rcpt'))
+        if 0 < max_rcpt < total_rcpt:
+            valdict = {'header': ','.join(list(hdrs.keys())), 'count': total_rcpt, 'max_hdr': max_rcpt}
+            message = apply_template(self.config.get(self.section, 'rejectmessage'), suspect, valdict)
+            return REJECT, message
+        
+        countstr = ' '.join([f'{k}={v}' for k,v in hdrs.items()])
+        self.logger.debug(f'{suspect.id} header rcpt total={total_rcpt} {countstr}')
+        
+        return DUNNO, None
+    
+    
+    def lint(self):
+        values = []
+        for option in ['max_to', 'max_cc', 'max_rcpt']:
+            value = self.config.getint(self.section, option)
+            if value < 0:
+                print(f'ERROR: negative value {values} for option {option}')
+                return False
+            values.append(value)
+        if not any(values):
+            print(f'INFO: all config values are set to 0, this plugin will do nothing')
+        return True
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/p_blwl.py` & `fuglu-1.5.0/src/fuglu/plugins/p_blwl.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,22 +46,14 @@
         return value and '@' in value
     def email_normalise_ebl(value:str) -> str:
         return value.lower()
     def strip_batv(value:str) -> str:
         return value
     DOMAINMAGIC_AVAILABLE = False
 
-try:
-    import requests
-    requests.packages.urllib3.disable_warnings()
-    REQUESTS_AVAILABLE = True
-except ImportError:
-    REQUESTS_AVAILABLE = False
-
-
 class BlockWelcomeEntry(object):
     """
     Fuglu block/welcome listing basic object
     """
     TYPE_BLOCK = 'block'
     TYPE_WELCOME = 'welcome'
     SCOPE_ANY = 'any'
@@ -89,15 +81,15 @@
     def _is_wildcard(self, hostname):
         return hostname and self._is_hostname(hostname) and hostname.startswith('*')
 
     def __init__(self, **kw):
         for key in kw:
             if hasattr(self, key):
                 value = kw[key]
-                if key in ['netmask', 'hitcount']:
+                if key in ['netmask', 'hitcount', 'list_id']:
                     try:
                         value = int(value)
                     except (TypeError, ValueError):
                         pass  # well... best effort.
                 setattr(self, key, value)
 
     def __str__(self):
@@ -217,15 +209,18 @@
             if scope:
                 item = {self.key_map.get(k, k): v for k, v in item.items()}  # convert item keys from rest to sql naming
                 listing = BlockWelcomeEntry(**item)
                 try:
                     listings[scope].append(listing)
                 except KeyError:
                     listings[scope] = [listing]
-            
+        
+        for scope in listings:
+            listings[scope].sort()
+            listings[scope].reverse()
         return listings
     
 
 
 WELCOME = 0
 BLOCK = 1
 STAGE_PREPENDER = 'prepender'
@@ -398,14 +393,18 @@
             'default': 'False',
             'description': 'only check welcome listings with host specified against header (more secure)'
         },
         'fublwl_debug': {
             'default': 'False',
             'description': 'print debug output (extra verbose)',
         },
+        'fublwl_debug_rcpt': {
+            'default': '',
+            'description': 'print debug output (extra verbose) for recipients listed (comma separated list of emails or domains)',
+        },
     }
 
     def __init__(self, config, section):
         super().__init__(config, section)
         self.cache = get_default_cache()
         self.engine = 'FuBLWL'
         self.jsonfile = None
@@ -506,16 +505,15 @@
         listing_net = listing_host = None
         try:
             listing_net = ipaddress.ip_network(f'{listing.sender_host}/{listing.netmask}', False)
         except ValueError:
             listing_host = listing.sender_host.lower()
         return listing_net, listing_host
 
-    def _check_listings(self, check_listings, sender_address, sender_hostname, sender_hostip, listscope, suspectid: str = ""):
-        debug = self.config.getboolean(self.section, 'fublwl_debug')
+    def _check_listings(self, check_listings, sender_address, sender_hostname, sender_hostip, listscope, suspectid: str = "", debug:bool=False):
         if sender_address:
             sender_address = sender_address.lower()
             sender_domain = sender_address.rsplit('@', 1)[-1]
             sender_domain_pct = f'%{sender_domain}'
             sender_domain_dot = f'.{sender_domain}'
         else:
             sender_domain_pct = None
@@ -525,18 +523,18 @@
             sender_hostname = sender_hostname.lower()
             sender_hostname_dot = f'.{sender_hostname}'
         else:
             sender_hostname_dot = None
 
         if sender_hostip:
             sender_hostip = ipaddress.ip_network(sender_hostip, False)
-        self.logger.debug(f"{suspectid} sender_domain_pct={sender_domain_pct} sender_domain_dot={sender_domain_dot} sender_hostip={sender_hostip}")
+        self.logger.debug(f"{suspectid} sender_domain_pct={sender_domain_pct} sender_domain_dot={sender_domain_dot} sender_hostip={sender_hostip} listings={len(check_listings)}")
 
         for listing in check_listings:
-            #print(f"Check listing: list_scope:{listing.list_scope}, sender_addr:{listing.sender_addr}, sender_host:{listing.sender_host}, sender_netmask:{listing.netmask}")
+            debug and self.logger.debug(f"{suspectid} checking {listing}")
             if not listing.list_scope in (BlockWelcomeEntry.SCOPE_ANY, listscope):
                 debug and self.logger.debug(f"{suspectid} checking listing: {listing} "
                                             f"-> skip due to listscope {listing.list_scope} "
                                             f"not in scopes {BlockWelcomeEntry.SCOPE_ANY}, {listscope}")
                 continue
             if listing.sender_addr is None and listing.sender_host is None:  # would allow any sender from any host
                 debug and self.logger.debug(f"{suspectid} checking listing: {listing} "
@@ -591,36 +589,47 @@
         check_listings = []
         for scope in scopes:
             scope_listings = all_listings.get(scope, [])
             if scope_listings and not block_before_welcome:
                 scope_listings = sorted(scope_listings, key=attrgetter('list_type'), reverse=True)
             check_listings.extend(scope_listings)
         return check_listings
+    
+    def _do_debug(self, suspect):
+        debug = self.config.getboolean(self.section, 'fublwl_debug')
+        if not debug:
+            rcpts = self.config.getlist(self.section, 'fublwl_debug_rcpt', lower=True)
+            debug = suspect.to_address.lower() in rcpts or suspect.to_domain.lower() in rcpts
+        return debug
 
     def _check_user_listings(self,
                              suspect: Suspect,
                              all_listings: tp.Dict[str, tp.List[tp.Union[BlockWelcomeEntry, BlockWelcomeTable]]],
                              stage: str) -> tp.Tuple[tp.Union[BlockWelcomeEntry, BlockWelcomeTable], str]:
         eval_order = self._get_eval_order(suspect, self.config.getlist(self.section, 'fublwl_eval_order', lower=True), have_global=True)
         check_listings = self._sort_listings(suspect, all_listings, eval_order)
-
+        debug = self._do_debug(suspect)
+        if debug:
+            self.logger.debug(f"{suspect.id} stage={stage} debug output enabled for {suspect.to_address}")
+            self.logger.debug(f"{suspect.id} stage={stage} {check_listings}")
+        
         clientinfo = suspect.get_client_info(self.config)
         if clientinfo is not None:
             helo, clientip, clienthostname = clientinfo
         else:
             helo, clientip, clienthostname = None, None, None
 
         sender_address = suspect.from_address
         list_scope = BlockWelcomeEntry.SCOPE_ENV
         listing = None
 
         # check envelope sender in eoh stage only if no check was run in rcpt stage
         if stage in [asm.RCPT, STAGE_PREPENDER] or stage == asm.EOH and not asm.RCPT in suspect.get_tag('listing.stages', []):
             #self.logger.debug(f"{suspect.id} Check listings with: sender={sender_address}, clienthostname={clienthostname}, clientip={clientip}, list_scope={list_scope}, listings={check_listings}")
-            listing = self._check_listings(check_listings, sender_address, clienthostname, clientip, list_scope, suspect.id)
+            listing = self._check_listings(check_listings, sender_address, clienthostname, clientip, list_scope, suspect.id, debug)
             self.logger.debug(f"{suspect.id} stage={stage} Check listings returned: {listing} for list_scope {list_scope}")
             try:
                 suspect.tags['listing.stages'].append(stage)
             except KeyError:
                 suspect.tags['listing.stages'] = [stage]
         if not listing and stage in [asm.EOH, STAGE_PREPENDER]:
             header = None
@@ -628,15 +637,15 @@
             headers = self.config.getlist(self.section, 'fublwl_header_checks')
             if self.config.getboolean(self.section, 'fublwl_header_host_only'):
                 check_listings = [l for l in check_listings if l.sender_host or l.list_type == BlockWelcomeEntry.TYPE_BLOCK]
             for header in headers:
                 hdr_addresses = [item[1] for item in suspect.parse_from_type_header(header=header, validate_mail=True)]
                 self.logger.debug(f'{suspect.id} checking {len(check_listings)} listings against header {header} with addresses {",".join(hdr_addresses)}')
                 for sender_address in hdr_addresses:
-                    listing = self._check_listings(check_listings, sender_address, clienthostname, clientip, list_scope, suspect.id)
+                    listing = self._check_listings(check_listings, sender_address, clienthostname, clientip, list_scope, suspect.id, debug)
                     if listing:
                         break
                 if listing:
                     break
             self.logger.debug(f'{suspect.id} Check listings returned: {listing} for list_scope {list_scope} in header {header}')
         return listing, list_scope
 
@@ -725,17 +734,14 @@
             if err is not None:
                 errors.append((listing, err))
         return errors
 
     def lint(self):
         if not SQL_EXTENSION_ENABLED and self.config.get(self.section, 'fublwl_dbconnection'):
             print('WARNING: SQL extension not enabled but DB connection specified. This backend will not query SQLDB.')
-
-        if not REQUESTS_AVAILABLE and self.config.get('databaseconfig', 'restapi_uri'):
-            print('WARNING: requests library not found but REST API URI specified. REST API will not be queried.')
         
         json_file = self.config.get(self.section, 'fublwl_json_file')
         if json_file:
             if not os.path.exists(json_file):
                 print(f'ERROR: no such json file {json_file}')
                 return False
             else:
@@ -781,42 +787,47 @@
                     return False
             except Exception as e:
                 print(f'ERROR: failed to test listings due to {e.__class__.__name__}: {str(e)}')
                 return False
         return True
 
     def evaluate(self, suspect: Suspect, stage: str):
+        if suspect.is_welcomelisted() or suspect.is_blocklisted():
+            self.logger.debug(f'{suspect.id} Skip because already welcomelisted={suspect.is_welcomelisted()} blocklisted={suspect.is_blocklisted()}')
+            return
+        
         self._init_jsonfile()
         if not SQL_EXTENSION_ENABLED and not self.config.get(self.section, 'fublwl_restapi_endpoint') and not self.jsonfile:
             self.logger.debug(f"{suspect.id} Skip because SQL_EXTENSION is not enabled and fublwl_restapi is not set")
             return
 
         try:
             listings = self._get_listings(suspectid=suspect.id)
-            #self.logger.debug(f"{suspect.id} Start with {len(listings)} listings")
+            self.logger.debug(f"{suspect.id} Checking {len(listings)} listings for {suspect.to_address}")
         except RESTAPIError as e:
             suspect.set_tag('restapi.error', e)
             return
 
         listing, list_scope = self._check_user_listings(suspect, listings, stage)
-        self.logger.debug(f"{suspect.id} stage={stage} after applying user -> listing: {listing}, list_scope: {list_scope}")
+        self.logger.debug(f"{suspect.id} stage={stage} after applying {len(listings)} user listings -> listing: {listing}, list_scope: {list_scope}")
 
         if listing and listing.list_type == BlockWelcomeEntry.TYPE_BLOCK:
             self._add_tag(suspect, BLOCK)
         elif listing and listing.list_type == BlockWelcomeEntry.TYPE_WELCOME:
             self._add_tag(suspect, WELCOME)
             if listing.scope == GLOBALSCOPE:
                 self._set_global_tag(suspect)
             if list_scope == BlockWelcomeEntry.SCOPE_HDR:
                 suspect.set_tag('welcomelisted.header', True)
             elif list_scope == BlockWelcomeEntry.SCOPE_ENV and listing.sender_addr and listing.sender_host:
                 suspect.set_tag('welcomelisted.confirmed', True)  # confirmed listings have both envelope sender address and sender host set
         
-        if listing and self.config.getboolean(self.section, 'fublwl_update_hitcount'):
+        if listing and self.config.getboolean(self.section, 'fublwl_update_hitcount') and not suspect.get_tag(f'hitcount-{listing.list_id}'):
             self._update_hit_count(suspect, listing)
+            suspect.set_tag(f'hitcount-{listing.list_id}', True)
         #elif listing:
         #    self.logger.debug(f'{suspect.id} stage={stage} not updating hitcount for {listing.list_id}')
         
         if listing:
             suspect.set_tag('listing_id', listing.list_id)
             self.logger.info(f'{suspect.id} stage={stage} hits on listing {listing}')
         else:
@@ -1176,26 +1187,26 @@
                 break
         else:
             if recipients_welcome:
                 self.logger.debug(f'{suspect.id} no rcpt in {",".join(suspect.recipients)} is in recipients welcome list {",".join(recipients_welcome)}')
 
         senders_welcome = self.config.getlist(self.section, 'static_senders_welcome')
         if suspect.from_address in senders_welcome or suspect.from_domain in senders_welcome:
-            self.logger.info(f'{suspect.id} is welcome (sender={suspect.from_address})')
+            self.logger.info(f'{suspect.id} is welcome (sender={suspect.from_address or "<>"})')
             self._add_tag(suspect, WELCOME)
             self._set_global_tag(suspect)
         elif senders_welcome:
-            self.logger.debug(f'{suspect.id} {suspect.from_address} is not in senders welcome list {",".join(senders_welcome)}')
+            self.logger.debug(f'{suspect.id} {suspect.from_address or "<>"} is not in senders welcome list {",".join(senders_welcome)}')
 
         senders_blocked = self.config.getlist(self.section, 'static_senders_blocked')
         if suspect.from_address in senders_blocked or suspect.from_domain in senders_blocked:
             self.logger.info(f'{suspect.id} is blocked')
             self._add_tag(suspect, BLOCK)
         elif senders_blocked:
-            self.logger.debug(f'{suspect.id} {suspect.from_address} is not in senders blocked list {",".join(senders_blocked)}')
+            self.logger.debug(f'{suspect.id} {suspect.from_address or "<>"} is not in senders blocked list {",".join(senders_blocked)}')
 
     def lint(self):
         return True
 
 
 class AutoListMixin(object):
     config = None
@@ -1209,18 +1220,14 @@
             'default': str(7 * 24 * 3600),
             'description': 'TTL in seconds',
         },
         'al_redis_timeout': {
             'default': '2',
             'description': 'redis timeout in seconds'
         },
-        'al_redis_pinginterval': {
-            'default': '0',
-            'description': 'ping redis interval to prevent disconnect (0: don\'t ping)'
-        },
         'al_skip_headers': {
             'default': '',
             'description': 'list of headers which disable autolist if header is found',
         },
         'al_max_count': {
             'default': '1000',
             'description': 'do not increase counter beyond this value (for performance reasons)'
@@ -1271,16 +1278,15 @@
         """
         if self.backend_redis is not None:
             return
         redis_conn = self.config.get(self.section, 'al_redis_conn')
         if redis_conn:
             ttl = self.config.getint(self.section, 'al_redis_ttl')
             socket_timeout = self.config.getint(self.section, 'al_redis_timeout'),
-            pinginterval = self.config.getint(self.section, 'al_redis_pinginterval')
-            redis_pool = RedisPooledConn(redis_conn, socket_keepalive=True, socket_timeout=socket_timeout, pinginterval=pinginterval)
+            redis_pool = RedisPooledConn(redis_conn, socket_timeout=socket_timeout)
             maxcount = self.config.getint(self.section, 'al_max_count')
             self.backend_redis = ExpiringCounter(redis_pool, ttl, maxcount=maxcount)
 
     def _address_normalise(self, address: str) -> str:
         if DOMAINMAGIC_AVAILABLE and address:
             return strip_batv(email_normalise_ebl(force_uString(address)))
         else:
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/p_debug.py` & `fuglu-1.5.0/src/fuglu/plugins/p_debug.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/p_fraction.py` & `fuglu-1.5.0/src/fuglu/plugins/p_fraction.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/p_skipper.py` & `fuglu-1.5.0/src/fuglu/plugins/p_skipper.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/ratelimit/dynfunction.py` & `fuglu-1.5.0/src/fuglu/plugins/ratelimit/dynfunction.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 
 def bla(*args, **kwargs):
     print(f"Hello from bla...\n"
           f"args: {args}\n"
           f"kwargs: {kwargs}")
 
 
+FUNCMAP = {f.__name__:f for f in [toint, isint, bla]}
+
+
 findargs = re.compile(r"^[^\(]+\((?P<arguments>\S*)\)")
 findreturn = re.compile(r"\[([0-9]+)\]")
 findinteger = re.compile(r"^\(int\)(?P<integer>[0-9]+)$")
 findfloat = re.compile(r"^\(float\)(?P<float>[0-9\.]+)$")
 findbool = re.compile(r"^\(bool\)(?P<boolean>[TtrueFfals]+)$")
 findfunctionname = re.compile(r"^[\w.]+")
 
@@ -144,20 +147,17 @@
                 module = __import__(modname, fromlist=[funcname])
                 func = getattr(module, funcname)
             except Exception:
                 func = None
         else:
             funcname = funcname[0]
             try:
-                func = locals()[funcname]
+                func = FUNCMAP[funcname]
             except KeyError:
-                try:
-                    func = globals()[funcname]
-                except KeyError:
-                    fun = None
+                func = None
         if func is None:
             raise Exception(f"Couldn't find function {functionname}")
 
         self.func = func
 
     def _process_return(self, result):
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/ratelimit/helperfuncs.py` & `fuglu-1.5.0/src/fuglu/plugins/ratelimit/helperfuncs.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,29 +22,31 @@
 from domainmagic.validators import is_url_tldcheck
 from fuglu.extensions import dnsquery
 from fuglu.stringencode import force_uString
 from fuglu.shared import Suspect
 from fuglu.plugins.uriextract import EXCLUDE_DOMAIN, EXCLUDE_FQDN
 from fuglu.extensions.dnsquery import lookup, revlookup, FuNXDOMAIN, FuTIMEOUT, FuSERVFAIL, FuNoNameserver, FuNoAnswer
 from fuglu.connectors.asyncmilterconnector import MilterSession
+from fuglu.logtools import get_context_logger
 
 BE_VERBOSE = False  # for debugging
 
 
 def ip2network(ipstring: str, prefixlen: int = 32) -> str:
     """
     Take an ip string and the prefixlen to calculate the network string
     which can be used as a key in the RateLimitPlugin
     """
-    try:
-        network = ia.ip_network(f"{ipstring}/{prefixlen}", False).with_prefixlen
-    except ValueError as e:
-        logging.getLogger('fuglu.ratelimit.helperfuncs.ip2network').error(str(e))
-        network = ''
-    return network
+    with get_context_logger('fuglu.ratelimit.helperfuncs.ip2network') as logger:
+        try:
+            network = ia.ip_network(f"{ipstring}/{prefixlen}", False).with_prefixlen
+        except ValueError as e:
+            logger.error(str(e))
+            network = ''
+        return network
 
 
 # Singleton implementation for Domainmagic
 class DomainMagic(object):
     _instance = None
 
     @classmethod
@@ -55,58 +57,63 @@
 
     def __init__(self):
         self.tldmagic = tld.TLDMagic()
 
 
 def get_domain_from_uri(uri: str, suspect=None) -> tp.Optional[str]:
     """Extract domain from uri"""
-    exclude_fqdn = ['www.w3.org', 'schemas.microsoft.com']
-    exclude_domain = ['avast.com']
-
-    if not uri:
-        return None
 
     suspectid = suspect.id if suspect else '<>'
-    uri = uri.strip()
-    if uri.startswith("[") and uri.endswith("]"):
-        uri = uri.lstrip("[").rstrip("]")
-    try:
-        fqdn = extractor.domain_from_uri(uri)
-        if fqdn in exclude_fqdn:
+    with get_context_logger(f'fuglu.ratelimit.helperfuncs.get_domain_from_uri(id={suspectid})') as logger:
+        exclude_fqdn = ['www.w3.org', 'schemas.microsoft.com']
+        exclude_domain = ['avast.com']
+
+        if not uri:
             return None
-    except Exception as e:
-        # log error
-        logging.getLogger('fuglu.ratelimit.helperfuncs.get_domain_from_uri').error(f"{suspectid} msg: {str(e)} uri: {uri}")
-        return None
 
-    try:
-        domain = DomainMagic.instance().tldmagic.get_domain(fqdn)
-    except Exception as e:
-        # log error
-        logging.getLogger('fuglu.ratelimit.helperfuncs.get_domain_from_uri').error(f"{suspectid} msg: {str(e)} fqdn: {fqdn}")
-        return None
+        uri = uri.strip()
+        if uri.startswith("["):
+            if uri.endswith("]"):
+                uri = uri.lstrip("[").rstrip("]")
+            else: # broken items, would result in "Invalid IPv6 URL uri"
+                return None
+        try:
+            fqdn = extractor.domain_from_uri(uri)
+            if fqdn in exclude_fqdn:
+                return None
+        except Exception as e:
+            # log error
+            logger.error(f"{suspectid} msg: {e.__class__.__name__}: {str(e)} uri: {uri}")
+            return None
 
-    if domain in exclude_domain:
-        return None
-    return domain
+        try:
+            domain = DomainMagic.instance().tldmagic.get_domain(fqdn)
+        except Exception as e:
+            # log error
+            logger.error(f"{suspectid} msg: {e.__class__.__name__}: {str(e)} fqdn: {fqdn}")
+            return None
+
+        if domain in exclude_domain:
+            return None
+        return domain
 
 
 def split_helo2host_domain(helo: str, suspect=None):
     """Split helo to host, domain"""
-    domain = get_domain_from_uri(helo, suspect=suspect)
     suspectid = suspect.id if suspect else '<>'
-    if not domain:
-        return helo, ""
-    try:
-        hostname = helo.rsplit("."+domain, 1)[0]
-    except Exception as e:
-        logging.getLogger('fuglu.ratelimit.helperfuncs.split_helo2host')\
-            .error(f"{suspectid} msg: {str(e)} helo: {helo}, domain: {domain}")
-        hostname = ""
-    return hostname, domain
+    with get_context_logger(f'fuglu.ratelimit.helperfuncs.split_helo2host(id={suspectid})') as logger:
+        domain = get_domain_from_uri(helo, suspect=suspect)
+        if not domain:
+            return helo, ""
+        try:
+            hostname = helo.rsplit("."+domain, 1)[0]
+        except Exception as e:
+            logger.error(f"{suspectid} msg: {str(e)} helo: {helo}, domain: {domain}")
+            hostname = ""
+        return hostname, domain
 
 
 # Singleton implementation for GeoIP
 class GeoIP(object):
     _instances = {}
 
     @classmethod
@@ -138,70 +145,74 @@
 def asn(ipaddr: tp.Union[str, ipaddress.IPv4Address, ipaddress.IPv6Address], geoipfilename: str)\
         -> tp.Union[None, tp.Tuple[int, str, str, tp.Union[ipaddress.IPv4Network, ipaddress.IPv6Network]]]:
     """Extract ASN properties
 
     geoipfilename is geoip filename containing as ndata
     """
     from geoip2.errors import AddressNotFoundError
-    try:
-        response = GeoIP.instance(geoipfilename).reader.asn(ipaddr)
-    except AddressNotFoundError:
-        return None
-    except FileNotFoundError:
-        logging.getLogger('fuglu.ratelimit.helperfuncs.asn').error(f"failed to load {geoipfilename}")
-        return None
+    with get_context_logger('fuglu.ratelimit.helperfuncs.asn') as logger:
+        try:
+            response = GeoIP.instance(geoipfilename).reader.asn(ipaddr)
+        except AddressNotFoundError:
+            return None
+        except FileNotFoundError:
+            logger.error(f"failed to load {geoipfilename}")
+            return None
 
-    try:
-        response_network = response.network
-    except AttributeError:
-        # older geoip versions
-        response_network = None
-
-    return (
-        response.autonomous_system_number,
-        response.autonomous_system_organization,
-        response.ip_address,
-        response_network,
-    )
+        try:
+            response_network = response.network
+        except AttributeError:
+            # older geoip versions
+            response_network = None
+
+        return (
+            response.autonomous_system_number,
+            response.autonomous_system_organization,
+            response.ip_address,
+            response_network,
+        )
 
 
 def match_key_in_array(inputarray: tp.Optional[tp.List[str]], searchstring: str = "", suspect=None) -> tp.Optional[str]:
     """Search for string in array"""
-    if inputarray is None:
-        return None
-
     suspectid = suspect.id if suspect else '<>'
-    foundaddr = None
-    if inputarray and searchstring in inputarray:
-        foundaddr = searchstring
-
-    if BE_VERBOSE:
-        logging.getLogger('fuglu.ratelimit.helperfuncs.match_key_in_array') \
-            .debug(f"{suspectid} found {foundaddr} in {inputarray}")
+    with get_context_logger(f'fuglu.ratelimit.helperfuncs.match_key_in_array(id={suspectid})') as logger:
+        if inputarray is None:
+            return None
+
+        foundaddr = None
+        if inputarray and searchstring in inputarray:
+            foundaddr = searchstring
+
+        if BE_VERBOSE:
+            logger.debug(f"{suspectid} found {foundaddr} in {inputarray}")
 
-    # don't return an empty list, return None in this case
-    return foundaddr if foundaddr else None
+        # don't return an empty list, return None in this case
+        return foundaddr if foundaddr else None
 
 
 def valid_fqdn(urilist: tp.Optional[tp.List[str]], suspect=None) -> tp.Optional[tp.List[str]]:
     """Reduce uri list to fqdn's only"""
-    if urilist is None:
-        return None
     suspectid = suspect.id if suspect else '<>'
-    domains = set()
-    for url in urilist:
+    with get_context_logger(f'fuglu.ratelimit.helperfuncs.match_key_in_array(id={suspectid})') as logger:
+        if urilist is None:
+            return None
+        domains = set()
         try:
-            if url and is_url_tldcheck(url, exclude_fqdn=EXCLUDE_FQDN, exclude_domain=EXCLUDE_DOMAIN):
-                domains.add(extractor.fqdn_from_uri(url))
-        except Exception as e:
-            logging.getLogger('fuglu.ratelimit.helperfuncs.match_key_in_array')\
-                .error(f"{suspectid} (examine:fqdn_from_uri): {e} for uri: {url}")
-    domains = list(domains)
-    # don't return an empty list, return None in this case
-    return domains if domains else None
+            for url in urilist:
+                try:
+                    if url and is_url_tldcheck(url, exclude_fqdn=EXCLUDE_FQDN, exclude_domain=EXCLUDE_DOMAIN):
+                        domains.add(extractor.fqdn_from_uri(url))
+                except Exception as e:
+                    logger.error(f"{suspectid} (examine:fqdn_from_uri): {e} for uri: {url}")
+        except Exception:
+            logger.exception(e)
+        domains = list(domains)
+        # don't return an empty list, return None in this case
+        return domains if domains else None
 
 
 def convert_truefalse(input: tp.Optional[str], suspect=None) -> str:
     """Split helo to host, domain"""
     return str(bool(input))
 
 
@@ -214,32 +225,33 @@
         - in: a.b.c.d.com
           out: [d.com, c.d.com, b.c.d.com, a.b.c.d.com]
         - in: a.b.c.d.com (reverse=True)
           out: [a.b.c.d.com, b.c.d.com, c.d.com, d.com]
     """
 
     suspectid = suspect.id if suspect else '<>'
+    with get_context_logger(f'fuglu.ratelimit.helperfuncs.create_subdomain_list(id={suspectid})') as logger:
 
-    try:
-        tldcount = DomainMagic.instance().tldmagic.get_tld_count(domain)
-    except Exception as e:
-        # log error
-        logging.getLogger('fuglu.ratelimit.helperfuncs.create_subdomain_list').error(f"{suspectid} msg: {str(e)} domain: {domain}")
-        return None
+        try:
+            tldcount = DomainMagic.instance().tldmagic.get_tld_count(domain)
+        except Exception as e:
+            # log error
+            logger.error(f"{suspectid} msg: {str(e)} domain: {domain}")
+            return None
 
-    parts = domain.split('.')
+        parts = domain.split('.')
 
-    subrange = range(tldcount + 1, len(parts) + 1)
-    checkstrings = []
-    for subindex in subrange:
-        subdomain = '.'.join(parts[-subindex:])
-        checkstrings.append(subdomain)
-    if checkstrings and reverse:
-        checkstrings = checkstrings[::-1]
-    return checkstrings
+        subrange = range(tldcount + 1, len(parts) + 1)
+        checkstrings = []
+        for subindex in subrange:
+            subdomain = '.'.join(parts[-subindex:])
+            checkstrings.append(subdomain)
+        if checkstrings and reverse:
+            checkstrings = checkstrings[::-1]
+        return checkstrings
 
 
 def packargs(*args, **kwargs):
     """
     Small helper function if result should be packed
     This is required if output of the previous function is an array
     and it should be passed as an array into the next function, because
@@ -250,33 +262,35 @@
         return (args,)
     else:
         return None
 
 
 def get_nameservers(idomain: tp.Union[str, tp.List[str]], suspect=None) -> tp.Optional[tp.List[str]]:
     """For input domain/list of domains return first set of nameservers found"""
+
     suspectid = suspect.id if suspect else '<>'
-    if isinstance(idomain, str):
-        dlist = [idomain]
-    else:
-        dlist = idomain
+    with get_context_logger(f'fuglu.ratelimit.helperfuncs.create_subdomain_list(id={suspectid})') as logger:
 
-    # check if list is nonempty
-    if dlist and isinstance(dlist, (list, tuple)):
-        for dom in dlist:
-            try:
-                answers: tp.List[str] = dnsquery.lookup(dom, dnsquery.QTYPE_NS)
-                answers = [a.rstrip('.') for a in answers if a and a.rstrip('.')] if answers else []
-                if len(answers):
-                    return answers
-            except Exception as e:
-                logger = logging.getLogger('fuglu.ratelimit.helperfuncs.create_subdomain_list')
-                logger.error(f"{suspectid} got: {str(e)} querying ns for: {dom}")
+        if isinstance(idomain, str):
+            dlist = [idomain]
+        else:
+            dlist = idomain
 
-    return None
+        # check if list is nonempty
+        if dlist and isinstance(dlist, (list, tuple)):
+            for dom in dlist:
+                try:
+                    answers: tp.List[str] = dnsquery.lookup(dom, dnsquery.QTYPE_NS)
+                    answers = [a.rstrip('.') for a in answers if a and a.rstrip('.')] if answers else []
+                    if len(answers):
+                        return answers
+                except Exception as e:
+                    logger.error(f"{suspectid} got: {str(e)} querying ns for: {dom}")
+
+        return None
 
 
 def filter4left_tuple(tuplelist: tp.Union[tp.Tuple, tp.List],
                       filter: str,
                       lowercase: bool = True,
                       suspect=None) -> tp.Optional[tp.List[str]]:
     suspectid = suspect.id if suspect else '<>'
@@ -294,28 +308,27 @@
         return newlist
     else:
         return None
 
 
 def arraylength_largerthan(array: tp.List, maxlength=0, suspect=None) -> bool:
     suspectid = suspect.id if suspect else '<>'
-    islarger = len(array) > maxlength
-    if suspect:
-        # set tags so values can be used in reject message
-        try:
-            # note: these tags will be prefixed by "tag_" if used in the reject message,
-            # Example: "array length exceeded ${tag_arraylength} > ${tag_maxlength}"
-            suspect.tags["arraylength"] = len(array)
-            suspect.tags["maxlength"] = maxlength
-        except Exception as e:
-            logging.getLogger('fuglu.ratelimit.helperfuncs.arraylength_largerthan')\
-                .debug(f"Problem setting tags: {str(e)}")
-    logging.getLogger('fuglu.ratelimit.helperfuncs.arraylength_largerthan')\
-        .debug(f"{suspectid} arraylength: {len(array)} {'>' if islarger else '<='} {maxlength}")
-    return islarger
+    with get_context_logger(f'fuglu.ratelimit.helperfuncs.arraylength_largerthan(id={suspectid})') as logger:
+        islarger = len(array) > maxlength
+        if suspect:
+            # set tags so values can be used in reject message
+            try:
+                # note: these tags will be prefixed by "tag_" if used in the reject message,
+                # Example: "array length exceeded ${tag_arraylength} > ${tag_maxlength}"
+                suspect.tags["arraylength"] = len(array)
+                suspect.tags["maxlength"] = maxlength
+            except Exception as e:
+                logger.debug(f"Problem setting tags: {str(e)}")
+        logger.debug(f"{suspectid} arraylength: {len(array)} {'>' if islarger else '<='} {maxlength}")
+        return islarger
 
 
 def decode_from_type_headers(tuplelist: tp.Union[tp.Tuple, tp.List], name="From", suspect=None) -> tp.Optional[tp.List[str]]:
     suspectid = suspect.id if suspect else '<>'
     if isinstance(tuplelist, tuple):
         tuplelist = tuplelist[0]
 
@@ -344,140 +357,140 @@
         return None
 
 
 def select_element_by_index(iterable: tp.Union[tp.Tuple, tp.List],
                             index: int,
                             suspect=None) -> tp.Optional[tp.List[str]]:
     suspectid = suspect.id if suspect else '<>'
-    try:
-        return iterable[index]
-    except Exception as e:
-        logger = logging.getLogger(f'fuglu.helperfuncs.get_element_by_index(id={suspectid})')
-        logger.error(f"Can't select element {index} of iterable {iterable}: {str(e)}")
-    return None
+    with get_context_logger(f'fuglu.helperfuncs.get_element_by_index(id={suspectid})') as logger:
+        try:
+            return iterable[index]
+        except Exception as e:
+            logger.error(f"Can't select element {index} of iterable {iterable}: {str(e)}")
+        return None
 
 
 def domain_from_email(emaillist: tp.List[str], suspect=None) -> tp.Optional[tp.List[str]]:
     if emaillist:
         out = list(set([m.rsplit("@", 1)[1] for m in emaillist if m and "@" in m]))
         if out:
             return out
     return None
 
 
 def get_skip_ptr_unknown(ptr: str, suspect=None) -> tp.Optional[str]:
     suspectid = f"{suspect.id if suspect else '<>'}"
-    logger = logging.getLogger(f'fuglu.helperfuncs.get_skip_ptr(id={suspectid})')
-    if ptr and isinstance(ptr, str) and ptr.lower() == "unknown":
-        logger.debug(f"Return None because ptr is unknown")
-        return None
-    else:
-        return ptr
+    with get_context_logger(f'fuglu.helperfuncs.get_skip_ptr(id={suspectid})') as logger:
+        if ptr and isinstance(ptr, str) and ptr.lower() == "unknown":
+            logger.debug(f"Return None because ptr is unknown")
+            return None
+        else:
+            return ptr
 
 
 def get_ptr(ipaddress: str, suspect=None, verify: bool = False) -> tp.Optional[str]:
     """get ptr, return 'unknown' if none is found to match MilterSession implementation"""
     suspectid = f"{suspect.id if suspect else '<>'}"
-    logger = logging.getLogger(f'fuglu.helperfuncs.get_ptr(id={suspectid})')
+    with get_context_logger(f'fuglu.helperfuncs.get_ptr(id={suspectid})') as logger:
 
-    # first, try to get ptr from milter suspect
-    if suspect and isinstance(suspect, MilterSession):
-        # shortcut -> if ptr is known: return directly
-        if suspect.ptr and suspect.ptr != "unknown":
-            logger.debug(f"ptr={suspect.ptr} defined in miltersession: don't recalculate")
-            return suspect.ptr
-        elif suspect.ptr:
-            logger.debug(f"no valid ptr={suspect.ptr} defined in miltersession -> recalculate")
+        # first, try to get ptr from milter suspect
+        if suspect and isinstance(suspect, MilterSession):
+            # shortcut -> if ptr is known: return directly
+            if suspect.ptr and suspect.ptr != "unknown":
+                logger.debug(f"ptr={suspect.ptr} defined in miltersession: don't recalculate")
+                return suspect.ptr
+            elif suspect.ptr:
+                logger.debug(f"no valid ptr={suspect.ptr} defined in miltersession -> recalculate")
 
-    logger.debug(f"no ptr defined in miltersession: recalculate")
+        logger.debug(f"no ptr defined in miltersession: recalculate")
 
-    try:
-        answers: tp.List[str] = revlookup(ipaddress, reraise=True)
-        answers = [a.rstrip('.') for a in answers if a and a.rstrip('.')] if answers else []
-        if len(answers):
-            if answers[0] and verify:
-                fwd = lookup(answers[0])
-                if not fwd or not ipaddress in answers:
-                    return 'unknown'
-            logger.debug(f"no ptr defined in miltersession: recalculated as {answers[0]}")
-            return answers[0]
-    except FuNXDOMAIN:
-        logger.debug(f"return nxdomain as ptr for: {ipaddress}")
-        return 'nxdomain'
-    except (FuTIMEOUT, FuSERVFAIL, FuNoNameserver, FuNoAnswer) as e:
-        logger.debug(f"got: {e.__class__.__name__}: {str(e)} querying PTR for: {ipaddress}")
-    except Exception as e:
-        logger.error(f"got: {e.__class__.__name__}: {str(e)} querying PTR for: {ipaddress}")
-    logger.debug(f"no ptr defined in miltersession: return unknown")
-    return "unknown"
+        try:
+            answers: tp.List[str] = revlookup(ipaddress, reraise=True)
+            answers = [a.rstrip('.') for a in answers if a and a.rstrip('.')] if answers else []
+            if len(answers):
+                if answers[0] and verify:
+                    fwd = lookup(answers[0])
+                    if not fwd or not ipaddress in answers:
+                        return 'unknown'
+                logger.debug(f"no ptr defined in miltersession: recalculated as {answers[0]}")
+                return answers[0]
+        except FuNXDOMAIN:
+            logger.debug(f"return nxdomain as ptr for: {ipaddress}")
+            return 'nxdomain'
+        except (FuTIMEOUT, FuSERVFAIL, FuNoNameserver, FuNoAnswer) as e:
+            logger.debug(f"got: {e.__class__.__name__}: {str(e)} querying PTR for: {ipaddress}")
+        except Exception as e:
+            logger.error(f"got: {e.__class__.__name__}: {str(e)} querying PTR for: {ipaddress}")
+        logger.debug(f"no ptr defined in miltersession: return unknown")
+        return "unknown"
 
 
 def suspecttagsummary(inputdictstring: tp.Optional[tp.Dict[str, bool]], suspect=None):
-    try:
-        for key in list(inputdictstring.keys()):
-            val = inputdictstring[key]
-            if val:
-                return True
-    except Exception as e:
-        suspectid = f"{suspect.id if suspect else '<>'}"
-        logger = logging.getLogger(f'fuglu.helperfuncs.suspecttagsummary(id={suspectid})')
-        logger.error(f"({type(e)}) {str(e)}")
-        pass
-    return None
+    suspectid = f"{suspect.id if suspect else '<>'}"
+    with get_context_logger(f'fuglu.helperfuncs.suspecttagsummary(id={suspectid})') as logger:
+        try:
+            for key in list(inputdictstring.keys()):
+                val = inputdictstring[key]
+                if val:
+                    return True
+        except Exception as e:
+            logger.error(f"({type(e)}) {str(e)}")
+            pass
+        return None
 
 
 def sender_recipient_match(recipient: str, suspect: tp.Optional[MilterSession] = None) -> tp.Optional[str]:
     """Return email if recipient matches sender of suspect, None otherwise"""
     suspectid = f"{suspect.id if suspect else '<>'}"
-    logger = logging.getLogger(f'fuglu.helperfuncs.sender_recipient_match(id={suspectid})')
-    if not suspect:
-        logger.debug("no suspect -> return")
-        return None
-    sender = force_uString(suspect.sender, convert_none=True)
-    if not (sender and sender.strip()):
-        logger.debug(f"no sender({suspect.sender}) -> return")
-        return None
-    if not (recipient and recipient.strip()):
-        logger.debug(f"no recipient({recipient}) suspect.recipients=[{force_uString(suspect.recipients)}]-> return")
-        return None
-    sender_norm = sender.strip().lower()
-    recipient_norm = recipient.strip().lower()
-    if sender_norm == recipient_norm:
-        logger.debug(f"sender({sender_norm}) == recipient({recipient})")
-        return sender_norm
-    else:
-        logger.debug(f"sender({sender_norm}) != recipient({recipient}) -> return")
-        return None
+    with get_context_logger(f'fuglu.helperfuncs.sender_recipient_match(id={suspectid})') as logger:
+        if not suspect:
+            logger.debug("no suspect -> return")
+            return None
+        sender = force_uString(suspect.sender, convert_none=True)
+        if not (sender and sender.strip()):
+            logger.debug(f"no sender({suspect.sender}) -> return")
+            return None
+        if not (recipient and recipient.strip()):
+            logger.debug(f"no recipient({recipient}) suspect.recipients=[{force_uString(suspect.recipients)}]-> return")
+            return None
+        sender_norm = sender.strip().lower()
+        recipient_norm = recipient.strip().lower()
+        if sender_norm == recipient_norm:
+            logger.debug(f"sender({sender_norm}) == recipient({recipient})")
+            return sender_norm
+        else:
+            logger.debug(f"sender({sender_norm}) != recipient({recipient}) -> return")
+            return None
 
 
 def sender_recipient_domainkey(recipient: str, keys: str, suspect: tp.Optional[MilterSession] = None) -> tp.Optional[str]:
     """Return key if key is found in sender and recipient domain, None otherwise"""
     suspectid = f"{suspect.id if suspect else '<>'}"
-    logger = logging.getLogger(f'fuglu.helperfuncs.sender_recipient_domainkey(id={suspectid})')
-    if not suspect:
-        logger.debug("no suspect -> return")
-        return None
+    with get_context_logger(f'fuglu.helperfuncs.sender_recipient_domainkey(id={suspectid})') as logger:
+        if not suspect:
+            logger.debug("no suspect -> return")
+            return None
 
-    sender = force_uString(suspect.sender, convert_none=True)
-    if not (sender and sender.strip()):
-        logger.debug(f"no sender({suspect.sender}) -> return")
-        return None
-    if not (recipient and recipient.strip()):
-        logger.debug(f"no recipient({recipient}) suspect.recipients=[{force_uString(suspect.recipients)}]-> return")
-        return None
+        sender = force_uString(suspect.sender, convert_none=True)
+        if not (sender and sender.strip()):
+            logger.debug(f"no sender({suspect.sender}) -> return")
+            return None
+        if not (recipient and recipient.strip()):
+            logger.debug(f"no recipient({recipient}) suspect.recipients=[{force_uString(suspect.recipients)}]-> return")
+            return None
 
-    sender_norm = sender.strip().lower()
-    recipient_norm = recipient.strip().lower()
+        sender_norm = sender.strip().lower()
+        recipient_norm = recipient.strip().lower()
 
-    sender_domain = sender_norm.rsplit("@", maxsplit=1)[-1]
-    recipient_domain = recipient_norm.rsplit("@", maxsplit=1)[-1]
+        sender_domain = sender_norm.rsplit("@", maxsplit=1)[-1]
+        recipient_domain = recipient_norm.rsplit("@", maxsplit=1)[-1]
 
-    keys = keys.lstrip("'").lstrip('"').rstrip("'").rstrip('"')
-    keys = [k.strip().lower() for k in keys.split(";") if (k and k.strip())]
+        keys = keys.lstrip("'").lstrip('"').rstrip("'").rstrip('"')
+        keys = [k.strip().lower() for k in keys.split(";") if (k and k.strip())]
 
-    for key in keys:
-        if key in sender_domain and key in recipient_domain:
-            logger.debug(f"key {key} found in sender&recipient domain!")
-            return key
+        for key in keys:
+            if key in sender_domain and key in recipient_domain:
+                logger.debug(f"key {key} found in sender&recipient domain!")
+                return key
 
-    logger.debug(f"non keys found in sender & recipient domains...")
-    return None
+        logger.debug(f"non keys found in sender & recipient domains...")
+        return None
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/ratelimit/main.py` & `fuglu-1.5.0/src/fuglu/plugins/ratelimit/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -640,19 +640,19 @@
         self.logger.debug(f"Init done")
 
     @staticmethod
     def yamlfile2dict(filename: str) -> tp.Dict:
         """Read yml file, return dict"""
         if not os.path.exists(filename):
             raise OSError(f"File {filename} does not exist!")
-        with open(filename, 'r', encoding='utf-8') as f:
+        with open(filename, 'r', encoding='utf-8') as fp:
             try:
-                rawdict = yaml.full_load(f)
+                rawdict = yaml.full_load(fp)
             except AttributeError:
-                rawdict = yaml.load(f)
+                rawdict = yaml.safe_load(fp)
         return rawdict
 
     def load_limiters(self, catch_exceptions: bool = True) -> tp.OrderedDict[str, Limiter]:
         # load file to dict, setup Limiters
         limiterdict = OrderedDict()
         try:
             # several files can be given
@@ -680,15 +680,15 @@
                 newlimiter = Limiter(name=lname, setupdict=ldict)
 
                 # prefix extension
                 prefixdef = ldict.get("prefix")
                 if prefixdef:
                     pldict = copy.deepcopy(ldict)
                     pprefname, pnumber, pframe, pmessage, count, action = Limiter._parse_prefix(prefixdef)
-                    # modify the dict fore the prefixed version
+                    # modify the dict for the prefixed version
                     pname = f"{lname}-{pprefname}"
                     if 'key' in pldict:
                         pldict['key'] = f"{pldict['key']}-{pprefname}"
                     if pnumber is not None and pframe is not None:
                         pldict['rate'] = f"{pnumber}/{pframe}"
                     if pmessage:
                         pldict['message'] = pmessage
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/__init__.py` & `fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/always_hit.py` & `fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/always_hit.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/backendint.py` & `fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/backendint.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def __init__(self, backendconfig: str):
         self.logger = logging.getLogger(f"fuglu.plugins.{self.__class__.__name__}")
 
     def _fix_eventname(self, eventname) -> str:
         if not isinstance(eventname, str):
             eventname = str(eventname)
         if len(eventname) > 255:
-            eventname = md5(eventname.encode()).hexdigest()
+            eventname = md5(eventname.encode()).hexdigest() # nosemgrep CWE-327
         return eventname
 
     def check_allowed(self,
                       eventname: str,
                       limit: tp.Union[int, float],
                       timespan: tp.Union[int, float],
                       increment: int,
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/fixed_ratelimit.py` & `fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/fixed_ratelimit.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/sliding_log_ratelimit.py` & `fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/sliding_log_ratelimit.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # based on the ratelimit plugin in the postomaat project (https://gitlab.com/fumail/postomaat)
 # developed by @ledgr
 import time
 from collections import defaultdict
 from threading import Lock
 from fuglu.extensions.sql import SQL_EXTENSION_ENABLED, get_session, DeclarativeBase
 from .backendint import BackendInterface
-from fuglu.extensions.redisext import RedisPooledConn, ENABLED as REDIS_AVAILABLE, REDIS2
+from fuglu.extensions.redisext import RedisPooledConn, ENABLED as REDIS_AVAILABLE
 
 STRATEGY = 'sliding-log'
 BACKENDS = defaultdict(dict)
 
 __all__ = ['STRATEGY', 'BACKENDS']
 
 
@@ -99,18 +99,15 @@
             now = time.time()
             then = now-timespan
             if then is None:
                 then = int(time.time())
 
             redisconn = self.redis_pool.get_conn()
             pipe = redisconn.pipeline()
-            if REDIS2:
-                pipe.zadd(eventname, now, now)
-            else:
-                pipe.zadd(eventname, {now: now})
+            pipe.zadd(eventname, {now: now})
             pipe.zremrangebyscore(eventname, '-inf', then)
             pipe.zcard(eventname)
             return pipe.execute()[2]
 
         def check_allowed(self, eventname, limit, timespan, increment):
             eventname = self._fix_eventname(eventname)
             if increment != 1:
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/ratelimit/strategies/sliding_window_ratelimit.py` & `fuglu-1.5.0/src/fuglu/plugins/ratelimit/strategies/sliding_window_ratelimit.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 #
 # based on the ratelimit plugin in the postomaat project (https://gitlab.com/fumail/postomaat)
 # developed by @ledgr
 import time
 import math
 from collections import defaultdict
 from datetime import timedelta
-
 from .backendint import BackendInterface
-from fuglu.extensions.redisext import RedisPooledConn, ENABLED as REDIS_AVAILABLE, REDIS2
+from fuglu.extensions.redisext import RedisPooledConn, ENABLED as REDIS_AVAILABLE
 from fuglu.extensions.aioredisext import AIORedisBaseBackend
+from fuglu.stringencode import force_bString
+import typing as tp
 
 AIOREDIS_AVAILABLE = 0
 AIOREDIS_TIMEOUT = 3.0
 AIOEDIS_MAXATTEMPTS = 3
 try:
     import asyncio
     import redis.asyncio as aioredis
@@ -79,43 +80,34 @@
                 b'bucket0': 0,
                 b'bucket1': 0,
                 b'last_bucket': present_bucket,
                 b'bucket_start_ts': now
             }
             redisconn = self.redis_pool.get_conn()
             pipe = redisconn.pipeline()
-            if REDIS2:
-                pipe.hmset(eventname, event_data)
-            else:
-                pipe.hset(eventname, mapping=event_data)
+            pipe.hset(eventname, mapping=event_data)
             if isinstance(ttl, float):
                 ttl = timedelta(seconds=ttl)
             pipe.expire(eventname, ttl)
             pipe.execute()
 
-        def get_event(self, eventname):
+        def get_event(self, eventname) -> tp.Dict[bytes,bytes]:
             redisconn = self.redis_pool.get_conn()
             return redisconn.hgetall(eventname)
 
         def update(self, eventname, event_data):
             redisconn = self.redis_pool.get_conn()
-            if REDIS2:
-                redisconn.hmset(eventname, event_data)
-            else:
-                redisconn.hset(eventname, mapping=event_data)
+            redisconn.hset(eventname, mapping=event_data)
 
         def set_mitigate(self, eventname, retry_after, now):
             newval = float(now) + float(retry_after)
             print(f"Setting mitigate to: {newval}")
             redisconn = self.redis_pool.get_conn()
-            if REDIS2:
-                redisconn.hmset(eventname, b'mitigate', newval)
-            else:
-                #pipe.hset(eventname, mapping=event_data)
-                redisconn.hmset(eventname, mapping={b'mitigate': newval})
+            redisconn.hset(eventname, mapping={b'mitigate': newval})
+            #redisconn.hmset(eventname, mapping={b'mitigate': newval})
 
         def get_buckets(self, timespan, now):
             """get time buckets where counters are saved
             we have two buckets only, but this formula can generate multiple
             math.floor((time_now / measurement_timespan) / bucket_interval)
             """
             present_bucket = int(math.floor((now % (timespan * 2)) / timespan))
@@ -199,15 +191,15 @@
                     retry_after = -1
 
                 self.logger.debug(f"{eventname} set mitigate flag, retry_after={retry_after}"
                                   f"{', negative because increment < 0' if increment < 0 else ''}")
 
                 #self.set_mitigate(eventname, retry_after)
                 newval = float(now) + float(retry_after)
-                event[b'mitigate'] = newval
+                event[b'mitigate'] = force_bString(newval)
 
                 self.logger.debug(f"{eventname} set mitigate flag, retry_after={retry_after}")
                 self.update(eventname, event)
                 return False, count
 
             self.increment(event, inc=increment, present_bucket=present_bucket)
             self.update(eventname, event)
@@ -228,39 +220,51 @@
             event_data = {
                 b'mitigate': 0,
                 b'bucket0': 0,
                 b'bucket1': 0,
                 b'last_bucket': present_bucket,
                 b'bucket_start_ts': now
             }
+            if isinstance(ttl, timedelta):
+                ttl = ttl.total_seconds()
+            elif isinstance(ttl, float):
+                ttl = int(ttl)
             try:
-                await self.hmset(key=eventname, mapping=event_data)
+                await self.hset(key=eventname, mapping=event_data)
+                if ttl > 0:
+                    await self.expire(eventname, ttl)
                 success = True
             except Exception as e:
                 self.logger.exception(e)
             return success
 
-        async def get_event(self, eventname):
+        async def get_event(self, eventname) -> tp.Tuple[tp.Dict[bytes,bytes], bool]:
             event = None
             success = False
             try:
                 event = await self.hgetall(key=eventname)
                 success = True
             except Exception as e:
                 self.logger.exception(e)
             return event, success
-
-        async def update(self, eventname, event_data):
-            await self.hmset(key=eventname, mapping=event_data)
-
+        
+        async def update(self, eventname, event_data, ttl):
+            await self.hset(key=eventname, mapping=event_data)
+            if isinstance(ttl, timedelta):
+                ttl = ttl.total_seconds()
+            elif isinstance(ttl, float):
+                ttl = int(ttl)
+            if ttl > 0:
+                await self.expire(eventname, ttl)
+        
         async def set_mitigate(self, eventname, retry_after, now):
             newval = float(now) + float(retry_after)
             self.logger.debug(f"Setting mitigate to: {newval}")
             event_data = {b"mitigate": newval}
-            await self.hmset(key=eventname, mapping=event_data)
+            await self.hset(key=eventname, mapping=event_data)
 
         def get_buckets(self, timespan, now):
             """get time buckets where counters are saved
             we have two buckets only, but this formula can generate multiple
             math.floor((time_now / measurement_timespan) / bucket_interval)
             """
             present_bucket = int(math.floor((now % (timespan * 2)) / timespan))
@@ -352,19 +356,19 @@
                     retry_after = -1
 
                 self.logger.debug(f"{eventname} set mitigate flag, retry_after={retry_after}"
                                   f"{', negative because increment < 0' if increment < 0 else ''}")
                 #self.set_mitigate(eventname, retry_after)
                 newval = float(now) + float(retry_after)
 
-                event[b'mitigate'] = newval
+                event[b'mitigate'] = force_bString(newval)
 
                 self.logger.debug(f"{eventname} set mitigate flag, retry_after={retry_after}")
-                await self.update(eventname, event)
+                await self.update(eventname, event, timespan*3)
                 return False, count
 
             self.increment(event, inc=increment, present_bucket=present_bucket)
-            await self.update(eventname, event)
+            await self.update(eventname, event, timespan*3)
 
             return True, count
 
     BACKENDS[STRATEGY]['aioredis'] = AIORedisBackend
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/restrictions.py` & `fuglu-1.5.0/src/fuglu/plugins/restrictions.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,19 +531,19 @@
 
     @staticmethod
     def _load_yamlfile(filename: str) -> tp.Union[tp.Dict, tp.OrderedDict]:
         if not os.path.exists(filename):
             raise OSError(f"File {filename} does not exist!")
 
         # load yaml config file
-        with open(filename, 'r', encoding='utf-8') as f:
+        with open(filename, 'r', encoding='utf-8') as fp:
             try:
-                configdict = yaml.full_load(f)
+                configdict = yaml.full_load(fp)
             except AttributeError:
-                configdict = yaml.load(f)
+                configdict = yaml.safe_load(fp)
         return configdict
 
     def __init__(self, config, section=None):
         super().__init__(config, section)
         self.requiredvars = {
             'restrictionfile': {
                 'default': '${confdir}/accessrestrictions.yml',
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/rspamd.py` & `fuglu-1.5.0/src/fuglu/plugins/rspamd.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/sa.py` & `fuglu-1.5.0/src/fuglu/plugins/sa.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,19 @@
 
             'oversize_attach_suspect_tags': {
                 'default': '',
                 'description': "Suspect tags to attach as text part to message for scanning if message "
                                "has been stripped due to size",
             },
 
+            'original_sender_header': {
+                'default': '',
+                'description': 'use original sender from this header instead of suspect.from_address'
+            },
+
         }
         self.logger = self._logger()
 
     def __str__(self):
         return "SpamAssassin"
 
     def lint(self):
@@ -250,15 +255,15 @@
                 print('SPAMD socket error: %s' % str(e))
 
             time.sleep(retry_sleep)
         return False
 
     def _lint_spam(self):
         values = self.safilter_symbols(GTUBE, 'test', fid="<no-suspect>")
-        if len(values) != 3:
+        if values is None or len(values) != 3:
             print(f'Invalid SPAMD response to GTUBE: {values}')
             return False
 
         spamflag, score, rules = values
         if 'GTUBE' in rules:
             print("GTUBE Has been detected correctly")
             return True
@@ -404,15 +409,19 @@
             content = portheader + content
         except (TypeError, ValueError) as e:
             self.logger.error(f'{suspect.id} could not add incomingport header: {str(e)}')
 
         # add envelope sender information
         msgrep = suspect.get_message_rep()
         if not 'Return-Path' in msgrep.keys():
-            from_address = suspect.from_address or '<>'  # bounce address should be <>
+            original_sender_header = self.config.get(self.section, 'original_sender_header')
+            if original_sender_header and original_sender_header in msgrep:
+                from_address = msgrep[original_sender_header] or '<>'
+            else:
+                from_address = suspect.from_address or '<>'  # bounce address should be <>
             content = force_bString(f'Return-Path: {from_address}\r\n') + content
             self.logger.info(f'{suspect.id} Set temp Return-Path header as {from_address}')
         else:
             self.logger.debug(f'{suspect.id} Return-Path already set as {msgrep["Return-Path"]}')
 
         extralines = self._text_from_tags(suspect=suspect, stripped=stripped)
         if extralines:
@@ -630,15 +639,15 @@
             s = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
             s.settimeout(self.config.getint(self.section, 'timeout'))
             try:
                 s.connect(sock)
             except socket.error:
                 raise socket.error(f'Could not reach spamd using unix socket {sock}')
         else:
-            host = self.config.get(self.section, 'host')
+            host = self.config.get(self.section, 'host', resolve_env=True)
             port = self.config.getint(self.section, 'port')
             timeout = self.config.getfloat(self.section, 'timeout')
             try:
                 s = socket.create_connection((host, port), timeout)
             except socket.error:
                 raise socket.error(f'Could not reach spamd using network ({host}, {port})')
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/script.py` & `fuglu-1.5.0/src/fuglu/plugins/script.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/taction.py` & `fuglu-1.5.0/src/fuglu/plugins/taction.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/tlspolicy.py` & `fuglu-1.5.0/src/fuglu/plugins/tlspolicy.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/plugins/uriextract.py` & `fuglu-1.5.0/src/fuglu/plugins/uriextract.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,24 +37,50 @@
 from urllib import parse as urlparse
 
 try:
     from domainmagic.extractor import URIExtractor, fqdn_from_uri, redirect_from_url, ip_convert_base10
     from domainmagic.rbl import RBLLookup
     from domainmagic.tld import TLDMagic
     from domainmagic.mailaddr import domain_from_mail
-    from domainmagic.validators import is_url_tldcheck, is_ip, is_hostname, is_ipv4
+    from domainmagic.validators import is_url_tldcheck, is_ip, is_hostname, is_ipv4, is_email
     DOMAINMAGIC_AVAILABLE = True
 except ImportError:
     DOMAINMAGIC_AVAILABLE = False
+    def is_email(value):
+        return value and '@' in value
 
 if HAVE_BEAUTIFULSOUP:
     import bs4 as BeautifulSoup
 else:
     BeautifulSoup = None
 
+
+HAVE_OPENCV = HAVE_NUMPY = False
+try:
+    from PIL import Image
+    HAVE_PIL = True
+except ImportError:
+    HAVE_PIL = False
+    try:
+        import cv2
+        HAVE_OPENCV = True
+    except ImportError:
+        pass
+    try:
+        import numpy
+        HAVE_NUMPY = True
+    except ImportError:
+        pass
+try:
+    from pyzbar import pyzbar
+    HAVE_PYZBAR = True
+except ImportError:
+    HAVE_PYZBAR = False
+HAVE_QRCODE = ((HAVE_OPENCV and HAVE_NUMPY) or HAVE_PIL) and HAVE_PYZBAR
+
 try:
     import vobject
     from contextlib import redirect_stdout
 except ImportError:
     vobject = None
     redirect_stdout = None
 # remove invisible characters
@@ -141,15 +167,15 @@
             # some uris will be returned in truncated form. in such case we want both variants.
             for exturi in exturis:
                 if exturi in uri:
                     newuris.append(uri)
                     break
         return newuris
 
-    def _normalise_components(self, uri):
+    def _normalise_components(self, uri, lazyhostname: bool = False):
         # - remove whitespace characters (unless encoded)
         # - decode urlencoding
         # - convert idn to punycode
         # - fix invalid protocol prefixes (double prefix, too many slashes)
         # - drop invalid ipv6-lookalike URIs
         # - drop URIs with invalid netloc
         try:
@@ -157,48 +183,54 @@
             parts = slashre.split(uri)
             for i in range(0, min(len(parts), 3)):
                 parts[i] = wsre.sub('', parts[i])
             uri = '/'.join(parts)
 
             uri = multishlashre.sub('://', uri)
             uri = doublehttpre.sub(r'\g<prot>', uri)
+            addproto = False
+            if not '://' in uri:
+                addproto = True
+                uri = 'http://' + uri
             parsed_uri = urlparse.urlparse(uri)
             #netloc = re.sub(r'\s', '', parsed_uri.netloc)
             netloc = urlparse.unquote(parsed_uri.netloc).encode('idna').decode()
             netloc = netloc.rstrip('%').strip('.').strip()
-
             # we want a syntactically valid hostname or ip address
-            if not is_hostname(uri) and not is_hostname(netloc) and not is_ip(netloc.strip('[]')):
+            if not is_hostname(uri, lazyhostname=lazyhostname) and not is_hostname(netloc, lazyhostname=lazyhostname) and not is_ip(netloc.strip('[]')):
                 return None
 
             netloc = ip_convert_base10(netloc)
             new_uri = parsed_uri._replace(netloc=netloc)
             path = new_uri.path.strip()
             new_uri = new_uri._replace(path=path)
-            return new_uri.geturl()
+            uri = new_uri.geturl()
+            if addproto:
+                uri = uri[7:]
+            return uri
         except ValueError:
             # usually: Invalid IPv6 URL
             return None
 
     def _removeprefixes(self, val, prefixes):  # str.removeprefix was only added in py3.9
         if not hasattr(val, 'removeprefix'):
             for prefix in prefixes:
                 if val.startswith(prefix):
                     val = val[len(prefix):]
         else:
             for prefix in prefixes:
                 val = val.removeprefix(prefix)
         return val
 
-    def _quickfilter(self, uris):
+    def _quickfilter(self, uris, lazyhostname: bool = False):
         # - ignore mail addresses (mailto:)
         # - ignore internal references, phone numbers, javascript and html tags (#...)
         # - ignore incomplete template replacements typically starting with square brackets
         uris = [self._normalise_components(self._removeprefixes(u.strip().lstrip(
-            '*').strip('"').rstrip('-'), ['blob:', ': ', '3D"', '=3D"', '='])) for u in uris]
+            '*').strip('"').rstrip('-'), ['blob:', ': ', '3D"', '=3D"', '=']), lazyhostname=lazyhostname) for u in uris]
         uris = [u for u in uris if u and
                 not u.lower().startswith((
                     "mailto:", "cid:", "tel:", "fax:", "javascript:", '#', "file:", "[",
                     "x-apple-data-detectors:", "applewebdata:", "viber:", ))
                 ]
         uris = list(set(uris))
         return uris
@@ -219,14 +251,21 @@
         timeout = suspect.get_tag('filtersettings', {}).get(f'{self.__class__.__name__.lower()}_timeout', default_timeout)
         self.logger.debug(f'{suspect.id} setting timeout to {timeout} config default is {default_timeout}')
         if timeout and timeout > 0:
             # use section name as timeout tag
             suspect.stimeout_set_timer(self.section, timeout)
 
     def _get_usehacks(self):
+        """
+        Domain magic hacks - see bitmask in domainmagic/extractor.py
+
+        EX_HACKS_PROCURL = 0x01  # Search & extract URLs in URL parameters
+        EX_HACKS_IDNA = 0x02  # convert characters using "Internationalizing Domain Names in Applications"
+        EX_HACKS_LAZYHOSTNAME = 0x04  # Use lazy hostname regex in is_hostname allowing "_"
+        """
         try:
             usehacks = self.config.getint(self.section, 'usehacks')
         except Exception:
             usehacks = self.config.getboolean(self.section, 'usehacks')
             usehacks = 1 if usehacks else 0
         return usehacks
 
@@ -279,15 +318,15 @@
             uris.extend(parturis)
             if loguris:
                 self.logger.debug(f'{suspect.id} Found URIs in subject part: {parturis}')
 
         rediruris = self._get_redirected_uris(suspect, uris)
         if rediruris:
             uris.extend(rediruris)
-        uris = self._quickfilter(list(set(uris)))  # remove duplicates and obvious bogons
+        uris = self._quickfilter(list(set(uris)), lazyhostname=usehacks>2)  # remove duplicates and obvious bogons
 
         # get uris extracted from headers (stored in headers.uris tag)
         headeruris = self._get_header_uris(suspect=suspect)
         if headeruris and loguris:
             self.logger.info(f'{suspect.id} Extracted {len(headeruris)} uris from headers')
             self.logger.debug(f'{suspect.id} Extracted uris "{headeruris}" from headers')
 
@@ -708,14 +747,129 @@
         if self.config.getboolean(self.section, 'loguris'):
             self.logger.info(f'{suspect.id} Extracted emails: {", ".join(all_emails)}')
             self.logger.info(f'{suspect.id} Extracted emaildomains: {", ".join(all_emaildomains)}')
 
         return DUNNO
 
 
+class QRExtract(ScannerPlugin):
+    def __init__(self, config, section=None):
+        super().__init__(config, section)
+        self.logger = self._logger()
+        self.requiredvars = {
+            'check_tags': {
+                'default': '',
+                'description': 'also get image data from tags',
+            },
+            'maxsize': {
+                'default': str(512*1204), # 512kb
+                'description': 'maximum size of image file to check (in bytes)'
+            }
+        }
+    
+    
+    def _extract_qrcode(self, suspect:Suspect, imagedata:bytes, imagename:str) -> tp.List[str]:
+        content = []
+        try:
+            if HAVE_OPENCV:
+                nimg = numpy.frombuffer(imagedata, dtype=numpy.uint8)
+                cimg = cv2.imdecode(nimg, cv2.IMREAD_COLOR)
+                result = pyzbar.decode(cimg)
+                del cimg
+            elif HAVE_PIL:
+                with Image.open(io.BytesIO(imagedata)) as cimg:
+                    result = pyzbar.decode(cimg)
+            else:
+                result = [] # we should never get here
+            for item in result:
+                try:
+                    value = getattr(item, 'data')
+                    content.append(force_uString(value))
+                except AttributeError:
+                    pass
+        except Exception as e:
+            self.logger.warning(f'{suspect.id} failed to decode image {imagename} due to {e.__class__.__name__}: {str(e)}')
+        if content:
+            self.logger.debug(f'{suspect.id} image {imagename} is qr code with content {"".join(content)}')
+            suspect.set_tag('qrcode.attached', True)
+            suspect.write_sa_temp_header('X-QRCode', str(len(content)))
+        return content
+    
+    
+    def _linkcheck(self, data:tp.Iterable[str], uris:tp.Set[str], emails:tp.Set[str]) -> tp.Tuple[tp.Set[str], tp.Set[str]]:
+        for item in data:
+            if item.lower().startswith('mailto:'):
+                item = item[7:]
+                if is_email(item):
+                    emails.add(item)
+            elif item.lower().startswith('matmsg:'):
+                fields = item[7:].split(';')
+                for field in fields:
+                    try:
+                        k,v = field.split(':',1)
+                        if k.lower()=='to' and is_email(v):
+                            emails.add(v)
+                    except ValueError:
+                        if is_email(item):
+                            emails.add(item)
+            elif is_email(item):
+                emails.add(item)
+            elif item.lower().startswith('http'):
+                uris.add(item)
+            elif is_hostname(item):
+                uris.add(f'http://{item}/')
+        return uris, emails
+    
+    
+    def examine(self, suspect: Suspect) -> tp.Optional[tp.Union[int, tp.Tuple[int, str]]]:
+        if not HAVE_QRCODE:
+            return DUNNO
+        
+        maxsize = self.config.getint(self.section, 'maxsize')
+        uris = set()
+        emails = set()
+        for attobj in suspect.att_mgr.get_objectlist(level=0):
+            if attobj.contenttype.startswith('image/'):
+                if attobj.filesize < maxsize:
+                    data = self._extract_qrcode(suspect, attobj.buffer, attobj.filename)
+                    uris, emails = self._linkcheck(data, uris, emails)
+        for tagname in self.config.getlist(self.section, 'check_tags'):
+            images = suspect.get_tag(tagname, [])
+            for image in images:
+                if len(image) < maxsize:
+                    data = self._extract_qrcode(suspect, image, 'buffer')
+                    uris, emails = self._linkcheck(data, uris, emails)
+        
+        if uris:
+            suspect.set_tag('qrcode.uris', list(uris))
+        if emails:
+            suspect.set_tag('qrcode.emails', list(emails))
+        
+        return DUNNO
+    
+    def lint(self):
+        if not self.check_config():
+            return False
+        if not HAVE_PIL and (not HAVE_OPENCV and not HAVE_NUMPY):
+            print('ERROR: missing dependency PIL')
+            return False
+        if not HAVE_PIL and not HAVE_OPENCV:
+            print('ERROR: missing dependency opencv (cv2)')
+            return False
+        if not HAVE_PIL and not HAVE_NUMPY:
+            print('ERROR: missing dependency numpy')
+            return False
+        if not HAVE_PYZBAR:
+            print('ERROR: missing dependency pyzbar')
+            return False
+        if not DOMAINMAGIC_AVAILABLE:
+            print('WARNING: missing dependency domainmagic')
+        return True
+
+
 class DomainAction(ScannerPlugin):
     """Perform Action based on Domains in message body"""
 
     def __init__(self, config, section=None):
         super().__init__(config, section)
         self.logger = self._logger()
 
@@ -1051,18 +1205,21 @@
             for subindex in subrange:
                 subdomain = '.'.join(parts[-subindex:])
                 if subdomain in checked:
                     continue
                 
                 try:
                     listings = self.rbllookup.listings(subdomain, skip_rbldomains=skip_rbldomains)
-                    self.logger.debug(f'{suspect.id} URL host {domain} listed by {", ".join(list(listings.keys()))}')
+                    if listings:
+                        self.logger.debug(f'{suspect.id} URL host {subdomain} in {domain} listed by {", ".join(list(listings.keys()))}')
+                    else:
+                        self.logger.debug(f'{suspect.id} URL host {subdomain} in {domain} not listed')
                     for identifier, humanreadable in iter(listings.items()):
                         if identifier in welcomelists:
-                            self.logger.debug(f'{suspect.id} skipping lookup of {domain} (welcomelisted by {identifier})')
+                            self.logger.debug(f'{suspect.id} skipping lookup of {subdomain} in {domain} (welcomelisted by {identifier})')
                             break
                         hits[domain] = identifier
                         suspect.set_tag('uri.rbl.listed', True)
                         suspect.set_tag('uri.rbl.address', domain)
                         suspect.set_tag('uri.rbl.list', identifier)
                         suspect.set_tag('uri.rbl.info', humanreadable)
                         self.logger.info(f'{suspect.id} URL host {domain} flagged as {identifier} because {humanreadable}')
```

### Comparing `fuglu-1.4.0/src/fuglu/plugins/vacation.py` & `fuglu-1.5.0/src/fuglu/plugins/vacation.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 #
 #
 #
 """
 Vacation/Autoreply Plugin
 """
 
-from fuglu.shared import ScannerPlugin, DUNNO, utcnow
+from fuglu.shared import ScannerPlugin, DUNNO, utcnow, make_header
 from fuglu.bounce import Bounce
 from fuglu.extensions.sql import SQL_EXTENSION_ENABLED, get_session, DeclarativeBase
 import time
 import re
 from threading import Lock
 from datetime import timedelta
 import logging
 import traceback
 from email.mime.text import MIMEText
-from email.header import Header
 
 # from address regex
 vacation_ignoresenderregex = [
     "^owner-",
     "^request-",
     "-request@",
     # everything with 'bounce' in the lefthandside is
@@ -431,16 +430,15 @@
             except UnicodeError:
                 pass
             else:
                 break
 
         msg = MIMEText(body, 'plain', body_charset)
 
-        h = Header(vacation.subject, 'ISO-8859-1')
-        msg['Subject'] = h
+        msg['Subject'] = make_header('subject', vacation.subject)
         msg['Precedence'] = 'bulk'
         msg['Auto-Submitted'] = 'auto-replied'
         msg['From'] = suspect.to_address
         msg['To'] = suspect.from_address
 
         msgcontent = msg.as_string()
         queueid = bounce.send_template_string(
```

### Comparing `fuglu-1.4.0/src/fuglu/procpool.py` & `fuglu-1.5.0/src/fuglu/procpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,20 +101,20 @@
             handler_classname (str): class name of handler
             port (int): original incoming port
         """
         try:
             task = compress_task(sock, handler_modulename, handler_classname, port)
             self.add_task(task)
         except Exception as e:
-            self.logger.error("Exception happened trying to add task to queue: %s" % str(e))
+            self.logger.error(f"Exception happened trying to add task to queue: {e.__class__.__name__}: {str(e)}")
             self.logger.exception(e)
 
     def _create_worker(self):
         self._child_id_counter += 1
-        worker_name = "Worker-%s" % self._child_id_counter
+        worker_name = f'Worker-{self._child_id_counter}'
         worker = multiprocessing.Process(target=fuglu_process_worker, name=worker_name,
                                          args=(self.tasks, self.config, self.shared_state, self.child_to_server_messages, self._logQueue))
         return worker
 
     def start(self):
         for i in range(self.numprocs):
             worker = self._create_worker()
@@ -141,15 +141,15 @@
             countmessages = 0
             while True:
                 task = self.tasks.get()
                 if task is None:  # poison pill
                     break
                 newmanager.add_task(task)
                 countmessages += 1
-            self.logger.info("Moved %u messages to queue of new manager" % countmessages)
+            self.logger.info(f"Moved {countmessages} messages to queue of new manager")
         else:
             self.logger.debug("Get rid of items in queue")
             return_message = "Temporarily unavailable... Please try again later."
             mark_defer_counter = 0
             while True:
                 # Don't wait
                 try:
@@ -158,20 +158,20 @@
                     self.logger.warning("Queue is empty! Take a poison pill!")
                     task = None
                 if task is None:  # poison pill
                     self.logger.debug("Got poison pill")
                     break
                 self.logger.debug("Got task, mark as defer")
                 mark_defer_counter += 1
-                sock, handler_modulename, handler_classname = uncompress_task(task)
+                sock, handler_modulename, handler_classname, port = uncompress_task(task)
                 handler_class = getattr(importlib.import_module(handler_modulename), handler_classname)
                 handler_instance = handler_class(sock, self.config)
                 handler_instance.defer(return_message)
             if mark_defer_counter > 0:
-                self.logger.info("Marked %s messages as '%s' to close queue" % (mark_defer_counter, return_message))
+                self.logger.info(f"Marked {mark_defer_counter} messages as '{return_message}' to close queue")
 
         # join the workers
         try:
             join_timeout = self.config.getfloat('performance', 'join_timeout')
         except Exception:
             if newmanager:
                 join_timeout = 120.0
```

### Comparing `fuglu-1.4.0/src/fuglu/scansession.py` & `fuglu-1.5.0/src/fuglu/scansession.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
 
                     except KeyboardInterrupt:
                         sys.exit()
                     except Exception as e:
                         message_is_deferred = True
                         trb = traceback.format_exc()
                         self.logger.error(f'{suspect.id} Could not commit message. Error: {trb}')
-                        self.logger.exception(e)
+                        #self.logger.exception(e)
                         self._defer()
 
                 elif result == DELETE:
                     self.logger.info(f'MESSAGE DELETED: {suspect.id}')
                     retmesg = self.message or 'OK'
                     retmesg = self._gen_retmessage(suspect, retmesg)
                     self.protohandler.discard(retmesg)
```

### Comparing `fuglu-1.4.0/src/fuglu/shared.py` & `fuglu-1.5.0/src/fuglu/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 
 from string import Template
 from email.header import Header, decode_header
 import email.utils
 from email.mime.base import MIMEBase
 from email.mime.message import MIMEMessage
 from email.mime.text import MIMEText
+from email.headerregistry import HeaderRegistry, BaseHeader
+from email.policy import SMTP
 from collections.abc import Mapping
 from html.parser import HTMLParser
 from functools import wraps
 from io import StringIO
 
 from .addrcheck import Addrcheck
 from .stringencode import force_uString, force_bString
@@ -83,14 +85,39 @@
     'ACCEPT': ACCEPT,
     'DELETE': DELETE,
     'REJECT': REJECT,
     'DEFER': DEFER,
 }
 
 
+headerregistry = HeaderRegistry()
+
+def make_header(header: str, value: str) -> BaseHeader:
+    """returns a header object based on class determined by headerregistry"""
+    hdrclass = headerregistry[header]
+    hdr = hdrclass(header, value)
+    return hdr
+
+_re_crlfws = re.compile(r'\r\n(?![ \t])') # CRFL not followed by space or tab (multline header separator)
+_re_nocrlf = re.compile(r'(?<!\r)\n') # single LF, not after CR
+_re_crnolf = re.compile(r'\r(?!\n)') # single CR, not followed by LF
+def fold_header(header: str, value: str, policy=SMTP, value_only: bool = False) -> str:
+    """returns a correctly folded and encoded (multiline) header as string"""
+    hdr = make_header(header, value)
+    hdrval = hdr.fold(policy=policy).strip()
+    hdrval = _re_crlfws.sub('=?utf-8?q?=0D=0A?=', hdrval) # replace CRLF
+    hdrval = _re_nocrlf.sub('=?utf-8?q?=0A?=', hdrval) # replace single LF
+    hdrval = _re_crnolf.sub('=?utf-8?q?=0D?=', hdrval) # replace single CR
+    if value_only:
+        hdrval = hdrval.split(':',1)[-1].strip()
+    else:
+        hdrval += policy.linesep
+    return hdrval
+
+
 def actioncode_to_string(actioncode):
     """Return the human-readable string for this code"""
     for key, val in list(ALLCODES.items()):
         if val == actioncode:
             return key
     if actioncode is None:
         return "NULL ACTION CODE"
@@ -488,14 +515,15 @@
                     raise ValueError(f"Could not extract helo from environment var '{helo}'")
                 outhelo = env_helo
             elif helo:
                 outhelo = helo
 
         if outhelo is None:
             outhelo = HOSTNAME
+        outhelo = outhelo.lower() # lowercase as some servers (e.g. m365) don't like uppercase hostnames
         return outhelo
 
 
 def get_outgoing_helo(config=None):
     """Use singleton implementation to store outgoing helo"""
     return HeloSingleton.outgoinghelo(config=config)
 
@@ -552,29 +580,38 @@
         if tempfile:
             self.size = os.path.getsize(tempfile)
         elif inbuffer:
             self.size = len(self.inbuffer)
         else:
             self.size = None
         self.from_address = force_uString(from_address)
+        from_address_stripped = self.from_address.strip() if self.from_address else self.from_address
+        if from_address_stripped != self.from_address:
+            self.logger.info(f"{self.id} Stripped whitespaces from from_adress '{self.from_address}' -> '{from_address_stripped}'")
+            self.from_address = from_address_stripped
 
         # backwards compatibility, recipients can be a single address
         if isinstance(recipients, list):
-            self.recipients = [force_uString(rec) for rec in recipients]
+            recipientlist = [force_uString(rec) for rec in recipients]
         else:
-            self.recipients = [force_uString(recipients), ]
+            recipientlist = [force_uString(recipients), ]
 
         # basic email validitiy check - nothing more than necessary for our internal assumptions
-        for rec in self.recipients:
+        self.recipients = []
+        for rec in recipientlist:
             if rec is None:
                 self.logger.warning(f"{self.id} Recipient address can not be None")
                 raise ValueError("Recipient address can not be None")
             if not Addrcheck().valid(rec, allow_postmaster=True):
                 self.logger.warning(f"{self.id} Invalid recipient address: {rec}")
                 raise ValueError(f"Invalid recipient address: {rec}")
+            rec_stripped = rec.strip()
+            if rec_stripped != rec:
+                self.logger.info(f"{self.id} Stripped whitespaces from recipient '{rec}' -> '{rec_stripped}'")
+            self.recipients.append(rec_stripped)
 
         # additional basic information
         self.timestamp = kwargs.get("timestamp", time.time())
         self.timestamp_utc = kwargs.get("timestamp_utc", utcnow().timestamp())
 
         # headers which are prepended before re-injecting the message
         self.addheaders = {}
@@ -890,14 +927,15 @@
         """returns the tag value. if the tag is not found, return defaultvalue instead (None if no defaultvalue passed)"""
         if key not in self.tags:
             return defaultvalue
         return self.tags[key]
 
     def set_tag(self, key:str, value:tp.Any) -> None:
         """Set a new tag"""
+        self.logger.debug(f"{self.id} setting tag {key}:{value}")
         self.tags[key] = value
 
     def __tagsummary(self, tagname:str) -> bool:
         for key in list(self.tags[tagname].keys()):
             val = self.tags[tagname][key]
             if val:
                 return True
@@ -949,32 +987,31 @@
         :param cb_params: additional parameters to be passed to subject_cb
         :return: True if subject was altered, False otherwise
         """
         msgrep = self.get_message_rep()
         oldsubj = msgrep.get("subject", None)
 
         oldsubj_exists = True
-
         if oldsubj is None:
             oldsubj = ""
             oldsubj_exists = False
 
-        newsubj = subject_cb(oldsubj, **cb_params)
+        decsubj = self.decode_msg_header(oldsubj)
+        newsubj = subject_cb(decsubj, **cb_params)
         if oldsubj != newsubj:
-            del msgrep["subject"]
-            msgrep["subject"] = newsubj
+            foldsubj = fold_header('subject', newsubj, value_only=True)
+            self.remove_headers_from_source({'subject'}, track_change=False)  # don't track change because it would add an additional remove in milter-mode
+            self.set_source(Suspect.prepend_header_to_source('subject', foldsubj, self.get_source(), raw=True), att_mgr_reset=False)
 
             # store as modified header
             if oldsubj_exists:
                 self.modified_headers["subject"] = newsubj
             else:
                 self.added_headers["subject"] = newsubj
 
-            # no need to reset attachment manager because of a header change
-            self.set_message_rep(msgrep, att_mgr_reset=False)
             if self.get_tag('origsubj') is None:
                 self.set_tag('origsubj', oldsubj)
             return True
         return False
 
     def set_header(self, key:str, value:str) -> None:
         """
@@ -993,45 +1030,95 @@
 
         oldvalue = msg.get(key, None)
         self.logger.debug(f"{self.id} set_header -> modify '{key}' from '{oldvalue}' to {value}")
         if oldvalue is not None:
             if force_uString(oldvalue) == value:
                 self.logger.debug(f"{self.id} set_header -> modify '{key}' unnecessary since oldvalue == newvalue")
                 return
-            del msg[key]
+            self.remove_headers_from_source({key}, track_change=False)  # don't track change because it would add an additional remove in milter mode
             self.modified_headers[key] = value
-            msg[key] = value
-            self.set_message_rep(msg, att_mgr_reset=False)
+            self.set_source(Suspect.prepend_header_to_source(key, value, self.get_source()), att_mgr_reset=False)
         else:
             self.logger.debug(f"{self.id} set_header -> add instead of modify '{key}' with '{oldvalue}' because header doesn't exist yet")
             self.add_header(key, value, immediate=True)
             
 
-    def remove_headers(self, key:str) -> None:
+    def remove_headers(self, key:str) -> bool:
         """
         Remove existing header(s) with given name
 
         Args:
             key (string): header key
 
         """
         msg = self.get_message_rep()
 
         # convert inputs if needed
         key = force_uString(key)
-
+        
+        removed = False
         oldvalues = msg.get_all(key, [])
         if oldvalues:
             del msg[key]
             self.logger.debug(f"{self.id} remove_headers -> remove headers '{key}' with '{oldvalues}'")
             if self.removed_headers.get(key):
                 self.removed_headers[key].extend(oldvalues)
             else:
                 self.removed_headers[key] = oldvalues
             self.set_message_rep(msg, att_mgr_reset=False)
+            removed = True
+        return removed
+    
+    
+    def remove_headers_from_source(self, headernames:tp.Iterable[str], track_change: bool = True) -> bool:
+        """
+        removes headers without changing body code e.g. by dumping source from msg rep
+        :param headernames: List of header names to remove
+        :param track_change: Track changes (to be applied in milter mode later on)
+        :return: True if anything was removed, False if no change in source
+        """
+        deleted = False
+        msgrep = self.get_message_rep()
+        delhdrs = {h.lower() for h in msgrep.keys()} & {h.lower() for h in headernames} # intersect sets
+        if delhdrs:
+            delhdrs = tuple({h.encode()+b':' for h in delhdrs})
+            source = self.get_source()
+            lines = source.splitlines(True) # preserve line endings
+            newlines = []
+            in_hdr = True
+            hdrname = b''
+            for line in lines:
+                if not line.strip(): # empty line indicates end of headers
+                    in_hdr = False
+                if in_hdr and (line.lower().startswith(delhdrs) or hdrname and line.startswith((b' ', b'\t'))): # skip header
+                    self.logger.debug(f'{self.id} delete header line {line}')
+                    deleted = True
+                    try:
+                        if not line.startswith((b' ', b'\t')):
+                            hdrname, value = line.split(b':',1)
+                            hdrname = hdrname.decode()
+                            value = value.decode()
+                            if track_change:
+                                try:
+                                    self.removed_headers[hdrname].append(value)
+                                except KeyError:
+                                    self.removed_headers[hdrname] = [value]
+                        else:
+                            value = line.decode()
+                            if track_change:
+                                self.removed_headers[hdrname][-1] += value
+                    except Exception as e:
+                        self.logger.warning(f'{self.id} failed to update removed_headers with {line} due to {e.__class__.__name__}: {str(e)}')
+                else: # keep line
+                    hdrname = b''
+                    newlines.append(line)
+            if deleted:
+                self.set_source(b''.join(newlines))
+        return deleted
+    
 
     @staticmethod
     def decode_msg_header(header: tp.Union[str, bytes, email.header.Header], decode_errors:str="replace") -> str:
         """
         Decode message header from email.message into unicode string
 
         Args:
@@ -1049,44 +1136,39 @@
             header_unicode = force_uString(header)
             headerstring = ''.join([force_uString(x[0], encodingGuess=x[1], errors=decode_errors) for x in decode_header(header_unicode)])
         except Exception:
             headerstring = header
         return force_uString(headerstring)
 
     @staticmethod
-    def prepend_header_to_source(key:tp.Union[str,bytes], value:tp.Union[str,bytes], source:bytes) -> bytes:
+    def prepend_header_to_source(key:tp.Union[str,bytes], value:tp.Union[str,bytes], source:bytes, raw: bool = False) -> bytes:
         """
         Prepend a header to the message
 
         Args:
             key (str): the header key
             value (str): the header value
             source (bytes): the message source
+            raw (bool): Just add header raw as 'key: value\r\n', caller is responsible for correct formatting
 
         Returns:
             bytes: the new message buffer
 
         """
 
         b_source = force_bString(source)
 
         # convert inputs if needed
-        u_key = force_uString(key)
-        u_value = force_uString(value)
-
-        # is "ignore" the right thing to do here?
-        # (moved from add_header) routine
-        try:
-            hdr = Header(u_value, header_name=u_key, continuation_ws=' ')
-        except (UnicodeDecodeError, UnicodeEncodeError):
-            b_value = force_bString(value)
-            hdr = Header(b_value, charset='utf-8', header_name=u_key, continuation_ws=' ')
-
-        hdrline = f'{u_key}: {hdr.encode()}\r\n'
-        src = force_bString(hdrline) + b_source
+        u_key = force_uString(key).strip()
+        u_value = force_uString(value).strip()
+        if raw:
+            hdr = f"{u_key}: {u_value}\r\n"
+        else:
+            hdr = fold_header(u_key, u_value)
+        src = force_bString(hdr) + b_source
         return src
 
     @staticmethod
     def getlist_space_comma_separated(inputstring:str) -> tp.List[str]:
         """Create list from string, splitting at ',' space"""
         BACKSLASH = '{BACKSLASH}'
         SPACE = '{SPACE}'
@@ -1267,30 +1349,34 @@
                 else:
                     self.logger.info(f'{self.id} Mail "{mailaddress}" is not valid, display name is "{displayname}"')
         else:
             from_addresses = from_addresses_decoded
         self._cache_from_type_headers[cachekey] = from_addresses
         return from_addresses
 
-    def add_header(self, key:str, value:str, immediate:bool=False) -> None:
+    def add_header(self, key:str, value:str, immediate:bool=False, raw: bool = False) -> None:
         """adds a header to the message. by default, headers will be added when re-injecting the message back to postfix
         if you set immediate=True the message source will be replaced immediately. Only set this to true if a header must be
         visible to later plugins (e.g. for spamassassin rules), otherwise, leave as False which is faster.
+
+        raw: Just add header raw as 'key: value\r\n', caller is responsible for correct formatting, only available if immediate is True
         """
 
         # convert inputs if needed
         key = force_uString(key)
         value = force_uString(value)
 
         if immediate:
             # no need to reset the attachment manager when just adding a header
-            self.set_source(Suspect.prepend_header_to_source(key, value, self.get_source()), att_mgr_reset=False)
+            self.set_source(Suspect.prepend_header_to_source(key, value, self.get_source(), raw=raw), att_mgr_reset=False)
             # keep track of headers already added
             self.added_headers[key] = value
         else:
+            if raw:
+                self.logger.warning(f"{self.id} (add_header) raw option is only available if immediate is True -> ignoring")
             self.addheaders[key] = value
 
     @deprecated
     def addheader(self, key, value, immediate=False):
         """old name for add_header"""
         return self.add_header(key, value, immediate)
 
@@ -1384,25 +1470,26 @@
         return msgrep
 
     @deprecated
     def getMessageRep(self):
         """old name for get_message_rep"""
         return self.get_message_rep()
 
-    def set_message_rep(self, msgrep:PatchedMessage, att_mgr_reset:bool=True) -> None:
+    def set_message_rep(self, msgrep: PatchedMessage, att_mgr_reset: bool = True) -> None:
         """replace the message content. this must be a standard python email representation
         Warning: setting the source via python email representation seems to break dkim signatures!
 
         The attachment manager is build based on the python mail representation. If no message
         attachments or content is modified there is no need to recreate the attachment manager.
 
         Args:
             msgrep (email): standard python email representation
             att_mgr_reset (bool): Reset the attachment manager
         """
+        self.logger.debug(f'{self.id} setting new message rep')
         try:
             self.set_source(msgrep.as_bytes(), att_mgr_reset=att_mgr_reset)
         except AttributeError:
             self.set_source(force_bString(msgrep.as_string()), att_mgr_reset=att_mgr_reset)
 
         # order is important, set_source sets _msgrep to None
         self._msgrep = msgrep
@@ -1412,20 +1499,23 @@
         """old name for set_message_rep"""
         return self.set_message_rep(msgrep)
 
     def is_modified(self) -> bool:
         """returns true if the message source has been modified"""
         return self.source is not None
 
-    def get_source(self, maxbytes:int=None) -> bytes:
+    def get_source(self, maxbytes:int=None, newline:tp.Optional[bytes]=None) -> bytes:
         """returns the current message source, possibly changed by plugins"""
         if self.source is not None:
-            return self.source[:maxbytes]
+            source = self.source[:maxbytes]
         else:
-            return self.get_original_source(maxbytes)
+            source = self.get_original_source(maxbytes)
+        if isinstance(newline, bytes):
+            source = source.replace(b'\r', b'').replace(b'\n', newline)
+        return source
 
     @deprecated
     def getSource(self, maxbytes=None):
         """old name for get_source"""
         return self.get_source(maxbytes)
 
     def set_source(self, source:tp.Union[bytes,str], encoding:str='utf-8', att_mgr_reset:bool=True) -> None:
@@ -1458,14 +1548,16 @@
             if self._tempfile:
                 if self.tempfile == "/dev/null":
                     # don't try to read from /dev/null
                     return b""
                 else:
                     with open(self.tempfile, 'rb') as fh:
                         source = fh.read(readbytes)
+                        #lines = fh.read(readbytes).splitlines(False)
+                        #source = b'\r\n'.join(lines)
             else:
                 source = bytes(self.inbuffer)
                 if readbytes > 0:
                     source = source[:readbytes]
         except Exception as e:
             self.logger.error(f'{self.id} Cannot retrieve original source from tempfile {self.tempfilename()} due to {e.__class__.__name__}: {str(e)}')
             raise e
@@ -1492,15 +1584,15 @@
             # set from Python message, this might modify (base64-encode)
             # subparts of the attached message
             p = MIMEMessage(self.get_message_rep())
             self.logger.debug(f"{self.id} -> Failed to attach as MIMEBase, use MIMEMessage")
         p.add_header('Content-Disposition', f"attachment; filename={filename}")
         return p
 
-    def wrap(self, sender:str, recipient:str, subject:str, body:tp.Optional[str]=None, filename:tp.Optional[str]=None, config:FuConfigParser=tp.Optional[None], hdr_autosub:tp.Optional[str]='auto-generated', hdr_arsupp:tp.Optional[str]='DR, RN, NRN, OOF, AutoReply') -> PatchedMIMEMultipart:
+    def wrap(self, sender:str, recipient:str, subject:str, body:tp.Optional[str]=None, filename:tp.Optional[str]=None, config:tp.Optional[FuConfigParser]=None, hdr_autosub:tp.Optional[str]='auto-generated', hdr_arsupp:tp.Optional[str]='DR, RN, NRN, OOF, AutoReply') -> PatchedMIMEMultipart:
         """
         attach original source to a new multipart email
         https://www.geeksforgeeks.org/send-mail-attachment-gmail-account-using-python/
         :param sender: wrapper From header address
         :param recipient: wrapper To header address
         :param subject: wrapper Subject header
         :param body: additional wrapper body, leave empty to omit
@@ -1527,27 +1619,27 @@
         msg.attach(p)
         return msg
 
     _re_newlines = re.compile(rb'(?:\n\n|\r\n\r\n)')
 
     def get_headers(self) -> str:
         """
-        Returns the message headers as string
+        Returns the message headers as string type
         :return: string of all headers
         """
         headers = self._re_newlines.split(self.get_source(maxbytes=1048576), 1)[0]
         return force_uString(headers)
     
     
     def get_header(self, headername:str, fallback:tp.Optional[str]=None, use_cache:bool=True) -> tp.Optional[str]:
         """
         Returns content of header. value is cached for fast repeated lookups of header.
         :param headername: name of header
         :param fallback: fallback value in case header is not present, defaults to None
-        :param use_cache: set False to get current value. Will update cache with the latest value
+        :param use_cache: set False to get current value. Will update cache with the latest value.
         :return: value of header or fallback value if header not present
         """
         headername = headername.lower()
         if use_cache:
             value = self._header_cache.get(headername)
             if value is not None:
                 return value
@@ -2334,15 +2426,16 @@
                 self.logger.debug(f'while reading {self.filename}: {e.__class__.__name__}: {str(e)}')
                 time.sleep(0.1)
                 lines = self._reload(retry=retry-1)
             else:
                 self.logger.error(f'while reading {self.filename}: {e.__class__.__name__}: {str(e)}')
                 raise
         except Exception as e:
-            self.logger.error(f'while reading {self.filename}: {e.__class__.__name__}: {str(e)}')
+            perm = oct(statinfo.st_mode)[-3:]
+            self.logger.error(f'while reading {self.filename} with uid={statinfo.st_uid} and perm={perm}: {e.__class__.__name__}: {str(e)}')
             raise
         return lines
 
     def _apply_linefilters(self, line):
         for func in self.linefilters:
             line = func(line)
             if line is None:
@@ -2438,15 +2531,15 @@
                 pattern = re.compile(sp[1], re.IGNORECASE | re.DOTALL)
             except Exception as e:
                 raise Exception(f'Could not compile regex {sp[1]} in file {self.filename} ({e.__class__.__name__}: {str(e)})')
 
         tup = (fieldname, pattern, args)
         return tup
 
-    _re_line = re.compile(r"""(?P<fieldname>[a-zA-Z0-9\-._:]+):?\s+/(?P<regex>(?:\\.|[^/\\])*)/(?P<flags>[IiMm]+)?((?:\s*$)|(?:\s+(?P<args>.*)))$""")
+    _re_line = re.compile(r"""(?P<fieldname>@?[a-zA-Z0-9\-._:]+):?\s+/(?P<regex>(?:\\.|[^/\\])*)/(?P<flags>[IiMm]+)?((?:\s*$)|(?:\s+(?P<args>.*)))$""")
 
     def _load_perlstyle_line(self, line):
         m = self._re_line.match(line)
         if m is None:
             return None
 
         regex = m['regex']
@@ -2757,15 +2850,15 @@
         else:
             valuelist = payload.get_all(headername, [])
 
         return valuelist
 
     def _numcmp(self, op, cmp, strval):
         """
-        compare two numbers using operator function
+        compare two numbers using given operator function.
         :param op: operator function lt, le, eq, ne, ge, gt
         :param cmp: numeric comparison value
         :param strval: string numeric comparison value
         :return: boolean: True if comparison matches, False if strval is not numeric or comparison is no match
         """
         if isinstance(cmp, float):
             try:
```

### Comparing `fuglu-1.4.0/src/fuglu/stats.py` & `fuglu-1.5.0/src/fuglu/stats.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/stringencode.py` & `fuglu-1.5.0/src/fuglu/stringencode.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/threadpool.py` & `fuglu-1.5.0/src/fuglu/threadpool.py`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/fuglu/utils/version.py` & `fuglu-1.5.0/src/fuglu/utils/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #
 #
 import datetime
 import os
-import subprocess
+import subprocess # nosemgrep CWE-78
 
 
 VERSION_ALPHA = 'alpha'
 VERSION_BETA = 'beta'
 VERSION_RC = 'rc'
 VERSION_FINAL = 'final'
 
@@ -123,17 +123,16 @@
     The result is the UTC timestamp of the changeset in YYYYMMDDHHMMSS format.
     This value isn't guaranteed to be unique, but collisions are very unlikely,
     so it's sufficient for generating the development version numbers.
     """
     repo_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
     try:
         timestamp = subprocess.check_output(
-            'git log --pretty=format:%ct --quiet -1 HEAD',
-            shell=True, cwd=repo_dir, universal_newlines=True,
-        )
+            ['git', 'log', '--pretty=format:%ct', '--quiet', '-1', 'HEAD'],
+            cwd=repo_dir).decode()
     except subprocess.CalledProcessError:
         return None
 
     try:
         timestamp = datetime.datetime.utcfromtimestamp(int(timestamp))
     except ValueError:
         return None
```

### Comparing `fuglu-1.4.0/src/fuglu.egg-info/PKG-INFO` & `fuglu-1.5.0/src/fuglu.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: fuglu
-Version: 1.4.0
+Version: 1.5.0
 Summary: FuGlu Mail Content Scanner
 Home-page: http://www.fuglu.org
+Download-URL: https://gitlab.com/fumail/fuglu/-/archive/master/fuglu-master.tar.gz
 Author: O. Schacher
 Author-email: oli@fuglu.org
 License: Apache Software License
-Download-URL: https://gitlab.com/fumail/fuglu/-/archive/master/fuglu-master.tar.gz
-Description: FuGlu is a modular pre-queue/after-queue content filter written in Python that
-        acts as the glue application between the MTA and SPAM, Virus, and other scanners.
-        It can be used to filter spam, viruses, unwanted attachments, and do other content filtering.
-        
-        FuGlu focuses on being solid, easy to manage, debug and monitor.
-        
-        Quick links:
-        
-         * `Overview and documentation <https://fumail.gitlab.io/fuglu/>`_
-         * `Download <https://pypi.python.org/pypi/fuglu/>`_
-         * `Issue Tracker <https://gitlab.com/fumail/fuglu/issues>`_
-         * `Extra Plugins Repository <https://gitlab.com/fumail/fuglu-extra-plugins/>`_
-        
-        .. image:: https://badge.fury.io/py/fuglu.svg
-            :target: https://pypi.python.org/pypi/fuglu/
-            :alt: Latest PyPI version
-        
-        .. image:: https://gitlab.com/fumail/fuglu/badges/master/build.svg
-            :target: https://gitlab.com/fumail/fuglu/pipelines
-            :alt: Build status
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Communications :: Email :: Filters
 Classifier: Topic :: Communications :: Email :: Mail Transport Agents
 Requires: domainmagic
 Requires-Python: >=3.6
+Provides-Extra: test
+License-File: LICENSE
+
+FuGlu is a modular pre-queue/after-queue content filter written in Python that
+acts as the glue application between the MTA and SPAM, Virus, and other scanners.
+It can be used to filter spam, viruses, unwanted attachments, and do other content filtering.
+
+FuGlu focuses on being solid, easy to manage, debug and monitor.
+
+Quick links:
+
+ * `Overview and documentation <https://fumail.gitlab.io/fuglu/>`_
+ * `Download <https://pypi.python.org/pypi/fuglu/>`_
+ * `Issue Tracker <https://gitlab.com/fumail/fuglu/issues>`_
+ * `Extra Plugins Repository <https://gitlab.com/fumail/fuglu-extra-plugins/>`_
+
+.. image:: https://badge.fury.io/py/fuglu.svg
+    :target: https://pypi.python.org/pypi/fuglu/
+    :alt: Latest PyPI version
+
+.. image:: https://gitlab.com/fumail/fuglu/badges/master/build.svg
+    :target: https://gitlab.com/fumail/fuglu/pipelines
+    :alt: Build status
```

### Comparing `fuglu-1.4.0/src/fuglu.egg-info/SOURCES.txt` & `fuglu-1.5.0/src/fuglu.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,25 @@
 conf/rules/default-archivefiletypes.conf.dist
 conf/rules/default-archivenames.conf.dist
 conf/rules/default-filenames.conf.dist
 conf/rules/default-filetypes.conf.dist
 conf/templates/blockedfile.tmpl.dist
 doc/CHANGELOG
 doc/INSTALL
+scripts/buildscripts/README.md
+scripts/buildscripts/build-deb.sh
 scripts/mrtg/fuglu_mrtg.sh
 scripts/startscripts/arch/fuglu.service
 scripts/startscripts/centos_rhel/6/fuglu
 scripts/startscripts/centos_rhel/7/fuglu.service
 scripts/startscripts/debian/7/fuglu
 scripts/startscripts/debian/8/fuglu.service
 scripts/startscripts/suse/13/fuglu
 src/fuglu/__init__.py
+src/fuglu/__main__.py
 src/fuglu/addrcheck.py
 src/fuglu/asyncprocpool.py
 src/fuglu/bounce.py
 src/fuglu/caching.py
 src/fuglu/core.py
 src/fuglu/daemon.py
 src/fuglu/debug.py
@@ -60,14 +63,15 @@
 src/fuglu/extensions/__init__.py
 src/fuglu/extensions/aioredisext.py
 src/fuglu/extensions/dnsquery.py
 src/fuglu/extensions/elastic.py
 src/fuglu/extensions/filearchives.py
 src/fuglu/extensions/filetype.py
 src/fuglu/extensions/fuzzyhashlib.py
+src/fuglu/extensions/matrixchat.py
 src/fuglu/extensions/redisext.py
 src/fuglu/extensions/sql.py
 src/fuglu/lib/__init__.py
 src/fuglu/lib/patcheddkimlib.py
 src/fuglu/lib/patchedlibmilter.py
 src/fuglu/lib/ppymilterbase.py
 src/fuglu/lib/patchedemail/__init__.py
@@ -99,14 +103,15 @@
 src/fuglu/plugins/p_debug.py
 src/fuglu/plugins/p_fraction.py
 src/fuglu/plugins/p_skipper.py
 src/fuglu/plugins/restrictions.py
 src/fuglu/plugins/rspamd.py
 src/fuglu/plugins/sa.py
 src/fuglu/plugins/script.py
+src/fuglu/plugins/sigenc.py
 src/fuglu/plugins/taction.py
 src/fuglu/plugins/tlspolicy.py
 src/fuglu/plugins/uriextract.py
 src/fuglu/plugins/vacation.py
 src/fuglu/plugins/ratelimit/__init__.py
 src/fuglu/plugins/ratelimit/dynfunction.py
 src/fuglu/plugins/ratelimit/helperfuncs.py
@@ -115,14 +120,13 @@
 src/fuglu/plugins/ratelimit/strategies/always_hit.py
 src/fuglu/plugins/ratelimit/strategies/backendint.py
 src/fuglu/plugins/ratelimit/strategies/fixed_ratelimit.py
 src/fuglu/plugins/ratelimit/strategies/sliding_log_ratelimit.py
 src/fuglu/plugins/ratelimit/strategies/sliding_window_ratelimit.py
 src/fuglu/utils/__init__.py
 src/fuglu/utils/version.py
-src/startscript/fuglu
 src/tools/fuglu_client
 src/tools/fuglu_conf
 src/tools/fuglu_control
 src/tools/fuglu_debug
 src/tools/fuglu_healthcheck
 src/tools/fuglu_suspectfilter
```

### Comparing `fuglu-1.4.0/src/startscript/fuglu` & `fuglu-1.5.0/src/fuglu/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: UTF-8 -*-
 
-#   Copyright Oli Schacher, Fumail Project
+#   Copyright Fumail Project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `fuglu-1.4.0/src/tools/fuglu_client` & `fuglu-1.5.0/src/tools/fuglu_client`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/tools/fuglu_conf` & `fuglu-1.5.0/src/tools/fuglu_conf`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/tools/fuglu_control` & `fuglu-1.5.0/src/tools/fuglu_control`

 * *Files 2% similar despite different names*

```diff
@@ -107,26 +107,26 @@
 try:
     iport = int(localport)
 except (TypeError, ValueError):
     pass
 
 cmd = " ".join(pargs)
 # connect to debug port
-if iport != None:
+if iport is not None:
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 else:
     s = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
 
 try:
-    if iport != None:
+    if iport is not None:
         s.connect(('127.0.0.1', iport))
     else:
         s.connect(localport)
 except Exception as e:
-    print("Cannot connect to fuglu control deamon (%s) - is fuglu running?" % localport)
-    print(str(e))
+    print(f"Cannot connect to fuglu control daemon ({localport}) - is fuglu running?")
+    print(f"{e.__class__.__name__}: {str(e)}")
     sys.exit(1)
 
 s.sendall(force_bString(cmd))
 data = s.recv(32768)
 s.close()
 print(force_uString(data))
```

### Comparing `fuglu-1.4.0/src/tools/fuglu_debug` & `fuglu-1.5.0/src/tools/fuglu_debug`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/tools/fuglu_healthcheck` & `fuglu-1.5.0/src/tools/fuglu_healthcheck`

 * *Files identical despite different names*

### Comparing `fuglu-1.4.0/src/tools/fuglu_suspectfilter` & `fuglu-1.5.0/src/tools/fuglu_suspectfilter`

 * *Files identical despite different names*

