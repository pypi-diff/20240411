# Comparing `tmp/django-field-logger-0.0.23.tar.gz` & `tmp/django-field-logger-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-field-logger-0.0.23.tar", last modified: Thu Apr 11 08:16:38 2024, max compression
+gzip compressed data, was "django-field-logger-0.0.24.tar", last modified: Thu Apr 11 16:55:48 2024, max compression
```

## Comparing `django-field-logger-0.0.23.tar` & `django-field-logger-0.0.24.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 08:16:38.005205 django-field-logger-0.0.23/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django-field-logger-0.0.23/LICENSE
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django-field-logger-0.0.23/MANIFEST.in
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9101 2024-04-11 08:16:38.005205 django-field-logger-0.0.23/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     7502 2024-04-11 08:14:00.000000 django-field-logger-0.0.23/README.rst
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 08:16:37.995205 django-field-logger-0.0.23/django_field_logger.egg-info/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9101 2024-04-11 08:16:37.000000 django-field-logger-0.0.23/django_field_logger.egg-info/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      530 2024-04-11 08:16:37.000000 django-field-logger-0.0.23/django_field_logger.egg-info/SOURCES.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-04-11 08:16:37.000000 django-field-logger-0.0.23/django_field_logger.egg-info/dependency_links.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-11 08:16:37.000000 django-field-logger-0.0.23/django_field_logger.egg-info/requires.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-11 08:16:37.000000 django-field-logger-0.0.23/django_field_logger.egg-info/top_level.txt
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 08:16:38.005205 django-field-logger-0.0.23/fieldlogger/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-01-16 20:05:29.000000 django-field-logger-0.0.23/fieldlogger/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-01-16 20:51:47.000000 django-field-logger-0.0.23/fieldlogger/apps.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3135 2024-04-08 14:39:49.000000 django-field-logger-0.0.23/fieldlogger/config.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      862 2024-04-01 09:39:30.000000 django-field-logger-0.0.23/fieldlogger/fieldlogger.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      350 2024-01-17 04:38:48.000000 django-field-logger-0.0.23/fieldlogger/mixins.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2621 2024-04-11 07:22:36.000000 django-field-logger-0.0.23/fieldlogger/models.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1563 2024-04-08 14:41:10.000000 django-field-logger-0.0.23/fieldlogger/signals.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      296 2024-03-27 00:36:10.000000 django-field-logger-0.0.23/fieldlogger/utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      415 2024-04-01 09:32:10.000000 django-field-logger-0.0.23/pyproject.toml
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      670 2024-04-11 08:16:38.005205 django-field-logger-0.0.23/setup.cfg
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       96 2024-04-11 08:00:46.000000 django-field-logger-0.0.23/setup.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 08:16:38.005205 django-field-logger-0.0.23/tests/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-03-27 02:22:33.000000 django-field-logger-0.0.23/tests/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2913 2024-04-11 07:12:55.000000 django-field-logger-0.0.23/tests/settings.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3943 2024-04-11 07:23:31.000000 django-field-logger-0.0.23/tests/test_utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1788 2024-04-11 07:26:07.000000 django-field-logger-0.0.23/tests/tests.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 16:55:48.645359 django-field-logger-0.0.24/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django-field-logger-0.0.24/LICENSE
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django-field-logger-0.0.24/MANIFEST.in
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9200 2024-04-11 16:55:48.645359 django-field-logger-0.0.24/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     7601 2024-04-11 16:53:44.000000 django-field-logger-0.0.24/README.rst
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 16:55:48.645359 django-field-logger-0.0.24/django_field_logger.egg-info/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9200 2024-04-11 16:55:48.000000 django-field-logger-0.0.24/django_field_logger.egg-info/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      530 2024-04-11 16:55:48.000000 django-field-logger-0.0.24/django_field_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-04-11 16:55:48.000000 django-field-logger-0.0.24/django_field_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-11 16:55:48.000000 django-field-logger-0.0.24/django_field_logger.egg-info/requires.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-11 16:55:48.000000 django-field-logger-0.0.24/django_field_logger.egg-info/top_level.txt
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 16:55:48.645359 django-field-logger-0.0.24/fieldlogger/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-01-16 20:05:29.000000 django-field-logger-0.0.24/fieldlogger/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-01-16 20:51:47.000000 django-field-logger-0.0.24/fieldlogger/apps.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3135 2024-04-08 14:39:49.000000 django-field-logger-0.0.24/fieldlogger/config.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      862 2024-04-01 09:39:30.000000 django-field-logger-0.0.24/fieldlogger/fieldlogger.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      350 2024-01-17 04:38:48.000000 django-field-logger-0.0.24/fieldlogger/mixins.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2621 2024-04-11 07:22:36.000000 django-field-logger-0.0.24/fieldlogger/models.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1563 2024-04-08 14:41:10.000000 django-field-logger-0.0.24/fieldlogger/signals.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      296 2024-03-27 00:36:10.000000 django-field-logger-0.0.24/fieldlogger/utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      415 2024-04-01 09:32:10.000000 django-field-logger-0.0.24/pyproject.toml
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      670 2024-04-11 16:55:48.645359 django-field-logger-0.0.24/setup.cfg
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       96 2024-04-11 16:55:39.000000 django-field-logger-0.0.24/setup.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 16:55:48.645359 django-field-logger-0.0.24/tests/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-03-27 02:22:33.000000 django-field-logger-0.0.24/tests/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2913 2024-04-11 07:12:55.000000 django-field-logger-0.0.24/tests/settings.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3943 2024-04-11 07:23:31.000000 django-field-logger-0.0.24/tests/test_utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1788 2024-04-11 07:26:07.000000 django-field-logger-0.0.24/tests/tests.py
```

### Comparing `django-field-logger-0.0.23/LICENSE` & `django-field-logger-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.23/PKG-INFO` & `django-field-logger-0.0.24/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-field-logger
-Version: 0.0.23
+Version: 0.0.24
 Summary: A Django app for logging changes in model fields.
 Home-page: https://github.com/nibblex/django-field-logger
 Author: Sergio Rodríguez
 Author-email: srodriguez3441@gmail.com
 Maintainer: Sergio Rodríguez
 Maintainer-email: srodriguez3441@gmail.com
 License: MIT
