# Comparing `tmp/xstate_machine-3.1.0.tar.gz` & `tmp/xstate_machine-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xstate_machine-3.1.0.tar", max compression
+gzip compressed data, was "xstate_machine-3.1.1.tar", max compression
```

## Comparing `xstate_machine-3.1.0.tar` & `xstate_machine-3.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1051 2024-04-10 22:05:15.923111 xstate_machine-3.1.0/LICENSE
--rw-r--r--   0        0        0    11243 2024-04-10 22:14:20.519343 xstate_machine-3.1.0/README.md
--rw-r--r--   0        0        0      439 2024-04-10 22:04:59.259867 xstate_machine-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    26230 2024-04-10 21:08:51.049539 xstate_machine-3.1.0/xstate_machine/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 21:06:22.891847 xstate_machine-3.1.0/xstate_machine/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 21:06:22.891952 xstate_machine-3.1.0/xstate_machine/management/commands/__init__.py
--rw-r--r--   0        0        0     9229 2024-04-10 21:08:51.050312 xstate_machine-3.1.0/xstate_machine/management/commands/graph_transitions.py
--rw-r--r--   0        0        0       88 2024-04-10 21:06:22.892217 xstate_machine-3.1.0/xstate_machine/models.py
--rw-r--r--   0        0        0      113 2024-04-10 21:06:22.892308 xstate_machine-3.1.0/xstate_machine/signals.py
--rw-r--r--   0        0        0        0 2024-04-10 21:06:22.892392 xstate_machine-3.1.0/xstate_machine/tests/__init__.py
--rw-r--r--   0        0        0     1842 2024-04-10 21:08:51.049524 xstate_machine-3.1.0/xstate_machine/tests/test_abstract_inheritance.py
--rw-r--r--   0        0        0     8522 2024-04-10 21:08:51.062559 xstate_machine-3.1.0/xstate_machine/tests/test_basic_transitions.py
--rw-r--r--   0        0        0     1390 2024-04-10 21:08:51.049651 xstate_machine-3.1.0/xstate_machine/tests/test_conditions.py
--rw-r--r--   0        0        0     1070 2024-04-10 21:08:51.049900 xstate_machine-3.1.0/xstate_machine/tests/test_integer_field.py
--rw-r--r--   0        0        0     4501 2024-04-10 21:08:51.049925 xstate_machine-3.1.0/xstate_machine/tests/test_key_field.py
--rw-r--r--   0        0        0     1161 2024-04-10 21:08:51.056695 xstate_machine-3.1.0/xstate_machine/tests/test_protected_field.py
--rw-r--r--   0        0        0     1133 2024-04-10 21:08:51.056838 xstate_machine-3.1.0/xstate_machine/tests/test_protected_fields.py
--rw-r--r--   0        0        0     1678 2024-04-10 21:08:51.060000 xstate_machine-3.1.0/xstate_machine/tests/test_proxy_inheritance.py
--rw-r--r--   0        0        0    11794 1970-01-01 00:00:00.000000 xstate_machine-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1051 2024-04-10 22:58:19.454418 xstate_machine-3.1.1/LICENSE
+-rw-r--r--   0        0        0    11243 2024-04-10 22:58:19.454584 xstate_machine-3.1.1/README.md
+-rw-r--r--   0        0        0     2187 2024-04-10 23:16:10.761786 xstate_machine-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0    25632 2024-04-10 22:58:19.459060 xstate_machine-3.1.1/xstate_machine/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-10 23:16:10.761989 xstate_machine-3.1.1/xstate_machine/management/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-10 23:16:10.762207 xstate_machine-3.1.1/xstate_machine/management/commands/__init__.py
+-rw-r--r--   0        0        0     9229 2024-04-10 22:58:19.459370 xstate_machine-3.1.1/xstate_machine/management/commands/graph_transitions.py
+-rw-r--r--   0        0        0       88 2024-04-10 22:58:19.459456 xstate_machine-3.1.1/xstate_machine/models.py
+-rw-r--r--   0        0        0      113 2024-04-10 22:58:19.459540 xstate_machine-3.1.1/xstate_machine/signals.py
+-rw-r--r--   0        0        0        0 2024-04-10 22:58:19.459574 xstate_machine-3.1.1/xstate_machine/tests/__init__.py
+-rw-r--r--   0        0        0     1842 2024-04-10 22:58:19.459720 xstate_machine-3.1.1/xstate_machine/tests/test_abstract_inheritance.py
+-rw-r--r--   0        0        0     8522 2024-04-10 22:58:19.459874 xstate_machine-3.1.1/xstate_machine/tests/test_basic_transitions.py
+-rw-r--r--   0        0        0     1390 2024-04-10 22:58:19.460161 xstate_machine-3.1.1/xstate_machine/tests/test_conditions.py
+-rw-r--r--   0        0        0     1070 2024-04-10 22:58:19.460308 xstate_machine-3.1.1/xstate_machine/tests/test_integer_field.py
+-rw-r--r--   0        0        0     4527 2024-04-10 22:58:19.460443 xstate_machine-3.1.1/xstate_machine/tests/test_key_field.py
+-rw-r--r--   0        0        0     1169 2024-04-10 22:58:19.460569 xstate_machine-3.1.1/xstate_machine/tests/test_protected_field.py
+-rw-r--r--   0        0        0     1137 2024-04-10 22:58:19.460696 xstate_machine-3.1.1/xstate_machine/tests/test_protected_fields.py
+-rw-r--r--   0        0        0     1678 2024-04-10 22:58:19.460843 xstate_machine-3.1.1/xstate_machine/tests/test_proxy_inheritance.py
+-rw-r--r--   0        0        0    13285 1970-01-01 00:00:00.000000 xstate_machine-3.1.1/PKG-INFO
```

### Comparing `xstate_machine-3.1.0/LICENSE` & `xstate_machine-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xstate_machine-3.1.0/README.md` & `xstate_machine-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xstate_machine-3.1.0/xstate_machine/__init__.py` & `xstate_machine-3.1.1/xstate_machine/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,31 +42,14 @@
     "can_proceed",
     "has_transition_perm",
     "GET_STATE",
     "RETURN_VALUE",
 ]
 
 
