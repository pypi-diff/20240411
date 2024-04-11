# Comparing `tmp/django_ses-3.5.2.tar.gz` & `tmp/django_ses-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ses-3.5.2.tar", max compression
+gzip compressed data, was "django_ses-3.6.0.tar", max compression
```

## Comparing `django_ses-3.5.2.tar` & `django_ses-3.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1057 2023-12-01 19:36:07.204285 django_ses-3.5.2/LICENSE
--rw-r--r--   0        0        0    22619 2023-12-01 19:36:07.204285 django_ses-3.5.2/README.rst
--rw-r--r--   0        0        0    14037 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/__init__.py
--rw-r--r--   0        0        0      232 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/admin.py
--rw-r--r--   0        0        0      181 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/apps.py
--rw-r--r--   0        0        0       65 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/deprecation.py
--rw-r--r--   0        0        0        0 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/management/__init__.py
--rw-r--r--   0        0        0        0 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/management/commands/__init__.py
--rw-r--r--   0        0        0     2328 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/management/commands/get_ses_statistics.py
--rw-r--r--   0        0        0     2700 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/management/commands/ses_email_address.py
--rw-r--r--   0        0        0      897 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/migrations/__init__.py
--rw-r--r--   0        0        0      455 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/models.py
--rw-r--r--   0        0        0     2677 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/settings.py
--rw-r--r--   0        0        0      290 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/signals.py
--rw-r--r--   0        0        0     4894 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/templates/django_ses/send_stats.html
--rw-r--r--   0        0        0      157 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/urls.py
--rw-r--r--   0        0        0     9943 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/utils.py
--rw-r--r--   0        0        0    20602 2023-12-01 19:36:07.204285 django_ses-3.5.2/django_ses/views.py
--rw-r--r--   0        0        0        0 2023-12-01 19:36:07.204285 django_ses-3.5.2/example/__init__.py
--rw-r--r--   0        0        0       90 2023-12-01 19:36:07.204285 django_ses-3.5.2/example/local_settings.template.py
--rw-r--r--   0        0        0      215 2023-12-01 19:36:07.204285 django_ses-3.5.2/example/middleware.py
--rw-r--r--   0        0        0     2173 2023-12-01 19:36:07.204285 django_ses-3.5.2/example/settings.py
--rw-r--r--   0        0        0      295 2023-12-01 19:36:07.204285 django_ses-3.5.2/example/templates/base.html
--rw-r--r--   0        0        0      220 2023-12-01 19:36:07.204285 django_ses-3.5.2/example/templates/index.html
--rw-r--r--   0        0        0      756 2023-12-01 19:36:07.204285 django_ses-3.5.2/example/templates/send-email.html
--rw-r--r--   0        0        0      818 2023-12-01 19:36:07.208285 django_ses-3.5.2/example/urls.py
--rw-r--r--   0        0        0      885 2023-12-01 19:36:07.208285 django_ses-3.5.2/example/views.py
--rw-r--r--   0        0        0     1660 2023-12-01 19:36:07.208285 django_ses-3.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-01 19:36:07.208285 django_ses-3.5.2/tests/__init__.py
--rw-r--r--   0        0        0    15650 2023-12-01 19:36:07.208285 django_ses-3.5.2/tests/test_backend.py
--rw-r--r--   0        0        0     2481 2023-12-01 19:36:07.208285 django_ses-3.5.2/tests/test_commands.py
--rw-r--r--   0        0        0     2609 2023-12-01 19:36:07.208285 django_ses-3.5.2/tests/test_settings.py
--rw-r--r--   0        0        0     5200 2023-12-01 19:36:07.208285 django_ses-3.5.2/tests/test_stats.py
--rw-r--r--   0        0        0      366 2023-12-01 19:36:07.208285 django_ses-3.5.2/tests/test_urls.py
--rw-r--r--   0        0        0    12227 2023-12-01 19:36:07.208285 django_ses-3.5.2/tests/test_verifier.py
--rw-r--r--   0        0        0    13333 2023-12-01 19:36:07.208285 django_ses-3.5.2/tests/test_views.py
--rw-r--r--   0        0        0      115 2023-12-01 19:36:07.208285 django_ses-3.5.2/tests/utils.py
--rw-r--r--   0        0        0    24194 1970-01-01 00:00:00.000000 django_ses-3.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-04-11 15:14:56.970438 django_ses-3.6.0/LICENSE
+-rw-r--r--   0        0        0    23820 2024-04-11 15:14:56.970438 django_ses-3.6.0/README.rst
+-rw-r--r--   0        0        0    14050 2024-04-11 15:14:56.970438 django_ses-3.6.0/django_ses/__init__.py
+-rw-r--r--   0        0        0      232 2024-04-11 15:14:56.970438 django_ses-3.6.0/django_ses/admin.py
+-rw-r--r--   0        0        0      181 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/apps.py
+-rw-r--r--   0        0        0       65 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/deprecation.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/management/commands/__init__.py
+-rw-r--r--   0        0        0     2328 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/management/commands/get_ses_statistics.py
+-rw-r--r--   0        0        0     2700 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/management/commands/ses_email_address.py
+-rw-r--r--   0        0        0      897 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/migrations/__init__.py
+-rw-r--r--   0        0        0      455 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/models.py
+-rw-r--r--   0        0        0     2677 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/settings.py
+-rw-r--r--   0        0        0      290 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/signals.py
+-rw-r--r--   0        0        0     4894 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/templates/django_ses/send_stats.html
+-rw-r--r--   0        0        0      156 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/urls.py
+-rw-r--r--   0        0        0     9957 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/utils.py
+-rw-r--r--   0        0        0    20556 2024-04-11 15:14:56.974438 django_ses-3.6.0/django_ses/views.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/__init__.py
+-rw-r--r--   0        0        0      103 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/local_settings.template.py
+-rw-r--r--   0        0        0      215 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/middleware.py
+-rw-r--r--   0        0        0     2173 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/settings.py
+-rw-r--r--   0        0        0      295 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/templates/base.html
+-rw-r--r--   0        0        0      220 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/templates/index.html
+-rw-r--r--   0        0        0      756 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/templates/send-email.html
+-rw-r--r--   0        0        0      812 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/urls.py
+-rw-r--r--   0        0        0      885 2024-04-11 15:14:56.974438 django_ses-3.6.0/example/views.py
+-rw-r--r--   0        0        0     2608 2024-04-11 15:14:56.974438 django_ses-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/__init__.py
+-rw-r--r--   0        0        0    16378 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_backend.py
+-rw-r--r--   0        0        0     2481 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_commands.py
+-rw-r--r--   0        0        0     2636 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_settings.py
+-rw-r--r--   0        0        0     5200 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_stats.py
+-rw-r--r--   0        0        0      366 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_urls.py
+-rw-r--r--   0        0        0    13660 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_verifier.py
+-rw-r--r--   0        0        0    13740 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/test_views.py
+-rw-r--r--   0        0        0      115 2024-04-11 15:14:56.974438 django_ses-3.6.0/tests/utils.py
+-rw-r--r--   0        0        0    25644 1970-01-01 00:00:00.000000 django_ses-3.6.0/PKG-INFO
```

### Comparing `django_ses-3.5.2/LICENSE` & `django_ses-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ses-3.5.2/README.rst` & `django_ses-3.6.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -338,14 +338,25 @@
 =================
 
 Django SES comes with two ways of viewing sending statistics.
 
 The first one is a simple read-only report on your 24 hour sending quota,
 verified email addresses and bi-weekly sending statistics.
 