@@ -13,25 +13,22 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 License-File: LICENSE
 
 Django Field Logger
 ===================
 
-Quick Description
-~~~~~~~~~~~~~~~~~
-
 A Django app for logging changes in model fields.
 
 How to set up?
 ~~~~~~~~~~~~~~
 
 1) Add ``fieldlogger`` to your ``INSTALLED_APPS``
 2) Run ``python manage.py migrate`` to initialize the model
-3) Add ``FIELD_LOGGER_SETTINGS`` to your settings.py file.
+3) Add ``FIELD_LOGGER_SETTINGS`` to your ``settings.py`` file.
 
 .. code:: python
 
    FIELD_LOGGER_SETTINGS={
        'ENCODER': 'path.to.your.json.Encoder', # (default: None)
        'DECODER': 'path.to.your.json.Decoder', # (default: None)
        'LOGGING_ENABLED': True, # (default: True)
@@ -83,15 +80,15 @@
          all fields in the model will be logged except the ones
          specified here.
       -  ``callbacks`` is optional. If you want to add a callback
          function to be called after logging all models in all apps, you
          can add it here. Callback functions must be callable objects.
          You can optionally specify a callback function path in your
          configuration. The best practice is to place your callback
-         function in yourapp/callbacks.py Callback functions must have
+         function in yourapp/callbacks.py. Callback functions must have
          the following signature:
          ``python   def callback(instance, fields, logs):       pass``
 
          -  ``instance`` the model instance that is being logged.
          -  ``fields`` list of fields that are being logged.
          -  ``logs`` dict of logs that are being created. The key is the
             field name and the value is the ``FieldLog`` instance.
@@ -99,22 +96,22 @@
 How it works?
 ~~~~~~~~~~~~~
 
 -  Obtains the ``FIELD_LOGGER_SETTINGS`` from your respective settings
    file based on your environment.
 -  Initializes ``LOGGING_APPS`` with the relative project paths of your
    models based on your configuration variable.
--  Binds to pre_save signal of each loggable model
+-  Binds to pre_save signal of each loggable model.
 -  For each field specified in the configuration variable, creates a
-   record in the ``FieldLog`` model in each instance update.
+   record in the ``FieldLog`` model for each instance update.
 
 Example
 ~~~~~~~
 
-This section serves as a small example to demonstrate this package.
+This section serves as a small example to demonstrate how to use this package.
 
 Supposing you have this configuration in your settings.py file:
 
 .. code:: python
 
    FIELD_LOGGER_SETTINGS={
        'LOGGING_APPS': {
@@ -124,16 +121,16 @@
                        'fields': ['driver_name']
                    },
                },
            },
        },
    }
 