-import warnings
-
-
-def show_deprecation_warning():
-    message = (
-        "The 'django-fsm' package has been integrated into 'viewflow' as 'viewflow.fsm' starting from version 3.0. "
-        "This version of 'django-fsm' is no longer maintained and will not receive further updates. "
-        "If you require new functionality introduced in 'django-fsm' version 3.0 or later, "
-        "please migrate to 'viewflow.fsm'. For detailed instructions on the migration process and accessing new features, "
-        "refer to the official documentation at https://docs.viewflow.io/fsm/index.html"
-    )
-    warnings.warn(message, UserWarning, stacklevel=2)
-
-
-show_deprecation_warning()
-
-
 if sys.version_info[:2] == (2, 6):
     # Backport of Python 2.7 inspect.getmembers,
     # since Python 2.6 ships buggy implementation
     def __getmembers(object, predicate=None):
         """Return all members of an object as (name, value) pairs sorted by name.
         Optionally, only return members that satisfy a given predicate."""
         results = []
@@ -84,17 +67,17 @@
 
 # South support; see http://south.aeracode.org/docs/tutorial/part4.html#simple-inheritance
 try:
     from south.modelsinspector import add_introspection_rules
 except ImportError:
     pass
 else:
-    add_introspection_rules([], [r"^django_fsm\.FSMField"])
-    add_introspection_rules([], [r"^django_fsm\.FSMIntegerField"])
-    add_introspection_rules([], [r"^django_fsm\.FSMKeyField"])
+    add_introspection_rules([], [r"^xstate_machine\.FSMField"])
+    add_introspection_rules([], [r"^xstate_machine\.FSMIntegerField"])
+    add_introspection_rules([], [r"^xstate_machine\.FSMKeyField"])
 
 
 class TransitionNotAllowed(Exception):
     """Raised when a transition is not allowed"""
 
     def __init__(self, *args, **kwargs):
         self.object = kwargs.pop("object", None)
