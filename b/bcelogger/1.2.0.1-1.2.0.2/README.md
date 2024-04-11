# Comparing `tmp/bcelogger-1.2.0.1-py3-none-any.whl.zip` & `tmp/bcelogger-1.2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9265 bytes, number of entries: 13
--rw-r--r--  2.0 unx      611 b- defN 24-Apr-01 06:45 bcelogger/__init__.py
--rw-r--r--  2.0 unx     6547 b- defN 24-Apr-01 06:41 bcelogger/base_logger.py
--rw-r--r--  2.0 unx     2537 b- defN 24-Mar-06 03:13 bcelogger/db_logger.py
--rw-r--r--  2.0 unx     2286 b- defN 24-Mar-06 03:21 bcelogger/default_logger.py
--rw-r--r--  2.0 unx     1501 b- defN 24-Mar-06 03:13 bcelogger/multi_logger.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-06 03:13 bcelogger/conf/__init__.py
--rw-r--r--  2.0 unx     1456 b- defN 24-Mar-06 03:13 bcelogger/conf/logit_conf.py
--rw-r--r--  2.0 unx     1373 b- defN 24-Mar-06 03:13 bcelogger/conf/logit_db_conf.py
--rw-r--r--  2.0 unx     1596 b- defN 24-Mar-06 03:13 bcelogger/conf/logit_multi_conf.py
--rw-r--r--  2.0 unx      218 b- defN 24-Apr-01 07:06 bcelogger-1.2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 07:06 bcelogger-1.2.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Apr-01 07:06 bcelogger-1.2.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1060 b- defN 24-Apr-01 07:06 bcelogger-1.2.0.1.dist-info/RECORD
-13 files, 19287 bytes uncompressed, 7491 bytes compressed:  61.2%
+Zip file size: 9275 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      611 b- defN 24-Apr-11 11:35 bcelogger/__init__.py
+-rw-r--r--  2.0 unx     6565 b- defN 24-Apr-11 11:36 bcelogger/base_logger.py
+-rw-r--r--  2.0 unx     2537 b- defN 24-Apr-11 11:35 bcelogger/db_logger.py
+-rw-r--r--  2.0 unx     2286 b- defN 24-Apr-11 11:35 bcelogger/default_logger.py
+-rw-r--r--  2.0 unx     1501 b- defN 24-Apr-11 11:35 bcelogger/multi_logger.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-11 11:35 bcelogger/conf/__init__.py
+-rw-r--r--  2.0 unx     1456 b- defN 24-Apr-11 11:35 bcelogger/conf/logit_conf.py
+-rw-r--r--  2.0 unx     1373 b- defN 24-Apr-11 11:35 bcelogger/conf/logit_db_conf.py
+-rw-r--r--  2.0 unx     1596 b- defN 24-Apr-11 11:35 bcelogger/conf/logit_multi_conf.py
+-rw-r--r--  2.0 unx      218 b- defN 24-Apr-11 11:37 bcelogger-1.2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 11:37 bcelogger-1.2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-11 11:37 bcelogger-1.2.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1060 b- defN 24-Apr-11 11:37 bcelogger-1.2.0.2.dist-info/RECORD
+13 files, 19305 bytes uncompressed, 7501 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: bcelogger/conf/logit_db_conf.py
 Comment: 
 
 Filename: bcelogger/conf/logit_multi_conf.py
 Comment: 
 
-Filename: bcelogger-1.2.0.1.dist-info/METADATA
+Filename: bcelogger-1.2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: bcelogger-1.2.0.1.dist-info/WHEEL
+Filename: bcelogger-1.2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: bcelogger-1.2.0.1.dist-info/top_level.txt
+Filename: bcelogger-1.2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bcelogger-1.2.0.1.dist-info/RECORD
+Filename: bcelogger-1.2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bcelogger/base_logger.py

```diff
@@ -65,15 +65,15 @@
         Logger.make_log_dir(log_dir)
 
         logger_name = config_dict.get("logger_name")
         self.logger = logging.getLogger(logger_name)
         self.logger.setLevel(logging.DEBUG)
 
         # 日志格式
-        log_fmt = '%(levelname)s: %(asctime)s %(filename)s[line:%(lineno)d] %(message)s'
+        log_fmt = '%(levelname)s: %(asctime)s %(filename)s[line:%(lineno)d] Thread:%(thread)d %(message)s'
         # 默认日志时间精确到秒，default_ms参数精确到毫秒
         date_fmt = '%Y-%m-%d %H:%M:%S'
         if config_dict.get("prefix") == 'default_ms':
             date_fmt = None
         format_str = logging.Formatter(log_fmt, datefmt=date_fmt)  # 设置日志格式
 
         # 输出日志到控制台
```

## Comparing `bcelogger-1.2.0.1.dist-info/RECORD` & `bcelogger-1.2.0.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 bcelogger/__init__.py,sha256=fzyR90Doifln9F8-Aaf8bxX26Sk4Yz7hOwJKhdW9u9Y,611
-bcelogger/base_logger.py,sha256=TefCaWR2l2FWHNmZADd2w7gO1eY171XocOIR2VZZR1s,6547
+bcelogger/base_logger.py,sha256=5XkNj6ix9sN9Wqueo9N4yNJ5zO4vmsNULLbyqU43EOQ,6565
 bcelogger/db_logger.py,sha256=D0Idd_U83xqIOXEwZIPz6u4Qmee_6PYwXByK_rrpyb8,2537
 bcelogger/default_logger.py,sha256=ykrwCKVB0iwhX4yvl8ABDOBltw1xCr-0AgdmzjR9W9g,2286
 bcelogger/multi_logger.py,sha256=-FyFwTDdyreMt57tDPWGAbsV7eYoHyplY_2dFyBDwXw,1501
 bcelogger/conf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bcelogger/conf/logit_conf.py,sha256=MgcyXPP8_mXTzHwJLv97cqDi3W4Dci-je0OEeBawDhw,1456
 bcelogger/conf/logit_db_conf.py,sha256=67FELUBhEkyy8SJRTU8VObC8LbVw2DvMS8LsuoI6-1A,1373
 bcelogger/conf/logit_multi_conf.py,sha256=JrX2tq-TPekHih7zrv4691RBgSS0rKYoj6P8Bc5DCKs,1596
-bcelogger-1.2.0.1.dist-info/METADATA,sha256=biDpNVctL0HrhmllJnjpTZ6Q6LDHRIe8QFcshzBFE9s,218
-bcelogger-1.2.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bcelogger-1.2.0.1.dist-info/top_level.txt,sha256=rDEUh-gQmZsqA3zqupaEAjWpMYrYpB9nEo-yOc4I2-w,10
-bcelogger-1.2.0.1.dist-info/RECORD,,
+bcelogger-1.2.0.2.dist-info/METADATA,sha256=I8t69YamdpfyBOTbwWp4Jccx1vxyw-Hn6ieJc6fDLRE,218
+bcelogger-1.2.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bcelogger-1.2.0.2.dist-info/top_level.txt,sha256=rDEUh-gQmZsqA3zqupaEAjWpMYrYpB9nEo-yOc4I2-w,10
+bcelogger-1.2.0.2.dist-info/RECORD,,
```