-Supposing you have a model called ``Driver`` and fields called
-``latest_speed`` and ``driver_name`` and ``driver_id``:
+Supposing you have a model called ``Driver`` with fields called
+``latest_speed``, ``driver_name``, ``driver_id``:
 
 .. code:: python
 
        driver = Driver.objects.last()
        driver.latest_speed = 5
        driver.save()  # fieldlogger won't create a record since 'latest_speed' was not among the loggable fields
 
@@ -162,15 +159,15 @@
        log = logs.get('driver_name')
        if log:
            log.extra_data = {
                'name_length': len(log.new_value)
            }
            log.save()
 
-You can add this function to your configuration like this:
+Then you can add this callback function to your configuration like this:
 
 .. code:: python
 
    FIELD_LOGGER_SETTINGS={
        'LOGGING_APPS': {
            'drivers': {
                'models': {
@@ -181,17 +178,17 @@
                        ]
                    },
                },
            },
        },
    }
 
-   If 'fail_silently' is set to False, exceptions will be raised if the callback function fails.
+.. note::
 
-   note: you can also add lambda functions to your callbacks
+    You can also add lambda functions to your callbacks
 
 The model structure
 ~~~~~~~~~~~~~~~~~~~
 
 This package provides you a django model which is called ``FieldLog``;
 which tracks each change to a model instance specified in your
 configuration mapping. An example record is as follows:
@@ -222,16 +219,22 @@
 The FieldLoggerMixin
 ~~~~~~~~~~~~~~~~~~~~
 
 This package provides you a mixin class which is called
 ``FieldLoggerMixin``. This mixin class provides you the following
 property:
 
--  ``fieldlog_set`` returns the ``FieldLog`` queryset of the instance
-   that is being logged.
+-  ``fieldlog_set`` since the ``FieldLog`` model has not a direct
+   relation to the model that is being logged, you can use this property
+   to get the logs of the instance that is being logged.
+
+   .. code:: python
+
+       driver = Driver.objects.last()
+       logs = driver.fieldlog_set.all()
 
 MIT License
 
 Copyright (c) 2024 Sergio Rodríguez
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `django-field-logger-0.0.23/README.rst` & `django-field-logger-0.0.24/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Django Field Logger
 ===================
 
-Quick Description
-~~~~~~~~~~~~~~~~~
-
 A Django app for logging changes in model fields.
 
 How to set up?
 ~~~~~~~~~~~~~~
 
 1) Add ``fieldlogger`` to your ``INSTALLED_APPS``
 2) Run ``python manage.py migrate`` to initialize the model
-3) Add ``FIELD_LOGGER_SETTINGS`` to your settings.py file.
+3) Add ``FIELD_LOGGER_SETTINGS`` to your ``settings.py`` file.
 
 .. code:: python
 
    FIELD_LOGGER_SETTINGS={
        'ENCODER': 'path.to.your.json.Encoder', # (default: None)
        'DECODER': 'path.to.your.json.Decoder', # (default: None)
        'LOGGING_ENABLED': True, # (default: True)
@@ -67,15 +64,15 @@
          all fields in the model will be logged except the ones
          specified here.
       -  ``callbacks`` is optional. If you want to add a callback
          function to be called after logging all models in all apps, you
          can add it here. Callback functions must be callable objects.
          You can optionally specify a callback function path in your
          configuration. The best practice is to place your callback
-         function in yourapp/callbacks.py Callback functions must have
+         function in yourapp/callbacks.py. Callback functions must have
          the following signature:
          ``python   def callback(instance, fields, logs):       pass``
 
          -  ``instance`` the model instance that is being logged.
          -  ``fields`` list of fields that are being logged.
          -  ``logs`` dict of logs that are being created. The key is the
             field name and the value is the ``FieldLog`` instance.
@@ -83,22 +80,22 @@
 How it works?
 ~~~~~~~~~~~~~
 
 -  Obtains the ``FIELD_LOGGER_SETTINGS`` from your respective settings
    file based on your environment.
 -  Initializes ``LOGGING_APPS`` with the relative project paths of your
    models based on your configuration variable.
--  Binds to pre_save signal of each loggable model
+-  Binds to pre_save signal of each loggable model.
 -  For each field specified in the configuration variable, creates a
-   record in the ``FieldLog`` model in each instance update.
+   record in the ``FieldLog`` model for each instance update.
 
 Example
 ~~~~~~~
 
-This section serves as a small example to demonstrate this package.
+This section serves as a small example to demonstrate how to use this package.
 
 Supposing you have this configuration in your settings.py file:
 
 .. code:: python
 
    FIELD_LOGGER_SETTINGS={
        'LOGGING_APPS': {
@@ -108,16 +105,16 @@
                        'fields': ['driver_name']
                    },
                },
            },
        },
    }
 
-Supposing you have a model called ``Driver`` and fields called
-``latest_speed`` and ``driver_name`` and ``driver_id``:
+Supposing you have a model called ``Driver`` with fields called
+``latest_speed``, ``driver_name``, ``driver_id``:
 
 .. code:: python
 
        driver = Driver.objects.last()
        driver.latest_speed = 5
        driver.save()  # fieldlogger won't create a record since 'latest_speed' was not among the loggable fields
 
@@ -146,15 +143,15 @@
        log = logs.get('driver_name')
        if log:
            log.extra_data = {
                'name_length': len(log.new_value)
            }
            log.save()
 
-You can add this function to your configuration like this:
+Then you can add this callback function to your configuration like this:
 
 .. code:: python
 
    FIELD_LOGGER_SETTINGS={
        'LOGGING_APPS': {
            'drivers': {
                'models': {
@@ -165,17 +162,17 @@
                        ]
                    },
                },
            },
        },
    }
 
-   If 'fail_silently' is set to False, exceptions will be raised if the callback function fails.
+.. note::
 
-   note: you can also add lambda functions to your callbacks
+    You can also add lambda functions to your callbacks
 
 The model structure
 ~~~~~~~~~~~~~~~~~~~
 
 This package provides you a django model which is called ``FieldLog``;
 which tracks each change to a model instance specified in your
 configuration mapping. An example record is as follows:
@@ -206,9 +203,15 @@
 The FieldLoggerMixin
 ~~~~~~~~~~~~~~~~~~~~
 
 This package provides you a mixin class which is called
 ``FieldLoggerMixin``. This mixin class provides you the following
 property:
 
--  ``fieldlog_set`` returns the ``FieldLog`` queryset of the instance
-   that is being logged.
+-  ``fieldlog_set`` since the ``FieldLog`` model has not a direct
+   relation to the model that is being logged, you can use this property
+   to get the logs of the instance that is being logged.
+
+   .. code:: python
+
+       driver = Driver.objects.last()
+       logs = driver.fieldlog_set.all()
```