@@ -159,15 +142,15 @@
     List of transitions available in current model state
     with all conditions met
     """
     curr_state = field.get_state(instance)
     transitions = field.transitions[instance.__class__]
 
     for name, transition in transitions.items():
-        meta = transition._django_fsm
+        meta = transition._xstate_machine
         if meta.has_transition(curr_state) and meta.conditions_met(
             instance, curr_state
         ):
             yield meta.get_transition(curr_state)
 
 
 def get_all_FIELD_transitions(instance, field):
@@ -333,15 +316,15 @@
     def get_state(self, instance):
         # The state field may be deferred. We delegate the logic of figuring
         # this out and loading the deferred field on-demand to Django's
         # built-in DeferredAttribute class. DeferredAttribute's instantiation
         # signature changed over time, so we need to check Django version
         # before proceeding to call DeferredAttribute. An alternative to this
         # would be copying the latest implementation of DeferredAttribute to
-        # django_fsm, but this comes with the added responsibility of keeping
+        # xstate_machine, but this comes with the added responsibility of keeping
         # the copied code up to date.
         if django.VERSION[:3] >= (3, 0, 0):
             return DeferredAttribute(self).__get__(instance)
         elif django.VERSION[:3] >= (2, 1, 0):
             return DeferredAttribute(self.name).__get__(instance)
         elif django.VERSION[:3] >= (1, 10, 0):
             return DeferredAttribute(self.name, model=None).__get__(instance)
@@ -372,15 +355,15 @@
             model = get_model(app_label, model_name)
             if model is None:
                 raise ValueError("No model found {0}".format(state_proxy))
 
             instance.__class__ = model
 
     def change_state(self, instance, method, *args, **kwargs):
-        meta = method._django_fsm
+        meta = method._xstate_machine
         method_name = method.__name__
         current_state = self.get_state(instance)
 
         if not meta.has_transition(current_state):
             raise TransitionNotAllowed(
                 "Can't switch from state '{0}' using method '{1}'".format(
                     current_state, method_name
@@ -439,15 +422,15 @@
     def get_all_transitions(self, instance_cls):
         """
         Returns [(source, target, name, method)] for all field transitions
         """
         transitions = self.transitions[instance_cls]
 
         for name, transition in transitions.items():
-            meta = transition._django_fsm
+            meta = transition._xstate_machine
 
             for transition in meta.transitions.values():
                 yield transition
 
     def contribute_to_class(self, cls, name, **kwargs):
         self.base_cls = cls
 
@@ -476,30 +459,30 @@
 
         if not issubclass(sender, self.base_cls):
             return
 
         def is_field_transition_method(attr):
             return (
                 (inspect.ismethod(attr) or inspect.isfunction(attr))
-                and hasattr(attr, "_django_fsm")
+                and hasattr(attr, "_xstate_machine")
                 and (
-                    attr._django_fsm.field in [self, self.name]
+                    attr._xstate_machine.field in [self, self.name]
                     or (
-                        isinstance(attr._django_fsm.field, Field)
-                        and attr._django_fsm.field.name == self.name
-                        and attr._django_fsm.field.creation_counter
+                        isinstance(attr._xstate_machine.field, Field)
+                        and attr._xstate_machine.field.name == self.name
+                        and attr._xstate_machine.field.creation_counter
                         == self.creation_counter
                     )
                 )
             )
 
         sender_transitions = {}
         transitions = inspect.getmembers(sender, predicate=is_field_transition_method)
         for method_name, method in transitions:
-            method._django_fsm.field = self
+            method._xstate_machine.field = self
             sender_transitions[method_name] = method
 
         self.transitions[sender] = sender_transitions
 
 
 class FSMField(FSMFieldMixin, models.CharField):
     """
