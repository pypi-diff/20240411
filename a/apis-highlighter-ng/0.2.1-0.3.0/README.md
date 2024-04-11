# Comparing `tmp/apis_highlighter_ng-0.2.1.tar.gz` & `tmp/apis_highlighter_ng-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apis_highlighter_ng-0.2.1.tar", max compression
+gzip compressed data, was "apis_highlighter_ng-0.3.0.tar", max compression
```

## Comparing `apis_highlighter_ng-0.2.1.tar` & `apis_highlighter_ng-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1163 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/LICENSE
--rw-r--r--   0        0        0      107 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/__init__.py
--rw-r--r--   0        0        0      183 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/admin.py
--rw-r--r--   0        0        0      220 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/apps.py
--rw-r--r--   0        0        0     2845 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/helpers.py
--rw-r--r--   0        0        0     2852 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/migrations/0001_initial.py
--rw-r--r--   0        0        0      571 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/migrations/0002_rename_annotation_project_annotation_project_and_more.py
--rw-r--r--   0        0        0        0 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/migrations/__init__.py
--rw-r--r--   0        0        0     1316 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/models.py
--rw-r--r--   0        0        0     1164 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/signals.py
--rw-r--r--   0        0        0      504 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/static/css/highlighter.css
--rw-r--r--   0        0        0     6452 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/static/js/highlighter.js
--rw-r--r--   0        0        0      949 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/templates/apis_highlighter/annotation_confirm_delete.html
--rw-r--r--   0        0        0      857 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/templates/apis_highlighter/apis_highlighter.html
--rw-r--r--   0        0        0      299 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/templates/apis_highlighter/select_project.html
--rw-r--r--   0        0        0     3274 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/templatetags/apis_highlighter.py
--rw-r--r--   0        0        0      749 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/urls.py
--rw-r--r--   0        0        0     2320 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/apis_highlighter/views.py
--rw-r--r--   0        0        0      677 2024-03-15 09:42:32.437448 apis_highlighter_ng-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 apis_highlighter_ng-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1163 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/LICENSE
+-rw-r--r--   0        0        0      107 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/__init__.py
+-rw-r--r--   0        0        0      183 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/admin.py
+-rw-r--r--   0        0        0      220 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/apps.py
+-rw-r--r--   0        0        0     2845 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/helpers.py
+-rw-r--r--   0        0        0     2852 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/migrations/0001_initial.py
+-rw-r--r--   0        0        0      571 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/migrations/0002_rename_annotation_project_annotation_project_and_more.py
+-rw-r--r--   0        0        0      478 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/migrations/0003_annotation_text_field_name.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/migrations/__init__.py
+-rw-r--r--   0        0        0     1371 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/models.py
+-rw-r--r--   0        0        0     1164 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/signals.py
+-rw-r--r--   0        0        0      504 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/static/css/highlighter.css
+-rw-r--r--   0        0        0     6531 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/static/js/highlighter.js
+-rw-r--r--   0        0        0      949 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/templates/apis_highlighter/annotation_confirm_delete.html
+-rw-r--r--   0        0        0      857 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/templates/apis_highlighter/apis_highlighter.html
+-rw-r--r--   0        0        0      299 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/templates/apis_highlighter/select_project.html
+-rw-r--r--   0        0        0     3380 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/templatetags/apis_highlighter.py
+-rw-r--r--   0        0        0      785 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/urls.py
+-rw-r--r--   0        0        0     2456 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/apis_highlighter/views.py
+-rw-r--r--   0        0        0      677 2024-04-11 07:11:26.780631 apis_highlighter_ng-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 apis_highlighter_ng-0.3.0/PKG-INFO
```

### Comparing `apis_highlighter_ng-0.2.1/LICENSE` & `apis_highlighter_ng-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apis_highlighter_ng-0.2.1/apis_highlighter/helpers.py` & `apis_highlighter_ng-0.3.0/apis_highlighter/helpers.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter_ng-0.2.1/apis_highlighter/migrations/0001_initial.py` & `apis_highlighter_ng-0.3.0/apis_highlighter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter_ng-0.2.1/apis_highlighter/migrations/0002_rename_annotation_project_annotation_project_and_more.py` & `apis_highlighter_ng-0.3.0/apis_highlighter/migrations/0002_rename_annotation_project_annotation_project_and_more.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter_ng-0.2.1/apis_highlighter/models.py` & `apis_highlighter_ng-0.3.0/apis_highlighter/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         ContentType,
         related_name="text_annotation_set",
         on_delete=models.CASCADE,
         null=True,
     )
     text_object_id = models.PositiveIntegerField(null=True)
     text_content_object = GenericForeignKey("text_content_type", "text_object_id")
+    text_field_name = models.CharField(default="text")
 
     user = models.ForeignKey(User, blank=True, null=True, on_delete=models.SET_NULL)
 
     project = models.ForeignKey(
         AnnotationProject, blank=True, null=True, on_delete=models.CASCADE
     )