+To enable the dashboard to retrieve data from AWS, you need to update the IAM policy by adding the following actions::
+
+    {
+        "Effect": "Allow",
+        "Action": [
+            "ses:ListVerifiedEmailAddresses",
+            "ses:GetSendStatistics"
+        ],
+        "Resource": "*"
+    }
+
 To generate and view SES sending statistics reports, include, update
 ``INSTALLED_APPS``::
 
     INSTALLED_APPS = (
         # ...
         'django.contrib.admin',
         'django_ses',
@@ -569,14 +580,40 @@
 #. Check your code for errors, complaints.
     Use `check.py <https://github.com/jbalogh/check>`_
 
 #. Write and run tests.
     Write your own test showing the issue has been resolved, or the feature
     works as intended.
 
+Git hooks (via pre-commit)
+==========================
+
+We use pre-push hooks to ensure that only linted code reaches our remote repository and pipelines aren't triggered in
+vain.
+
+To enable the configured pre-push hooks, you need to [install](https://pre-commit.com/) pre-commit and run once::
+
+    pre-commit install -t pre-push -t pre-commit --install-hooks
+
+This will permanently install the git hooks for both, frontend and backend, in your local
+[`.git/hooks`](./.git/hooks) folder.
+The hooks are configured in the [`.pre-commit-config.yaml`](.pre-commit-config.yaml).
+
+You can check whether hooks work as intended using the [run](https://pre-commit.com/#pre-commit-run) command::
+
+    pre-commit run [hook-id] [options]
+
+Example: run single hook::
+
+    pre-commit run ruff --all-files --hook-stage push
+
+Example: run all hooks of pre-push stage::
+
+    pre-commit run --all-files --hook-stage push
+
 Running Tests
 =============
 To run the tests::
 
     python runtests.py
 
 If you want to debug the tests, just add this file as a python script to your IDE run configuration.
```

### Comparing `django_ses-3.5.2/django_ses/__init__.py` & `django_ses-3.6.0/django_ses/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import logging
+from datetime import datetime, timedelta
+from time import sleep
 
 import boto3
 from botocore.vendored.requests.packages.urllib3.exceptions import ResponseError
 from django.core.mail.backends.base import BaseEmailBackend
-from django_ses import settings
-
-from datetime import datetime, timedelta
-from time import sleep
 
+from django_ses import settings
 
 try:
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:
     # Shim for Python 3.7. Remove when support is dropped.
     import importlib_metadata
 
@@ -252,38 +251,38 @@
         params = dict(
             FromEmailAddress=source or message.from_email,
             Destination={
                 'ToAddresses': message.recipients()
             },
             Content={
                 'Raw': {
-                    'Data': dkim_sign(message.message().as_string(),
+                    'Data': dkim_sign(message.message().as_bytes(linesep="\r\n"),
                                       dkim_key=self.dkim_key,
                                       dkim_domain=self.dkim_domain,
                                       dkim_selector=self.dkim_selector,
                                       dkim_headers=self.dkim_headers)
                 }
             }
         )
         if self.ses_from_arn or self.ses_source_arn:
             params['FromEmailAddressIdentityArn'] = self.ses_from_arn or self.ses_source_arn
         if email_feedback is not None:
             params['FeedbackForwardingEmailAddress'] = email_feedback
-            
+
         return params
 
     def _get_v1_parameters(self, message, source):
         """V1-Style raw payload for `send_raw_email`
 
         https://boto3.amazonaws.com/v1/documentation/api/1.26.31/reference/services/ses.html#SES.Client.send_raw_email
         """
         params = dict(
             Source=source or message.from_email,
             Destinations=message.recipients(),
-            RawMessage={'Data': dkim_sign(message.message().as_string(),
+            RawMessage={'Data': dkim_sign(message.message().as_bytes(linesep="\r\n"),
                                           dkim_key=self.dkim_key,
                                           dkim_domain=self.dkim_domain,
                                           dkim_selector=self.dkim_selector,
                                           dkim_headers=self.dkim_headers)}
         )
         if self.ses_source_arn:
             params['SourceArn'] = self.ses_source_arn
```

### Comparing `django_ses-3.5.2/django_ses/management/commands/get_ses_statistics.py` & `django_ses-3.6.0/django_ses/management/commands/get_ses_statistics.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.5.2/django_ses/management/commands/ses_email_address.py` & `django_ses-3.6.0/django_ses/management/commands/ses_email_address.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.5.2/django_ses/migrations/0001_initial.py` & `django_ses-3.6.0/django_ses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.5.2/django_ses/settings.py` & `django_ses-3.6.0/django_ses/settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.5.2/django_ses/templates/django_ses/send_stats.html` & `django_ses-3.6.0/django_ses/templates/django_ses/send_stats.html`

 * *Files identical despite different names*

### Comparing `django_ses-3.5.2/django_ses/utils.py` & `django_ses-3.6.0/django_ses/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
             # Some notification types do not have all fields. Only add fields
             # with values.
             bytes_to_sign.append(f"{field}\n{field_value}\n")
 
         return "".join(bytes_to_sign).encode()
 
 
-def BounceMessageVerifier(*args, **kwargs):
+def BounceMessageVerifier(*args, **kwargs):  # noqa: N802
     warnings.warn(
         "utils.BounceMessageVerifier is deprecated. It is renamed to EventMessageVerifier.",
         RemovedInDjangoSES20Warning,
     )
 
     # parameter name is renamed from bounce_dict to notification.
     if "bounce_dict" in kwargs:
```

### Comparing `django_ses-3.5.2/django_ses/views.py` & `django_ses-3.6.0/django_ses/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,28 @@
+import copy
 import json
+import logging
 import warnings
+from urllib.error import URLError
+from urllib.request import urlopen
 
 import boto3
 import pytz
+from django.core.cache import cache
+from django.core.exceptions import PermissionDenied
+from django.http import HttpResponse, HttpResponseBadRequest
+from django.shortcuts import render
 from django.utils.decorators import method_decorator
 from django.views.decorators.csrf import csrf_exempt
+from django.views.decorators.http import require_POST
 from django.views.generic.base import TemplateView, View
 
+from django_ses import settings, signals, utils
 from django_ses.deprecation import RemovedInDjangoSES20Warning
 
-from urllib.request import urlopen
-from urllib.error import URLError
-import copy
-import logging
-
-
-from django.http import HttpResponse, HttpResponseBadRequest
-from django.views.decorators.http import require_POST
-from django.core.cache import cache
-from django.core.exceptions import PermissionDenied
-from django.shortcuts import render
-
-from django_ses import settings
-from django_ses import signals
-from django_ses import utils
-
 logger = logging.getLogger(__name__)
 
 
 def superuser_only(view_func):
     """
     Limit a view to superuser only.
     """
@@ -95,15 +89,16 @@
 
 
 @superuser_only
 def dashboard(request):
     """
     Graph SES send statistics over time.
     """
-    warnings.warn('This view will be removed in future versions. Consider using DashboardView instead', DeprecationWarning)
+    warnings.warn('This view will be removed in future versions. Consider using DashboardView instead',
+                  DeprecationWarning)
     cache_key = 'vhash:django_ses_stats'
     cached_view = cache.get(cache_key)
     if cached_view:
         return cached_view
 
     ses_conn = boto3.client(
         'ses',
@@ -166,15 +161,15 @@
 
         quota_dict = ses_conn.get_send_quota()
         verified_emails_dict = ses_conn.list_verified_email_addresses()
         stats = ses_conn.get_send_statistics()
         verified_emails = emails_parse(verified_emails_dict)
         ordered_data = stats_to_list(stats)
         summary = sum_stats(ordered_data)
-        
+
         context.update({
             'title': 'SES Statistics',
             'datapoints': ordered_data,
             '24hour_quota': quota_dict['Max24HourSend'],
             '24hour_sent': quota_dict['SentLast24Hours'],
             '24hour_remaining':
                 quota_dict['Max24HourSend'] -
@@ -189,15 +184,15 @@
         return context
 
     def get(self, request, *args, **kwargs):
         cache_key = 'vhash:django_ses_stats'
         cached_view = cache.get(cache_key)
         if cached_view:
             return cached_view
-        
+
         response = super().get(request, *args, **kwargs).render()
         cache.set(cache_key, response, 60 * 15)  # Cache for 15 minutes
         return response
 
 
 @require_POST
 def handle_bounce(request):
```

### Comparing `django_ses-3.5.2/example/settings.py` & `django_ses-3.6.0/example/settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.5.2/example/templates/send-email.html` & `django_ses-3.6.0/example/templates/send-email.html`

 * *Files identical despite different names*

### Comparing `django_ses-3.5.2/example/urls.py` & `django_ses-3.6.0/example/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,12 @@
     re_path(r'^admin/doc/', include('django.contrib.admindocs.urls')),
     re_path(r'^admin/', include(admin.site.urls)),
 
     re_path(r'^$', views.index, name='index'),
     re_path(r'^send-email/$', views.send_email, name='send-email'),
     re_path(r'^reporting/', include('django_ses.urls')),
 
-    re_path(r'^bounce/', 'django_ses.views.handle_bounce', name='handle_bounce'),       # Deprecated, see SESEventWebhookView.
+    re_path(r'^bounce/', 'django_ses.views.handle_bounce', name='handle_bounce'),  # Deprecated, see SESEventWebhookView
     re_path(r'^event-webhook/', SESEventWebhookView.as_view(), name='event_webhook'),
 ]
 
 urlpatterns += staticfiles_urlpatterns()
```

### Comparing `django_ses-3.5.2/example/views.py` & `django_ses-3.6.0/example/views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.5.2/tests/test_backend.py` & `django_ses-3.6.0/tests/test_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import email
 
 from django.conf import settings as django_settings
-from django.utils.encoding import smart_str
 from django.core.mail import send_mail
 from django.test import TestCase
+from django.utils.encoding import smart_str
 
 import django_ses
 from django_ses import settings
 
 # random key generated with `openssl genrsa 512`
 DKIM_PRIVATE_KEY = '''
 -----BEGIN RSA PRIVATE KEY-----
@@ -111,25 +111,39 @@
         unicode_from_addr = 'Unicode Name óóóóóó <from@example.com>'
         rfc2047_encoded_from_addr = '=?utf-8?b?VW5pY29kZSBOYW1lIMOzw7PDs8Ozw7PDsw==?= <from@example.com>'
         self.assertEqual(self._rfc2047_helper(unicode_from_addr), rfc2047_encoded_from_addr)
 
     def test_send_mail(self):
         settings.AWS_SES_CONFIGURATION_SET = None
 
-        unicode_from_addr = 'Unicode Name óóóóóó <from@example.com>'
+        from_addr = 'Albertus Magnus <albertus.magnus@example.com>'
 
-        send_mail('subject', 'body', unicode_from_addr, ['to@example.com'])
+        send_mail('subject', 'body', from_addr, ['to@example.com'])
         message = self.outbox.pop()
         mail = email.message_from_string(smart_str(message['RawMessage']['Data']))
         self.assertTrue('X-SES-CONFIGURAITON-SET' not in mail.keys())
         self.assertEqual(mail['subject'], 'subject')
-        self.assertEqual(mail['from'], self._rfc2047_helper(unicode_from_addr))
+        self.assertEqual(mail['from'], self._rfc2047_helper(from_addr))
         self.assertEqual(mail['to'], 'to@example.com')
         self.assertEqual(mail.get_payload(), 'body')
 
+    def test_send_mail_unicode_body(self):
+        settings.AWS_SES_CONFIGURATION_SET = None
+
+        unicode_from_addr = 'Unicode Name óóóóóó <from@example.com>'
+
+        send_mail('Scandinavian', 'Sören & Björn', unicode_from_addr, ['to@example.com'])
+        message = self.outbox.pop()
+        mail = email.message_from_string(smart_str(message['RawMessage']['Data']))
+        self.assertTrue('X-SES-CONFIGURAITON-SET' not in mail.keys())
+        self.assertEqual(mail['subject'], 'Scandinavian')
+        self.assertEqual(mail['from'], self._rfc2047_helper(unicode_from_addr))
+        self.assertEqual(mail['to'], 'to@example.com')
+        self.assertEqual(mail.get_payload(), 'Sören & Björn')
+
     def test_configuration_set_send_mail(self):
         settings.AWS_SES_CONFIGURATION_SET = 'test-set'
         send_mail('subject', 'body', 'from@example.com', ['to@example.com'])
         message = self.outbox.pop()
         mail = email.message_from_string(smart_str(message['RawMessage']['Data']))
         self.assertEqual(mail['X-SES-CONFIGURATION-SET'], 'test-set')
         self.assertEqual(mail['subject'], 'subject')
@@ -268,15 +282,15 @@
         """
         Ensure that the notification address argument uses FeedbackForwardingEmailAddress.
         """
         settings.AWS_SES_RETURN_PATH = 'reply@example.com'
         send_mail('subject', 'body', 'from@example.com', ['to@example.com'])
         self.assertEqual(self.outbox.pop()['FeedbackForwardingEmailAddress'], 'reply@example.com')
 
-    def test_source_arn_is_NOT_set(self):
+    def test_source_arn_is_not_set(self):
         """
         Ensure that the helpers for Identity Owner for SES Sending Authorization are not present, if nothing has been
         configured.
         """
         send_mail('subject', 'body', 'from@example.com', ['to@example.com'])
         mail = self.outbox.pop()
         self.assertNotIn('FromEmailAddressIdentityArn', mail)
@@ -284,26 +298,28 @@
     def test_source_arn_is_set(self):
         """
         Ensure that the helpers for Identity Owner for SES Sending Authorization are set correctly.
         """
         settings.AWS_SES_SOURCE_ARN = 'arn:aws:ses:eu-central-1:111111111111:identity/example.com'
         send_mail('subject', 'body', 'from@example.com', ['to@example.com'])
         mail = self.outbox.pop()
-        self.assertEqual(mail['FromEmailAddressIdentityArn'], 'arn:aws:ses:eu-central-1:111111111111:identity/example.com')
+        self.assertEqual(mail['FromEmailAddressIdentityArn'],
+                         'arn:aws:ses:eu-central-1:111111111111:identity/example.com')
 
     def test_from_arn_takes_precedence_when_source_arn_is_set(self):
         """
         Ensure that the helpers for Identity Owner for SES Sending Authorization are set correctly.
         """
         settings.AWS_SES_SOURCE_ARN = 'arn:aws:ses:eu-central-1:111111111111:identity/example.com'
         settings.AWS_SES_FROM_ARN = 'arn:aws:ses:eu-central-1:222222222222:identity/example.com'
         settings.AWS_SES_RETURN_PATH_ARN = 'arn:aws:ses:eu-central-1:333333333333:identity/example.com'
         send_mail('subject', 'body', 'from@example.com', ['to@example.com'])
         mail = self.outbox.pop()
-        self.assertEqual(mail['FromEmailAddressIdentityArn'], 'arn:aws:ses:eu-central-1:222222222222:identity/example.com')
+        self.assertEqual(mail['FromEmailAddressIdentityArn'],
+                         'arn:aws:ses:eu-central-1:222222222222:identity/example.com')
 
 
 class SESBackendTestInitialize(TestCase):
     def test_auto_throttle(self):
         """
         Ensure that SESBackend handles aws_auto_throttle correctly
         """
@@ -330,20 +346,20 @@
         django_settings.EMAIL_BACKEND = 'tests.test_backend.FakeSESBackend'
         django_ses.SESConnection = FakeSESConnection
         self.outbox = FakeSESConnection.outbox
 
     def tearDown(self):
         # Empty outbox everytime test finishes
         FakeSESConnection.outbox = []
-    
+
     def test_from_email(self):
         settings.AWS_SES_FROM_EMAIL = "my_default_from@example.com"
         send_mail('subject', 'body', 'ignored_from@example.com', ['to@example.com'])
         self.assertEqual(self.outbox.pop()['Source'], 'my_default_from@example.com')
-    
+
     def test_return_path(self):
         settings.USE_SES_V2 = True
         settings.AWS_SES_RETURN_PATH = "return@example.com"
         send_mail('subject', 'body', 'from@example.com', ['to@example.com'])
         message = self.outbox.pop()
 
         self.assertEqual(message['FromEmailAddress'], 'my_default_from@example.com')
```

### Comparing `django_ses-3.5.2/tests/test_commands.py` & `django_ses-3.6.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.5.2/tests/test_settings.py` & `django_ses-3.6.0/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from django.test import TestCase
 from django.conf import settings
+from django.test import TestCase
+
 from tests.utils import unload_django_ses
 
 
 class SettingsImportTest(TestCase):
     def test_aws_access_key_given(self):
         settings.AWS_ACCESS_KEY_ID = "Yjc4MzQ4MGYzMTBhOWY3ODJhODhmNTBkN2QwY2IyZTdhZmU1NDM1ZQo"
         settings.AWS_SECRET_ACCESS_KEY = "NTBjYzAzNzVlMTA0N2FiMmFlODlhYjY5OTYwZjNkNjZmMWNhNzRhOQo"
@@ -38,15 +39,16 @@
         import django_ses
         self.assertEqual(django_ses.settings.AWS_SES_CONFIGURATION_SET, settings.AWS_SES_CONFIGURATION_SET)
 
     def test_ses_region_to_endpoint_default_given(self):
         unload_django_ses()
         import django_ses
         self.assertEqual(django_ses.settings.AWS_SES_REGION_NAME, 'us-east-1')
-        self.assertEqual(django_ses.settings.AWS_SES_REGION_ENDPOINT, f'email.{django_ses.settings.AWS_SES_REGION_NAME}.amazonaws.com')
+        self.assertEqual(django_ses.settings.AWS_SES_REGION_ENDPOINT,
+                         f'email.{django_ses.settings.AWS_SES_REGION_NAME}.amazonaws.com')
 
     def test_ses_region_to_endpoint_set_given(self):
         settings.AWS_SES_REGION_NAME = 'eu-west-1'
         unload_django_ses()
         import django_ses
         self.assertEqual(django_ses.settings.AWS_SES_REGION_NAME, 'eu-west-1')
-        self.assertEqual(django_ses.settings.AWS_SES_REGION_ENDPOINT, 'email.eu-west-1.amazonaws.com')
+        self.assertEqual(django_ses.settings.AWS_SES_REGION_ENDPOINT, 'email.eu-west-1.amazonaws.com')
```

### Comparing `django_ses-3.5.2/tests/test_stats.py` & `django_ses-3.6.0/tests/test_stats.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import pytz
 from datetime import datetime
 
+import pytz
 from django.test import TestCase
 
 from django_ses.views import emails_parse, stats_to_list, sum_stats
 
 # Mock of what boto's SESConnection.get_send_statistics() returns
 STATS_DICT = {
     'SendDataPoints': [
```

### Comparing `django_ses-3.5.2/tests/test_verifier.py` & `django_ses-3.6.0/tests/test_verifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,41 +28,105 @@
         "MessageId": "Some ID",
         "Subject": "Equity for all",
         "Timestamp": "Yesterday",
         "TopicArn": "arn:aws...",
         "Type": "Notification",
     }
 
-    VALID_CERT = b"-----BEGIN CERTIFICATE-----\nMIIF1zCCBL+gAwIBAgIQB9pYWG3Mi7xej22g9pobJTANBgkqhkiG9w0BAQsFADBG\nMQswCQYDVQQGEwJVUzEPMA0GA1UEChMGQW1hem9uMRUwEwYDVQQLEwxTZXJ2ZXIg\nQ0EgMUIxDzANBgNVBAMTBkFtYXpvbjAeFw0yMTA5MDcwMDAwMDBaFw0yMjA4MTcy\nMzU5NTlaMBwxGjAYBgNVBAMTEXNucy5hbWF6b25hd3MuY29tMIIBIjANBgkqhkiG\n9w0BAQEFAAOCAQ8AMIIBCgKCAQEAutFqueT3XgP13udzxE6UpbdjOtVO5DwoMpSM\niDNMnGzF1TYH5/R2LPUOBeTB0SkKnR4kpNcUZhicpGD4aKciz/GEZ6wu65xncfT9\nH/KBOQwoXYTuClHwp6fYpGzcGFaFoEYMnijL/o4qmTSd+ukglQUgKpsDw4ofw6rU\nm2CttJo+GQSNQ9NfGR1h/0J+zsApkeSYrXRx5wNlu87z8os1C/6PBrUHwt3xXeaf\nXzfwut8aRRYsS8BySOA9DAgLfNHlfdQCjKPXKrG/ussgReyWD6n/HH+j7Uha3xos\nTzQqJifcxlTq6MxWdPR6fDaJNvqw6DOE7UjUNxHguXHlVfxhlQIDAQABo4IC6TCC\nAuUwHwYDVR0jBBgwFoAUWaRmBlKge5WSPKOUByeWdFv5PdAwHQYDVR0OBBYEFAqz\nC+vyouneE7mWWLbi9i0UsWUbMBwGA1UdEQQVMBOCEXNucy5hbWF6b25hd3MuY29t\nMA4GA1UdDwEB/wQEAwIFoDAdBgNVHSUEFjAUBggrBgEFBQcDAQYIKwYBBQUHAwIw\nOwYDVR0fBDQwMjAwoC6gLIYqaHR0cDovL2NybC5zY2ExYi5hbWF6b250cnVzdC5j\nb20vc2NhMWIuY3JsMBMGA1UdIAQMMAowCAYGZ4EMAQIBMHUGCCsGAQUFBwEBBGkw\nZzAtBggrBgEFBQcwAYYhaHR0cDovL29jc3Auc2NhMWIuYW1hem9udHJ1c3QuY29t\nMDYGCCsGAQUFBzAChipodHRwOi8vY3J0LnNjYTFiLmFtYXpvbnRydXN0LmNvbS9z\nY2ExYi5jcnQwDAYDVR0TAQH/BAIwADCCAX0GCisGAQQB1nkCBAIEggFtBIIBaQFn\nAHYAKXm+8J45OSHwVnOfY6V35b5XfZxgCvj5TV0mXCVdx4QAAAF7vfDVkQAABAMA\nRzBFAiEA2XfHuy36aqRFiaL8c3md2mH451go8707+fRE0pEdSRACIE/g5FXTUXUZ\nPFcmOhm9TZ+uMY1i4CIQ/CKVWln6C3t+AHYAUaOw9f0BeZxWbbg3eI8MpHrMGyfL\n956IQpoN/tSLBeUAAAF7vfDVjAAABAMARzBFAiBF1MhhFP0+FQt3daDFfMYoWwnr\nmuTInrjNpwfzlvQBugIhAPYadFzr+LaxSJoiZEbEHBvTts7bT0M3eCQONA2O7w6n\nAHUAQcjKsd8iRkoQxqE6CUKHXk4xixsD6+tLx2jwkGKWBvYAAAF7vfDVdAAABAMA\nRjBEAiAtPapmFAuA71ih4NoSd5hJelzAltNQpxDMcDfDyHyU8gIgWxmaa6+2KbBu\n9xdv379zvnJACFR7jc+4asl08Dn4aagwDQYJKoZIhvcNAQELBQADggEBAA54QX0u\noFWXfMmv02CGZv4NWo5TapyeeixQ2kKpZHRdVZjxZrw+hoF6HD7P3kGjH8ztyJll\ntDxB0qgMltbPhQdScwhA6iTgoaBYqEUC/VHKd4PmmPT6yIsM36NBZVmkGlzl5uNo\n/dBgBaG0SsVJnhr5zro3c2quC7n6fVGEZhf/UgQwRnnvThnvbNKguglDMq4uEqv8\nnjKyleht+glkcmXO0m9qLKt6BOS0amy6U2GlAwRn0Wx02ndJtnRCSC6kPuRWK/SQ\nFEjB7gCK4hdKaAOuWdZpI55vF6ifOeM8toC3g7ofO8qLTnJupAG+ZitY5J3cvHWr\nHqOUdKigPDHYLRo=\n-----END CERTIFICATE-----\n"
+    VALID_CERT = (b"-----BEGIN CERTIFICATE-----\nMIIF1zCCBL+gAwIBAgIQB9pYWG3Mi7xej22g9pobJTANBgkqhkiG9w0BAQsFADBG\n"
+                  b"MQswCQYDVQQGEwJVUzEPMA0GA1UEChMGQW1hem9uMRUwEwYDVQQLEwxTZXJ2ZXIg\nQ0EgMUIxDzANBgNVBAMTBkFtYXpvb"
+                  b"jAeFw0yMTA5MDcwMDAwMDBaFw0yMjA4MTcy\nMzU5NTlaMBwxGjAYBgNVBAMTEXNucy5hbWF6b25hd3MuY29tMIIBIjANBg"
+                  b"kqhkiG\n9w0BAQEFAAOCAQ8AMIIBCgKCAQEAutFqueT3XgP13udzxE6UpbdjOtVO5DwoMpSM\niDNMnGzF1TYH5/R2LPUOB"
+                  b"eTB0SkKnR4kpNcUZhicpGD4aKciz/GEZ6wu65xncfT9\nH/KBOQwoXYTuClHwp6fYpGzcGFaFoEYMnijL/o4qmTSd+ukglQ"
+                  b"UgKpsDw4ofw6rU\nm2CttJo+GQSNQ9NfGR1h/0J+zsApkeSYrXRx5wNlu87z8os1C/6PBrUHwt3xXeaf\nXzfwut8aRRYsS"
+                  b"8BySOA9DAgLfNHlfdQCjKPXKrG/ussgReyWD6n/HH+j7Uha3xos\nTzQqJifcxlTq6MxWdPR6fDaJNvqw6DOE7UjUNxHguX"
+                  b"HlVfxhlQIDAQABo4IC6TCC\nAuUwHwYDVR0jBBgwFoAUWaRmBlKge5WSPKOUByeWdFv5PdAwHQYDVR0OBBYEFAqz\nC+vyo"
+                  b"uneE7mWWLbi9i0UsWUbMBwGA1UdEQQVMBOCEXNucy5hbWF6b25hd3MuY29t\nMA4GA1UdDwEB/wQEAwIFoDAdBgNVHSUEFj"
+                  b"AUBggrBgEFBQcDAQYIKwYBBQUHAwIw\nOwYDVR0fBDQwMjAwoC6gLIYqaHR0cDovL2NybC5zY2ExYi5hbWF6b250cnVzdC5"
+                  b"j\nb20vc2NhMWIuY3JsMBMGA1UdIAQMMAowCAYGZ4EMAQIBMHUGCCsGAQUFBwEBBGkw\nZzAtBggrBgEFBQcwAYYhaHR0cD"
+                  b"ovL29jc3Auc2NhMWIuYW1hem9udHJ1c3QuY29t\nMDYGCCsGAQUFBzAChipodHRwOi8vY3J0LnNjYTFiLmFtYXpvbnRydXN"
+                  b"0LmNvbS9z\nY2ExYi5jcnQwDAYDVR0TAQH/BAIwADCCAX0GCisGAQQB1nkCBAIEggFtBIIBaQFn\nAHYAKXm+8J45OSHwVn"
+                  b"OfY6V35b5XfZxgCvj5TV0mXCVdx4QAAAF7vfDVkQAABAMA\nRzBFAiEA2XfHuy36aqRFiaL8c3md2mH451go8707+fRE0pE"
+                  b"dSRACIE/g5FXTUXUZ\nPFcmOhm9TZ+uMY1i4CIQ/CKVWln6C3t+AHYAUaOw9f0BeZxWbbg3eI8MpHrMGyfL\n956IQpoN/t"
+                  b"SLBeUAAAF7vfDVjAAABAMARzBFAiBF1MhhFP0+FQt3daDFfMYoWwnr\nmuTInrjNpwfzlvQBugIhAPYadFzr+LaxSJoiZEb"
+                  b"EHBvTts7bT0M3eCQONA2O7w6n\nAHUAQcjKsd8iRkoQxqE6CUKHXk4xixsD6+tLx2jwkGKWBvYAAAF7vfDVdAAABAMA\nRj"
+                  b"BEAiAtPapmFAuA71ih4NoSd5hJelzAltNQpxDMcDfDyHyU8gIgWxmaa6+2KbBu\n9xdv379zvnJACFR7jc+4asl08Dn4aag"
+                  b"wDQYJKoZIhvcNAQELBQADggEBAA54QX0u\noFWXfMmv02CGZv4NWo5TapyeeixQ2kKpZHRdVZjxZrw+hoF6HD7P3kGjH8zt"
+                  b"yJll\ntDxB0qgMltbPhQdScwhA6iTgoaBYqEUC/VHKd4PmmPT6yIsM36NBZVmkGlzl5uNo\n/dBgBaG0SsVJnhr5zro3c2q"
+                  b"uC7n6fVGEZhf/UgQwRnnvThnvbNKguglDMq4uEqv8\nnjKyleht+glkcmXO0m9qLKt6BOS0amy6U2GlAwRn0Wx02ndJtnRC"
+                  b"SC6kPuRWK/SQ\nFEjB7gCK4hdKaAOuWdZpI55vF6ifOeM8toC3g7ofO8qLTnJupAG+ZitY5J3cvHWr\nHqOUdKigPDHYLRo"
+                  b"=\n-----END CERTIFICATE-----\n")
     # Any changes to this message will break the signature validity test.
     valid_msg = {
         "Type": "Notification",
         "MessageId": "97903a0c-8818-5442-94b2-60b0c63d3da0",
         "TopicArn": "arn:aws:sns:us-east-1:364852123998:test-email",
         "Subject": "Amazon SES Email Event Notification",
-        "Message": '{"eventType":"Complaint","complaint":{"feedbackId":"0100017fd2f87864-7f070191-4eb1-49e3-a42e-7e996b718724-000000","complaintSubType":null,"complainedRecipients":[{"emailAddress":"complaint@simulator.amazonses.com"}],"timestamp":"2022-03-28T23:59:33.564Z","userAgent":"Amazon SES Mailbox Simulator","complaintFeedbackType":"abuse","arrivalDate":"2022-03-28T23:59:33.564Z"},"mail":{"timestamp":"2022-03-28T23:59:32.804Z","source":"jesus.islasf@alumno.buap.mx","sourceArn":"arn:aws:ses:us-east-1:364852123998:identity/jesus.islasf@alumno.buap.mx","sendingAccountId":"364852123998","messageId":"0100017fd2f875c4-c2929163-2767-49b1-8513-1a29e428e134-000000","destination":["complaint@simulator.amazonses.com"],"headersTruncated":false,"headers":[{"name":"From","value":"jesus.islasf@alumno.buap.mx"},{"name":"To","value":"complaint@simulator.amazonses.com"},{"name":"Subject","value":"Complaint Notification"},{"name":"MIME-Version","value":"1.0"},{"name":"Content-Type","value":"multipart/alternative;  boundary=\\"----=_Part_1160373_1543555432.1648511972808\\""}],"commonHeaders":{"from":["jesus.islasf@alumno.buap.mx"],"to":["complaint@simulator.amazonses.com"],"messageId":"0100017fd2f875c4-c2929163-2767-49b1-8513-1a29e428e134-000000","subject":"Complaint Notification"},"tags":{"ses:operation":["SendEmail"],"ses:configuration-set":["test-set"],"ses:source-ip":["189.203.131.80"],"ses:from-domain":["alumno.buap.mx"],"ses:caller-identity":["root"]}}}\n',
+        "Message": '{"eventType":"Complaint","complaint":{"feedbackId":"0100017fd2f87864-7f070191-4eb1-49e3-a42e-'
+                   '7e996b718724-000000","complaintSubType":null,"complainedRecipients":[{"emailAddress":'
+                   '"complaint@simulator.amazonses.com"}],"timestamp":"2022-03-28T23:59:33.564Z","userAgent":'
+                   '"Amazon SES Mailbox Simulator","complaintFeedbackType":"abuse","arrivalDate":'
+                   '"2022-03-28T23:59:33.564Z"},"mail":{"timestamp":"2022-03-28T23:59:32.804Z","source":'
+                   '"jesus.islasf@alumno.buap.mx","sourceArn":"arn:aws:ses:us-east-1:364852123998:'
+                   'identity/jesus.islasf@alumno.buap.mx","sendingAccountId":"364852123998","messageId":'
+                   '"0100017fd2f875c4-c2929163-2767-49b1-8513-1a29e428e134-000000","destination":'
+                   '["complaint@simulator.amazonses.com"],"headersTruncated":false,"headers":[{"name":"From",'
+                   '"value":"jesus.islasf@alumno.buap.mx"},{"name":"To","value":"complaint@simulator.amazonses.com"},'
+                   '{"name":"Subject","value":"Complaint Notification"},{"name":"MIME-Version","value":"1.0"},'
+                   '{"name":"Content-Type","value":"multipart/alternative;  '
+                   'boundary=\\"----=_Part_1160373_1543555432.1648511972808\\""}],"commonHeaders":{"from":'
+                   '["jesus.islasf@alumno.buap.mx"],"to":["complaint@simulator.amazonses.com"],"messageId":'
+                   '"0100017fd2f875c4-c2929163-2767-49b1-8513-1a29e428e134-000000","subject":'
+                   '"Complaint Notification"},"tags":{"ses:operation":["SendEmail"],"ses:configuration-set":'
+                   '["test-set"],"ses:source-ip":["189.203.131.80"],"ses:from-domain":["alumno.buap.mx"],'
+                   '"ses:caller-identity":["root"]}}}\n',
         "Timestamp": "2022-03-28T23:59:33.713Z",
         "SignatureVersion": "1",
-        "Signature": "MAnUSvI5C6S0GERh05oFiMtpZuGTW0J/6I/AaBinsZWK+Na8TwJsiNSUjShgZ8NItzQkjBnY1R1qT0wtPf6FfNXxGu3oQRaYsj1alz5NJyiuZwGlryX9LHuOoSJ7tGhrKA5yfYI1JPZsdUJKnkI3+UgKbIg7ml2FoSMU8s3HP3V/FOhvp6V5P6yt2okxABbw13WQPrzeUCZ9pRLgB3TnY59wsWM2SlynWEG/u/pFHyzuvkmtrGZtjZfITm7bfMnGy8FTOox4PfzCu4bysKlUbhc/yJ0fzI/+XsT2gKasXETzlmx6vd4qKgKWP5U9OJVh+Cx//npFDCBI2Tba8JK+Cg==",
-        "SigningCertURL": "https://sns.us-east-1.amazonaws.com/SimpleNotificationService-7ff5318490ec183fbaddaa2a969abfda.pem",
-        "UnsubscribeURL": "https://sns.us-east-1.amazonaws.com/?Action=Unsubscribe&SubscriptionArn=arn:aws:sns:us-east-1:364852123998:test-email:0fe0bffc-6470-4502-9414-d5e3d9fdd71e",
+        "Signature": "MAnUSvI5C6S0GERh05oFiMtpZuGTW0J/6I/AaBinsZWK+Na8TwJsiNSUjShgZ8NItzQkjBnY1R1qT0wtPf6FfNXxGu3"
+                     "oQRaYsj1alz5NJyiuZwGlryX9LHuOoSJ7tGhrKA5yfYI1JPZsdUJKnkI3+UgKbIg7ml2FoSMU8s3HP3V/FOhvp6V5P6y"
+                     "t2okxABbw13WQPrzeUCZ9pRLgB3TnY59wsWM2SlynWEG/u/pFHyzuvkmtrGZtjZfITm7bfMnGy8FTOox4PfzCu4bysKl"
+                     "Ubhc/yJ0fzI/+XsT2gKasXETzlmx6vd4qKgKWP5U9OJVh+Cx//npFDCBI2Tba8JK+Cg==",
+        "SigningCertURL":
+            "https://sns.us-east-1.amazonaws.com/SimpleNotificationService-7ff5318490ec183fbaddaa2a969abfda.pem",
+        "UnsubscribeURL": "https://sns.us-east-1.amazonaws.com/?Action=Unsubscribe&SubscriptionArn=arn:aws:sns:"
+                          "us-east-1:364852123998:test-email:0fe0bffc-6470-4502-9414-d5e3d9fdd71e",
     }
 
     valid_msg_missing_fields = {
         "Type": "Notification",
         "MessageId": "71a6b82e-0f1a-58db-b902-e2ef60f87541",
         "TopicArn": "arn:aws:sns:us-east-1:364852123998:test-email",
         # Normally you'd see a subject key/value pair here, but not on this
         # notification.
-        "Message": '{"notificationType":"Bounce","bounce":{"feedbackId":"0100017fe7044080-b95aeb18-3fb8-408a-be9b-15fdbac3945a-000000","bounceType":"Permanent","bounceSubType":"General","bouncedRecipients":[{"emailAddress":"bounce@simulator.amazonses.com","action":"failed","status":"5.1.1","diagnosticCode":"smtp; 550 5.1.1 user unknown"}],"timestamp":"2022-04-01T21:24:49.000Z","remoteMtaIp":"3.231.136.178","reportingMTA":"dns; a48-30.smtp-out.amazonses.com"},"mail":{"timestamp":"2022-04-01T21:24:49.422Z","source":"jesus.islasf@alumno.buap.mx","sourceArn":"arn:aws:ses:us-east-1:364852123998:identity/jesus.islasf@alumno.buap.mx","sourceIp":"189.203.131.80","sendingAccountId":"364852123998","messageId":"0100017fe7043e8e-fc9c357d-a9a4-49bc-a4b4-fa984009d568-000000","destination":["bounce@simulator.amazonses.com"],"headersTruncated":false,"headers":[{"name":"From","value":"jesus.islasf@alumno.buap.mx"},{"name":"To","value":"bounce@simulator.amazonses.com"},{"name":"Subject","value":"Subject Test"},{"name":"MIME-Version","value":"1.0"},{"name":"Content-Type","value":"multipart/alternative;  boundary=\\"----=_Part_2196631_1474166380.1648848289426\\""}],"commonHeaders":{"from":["jesus.islasf@alumno.buap.mx"],"to":["bounce@simulator.amazonses.com"],"subject":"Subject Test"}}}',
+        "Message": '{"notificationType":"Bounce","bounce":{"feedbackId":"0100017fe7044080-b95aeb18-3fb8-408a-be9b-'
+                   '15fdbac3945a-000000","bounceType":"Permanent","bounceSubType":"General","bouncedRecipients":['
+                   '{"emailAddress":"bounce@simulator.amazonses.com","action":"failed","status":"5.1.1",'
+                   '"diagnosticCode":"smtp; 550 5.1.1 user unknown"}],"timestamp":"2022-04-01T21:24:49.000Z",'
+                   '"remoteMtaIp":"3.231.136.178","reportingMTA":"dns; a48-30.smtp-out.amazonses.com"},"mail":'
+                   '{"timestamp":"2022-04-01T21:24:49.422Z","source":"jesus.islasf@alumno.buap.mx","sourceArn":'
+                   '"arn:aws:ses:us-east-1:364852123998:identity/jesus.islasf@alumno.buap.mx","sourceIp":'
+                   '"189.203.131.80","sendingAccountId":"364852123998","messageId":'
+                   '"0100017fe7043e8e-fc9c357d-a9a4-49bc-a4b4-fa984009d568-000000","destination":'
+                   '["bounce@simulator.amazonses.com"],"headersTruncated":false,"headers":[{"name":'
+                   '"From","value":"jesus.islasf@alumno.buap.mx"},{"name":"To","value":'
+                   '"bounce@simulator.amazonses.com"},{"name":"Subject","value":"Subject Test"},'
+                   '{"name":"MIME-Version","value":"1.0"},{"name":"Content-Type","value":'
+                   '"multipart/alternative;  boundary=\\"----=_Part_2196631_1474166380.1648848289426\\""}],'
+                   '"commonHeaders":{"from":["jesus.islasf@alumno.buap.mx"],"to":["bounce@simulator.amazonses.com"],'
+                   '"subject":"Subject Test"}}}',
         "Timestamp": "2022-04-01T21:24:50.200Z",
         "SignatureVersion": "1",
-        "Signature": "K27nwTcT0qTPKEQP3noOWV21gDGB6XnLXSwN2i+4176naErwyDSd72w44UesYE/KaRXU+Kusi7b8uoLYPOcYXHH45UCFMrStf9nzu0uIZdMSd7cFGPm0KAxqoDcP9UQw0+ssK1rjVWkywTYmeDyFF/j3IQZxTA/vINOLYbrmMKhyJUPjcZZwdgLmlKcNfKJ5PKmg5WXlr8nWtjW3K+k725nkoAZemuAFt3PmA2k35JoHphkcOBjV2f1qR9zJTOgrVQ1d6k2v6t8G7Nlg6FP5OiwThgKHkehIPfJfLhTmo05tfPCBzXYMzDbnX+HLidvkyibHlalRl/DuDxXXL7SUiA==",
-        "SigningCertURL": "https://sns.us-east-1.amazonaws.com/SimpleNotificationService-7ff5318490ec183fbaddaa2a969abfda.pem",
-        "UnsubscribeURL": "https://sns.us-east-1.amazonaws.com/?Action=Unsubscribe&SubscriptionArn=arn:aws:sns:us-east-1:364852123998:test-email:0fe0bffc-6470-4502-9414-d5e3d9fdd71e",
+        "Signature": "K27nwTcT0qTPKEQP3noOWV21gDGB6XnLXSwN2i+4176naErwyDSd72w44UesYE/KaRXU+Kusi7b8uoLYPOcYXHH45UCFMrSt"
+                     "f9nzu0uIZdMSd7cFGPm0KAxqoDcP9UQw0+ssK1rjVWkywTYmeDyFF/j3IQZxTA/vINOLYbrmMKhyJUPjcZZwdgLmlKcNfKJ5"
+                     "PKmg5WXlr8nWtjW3K+k725nkoAZemuAFt3PmA2k35JoHphkcOBjV2f1qR9zJTOgrVQ1d6k2v6t8G7Nlg6FP5OiwThgKHkehI"
+                     "PfJfLhTmo05tfPCBzXYMzDbnX+HLidvkyibHlalRl/DuDxXXL7SUiA==",
+        "SigningCertURL": "https://sns.us-east-1.amazonaws.com/SimpleNotificationService-"
+                          "7ff5318490ec183fbaddaa2a969abfda.pem",
+        "UnsubscribeURL": "https://sns.us-east-1.amazonaws.com/?Action=Unsubscribe&SubscriptionArn="
+                          "arn:aws:sns:us-east-1:364852123998:test-email:0fe0bffc-6470-4502-9414-d5e3d9fdd71e",
     }
 
     def tearDown(self):
         # Reset the cache after each test
         clear_cert_cache()
 
     @skipIf(requests is None, "requests is not installed")
```

### Comparing `django_ses-3.5.2/tests/test_views.py` & `django_ses-3.6.0/tests/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,23 @@
     from unittest import mock
 except ImportError:
     import mock
 
 from django.test import TestCase
 from django.urls import reverse
 
-from django_ses.signals import bounce_received, complaint_received, send_received, delivery_received, open_received, \
-    click_received
 from django_ses import utils as ses_utils
+from django_ses.signals import (
+    bounce_received,
+    click_received,
+    complaint_received,
+    delivery_received,
+    open_received,
+    send_received,
+)
 
 
 def get_mock_email():
     return {
         "timestamp": "2012-05-25T14:59:38.623-07:00",
         "messageId": "000001378603177f-7a5433e7-8edb-42ae-af10-f0181f34d6ee-000000",
         "source": "sender@example.com",
@@ -121,15 +127,16 @@
 
 
 def get_mock_click():
     mail = get_mock_email()
     click = {
         "timestamp": "2021-01-26T14:38:55.540Z",
         "ipAddress": "11.111.11.111",
-        "userAgent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15",
+        "userAgent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) "
+                     "Version/14.0 Safari/605.1.15",
         "link": "github.com/django-ses/django-ses",
         "linkTags": None
     }
     message = {
         "eventType": "Click",
         "mail": mail,
         "click": click,
@@ -167,15 +174,16 @@
         _handler.call_count = 0
         bounce_received.connect(_handler)
 
         # Mock the verification
         with mock.patch.object(ses_utils, "verify_event_message") as verify:
             verify.return_value = True
 
-            response = self.client.post(reverse("django_ses_bounce"), json.dumps(notification), content_type="application/json")
+            response = self.client.post(reverse("django_ses_bounce"), json.dumps(notification),
+                                        content_type="application/json")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(_handler.call_count, 1)
 
     def test_handle_bounce_notification(self):
         """
         Test handling a normal bounce request.
         """
@@ -189,15 +197,16 @@
         _handler.call_count = 0
         bounce_received.connect(_handler)
 
         # Mock the verification
         with mock.patch.object(ses_utils, "verify_event_message") as verify:
             verify.return_value = True
 
-            response = self.client.post(reverse("django_ses_bounce"), json.dumps(notification), content_type="application/json")
+            response = self.client.post(reverse("django_ses_bounce"), json.dumps(notification),
+                                        content_type="application/json")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(_handler.call_count, 1)
 
 
 class HandleEventTestCase(TestCase):
     """
     Test the event web hook handler.
@@ -226,15 +235,16 @@
             self.assertEqual(raw_message, json.dumps(notification).encode())
         _handler.call_count = 0
         bounce_received.connect(_handler)
 
         # Mock the verification
         with mock.patch.object(ses_utils, "verify_event_message") as verify:
             verify.return_value = True
-            response = self.client.post(reverse("event_webhook"), json.dumps(notification), content_type="application/json")
+            response = self.client.post(reverse("event_webhook"), json.dumps(notification),
+                                        content_type="application/json")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(_handler.call_count, 1)
 
 
     def test_handle_bounce_notification(self):
         """
         Test handling a normal bounce request.
@@ -248,15 +258,16 @@
             self.assertEqual(raw_message, json.dumps(notification).encode())
         _handler.call_count = 0
         bounce_received.connect(_handler)
 
         # Mock the verification
         with mock.patch.object(ses_utils, "verify_event_message") as verify:
             verify.return_value = True
-            response = self.client.post(reverse("event_webhook"), json.dumps(notification), content_type="application/json")
+            response = self.client.post(reverse("event_webhook"), json.dumps(notification),
+                                        content_type="application/json")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(_handler.call_count, 1)
 
 
     def test_handle_send_event(self):
         """
         Test handling a send event request.
@@ -270,15 +281,16 @@
             self.assertEqual(raw_message, json.dumps(notification).encode())
         _handler.call_count = 0
         send_received.connect(_handler)
 
         # Mock the verification
         with mock.patch.object(ses_utils, "verify_event_message") as verify:
             verify.return_value = True
-            response = self.client.post(reverse("event_webhook"), json.dumps(notification), content_type="application/json")
+            response = self.client.post(reverse("event_webhook"), json.dumps(notification),
+                                        content_type="application/json")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(_handler.call_count, 1)
 
     def test_handle_delivery_event(self):
         """
         Test handling a delivery event request.
         """
@@ -291,15 +303,16 @@
             self.assertEqual(raw_message, json.dumps(notification).encode())
         _handler.call_count = 0
         delivery_received.connect(_handler)
 
         # Mock the verification
         with mock.patch.object(ses_utils, "verify_event_message") as verify:
             verify.return_value = True
-            response = self.client.post(reverse("event_webhook"), json.dumps(notification), content_type="application/json")
+            response = self.client.post(reverse("event_webhook"), json.dumps(notification),
+                                        content_type="application/json")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(_handler.call_count, 1)
 
     def test_handle_open_event(self):
         """
         Test handling a open event request.
         """
@@ -312,15 +325,16 @@
             self.assertEqual(raw_message, json.dumps(notification).encode())
         _handler.call_count = 0
         open_received.connect(_handler)
 
         # Mock the verification
         with mock.patch.object(ses_utils, "verify_event_message") as verify:
             verify.return_value = True
-            response = self.client.post(reverse("event_webhook"), json.dumps(notification), content_type="application/json")
+            response = self.client.post(reverse("event_webhook"), json.dumps(notification),
+                                        content_type="application/json")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(_handler.call_count, 1)
 
     def test_handle_click_event(self):
         """
         Test handling a click event request.
         """
@@ -333,15 +347,16 @@
             self.assertEqual(raw_message, json.dumps(notification).encode())
         _handler.call_count = 0
         click_received.connect(_handler)
 
         # Mock the verification
         with mock.patch.object(ses_utils, "verify_event_message") as verify:
             verify.return_value = True
-            response = self.client.post(reverse("event_webhook"), json.dumps(notification), content_type="application/json")
+            response = self.client.post(reverse("event_webhook"), json.dumps(notification),
+                                        content_type="application/json")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(_handler.call_count, 1)
 
     def test_bad_json(self):
         """
         Test request with invalid JSON.
         """
@@ -354,10 +369,11 @@
         Test handling a click event request.
         """
         req_mail_obj, req_click_obj, notification = get_mock_click()
 
         # Mock the verification
         with mock.patch.object(ses_utils, "verify_event_message") as verify:
             verify.return_value = False
-            response = self.client.post(reverse("event_webhook"), json.dumps(notification), content_type="application/json")
+            response = self.client.post(reverse("event_webhook"), json.dumps(notification),
+                                        content_type="application/json")
         self.assertEqual(response.status_code, 400)
         self.assertEqual(response.content, "Signature verification failed.".encode())
```

### Comparing `django_ses-3.5.2/PKG-INFO` & `django_ses-3.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ses
-Version: 3.5.2
+Version: 3.6.0
 Summary: A Django email backend for Amazon's Simple Email Service (SES)
 Home-page: https://github.com/django-ses/django-ses
 License: MIT
 Author: Harry Marr
 Author-email: harry@hmarr.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,14 +29,17 @@
 Provides-Extra: events
 Requires-Dist: boto3 (>=1.0.0)
 Requires-Dist: cryptography (>=36.0.2) ; extra == "bounce" or extra == "events"
 Requires-Dist: django (>=2.2)
 Requires-Dist: importlib-metadata (>=1) ; python_version < "3.8"
 Requires-Dist: pytz (>=2016.10)
 Requires-Dist: requests (>=2.27.1) ; extra == "bounce" or extra == "events"
+Project-URL: Bugtracker, https://github.com/django-ses/django-ses/issues
+Project-URL: Changelog, https://github.com/django-ses/django-ses/blob/main/CHANGES.md
+Project-URL: Documentation, https://github.com/django-ses/django-ses/blob/main/README.rst
 Project-URL: Repository, https://github.com/django-ses/django-ses
 Description-Content-Type: text/x-rst
 
 ==========
 Django-SES
 ==========
 :Info: A Django email backend for Amazon's Simple Email Service
@@ -376,14 +379,25 @@
 =================
 
 Django SES comes with two ways of viewing sending statistics.
 
 The first one is a simple read-only report on your 24 hour sending quota,
 verified email addresses and bi-weekly sending statistics.
 
+To enable the dashboard to retrieve data from AWS, you need to update the IAM policy by adding the following actions::
+
+    {
+        "Effect": "Allow",
+        "Action": [
+            "ses:ListVerifiedEmailAddresses",
+            "ses:GetSendStatistics"
+        ],
+        "Resource": "*"
+    }
+
 To generate and view SES sending statistics reports, include, update
 ``INSTALLED_APPS``::
 
     INSTALLED_APPS = (
         # ...
         'django.contrib.admin',
         'django_ses',
@@ -607,14 +621,40 @@
 #. Check your code for errors, complaints.
     Use `check.py <https://github.com/jbalogh/check>`_
 
 #. Write and run tests.
     Write your own test showing the issue has been resolved, or the feature
     works as intended.
 
+Git hooks (via pre-commit)
+==========================
+
+We use pre-push hooks to ensure that only linted code reaches our remote repository and pipelines aren't triggered in
+vain.
+
+To enable the configured pre-push hooks, you need to [install](https://pre-commit.com/) pre-commit and run once::
+
+    pre-commit install -t pre-push -t pre-commit --install-hooks
+
+This will permanently install the git hooks for both, frontend and backend, in your local
+[`.git/hooks`](./.git/hooks) folder.
+The hooks are configured in the [`.pre-commit-config.yaml`](.pre-commit-config.yaml).
+
+You can check whether hooks work as intended using the [run](https://pre-commit.com/#pre-commit-run) command::
+
+    pre-commit run [hook-id] [options]
+
+Example: run single hook::
+
+    pre-commit run ruff --all-files --hook-stage push
+
+Example: run all hooks of pre-push stage::
+
+    pre-commit run --all-files --hook-stage push
+
 Running Tests
 =============
 To run the tests::
 
     python runtests.py
 
 If you want to debug the tests, just add this file as a python script to your IDE run configuration.
```