@@ -660,27 +643,27 @@
     Method decorator to mark allowed transitions.
 
     Set target to None if current state needs to be validated and
     has not changed after the function call.
     """
 
     def inner_transition(func):
-        wrapper_installed, fsm_meta = True, getattr(func, "_django_fsm", None)
+        wrapper_installed, fsm_meta = True, getattr(func, "_xstate_machine", None)
         if not fsm_meta:
             wrapper_installed = False
             fsm_meta = FSMMeta(field=field, method=func)
-            setattr(func, "_django_fsm", fsm_meta)
+            setattr(func, "_xstate_machine", fsm_meta)
 
         if isinstance(source, (list, tuple, set)):
             for state in source:
-                func._django_fsm.add_transition(
+                func._xstate_machine.add_transition(
                     func, state, target, on_error, conditions, permission, custom
                 )
         else:
-            func._django_fsm.add_transition(
+            func._xstate_machine.add_transition(
                 func, source, target, on_error, conditions, permission, custom
             )
 
         @wraps(func)
         def _change_state(instance, *args, **kwargs):
             return fsm_meta.field.change_state(instance, func, *args, **kwargs)
 
@@ -695,36 +678,36 @@
 def can_proceed(bound_method, check_conditions=True):
     """
     Returns True if model in state allows to call bound_method
 
     Set ``check_conditions`` argument to ``False`` to skip checking
     conditions.
     """
-    if not hasattr(bound_method, "_django_fsm"):
+    if not hasattr(bound_method, "_xstate_machine"):
         im_func = getattr(bound_method, "im_func", getattr(bound_method, "__func__"))
         raise TypeError("%s method is not transition" % im_func.__name__)
 
-    meta = bound_method._django_fsm
+    meta = bound_method._xstate_machine
     im_self = getattr(bound_method, "im_self", getattr(bound_method, "__self__"))
     current_state = meta.field.get_state(im_self)
 
     return meta.has_transition(current_state) and (
         not check_conditions or meta.conditions_met(im_self, current_state)
     )
 
 
 def has_transition_perm(bound_method, user):
     """
     Returns True if model in state allows to call bound_method and user have rights on it
     """
-    if not hasattr(bound_method, "_django_fsm"):
+    if not hasattr(bound_method, "_xstate_machine"):
         im_func = getattr(bound_method, "im_func", getattr(bound_method, "__func__"))
         raise TypeError("%s method is not transition" % im_func.__name__)
 
-    meta = bound_method._django_fsm
+    meta = bound_method._xstate_machine
     im_self = getattr(bound_method, "im_self", getattr(bound_method, "__self__"))
     current_state = meta.field.get_state(im_self)
 
     return (
         meta.has_transition(current_state)
         and meta.conditions_met(im_self, current_state)
         and meta.has_transition_perm(im_self, current_state, user)
```

### Comparing `xstate_machine-3.1.0/xstate_machine/management/commands/graph_transitions.py` & `xstate_machine-3.1.1/xstate_machine/management/commands/graph_transitions.py`

 * *Files identical despite different names*

### Comparing `xstate_machine-3.1.0/xstate_machine/tests/test_abstract_inheritance.py` & `xstate_machine-3.1.1/xstate_machine/tests/test_abstract_inheritance.py`

 * *Files identical despite different names*

### Comparing `xstate_machine-3.1.0/xstate_machine/tests/test_basic_transitions.py` & `xstate_machine-3.1.1/xstate_machine/tests/test_basic_transitions.py`

 * *Files identical despite different names*

### Comparing `xstate_machine-3.1.0/xstate_machine/tests/test_conditions.py` & `xstate_machine-3.1.1/xstate_machine/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `xstate_machine-3.1.0/xstate_machine/tests/test_integer_field.py` & `xstate_machine-3.1.1/xstate_machine/tests/test_integer_field.py`

 * *Files identical despite different names*

### Comparing `xstate_machine-3.1.0/xstate_machine/tests/test_key_field.py` & `xstate_machine-3.1.1/xstate_machine/tests/test_key_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 
     label = models.CharField(max_length=255)
 
     def __unicode__(self):
         return self.label
 
     class Meta:
-        app_label = "django_fsm"
+        app_label = "xstate_machine"
 
 
 class FKBlogPost(models.Model):
-    state = FSMKeyField(DBState, default="new", protected=True, on_delete=models.CASCADE)
+    state = FSMKeyField(
+        DBState, default="new", protected=True, on_delete=models.CASCADE
+    )
 
     @transition(field=state, source="new", target="published")
     def publish(self):
         pass
 
     @transition(field=state, source="published")
     def notify_all(self):
@@ -49,15 +51,15 @@
         pass
 
     @transition(field=state, source="*", target="moderated")
     def moderate(self):
         pass
 
     class Meta:
-        app_label = "django_fsm"
+        app_label = "xstate_machine"
 
 
 class FSMKeyFieldTest(TestCase):
     def setUp(self):
         for item in FK_AVAILABLE_STATES:
             DBState.objects.create(pk=item[0], label=item[1])
         self.model = FKBlogPost()
@@ -116,15 +118,15 @@
 """
 TODO FIX it
 class BlogPostStatus(models.Model):
     name = models.CharField(max_length=10, unique=True)
     objects = models.Manager()
 
     class Meta:
-        app_label = 'django_fsm'
+        app_label = 'xstate_machine'
 
 
 class BlogPostWithFKState(models.Model):
     status = FSMKeyField(BlogPostStatus, default=lambda: BlogPostStatus.objects.get(name="new"))
 
     @transition(field=status, source='new', target='published')
     def publish(self):
```

### Comparing `xstate_machine-3.1.0/xstate_machine/tests/test_protected_field.py` & `xstate_machine-3.1.1/xstate_machine/tests/test_protected_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     status = FSMField(default="new", protected=True)
 
     @transition(field=status, source="new", target="published")
     def publish(self):
         pass
 
     class Meta:
-        app_label = "django_fsm"
+        app_label = "xstate_machine"
 
 
 class MultiProtectedAccessModel(models.Model):
     status1 = FSMField(default="new", protected=True)
     status2 = FSMField(default="new", protected=True)
 
     class Meta:
-        app_label = "django_fsm"
+        app_label = "xstate_machine"
 
 
 class TestDirectAccessModels(TestCase):
     def test_multi_protected_field_create(self):
         obj = MultiProtectedAccessModel.objects.create()
         self.assertEqual(obj.status1, "new")
         self.assertEqual(obj.status2, "new")
```

### Comparing `xstate_machine-3.1.0/xstate_machine/tests/test_protected_fields.py` & `xstate_machine-3.1.1/xstate_machine/tests/test_protected_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     status = FSMField(default='new', protected=True)
 
     @transition(field=status, source='new', target='published')
     def publish(self):
         pass
 
     class Meta:
-        app_label = 'django_fsm'
+        app_label = 'xstate_machine'
 
 
 class RefreshableModel(FSMModelMixin, RefreshableProtectedAccessModel):
     pass
 
 
 class TestDirectAccessModels(TestCase):
```

### Comparing `xstate_machine-3.1.0/xstate_machine/tests/test_proxy_inheritance.py` & `xstate_machine-3.1.1/xstate_machine/tests/test_proxy_inheritance.py`

 * *Files identical despite different names*

### Comparing `xstate_machine-3.1.0/PKG-INFO` & `xstate_machine-3.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,54 @@
 Metadata-Version: 2.1
 Name: xstate-machine
-Version: 3.1.0
+Version: 3.1.1
 Summary: Django friendly finite state machine support.
+Home-page: https://github.com/xpendit/xstate-machine
 License: MIT
 Author: Nicolas Quiroz
 Author-email: nicolasquirozpa@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 7 - Inactive
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 1.10
+Classifier: Framework :: Django :: 1.11
+Classifier: Framework :: Django :: 1.6
+Classifier: Framework :: Django :: 1.8
+Classifier: Framework :: Django :: 1.9
+Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 2.1
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 5.0
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.13
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Django (>=5.0.4,<6.0.0)
+Requires-Dist: graphviz (>=0.20.3,<0.21.0)
+Requires-Dist: pytest (>=8.1.1,<9.0.0)
+Project-URL: Repository, https://github.com/xpendit/xstate-machine
 Description-Content-Type: text/markdown
 
 
 # Django friendly finite state machine support
 
 `xstate-machine` adds simple declarative state management for django models.
 Based on the [django-fsm](
```