```

### Comparing `apis_highlighter_ng-0.2.1/apis_highlighter/signals.py` & `apis_highlighter_ng-0.3.0/apis_highlighter/signals.py`

 * *Files identical despite different names*

### Comparing `apis_highlighter_ng-0.2.1/apis_highlighter/static/js/highlighter.js` & `apis_highlighter_ng-0.3.0/apis_highlighter/static/js/highlighter.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -25,14 +25,15 @@
             const num_brs = shadow_selection.querySelectorAll("br").length;
             start = priorRange.toString().length + num_brs;
             end = start + range.toString().length;
 
             var annotationdata = {};
             annotationdata.text_object_id = highlight_text.dataset.text_object_id;
             annotationdata.text_content_type_id = highlight_text.dataset.text_content_type_id;
+            annotationdata.text_field_name = highlight_text.dataset.text_field_name;
             annotationdata.project_id = highlight_text.dataset.project_id;
             annotationdata.orig_string = selection.toString();
             annotationdata.start = start;
             annotationdata.end = end;
             console.log(JSON.stringify(annotationdata));
 
             // add a helper span around the selection,
```

### Comparing `apis_highlighter_ng-0.2.1/apis_highlighter/templates/apis_highlighter/annotation_confirm_delete.html` & `apis_highlighter_ng-0.3.0/apis_highlighter/templates/apis_highlighter/annotation_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `apis_highlighter_ng-0.2.1/apis_highlighter/templates/apis_highlighter/apis_highlighter.html` & `apis_highlighter_ng-0.3.0/apis_highlighter/templates/apis_highlighter/apis_highlighter.html`

 * *Files identical despite different names*

### Comparing `apis_highlighter_ng-0.2.1/apis_highlighter/templatetags/apis_highlighter.py` & `apis_highlighter_ng-0.3.0/apis_highlighter/templatetags/apis_highlighter.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,42 +9,45 @@
 
 
 def overlap(range_one, range_two) -> bool:
     r = range(max(range_one[0], range_two[0]), min(range_one[1], range_two[1]))
     return bool(r)
 
 
-@register.filter()
-def highlight_text(obj, request=None, fieldname="text", project_id=None):
+@register.simple_tag
+def highlight_text(obj, request=None, field_name="text", project_id=None):
     if project_id is None:
         default_project = getattr(
             settings,
             "DEFAULT_HIGHLIGTHER_PROJECT",
             AnnotationProject.objects.first().id,
         )
         project_id = request.GET.get("highlighter_project", default_project)
 
     ct = ContentType.objects.get_for_model(obj)
-    annotations = Annotation.objects.filter(text_content_type=ct, text_object_id=obj.id)
-    args = [ct.id, obj.id]
+    annotations = Annotation.objects.filter(
+        text_content_type=ct, text_object_id=obj.id, text_field_name=field_name
+    )
+    args = [ct.id, obj.id, field_name]
     if project_id:
         annotations = annotations.filter(project__id=project_id)
         args.append(project_id)
 
     annotations_url = reverse("apis_highlighter:annotations", args=args)
     prefix = (
         f"<div class='highlight-text'"
         f" data-text_object_id='{obj.id}'"
         f" data-text_content_type_id='{ct.id}'"
+        f" data-text_field_name='{field_name}'"
         f" data-project_id='{project_id}'"
         f" data-source='{annotations_url}'>"
     )
     suffix = "</div>"
 
-    text = getattr(obj, fieldname)
+    text = getattr(obj, field_name)
     annotated_ranges = []
     for ann in annotations.order_by("-start"):
         if not any(map(lambda x: overlap((ann.start, ann.end), x), annotated_ranges)):
             annotated_ranges.append((ann.start, ann.end))
             title = (
                 f'Annotation "{ann.orig_string}" '
                 + f"from {ann.user} in project {ann.project}; "
```

### Comparing `apis_highlighter_ng-0.2.1/apis_highlighter/views.py` & `apis_highlighter_ng-0.3.0/apis_highlighter/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,19 +16,24 @@
     def dispatch(self, request, *args, **kwargs):
         text_content_type = kwargs.get("text_content_type")
         text_object_id = kwargs.get("text_object_id")
         ct = ContentType.objects.get_for_id(text_content_type)
         # return 404 if not exist
         self.object = ct.get_object_for_this_type(pk=text_object_id)
         self.project_id = kwargs.get("project_id")
+        self.field_name = kwargs.get("text_field_name")
 
         return super().dispatch(request, *args, **kwargs)
 
     def get(self, request, *args, **kwargs):
-        return HttpResponse(highlight_text(self.object, project_id=self.project_id))
+        return HttpResponse(
+            highlight_text(
+                self.object, field_name=self.field_name, project_id=self.project_id
+            )
+        )
 
 
 class AnnotationDelete(DeleteView):
     model = Annotation
 
     def get_template_names(self):
         return ["confirm_delete", "apis_highlighter/annotation_confirm_delete.html"]
```

### Comparing `apis_highlighter_ng-0.2.1/pyproject.toml` & `apis_highlighter_ng-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apis-highlighter-ng"
-version = "0.2.1"
+version = "0.3.0"
 description = "Highlighter for the APIS project"
 authors = ["Birger Schacht <birger.schacht@oeaw.ac.at>"]
 license = "MIT"
 packages = [{include = "apis_highlighter"}]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `apis_highlighter_ng-0.2.1/PKG-INFO` & `apis_highlighter_ng-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apis-highlighter-ng
-Version: 0.2.1
+Version: 0.3.0
 Summary: Highlighter for the APIS project
 License: MIT
 Author: Birger Schacht
 Author-email: birger.schacht@oeaw.ac.at
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

