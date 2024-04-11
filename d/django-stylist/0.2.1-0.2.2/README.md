# Comparing `tmp/django-stylist-0.2.1.tar.gz` & `tmp/django-stylist-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-stylist-0.2.1.tar", last modified: Wed Mar  1 00:31:19 2023, max compression
+gzip compressed data, was "dist/django-stylist-0.2.2.tar", last modified: Thu Apr 11 15:38:11 2024, max compression
```

## Comparing `django-stylist-0.2.1.tar` & `django-stylist-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:31:19.000000 django-stylist-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-01 00:31:19.000000 django-stylist-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-01 00:30:52.000000 django-stylist-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:31:19.000000 django-stylist-0.2.1/django_stylist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-01 00:31:19.000000 django-stylist-0.2.1/django_stylist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-01 00:31:19.000000 django-stylist-0.2.1/django_stylist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 00:31:19.000000 django-stylist-0.2.1/django_stylist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-01 00:31:19.000000 django-stylist-0.2.1/django_stylist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-01 00:31:19.000000 django-stylist-0.2.1/django_stylist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 00:31:19.000000 django-stylist-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-01 00:30:52.000000 django-stylist-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:31:19.000000 django-stylist-0.2.1/stylist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:31:19.000000 django-stylist-0.2.1/stylist/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:31:19.000000 django-stylist-0.2.1/stylist/management/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:31:19.000000 django-stylist-0.2.1/stylist/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/management/commands/build_scss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 00:31:19.000000 django-stylist-0.2.1/stylist/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/migrations/0002_auto_20210114_1901.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-03-01 00:30:52.000000 django-stylist-0.2.1/stylist/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:11.000000 django-stylist-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:37:37.000000 django-stylist-0.2.2/LICENSE.mit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-11 15:38:11.000000 django-stylist-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-11 15:37:37.000000 django-stylist-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:11.000000 django-stylist-0.2.2/django_stylist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-11 15:38:11.000000 django-stylist-0.2.2/django_stylist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-11 15:38:11.000000 django-stylist-0.2.2/django_stylist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:38:11.000000 django-stylist-0.2.2/django_stylist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-11 15:38:11.000000 django-stylist-0.2.2/django_stylist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 15:38:11.000000 django-stylist-0.2.2/django_stylist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:38:11.000000 django-stylist-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-11 15:37:37.000000 django-stylist-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:11.000000 django-stylist-0.2.2/stylist/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:11.000000 django-stylist-0.2.2/stylist/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:11.000000 django-stylist-0.2.2/stylist/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:11.000000 django-stylist-0.2.2/stylist/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/management/commands/build_scss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/management/commands/sync_google_fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:11.000000 django-stylist-0.2.2/stylist/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/migrations/0002_auto_20210114_1901.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/migrations/0003_font.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:11.000000 django-stylist-0.2.2/stylist/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:38:11.000000 django-stylist-0.2.2/stylist/templates/stylist/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/templates/stylist/active_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/templates/stylist/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/templates/stylist/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/templates/stylist/style_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/templates/stylist/style_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-11 15:37:37.000000 django-stylist-0.2.2/stylist/views.py
```

### Comparing `django-stylist-0.2.1/PKG-INFO` & `django-stylist-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stylist
-Version: 0.2.1
+Version: 0.2.2
 Summary: App for updating and manipulating SASS/SCSS compiling & caching on the fly
 Home-page: https://github.com/renderbox/django-stylist/
 Author: Grant Viklund
 Author-email: renderbox@gmail.com
 License: MIT license
 Description:
```

### Comparing `django-stylist-0.2.1/README.md` & `django-stylist-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django-stylist-0.2.1/django_stylist.egg-info/PKG-INFO` & `django-stylist-0.2.2/django_stylist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stylist
-Version: 0.2.1
+Version: 0.2.2
 Summary: App for updating and manipulating SASS/SCSS compiling & caching on the fly
 Home-page: https://github.com/renderbox/django-stylist/
 Author: Grant Viklund
 Author-email: renderbox@gmail.com
 License: MIT license
 Description:
```

### Comparing `django-stylist-0.2.1/django_stylist.egg-info/SOURCES.txt` & `django-stylist-0.2.2/django_stylist.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.mit.txt
 README.md
 setup.py
 django_stylist.egg-info/PKG-INFO
 django_stylist.egg-info/SOURCES.txt
 django_stylist.egg-info/dependency_links.txt
 django_stylist.egg-info/requires.txt
 django_stylist.egg-info/top_level.txt
@@ -11,18 +12,26 @@
 stylist/apps.py
 stylist/context_processors.py
 stylist/forms.py
 stylist/models.py
 stylist/settings.py
 stylist/tests.py
 stylist/urls.py