### Comparing `django-field-logger-0.0.23/django_field_logger.egg-info/PKG-INFO` & `django-field-logger-0.0.24/django_field_logger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-field-logger
-Version: 0.0.23
+Version: 0.0.24
 Summary: A Django app for logging changes in model fields.
 Home-page: https://github.com/nibblex/django-field-logger
 Author: Sergio Rodríguez
 Author-email: srodriguez3441@gmail.com
 Maintainer: Sergio Rodríguez
 Maintainer-email: srodriguez3441@gmail.com
 License: MIT
@@ -13,25 +13,22 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 License-File: LICENSE
 
 Django Field Logger
 ===================
 
-Quick Description
-~~~~~~~~~~~~~~~~~
-
 A Django app for logging changes in model fields.
 
 How to set up?
 ~~~~~~~~~~~~~~
 
 1) Add ``fieldlogger`` to your ``INSTALLED_APPS``
 2) Run ``python manage.py migrate`` to initialize the model
-3) Add ``FIELD_LOGGER_SETTINGS`` to your settings.py file.
+3) Add ``FIELD_LOGGER_SETTINGS`` to your ``settings.py`` file.
 
 .. code:: python
 
    FIELD_LOGGER_SETTINGS={
        'ENCODER': 'path.to.your.json.Encoder', # (default: None)
        'DECODER': 'path.to.your.json.Decoder', # (default: None)
        'LOGGING_ENABLED': True, # (default: True)
@@ -83,15 +80,15 @@
          all fields in the model will be logged except the ones
          specified here.
       -  ``callbacks`` is optional. If you want to add a callback
          function to be called after logging all models in all apps, you
          can add it here. Callback functions must be callable objects.
          You can optionally specify a callback function path in your
          configuration. The best practice is to place your callback
-         function in yourapp/callbacks.py Callback functions must have
+         function in yourapp/callbacks.py. Callback functions must have
          the following signature:
          ``python   def callback(instance, fields, logs):       pass``
 
          -  ``instance`` the model instance that is being logged.
          -  ``fields`` list of fields that are being logged.
          -  ``logs`` dict of logs that are being created. The key is the
             field name and the value is the ``FieldLog`` instance.
@@ -99,22 +96,22 @@
 How it works?
 ~~~~~~~~~~~~~
 
 -  Obtains the ``FIELD_LOGGER_SETTINGS`` from your respective settings
    file based on your environment.
 -  Initializes ``LOGGING_APPS`` with the relative project paths of your
    models based on your configuration variable.
--  Binds to pre_save signal of each loggable model
+-  Binds to pre_save signal of each loggable model.
 -  For each field specified in the configuration variable, creates a
-   record in the ``FieldLog`` model in each instance update.
+   record in the ``FieldLog`` model for each instance update.
 
 Example
 ~~~~~~~
 
-This section serves as a small example to demonstrate this package.
+This section serves as a small example to demonstrate how to use this package.
 
 Supposing you have this configuration in your settings.py file:
 
 .. code:: python
 
    FIELD_LOGGER_SETTINGS={
        'LOGGING_APPS': {
@@ -124,16 +121,16 @@
                        'fields': ['driver_name']
                    },
                },
            },
        },
    }
 