+stylist/utils.py
 stylist/views.py
 stylist/api/__init__.py
 stylist/api/serializers.py
 stylist/api/urls.py
 stylist/api/views.py
 stylist/management/__init__.py
 stylist/management/commands/__init__.py
 stylist/management/commands/build_scss.py
+stylist/management/commands/sync_google_fonts.py
 stylist/migrations/0001_initial.py
 stylist/migrations/0002_auto_20210114_1901.py
-stylist/migrations/__init__.py
+stylist/migrations/0003_font.py
+stylist/migrations/__init__.py
+stylist/templates/stylist/active_form.html
+stylist/templates/stylist/base.html
+stylist/templates/stylist/index.html
+stylist/templates/stylist/style_delete.html
+stylist/templates/stylist/style_form.html
```

### Comparing `django-stylist-0.2.1/setup.py` & `django-stylist-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-stylist-0.2.1/stylist/api/views.py` & `django-stylist-0.2.2/stylist/api/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-from rest_framework.generics import CreateAPIView
-from django.conf import settings
 from django.contrib.sites.models import Site
 from django.shortcuts import redirect
 
-from stylist.models import Style 
-from stylist.api.serializers import StyleSerializer
+from rest_framework import viewsets, filters
+from rest_framework.generics import CreateAPIView
+from rest_framework.pagination import PageNumberPagination
+
+
+from stylist.models import Style, Font
+from stylist.api.serializers import StyleSerializer, FontSerializer
 from stylist.settings import app_settings
 
 
 class StyleCreateAPIView(CreateAPIView):
      queryset = Style.objects.all()
      serializer_class = StyleSerializer
 
@@ -48,7 +51,19 @@
           if not Style.objects.filter(site=site, enabled=True):
                instance.enabled = True
                instance.save()
 
      def create(self, request, *args, **kwargs):
           response = super().create(request, *args, **kwargs)
           return redirect('stylist:stylist-index')
+
+class FontPagination(PageNumberPagination):
+    page_size = 20
+    
+class FontViewset(
+   viewsets.ReadOnlyModelViewSet
+):
+    queryset = Font.objects.all()
+    serializer_class = FontSerializer
+    pagination_class = FontPagination
+    filter_backends = [filters.SearchFilter]
+    search_fields = ['family']
```

### Comparing `django-stylist-0.2.1/stylist/context_processors.py` & `django-stylist-0.2.2/stylist/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-stylist-0.2.1/stylist/forms.py` & `django-stylist-0.2.2/stylist/forms.py`

 * *Files identical despite different names*

### Comparing `django-stylist-0.2.1/stylist/management/commands/build_scss.py` & `django-stylist-0.2.2/stylist/management/commands/build_scss.py`

 * *Files identical despite different names*

### Comparing `django-stylist-0.2.1/stylist/migrations/0001_initial.py` & `django-stylist-0.2.2/stylist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-stylist-0.2.1/stylist/migrations/0002_auto_20210114_1901.py` & `django-stylist-0.2.2/stylist/migrations/0002_auto_20210114_1901.py`

 * *Files identical despite different names*

### Comparing `django-stylist-0.2.1/stylist/models.py` & `django-stylist-0.2.2/stylist/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,11 +92,35 @@
             custom_vars.seek(0)
 
             content = sass.compile(filename=STYLIST_SCSS_TEMPLATE, include_paths=[gettempdir()])
             self.css_file.save(self.name + ".css", ContentFile(content.encode()))
             os.remove(custom_vars.name)
 
 
+class Font(models.Model):
+    """
+    Model for Fonts
+    """
+
+    family = models.CharField(_("Font Family"), max_length=50)
+    href = models.URLField(_("URL"), max_length=200)
+    provider = models.CharField(_("Provider"), max_length=50, help_text="Ex: google")
+    meta = models.JSONField(
+        blank=True,
+        default=dict,
+        help_text="any extra meta data we'd like to store as json",
+    )
+    weights = models.JSONField(blank=True, default=list)
+    preferred = models.BooleanField(_("Preferred"), default=False)
+
+    class Meta:
+        verbose_name = _("Font")
+        verbose_name_plural = _("Fonts")
+        ordering = ["-preferred", "family"]
+
+    def __str__(self):
+        return self.family
+
 @receiver(post_save, sender=Style)
 def only_one_active_style(sender, instance, **kwargs):
     if instance.enabled:
         Style.objects.filter(site=instance.site).exclude(pk=instance.pk).update(enabled=False)
```

### Comparing `django-stylist-0.2.1/stylist/tests.py` & `django-stylist-0.2.2/stylist/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,27 +47,27 @@
         super().setUp()
         self.client = Client()
         self.user = get_user_model().objects.create(username="testuser")
         self.client.force_login(self.user)
     
     def test_style_creation_api(self):
         try:
-            self.assertEquals(Style.objects.all().count(), 0)
+            self.assertEqual(Style.objects.all().count(), 0)
             url = reverse("api-create-style")
             response = self.client.post(url, {"name": "Test", "enabled": "False"}, follow=True)
-            self.assertEquals(Style.objects.all().count(), 1)
+            self.assertEqual(Style.objects.all().count(), 1)
             
             style = Style.objects.get(pk=1)
             # since it's the only style, it should be enabled
-            self.assertEquals(style.enabled, True)
+            self.assertEqual(style.enabled, True)
 
             site = Site.objects.get_current()
-            self.assertEquals(style.site, site)
+            self.assertEqual(style.site, site)
             css_path = settings.MEDIA_ROOT + "/site/" + site.domain + "/style/Test.css"
-            self.assertEquals(style.css_file.path, css_path)
+            self.assertEqual(style.css_file.path, css_path)
             # remove the new file, leaving any preexisting files
             if(os.path.exists(css_path)):
                 os.remove(css_path)
         except:
             print("")
             print(response.status_code)
             print(response.content.decode('utf-8'))
@@ -81,16 +81,16 @@
             
             data = style.attrs
             data["name"] = "Updated"
             data["primary"] = "#FF0000"
             response = self.client.post(url, data, follow=True)
 
             style.refresh_from_db()
-            self.assertEquals(style.name, "Updated")
-            self.assertEquals(style.attrs["primary"], "#FF0000")
+            self.assertEqual(style.name, "Updated")
+            self.assertEqual(style.attrs["primary"], "#FF0000")
             
             css_path = settings.MEDIA_ROOT + "/site/" + site.domain + "/style/Updated.css"
             # remove the new file, leaving any preexisting files
             if(os.path.exists(css_path)):
                 os.remove(css_path)
             
         except:
@@ -118,34 +118,34 @@
             print(response.status_code)
             print(response.content.decode('utf-8'))
             raise
    
     def test_style_delete(self):
         try:
             style = Style.objects.create(name="Test", enabled=True)
-            self.assertEquals(Style.objects.all().count(), 1)
+            self.assertEqual(Style.objects.all().count(), 1)
             
             url = reverse("stylist:stylist-delete", kwargs={"uuid": style.uuid})
             response = self.client.post(url, follow=True)
 
-            self.assertEquals(Style.objects.all().count(), 0)
+            self.assertEqual(Style.objects.all().count(), 0)
         except:
             print("")
             print(response.status_code)
             print(response.content.decode('utf-8'))
             raise
 
     def test_style_active(self):
         try:
             site = Site.objects.get_current()
             style = Style.objects.create(name="Test", enabled=False, site=site)
             url = reverse("stylist:stylist-make-active")
 
             response = self.client.post(url, {"active": 1}, follow=True)
-            self.assertEquals(response.context["active_theme"], style)
+            self.assertEqual(response.context["active_theme"], style)
         except:
             print("")
             print(response.status_code)
             print(response.content.decode('utf-8'))
             raise
 
 
@@ -178,35 +178,35 @@
             url = reverse("stylist:stylist-preview", kwargs={"uuid": style.uuid})
             data = style.attrs
             data["name"] = style.name
             response = self.client.post(url, data, follow=True)
 
             new_url = reverse("stylist:stylist-end-preview")
             new_response = self.client.get(new_url, HTTP_REFERER=reverse("stylist:stylist-index"), follow=True)
-            self.assertEquals(new_response.context.get("preview_style"), None)
+            self.assertEqual(new_response.context.get("preview_style"), None)
         except:
             print("")
             print(response.status_code)
             print(response.content.decode('utf-8'))
             raise
 
 
     def test_style_duplicate(self):
         try:
             site = Site.objects.get_current()
             style = Style.objects.create(name="Test", enabled=False, site=site)
-            self.assertEquals(Style.objects.all().count(), 1)
+            self.assertEqual(Style.objects.all().count(), 1)
             
             url = reverse("api-duplicate-style", kwargs={"uuid": style.uuid})
             response = self.client.post(url, {"name": style.name, "enabled": False}, follow=True)
 
-            self.assertEquals(Style.objects.all().count(), 2)
+            self.assertEqual(Style.objects.all().count(), 2)
             new_style = Style.objects.all().last()
-            self.assertEquals(new_style.name, "Test copy")
-            self.assertEquals(new_style.attrs, style.attrs)
+            self.assertEqual(new_style.name, "Test copy")
+            self.assertEqual(new_style.attrs, style.attrs)
         except:
             print("")
             print(response.status_code)
             print(response.content.decode('utf-8'))
             raise
 
 @override_settings(STYLIST_USE_SASS=True)
```

### Comparing `django-stylist-0.2.1/stylist/urls.py` & `django-stylist-0.2.2/stylist/urls.py`

 * *Files identical despite different names*

### Comparing `django-stylist-0.2.1/stylist/views.py` & `django-stylist-0.2.2/stylist/views.py`

 * *Files identical despite different names*