-Supposing you have a model called ``Driver`` and fields called
-``latest_speed`` and ``driver_name`` and ``driver_id``:
+Supposing you have a model called ``Driver`` with fields called
+``latest_speed``, ``driver_name``, ``driver_id``:
 
 .. code:: python
 
        driver = Driver.objects.last()
        driver.latest_speed = 5
        driver.save()  # fieldlogger won't create a record since 'latest_speed' was not among the loggable fields
 
@@ -162,15 +159,15 @@
        log = logs.get('driver_name')
        if log:
            log.extra_data = {
                'name_length': len(log.new_value)
            }
            log.save()
 
-You can add this function to your configuration like this:
+Then you can add this callback function to your configuration like this:
 
 .. code:: python
 
    FIELD_LOGGER_SETTINGS={
        'LOGGING_APPS': {
            'drivers': {
                'models': {
@@ -181,17 +178,17 @@
                        ]
                    },
                },
            },
        },
    }
 
-   If 'fail_silently' is set to False, exceptions will be raised if the callback function fails.
+.. note::
 
-   note: you can also add lambda functions to your callbacks
+    You can also add lambda functions to your callbacks
 
 The model structure
 ~~~~~~~~~~~~~~~~~~~
 
 This package provides you a django model which is called ``FieldLog``;
 which tracks each change to a model instance specified in your
 configuration mapping. An example record is as follows:
@@ -222,16 +219,22 @@
 The FieldLoggerMixin
 ~~~~~~~~~~~~~~~~~~~~
 
 This package provides you a mixin class which is called
 ``FieldLoggerMixin``. This mixin class provides you the following
 property:
 
--  ``fieldlog_set`` returns the ``FieldLog`` queryset of the instance
-   that is being logged.
+-  ``fieldlog_set`` since the ``FieldLog`` model has not a direct
+   relation to the model that is being logged, you can use this property
+   to get the logs of the instance that is being logged.
+
+   .. code:: python
+
+       driver = Driver.objects.last()
+       logs = driver.fieldlog_set.all()
 
 MIT License
 
 Copyright (c) 2024 Sergio Rodríguez
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `django-field-logger-0.0.23/django_field_logger.egg-info/SOURCES.txt` & `django-field-logger-0.0.24/django_field_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.23/fieldlogger/config.py` & `django-field-logger-0.0.24/fieldlogger/config.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.23/fieldlogger/fieldlogger.py` & `django-field-logger-0.0.24/fieldlogger/fieldlogger.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.23/fieldlogger/models.py` & `django-field-logger-0.0.24/fieldlogger/models.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.23/fieldlogger/signals.py` & `django-field-logger-0.0.24/fieldlogger/signals.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.23/setup.cfg` & `django-field-logger-0.0.24/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-field-logger
-version = 0.0.23
+version = 0.0.24
 description = A Django app for logging changes in model fields.
 long_description = file: README.rst, LICENSE
 author = Sergio Rodríguez
 author_email = srodriguez3441@gmail.com
 maintainer = Sergio Rodríguez
 maintainer_email = srodriguez3441@gmail.com
 url = https://github.com/nibblex/django-field-logger
```

### Comparing `django-field-logger-0.0.23/tests/settings.py` & `django-field-logger-0.0.24/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.23/tests/test_utils.py` & `django-field-logger-0.0.24/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.23/tests/tests.py` & `django-field-logger-0.0.24/tests/tests.py`

 * *Files identical despite different names*

