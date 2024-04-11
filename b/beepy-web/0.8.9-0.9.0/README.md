# Comparing `tmp/beepy_web-0.8.9.tar.gz` & `tmp/beepy_web-0.9.0.tar.gz`

## Comparing `beepy_web-0.8.9.tar` & `beepy_web-0.9.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 beepy_web-0.8.9/.env.template
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.8.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.8.9/.python-version
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.8.9/requirements.txt
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/__init__.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/attrs.py
--rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/children.py
--rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/components.py
--rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/context.py
--rwxr-xr-x   0        0        0     4050 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/dev.py
--rw-r--r--   0        0        0    22029 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/framework.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/listeners.py
--rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/router.py
--rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/style.py
--rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/tags.py
--rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/trackable.py
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/modules/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/modules/actions.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/modules/context_menu.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/modules/local_storage.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/modules/modal.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/modules/plot.py
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/modules/table.py
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/modules/tabs.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/utils/__init__.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/utils/api.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/utils/asyncio.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/utils/common.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/utils/dev.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/utils/import_hooks.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/utils/internal.py
--rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/utils/js.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 beepy_web-0.8.9/beepy/utils/js_py.py
--rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.8.9/web/package-lock.json
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 beepy_web-0.8.9/web/package.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.8.9/web/webpack.dev.js
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.8.9/web/webpack.prod.js
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 beepy_web-0.8.9/web/src/beepy.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.8.9/web/src/dev-server.js
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.8.9/web/src/files.js
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.8.9/web/src/index.js
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.8.9/web/src/main.css
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.8.9/web/src/python.js
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.8.9/web/src/utils.js
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.8.9/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.8.9/LICENSE
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 beepy_web-0.8.9/README.md
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 beepy_web-0.8.9/pyproject.toml
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 beepy_web-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 beepy_web-0.9.0/.env.template
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.0/.python-version
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.0/requirements.txt
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/__init__.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/attrs.py
+-rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/children.py
+-rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/components.py
+-rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/context.py
+-rw-r--r--   0        0        0    21167 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/framework.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/listeners.py
+-rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/router.py
+-rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/style.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/tags.py
+-rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/trackable.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/types.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/dev/__init__.py
+-rwxr-xr-x   0        0        0     5051 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/dev/__main__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/dev/example.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/dev/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/actions.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/context_menu.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/local_storage.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/modal.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/plot.py
+-rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/table.py
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/modules/tabs.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/__init__.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/api.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/asyncio.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/common.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/dev.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/import_hooks.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/internal.py
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/js.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.0/beepy/utils/js_py.py
+-rw-r--r--   0        0        0   179389 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/package-lock.json
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/package.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/webpack.dev.js
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/webpack.prod.js
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/beepy.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/dev-server.js
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/files.js
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/index.js
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/main.css
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/python.js
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.0/web/src/utils.js
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 beepy_web-0.9.0/README.md
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beepy_web-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 beepy_web-0.9.0/PKG-INFO
```

### Comparing `beepy_web-0.8.9/.pre-commit-config.yaml` & `beepy_web-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/__init__.py` & `beepy_web-0.9.0/beepy/__init__.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/attrs.py` & `beepy_web-0.9.0/beepy/attrs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/children.py` & `beepy_web-0.9.0/beepy/children.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/components.py` & `beepy_web-0.9.0/beepy/components.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,147 +1,169 @@
 from __future__ import annotations
 
 from collections import defaultdict
-from functools import partial, wraps
+from functools import partial
 from types import MethodType
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Self
 
 import beepy
 from beepy.attrs import set_html_attribute, state
 from beepy.context import Context, _MetaContext
 from beepy.listeners import on
 from beepy.types import AttrType, Renderer, WebBase
 from beepy.utils import IN_BROWSER, js
 from beepy.utils.common import NONE_TYPE, nested_copy
 from beepy.utils.dev import _debugger
 
 if TYPE_CHECKING:
-    from collections.abc import Callable
+    from collections.abc import Callable, Iterable
 
     from beepy.children import ComponentRef
     from beepy.framework import Tag
 
-_current__lifecycle_method: dict[str, dict[int, Component]] = {}
 
+class LifecycleMethod:
+    __slots__ = ('original_fn', 'steps', 'manager_fn', 'instance')
 
-def _lifecycle_method(*, hash_function=hash):
-    def _wrapper(fn):
-        name = fn.__name__
-        attr_name = f'_wrapper_{name}_calling'
-        _cache = _current__lifecycle_method[attr_name] = {}
+    original_fn: Callable
+    steps: Iterable[str]
+    manager_fn: Callable[[Component, str, tuple, dict], Any] | None
+    instance: Component | None
+
+    def __init__(self, original_fn, steps=(), manager_fn=None):
+        self.original_fn = original_fn
+        self.steps = steps
+        self.manager_fn = manager_fn
+        self.instance = None
+
+    def call_as_super(self, this, args, kwargs):
+        # This allows to call super()._method_() as usual function, not generator-function
+        # So it skips calling manager, but function is called fully, as expected
+        for _ in self.original_fn(this, *args, **kwargs):
+            pass
+
+    def __get__(self, instance, owner):
+        if instance is None:
+            return self
+        return self._with_instance(instance)
+
+    def _with_instance(self, instance):
+        this = type(self)(self.original_fn, self.steps, self.manager_fn)
+        this.instance = instance
+        return this
+
+    def _inherit(self, override_fn):
+        this = type(self)(override_fn, self.steps, self.manager_fn)
+        this.instance = self.instance
+        return this
+
+    def manager(self, steps: Iterable[str]):
+        if self.manager_fn is not None:
+            raise ValueError('Manager function is already set')
+
+        self.steps = steps
+
+        wrapper: Callable[[Component, str, tuple, dict], Any]
+
+        def wrapper(fn):
+            self.manager_fn = fn
+            return fn
 
-        @wraps(fn)
-        def lifecycle_method(original_func):
-            @wraps(original_func)
-            def original_method_wrapper(self, *args, **kwargs):
-                # prevent calling super() calls extra code twice
-                _hash = hash_function(self)
-                not_in_super_call = _hash not in _cache
-
-                if not_in_super_call:
-                    _cache[_hash] = self
-                    result = fn(self, args, kwargs, _original_func=original_func)
-                    del _cache[_hash]
-                else:
-                    result = original_func(self, *args, **kwargs)
-
-                return result
-
-            return original_method_wrapper
+        return wrapper
 
-        return lifecycle_method
+    def __call__(self, *args, **kwargs):
+        if self.instance is None:
+            raise ValueError("You can't call hook as class method")
+
+        gen = self.original_fn(self.instance, *args, **kwargs)
+        result = None
+
+        while True:
+            try:
+                step = gen.send(result)
+            except StopIteration:
+                break
 
-    return _wrapper
+            if step in self.steps:
+                result = self.manager_fn(self.instance, step, args, kwargs)
+            else:
+                raise ValueError(f'Invalid lifecycle step found: {step}. Available steps: {self.steps}')
 
 
 _COMPONENT_INITIALIZED = False
 
 
 class _MetaComponent(_MetaContext):
     def __new__(mcs, _name: str, bases: tuple, namespace: dict, **kwargs):
         initialized = _COMPONENT_INITIALIZED  # As base classes is also declared here, we must be sure base class exists
 
         static_onchange_handlers = []
+        _lifecycle_methods = []
 
-        if initialized:
-            for _attribute_name, child in tuple(mcs._clean_namespace(namespace)):
-                if not (callable(child) and hasattr(child, '_attrs_static_')):
-                    continue
+        base_cls: type[Component] | type = type.__new__(mcs, _name, bases, {})
+
+        for _attribute_name, child in tuple(mcs._clean_namespace(namespace)):
+            if isinstance(child, LifecycleMethod):
+                _lifecycle_methods.append(child.original_fn.__name__)
 
+            if initialized and callable(child) and hasattr(child, '_attrs_static_'):
                 _states_with_static_handler = defaultdict(list)
                 for trigger, _states in child._attrs_static_.items():
                     for _state in _states:
                         _states_with_static_handler[trigger].append(_state)
                         _state.handlers[trigger].remove(child)
                 static_onchange_handlers.append((child, _states_with_static_handler))
 
+        if initialized:
+            for method_name in base_cls._lifecycle_methods:
+                if method := namespace.get(method_name):
+                    # TO THINK: Maybe create base class "AutoInherit" with "_inherit" method?
+                    namespace[method_name] = getattr(base_cls, method_name)._inherit(method)
+
         cls: type[Component] | type = super().__new__(mcs, _name, bases, namespace, **kwargs)
 
         if initialized:
             cls._static_listeners = defaultdict(list, **nested_copy(cls._static_listeners))
             cls._static_onchange_handlers = cls._static_onchange_handlers.copy() + static_onchange_handlers
+            cls._lifecycle_methods = cls._lifecycle_methods.copy() + _lifecycle_methods
         else:
             cls._static_listeners = defaultdict(list)
             cls._static_onchange_handlers = []
+            cls._lifecycle_methods = _lifecycle_methods
 
         if hasattr(cls, '__extra_attributes__'):
             cls.__extra_attributes__ = {
                 key: value.as_child(None) if isinstance(value, Component) else value
                 for key, value in cls.__extra_attributes__.items()
             }
 
-        if '__mount__' in namespace:
-            cls.__mount__ = mcs.__mount(cls.__mount__)
-
-        if '__render__' in namespace:
-            cls.__render__ = mcs.__render(cls.__render__)
-
-        if '__init__' in namespace:
-            cls.__init__ = mcs.__init(cls.__init__)
-
-        if '__unmount__' in namespace:
-            cls.__unmount__ = mcs.__unmount(cls.__unmount__)
-
         return cls
 
-    @_lifecycle_method(hash_function=id)
-    def __init(self: Component, args, kwargs, _original_func):
-        return self.__class__.__META_init__(self, args, kwargs, _original_func)
-
-    @_lifecycle_method()
-    def __mount(self: Component, args, kwargs, _original_func):
-        return self.__class__.__META_mount__(self, args, kwargs, _original_func)
-
-    @_lifecycle_method()
-    def __unmount(self: Component, args, kwargs, _original_func):
-        return self.__class__.__META_unmount__(self, args, kwargs, _original_func)
-
-    @_lifecycle_method()
-    def __render(self: Component, args, kwargs, _original_func):
-        return self.__class__.__META_render__(self, args, kwargs, _original_func)
 
-    @classmethod
-    def __META_init__(cls, self: Component, args, kwargs, _original_func):
-        self._parent_ = None
-
-        self._dependents = []
-        self._listeners = defaultdict(list, **nested_copy(self._static_listeners))
-        self._event_listeners = defaultdict(list)
-        self._handlers = defaultdict(list)
+class Component(WebBase, Context, metaclass=_MetaComponent, _root=True):
+    __slots__ = ('_parent_', '_event_listeners', '_dependents', '_listeners', '_handlers', '_ref')
 
-        self._ref = None
+    parent: Tag | None
+    mount_element: js.HTMLElement | None
 
-        _original_func(self, *args, **kwargs)
+    _ref: ComponentRef | None
+    _force_ref: bool
 
-    @classmethod
-    def __META_mount__(cls, self: Component, args, kwargs, _original_func, *, _mount_attrs=True):
-        result = _original_func(self, *args, **kwargs) if _original_func else None
+    _event_listeners: defaultdict[str, list[Callable[[js.Event], None]]]
+    _static_listeners: defaultdict[str, list[on]]
+    _dependents: list[Renderer]
+    _listeners: defaultdict[str, list[on]]
+    _handlers: defaultdict[str, list[Callable[[Tag, js.Event, str, Any], None]]]
+    _static_onchange_handlers: list[tuple[Callable[[Tag, Any], Any], dict[str, list[state]]]]
+    _lifecycle_methods: list[str]
 
-        if _mount_attrs:
-            self._mount_attrs()
+    @LifecycleMethod
+    def __mount__(self, *args, **kwargs):
+        result = yield 'call'
+        yield 'attrs'
 
         for name, attribute in self.__states__.items():
             if callable(attribute) and not isinstance(attribute, MethodType):
                 setattr(self, name, MethodType(attribute, self.parent))
 
         self._post_mount_attrs()
 
@@ -151,68 +173,77 @@
 
         for onchange_handler, _states_with_static_handler in self._static_onchange_handlers:
             for trigger, _states in _states_with_static_handler.items():
                 for _state in _states:
                     # TODO: can we save order of triggers' call?
                     _state.handlers[trigger].append(MethodType(onchange_handler, self))
 
-        self.mount()
+        yield 'post_call'
 
         return result
 
-    @classmethod
-    def __META_unmount__(cls, self: Component, args, kwargs, _original_func, *, _post_mount=True):
-        if not _post_mount:
-            self.unmount()
-
-        result = _original_func(self, *args, **kwargs) if _original_func else None
+    @__mount__.manager(steps=('call', 'attrs', 'post_call'))
+    def __manager_mount(self, step: str, args: tuple, kwargs: dict):
+        match step:
+            case 'call':
+                return self._mount_(*args, **kwargs)
+            case 'attrs':
+                self._mount_attrs()
+            case 'post_call':
+                self.mount()
 
+    @LifecycleMethod
+    def __unmount__(self, *args, **kwargs):
         if IN_BROWSER:
             for event, event_listeners in self._event_listeners.items():
                 for event_listener in event_listeners:
                     on._remove_listener(event, self, event_listener)
 
-        if _post_mount:
-            self.unmount()
+        yield 'pre_call'
 
+        result = yield 'call'
+        yield 'post_call'
         return result
 
-    @classmethod
-    def __META_render__(cls, self: Component, args, kwargs, _original_func):
+    @__unmount__.manager(steps=('pre_call', 'call', 'post_call'))
+    def __manager_unmount(self, step, args, kwargs):
+        match step:
+            case 'pre_call':
+                self.unmount()
+            case 'call':
+                return self._unmount_(*args, **kwargs)
+            case 'post_call':
+                self.post_unmount()
+
+    @LifecycleMethod
+    def __render__(self, attrs: dict[str, AttrType] | None = None, *args, **kwargs):
         # TODO: maybe function 'render' could return some content, appended to args?
-        self.render()
+        yield 'pre_call'
 
-        attrs: dict[str, AttrType] = args[0] if len(args) > 0 else {}
+        if attrs is None:
+            attrs = {}
 
         for name, value in {**self.__attrs__, **attrs}.items():
             # TODO: optimize this - set only changed attributes
 
             type = _attr.type if (_attr := self.attrs.get(name)) else NONE_TYPE
             set_html_attribute(self.mount_element, name, value, type=type)
 
-        self.post_render()
+        yield 'post_call'
+        yield 'call'
 
-        _original_func(self, *args, **kwargs)
-
-
-class Component(WebBase, Context, metaclass=_MetaComponent, _root=True):
-    __slots__ = ('_parent_', '_event_listeners', '_dependents', '_listeners', '_handlers', '_ref')
-
-    parent: Tag | None
-    mount_element: js.HTMLElement | None
-
-    _ref: ComponentRef | None
-    _force_ref: bool
-
-    _event_listeners: defaultdict[str, list[Callable[[js.Event], None]]]
-    _static_listeners: defaultdict[str, list[on]]
-    _dependents: list[Renderer]
-    _listeners: defaultdict[str, list[on]]
-    _handlers: defaultdict[str, list[Callable[[Tag, js.Event, str, Any], None]]]
-    _static_onchange_handlers: list[tuple[Callable[[Tag, Any], Any], dict[str, list[state]]]]
+    @__render__.manager(steps=('pre_call', 'call', 'post_call'))
+    def __manager_render(self, step, args, kwargs):
+        match step:
+            case 'pre_call':
+                self.render()
+            case 'post_call':
+                self.post_render()
+            case 'call':
+                return self._render_(*args, **kwargs)
 
     @property
     def parent_defined(self):
         return self._parent_ is not None
 
     @property
     def parent(self):
@@ -234,25 +265,34 @@
         ref = beepy.children.ComponentRef(self)
         self.__set_ref__(parent, ref)
         return ref
 
     def __set_ref__(self, parent: Tag | None, ref: ComponentRef):
         self._ref = ref
 
-    def clone(self, parent=None) -> Component:
+    def clone(self, parent=None) -> Self:
         clone = super().clone(parent=parent)
         clone._listeners = defaultdict(list, **nested_copy(self._listeners))
         clone._handlers = defaultdict(list, **nested_copy(self._handlers))
         return clone
 
-    def __init__(self, *args, **kwargs: AttrType):
-        # DO NOT DELETE; This method must be wrapped by _MetaTag.__init
-        super().__init__(*args, **kwargs)
+    def __new__(cls, *args, **kwargs: AttrType):
+        self: Component = super().__new__(cls, *args, **kwargs)
+        self._parent_ = None
+
+        self._dependents = []
+        self._listeners = defaultdict(list, **nested_copy(self._static_listeners))
+        self._event_listeners = defaultdict(list)
+        self._handlers = defaultdict(list)
+
+        self._ref = None
+
+        return self
 
-    def __mount__(self, element, parent: Tag, index=None):
+    def _mount_(self, element, parent: Tag, index=None):  # noqa: ARG002 - unused `element`, `index`
         self.parent = parent
         self.pre_mount()
 
         args, kwargs = self.args_kwargs
         kwargs = self._attrs_defaults | kwargs
         self.init(*args, **kwargs)
 
@@ -266,20 +306,26 @@
 
     def pre_mount(self):
         """empty method for easy override with code for run before mount"""
 
     def mount(self):
         """empty method for easy override with code for run after mount"""
 
+    def _unmount_(self, element, parent, *, _unsafe=False):
+        pass
+
     def unmount(self):
         """empty method for easy override with code for run before unmount"""
 
     def post_unmount(self):
         """empty method for easy override with code for run after unmount"""
 
+    def _render_(self, *args, **kwargs):
+        pass
+
     def render(self):
         """empty method for easy override with code for run before render"""
 
     def post_render(self):
         """empty method for easy override with code for run after render"""
 
     def on(self, method: Callable | str):
@@ -315,22 +361,14 @@
 
 
 class Directive(Component, _root=True):
     _force_ref: bool = True
 
     element = state()
 
-    def __unmount__(self, element, parent, *, _unsafe=False):
-        # DO NOT DELETE; This method must be wrapped by _MetaTag.__unmount
-        pass
-
-    def __render__(self):
-        # DO NOT DELETE; This method must be wrapped by _MetaTag.__render
-        pass
-
     @property
     def el(self):
         if self.element:
             return getattr(self.parent, self.element)
         return self.parent
 
     @property
```

### Comparing `beepy_web-0.8.9/beepy/context.py` & `beepy_web-0.9.0/beepy/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     _contexts: list[Context]
 
     def __new__(mcs, _name: str, bases: tuple, namespace: dict, **kwargs):
         initialized = _CONTEXT_INITIALIZED  # if class Context is already defined
 
         # used for checking inheritance: attributes, methods, etc.
         # for example: extending classes Tag and WithRouter must produce correct state 'router'
+        # TODO: move this (or part of this) to _MetaContext.__init__
         base_cls: type[Context] | type = type.__new__(mcs, _name, bases, {})
 
         namespace = namespace.copy()
         namespace.setdefault('__slots__', ())
         static_attrs = {}
         attrs_defaults = {}
 
@@ -160,36 +161,36 @@
 
     _static_attrs: dict[str, attr]
     _attrs_defaults: dict[str, AttrType]
     attrs: dict[str, attr]
     _context_name_: str
 
     def __new__(cls, *args, **kwargs):
-        parent = kwargs.pop('__parent__', None)
         self = super().__new__(cls)
         self.attrs = self._static_attrs.copy()
 
         # define some attributes here, not in __init__, because they are used for __hash__ method
         self._id_ = get_random_name(log10_ceil(len(self._contexts) * len(self.__class__._context_classes)))
         self._args = args
         self._kwargs = kwargs
 
         if not _CONTEXT_INITIALIZED:
             return self
 
         for name, attribute in self.attrs.items():
             attribute._link_cmpt(name, self, force=False)
-            if parent and name in kwargs:
-                attribute.__set_first__(self, kwargs[name], parent)
-
-        if parent:
-            self.link_parent_attrs(parent)
 
         return self
 
+    def _clone_link_parent(self, parent):
+        for name, attribute in self.attrs.items():
+            if name in self._kwargs:
+                attribute.__set_first__(self, self._kwargs[name], parent)
+        self.link_parent_attrs(parent)
+
     def link_parent_attrs(self, parent):
         p_args, p_kwargs = parent.args_kwargs
         p_data = parent._attrs_defaults | p_kwargs
 
         for name, attr_to_move_on in parent.attrs.items():
             if attr_to_move_on.move_on:
                 attr_to_move_on._link_cmpt(name, self, force_cls_set=True)
@@ -245,16 +246,16 @@
         return hash((self._context_name_, self._id_))
 
     def __notify__(self, attr_name: str, attribute: attr, value: AttrType):
         pass
 
     def clone(self, parent=None) -> Self:
         args, kwargs = self.args_kwargs
-        if parent is not None:
-            kwargs = kwargs | {'__parent__': parent}
-        return type(self)(*args, **kwargs)
+        clone = type(self)(*args, **kwargs)
+        clone._clone_link_parent(parent)
+        return clone
 
 
 _CONTEXT_INITIALIZED = True
 
 
 __all__ = ['OVERWRITE', 'SUPER', 'CONTENT', '_SPECIAL_CHILD_STRINGS', '_MetaContext', 'Context']
```

### Comparing `beepy_web-0.8.9/beepy/framework.py` & `beepy_web-0.9.0/beepy/framework.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 import traceback
 from collections.abc import Callable, Iterable
 from functools import cache
 from types import MethodType
 
-from beepy.attrs import attr, set_html_attribute, state
+from beepy.attrs import attr, state
 from beepy.children import ChildRef, Children, ContentWrapper, CustomWrapper, StringWrapper, TagRef
 from beepy.components import Component, _MetaComponent
 from beepy.context import _SPECIAL_CHILD_STRINGS, CONTENT, OVERWRITE, SUPER
 from beepy.types import AttrType, ContentType, Mounter, Renderer
 from beepy.utils import __CONFIG__, js, log
 from beepy.utils.common import NONE_TYPE, get_random_name, to_kebab_case
 from beepy.utils.dev import _debugger
 from beepy.utils.internal import _PY_TAG_ATTRIBUTE
 
-__version__ = '0.8.9'  # For internal development set to 0.0a0
+__version__ = '0.9.0'  # For internal development set to 0.0a0
 __CONFIG__['version'] = __version__
 
 
 _TAG_INITIALIZED = False
 
 
 class _MetaTag(_MetaComponent):
@@ -163,59 +163,126 @@
         if cls.__ROOT__:
             cls.__root_declared__()
         else:
             cls.__class_declared__()
 
         return cls
 
+
+class Tag(Component, metaclass=_MetaTag, _root=True):
+    # TODO: add docstrings
+
+    __slots__ = (
+        '_content',
+        '_shadow_root',
+        'mount_parent',
+        '_mount_finished_',
+        'mount_element',
+        '_children',
+        '_children_element',
+        '_children_tag',
+    )
+
+    _root_parent: Tag = None  # see function mount in the bottom
+
+    _static_content: ContentType = ''
+
+    _content: ContentType
+    _shadow_root: js.HTMLElement
+    _ref: TagRef | None
+    _force_ref: bool = False
+
+    _tag_name_: str
+    _tags: list[Tag]
+    mount_element: js.HTMLElement
+    mount_parent: js.HTMLElement
+    _static_children: list[ContentType]
+    _children: list[Mounter]
+    _children_element: js.HTMLElement
+    _static_children_tag: Tag
+    _children_tag: Tag
+    _mount_finished_: bool
+
     @classmethod
-    def __META_mount__(cls, self: Tag, args, kwargs, _original_func):
+    def __root_declared__(cls):
+        """This method is called, when root Tag is defined"""
+
+    @classmethod
+    def __class_declared__(cls):
+        """This method is called, when common Tag is defined"""
+
+    def __mount__(self, *args, **kwargs):
         self.__class__._tags.append(self)
 
         self._mount_finished_ = False
 
-        result = _original_func(self, *args, **kwargs)
-
-        self._mount_attrs()
+        result = yield 'call'
+        yield 'attrs'
 
         for child in self.children:
             if isinstance(child, CustomWrapper):
                 child.__mount__(self.mount_element, self)
             elif isinstance(child, Mounter):
                 child.__mount__(self._children_element, self)
             else:
                 log.warn(f'Cannot mount: {child}')
+
         if self._children_tag:
             self.mount_element.insertChild(self._children_element)
 
-        if self.content_child is None:
-            _debugger(self)
+        if (content_child := self.get_content_child()) is None:
+            _debugger(self)  # wtf?
         else:
-            self.content_child._mount_children()
+            content_child._mount_children()
 
-        super().__META_mount__(self, args, kwargs, None, _mount_attrs=False)
+        super().__mount__.call_as_super(self, args, kwargs)
 
         self._mount_finished_ = True
 
+        yield 'post_call'
+
         return result
 
-    @classmethod
-    def __META_render__(cls, self: Tag, args, kwargs, _original_func):
+    def __unmount__(self, *args, **kwargs):
+        if self in self.__class__._tags:  # But why?
+            self.__class__._tags.remove(self)
+
+        super().__unmount__.call_as_super(self, args, kwargs)
+
+        yield 'pre_call'
+
+        for child in self.children:
+            if isinstance(child, CustomWrapper):
+                child.__unmount__(self.mount_element, self)
+            elif isinstance(child, Mounter):
+                child.__unmount__(self._children_element, self)
+        if self._children_tag:
+            self.mount_element.safeRemoveChild(self._children_element)
+
+        result = yield 'call'
+        yield 'post_call'
+        return result
+
+    def __render__(self, *args, **kwargs):
         if not self._mount_finished_ or (
             not self.mount_element.parentElement and self._root_parent != self  # dismounted
         ):
             return  # Prevent render before mount finished; Could be useful for setting intervals inside mount method
 
-        return super().__META_render__(self, args, kwargs, _original_func)
+        yield from super().__render__.original_fn(self, *args, **kwargs)
 
-    @classmethod
-    def __META_init__(cls, self: Tag, args, kwargs, _original_func):  # noqa: PLR0912, PLR0915
-        kwargs.pop('__parent__', None)  # called from clone
-        if hasattr(getattr(self, 'mount_element', None), _PY_TAG_ATTRIBUTE):
-            return
+    def __init__(self, *args, **kwargs: AttrType):
+        kwargs.setdefault('_load_children', False)
+        super().__init__(*args, **kwargs)
+
+    def __new__(cls, *args, **kwargs):  # noqa: PLR0915, PLR0912 - Statements (60 > 50)  +  Branches (23 > 12)
+        if hasattr(getattr(cls, 'mount_element', None), _PY_TAG_ATTRIBUTE):
+            return getattr(cls.mount_element, _PY_TAG_ATTRIBUTE)
+
+        self: Tag = super().__new__(cls, *args, **kwargs)
 
         self._children = self._static_children.copy()
         self._content = self._static_content
 
         children_argument: Callable | ContentType = kwargs.get('children') or args
         if children_argument and (not isinstance(children_argument, Iterable) or isinstance(children_argument, str)):
             children_argument = [children_argument]
@@ -278,90 +345,14 @@
             self._children_tag = self._static_children_tag.clone(self)
             self._children_element = self._children_tag.mount_element
             setattr(self._children_element, _PY_TAG_ATTRIBUTE, self)
         else:
             self._children_tag = None
             self._children_element = self.mount_element
 
-        super().__META_init__(self, args, kwargs, _original_func)
-
-    @classmethod
-    def __META_unmount__(cls, self: Tag, args, kwargs, _original_func):
-        if self in self.__class__._tags:  # But why?
-            self.__class__._tags.remove(self)
-
-        super().__META_unmount__(self, args, kwargs, None, _post_mount=False)
-
-        for child in self.children:
-            if isinstance(child, CustomWrapper):
-                child.__unmount__(self.mount_element, self)
-            elif isinstance(child, Mounter):
-                child.__unmount__(self._children_element, self)
-        if self._children_tag:
-            self.mount_element.safeRemoveChild(self._children_element)
-
-        result = _original_func(self, *args, **kwargs)
-
-        self.post_unmount()
-
-        return result
-
-
-class Tag(Component, metaclass=_MetaTag, _root=True):
-    # TODO: add docstrings
-
-    __slots__ = (
-        '_content',
-        '_shadow_root',
-        'mount_parent',
-        '_mount_finished_',
-        'mount_element',
-        '_children',
-        '_children_element',
-        '_children_tag',
-    )
-
-    _root_parent: Tag = None  # see function mount in the bottom
-
-    _static_content: ContentType = ''
-
-    _content: ContentType
-    _shadow_root: js.HTMLElement
-    _ref: TagRef | None
-    _force_ref: bool = False
-
-    _tag_name_: str
-    _tags: list[Tag]
-    mount_element: js.HTMLElement
-    mount_parent: js.HTMLElement
-    _static_children: list[ContentType]
-    _children: list[Mounter]
-    _children_element: js.HTMLElement
-    _static_children_tag: Tag
-    _children_tag: Tag
-    _mount_finished_: bool
-
-    @classmethod
-    def __root_declared__(cls):
-        """This method is called, when root Tag is defined"""
-
-    @classmethod
-    def __class_declared__(cls):
-        """This method is called, when common Tag is defined"""
-
-    def __init__(self, *args, **kwargs: AttrType):
-        kwargs.setdefault('_load_children', False)
-        super().__init__(*args, **kwargs)
-
-    def __new__(cls, *args, **kwargs):
-        if hasattr(getattr(cls, 'mount_element', None), _PY_TAG_ATTRIBUTE):
-            self = getattr(cls.mount_element, _PY_TAG_ATTRIBUTE)
-        else:
-            self = super().__new__(cls, *args, **kwargs)
-
         return self
 
     def __repr__(self):
         return f'{type(self).__name__}(<{self._tag_name_}/>, id#{self._id_})'
 
     def __hash__(self):
         # TODO: make force immutable this attributes
@@ -386,26 +377,17 @@
         self.__render__()
 
     def __set_ref__(self, parent: Tag | None, ref: TagRef):
         super().__set_ref__(parent, ref)
         if ref.inline_def:
             setattr(type(parent), ref.name, self)
 
-    def __render__(self, attrs: dict[str, AttrType] | None = None):
+    def _render_(self, attrs: dict[str, AttrType] | None = None):  # noqa: ARG002 - unused `attrs`
         self._current_render.append(self)
 
-        if attrs is None:
-            attrs = {}
-
-        for name, value in {**self.__attrs__, **attrs}.items():
-            # TODO: optimize this - set only changed attributes
-
-            type = _attr.type if (_attr := self.attrs.get(name)) else NONE_TYPE
-            set_html_attribute(self.mount_element, name, value, type=type)
-
         content_index = self.get_content_index()
         if content_index is not None:
             self.children[content_index].__render__()
 
         for index, child in enumerate(self.children):
             # TODO: optimize this - re-render the only children, that need this
             if isinstance(child, ChildRef):
@@ -433,22 +415,22 @@
                 continue
 
             if isinstance(value, Children):
                 getattr(self, name)[:] = kwargs[name]
 
         super().init(*args, **kwargs)
 
-    def __mount__(self, element, parent: Tag, index=None):
+    def _mount_(self, element, parent: Tag, index=None):
         self.mount_parent = element
 
-        super().__mount__(element, parent, index=index)
+        super()._mount_(element, parent, index=index)
 
         self.mount_parent.insertChild(self.mount_element, index)
 
-    def __unmount__(self, element, parent, *, _unsafe=False):
+    def _unmount_(self, element, parent, *, _unsafe=False):
         if not _unsafe and self.mount_parent is not None and self.mount_parent is not element:
             log.warn(
                 'Something went wrong!\n'
                 f'Real parent: {self.mount_parent} {self.parent}. Passed parent: {element} {parent} '
                 'If you override __mount__, you also should override __unmount__ too.'
             )
             log.warn(''.join(traceback.format_stack()[:-1]))
@@ -459,16 +441,15 @@
     def own_children(self) -> list[Mounter]:
         return [child for child in self.children if not isinstance(child, ChildRef | CustomWrapper)]
 
     @property
     def ref_children(self) -> dict[str, Mounter]:
         return {child.name: child.__get__(self) for child in self.children if isinstance(child, ChildRef)}
 
-    @property
-    def content_child(self) -> ContentWrapper:
+    def get_content_child(self) -> ContentWrapper:
         for child in self.children:
             if isinstance(child, ContentWrapper) and child.content.__func__.__name__ == 'content':
                 return child
 
     def get_content_index(self):
         for index, child in enumerate(self.children):
             if isinstance(child, ContentWrapper) and child.content.__func__.__name__ == 'content':
@@ -476,17 +457,14 @@
 
     @property
     def children(self) -> list[Mounter | Renderer | ChildRef | ContentWrapper]:
         return self._children
 
     @children.setter
     def children(self, children):
-        self._children = self._handle_children(children)
-
-    def _handle_children(self, children):
         result = []
 
         for new_child in children:
             child = new_child
 
             if isinstance(child, ContentWrapper):
                 child = child.content.__func__
@@ -511,17 +489,17 @@
             elif callable(child):
                 if not isinstance(child, MethodType):
                     child = MethodType(child, self)
                 child = ContentWrapper(child, self._content_tag, self._current_render)
 
             result.append(child)
 
-        return result
+        self._children = result
 
-    def clone(self, parent=None) -> Tag:
+    def clone(self, parent=None):
         clone = super().clone(parent=parent)
         clone._children = self.children
         return clone
 
     @property
     def _current_render(self):
         try:
```

### Comparing `beepy_web-0.8.9/beepy/listeners.py` & `beepy_web-0.9.0/beepy/listeners.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/router.py` & `beepy_web-0.9.0/beepy/router.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/style.py` & `beepy_web-0.9.0/beepy/style.py`

 * *Files 5% similar despite different names*

```diff
@@ -168,23 +168,23 @@
         self.options = {
             'global': False,
             'render_states': True,
             'render_children': True,
             'get_vars_callback': get_vars,
         } | options
 
-    def __mount__(self, element, parent, index=None):
+    def _mount_(self, element, parent, index=None):
         self.real_parent = parent
         if __CONFIG__['style_head']:
-            super().__mount__(Head.mount_element, Head)
+            super()._mount_(Head.mount_element, Head)
         else:
-            super().__mount__(element, parent, index)
+            super()._mount_(element, parent, index)
 
-    def __unmount__(self, element, parent, *, _unsafe=False):
-        return super().__unmount__(element, parent, _unsafe=True)
+    def _unmount_(self, element, parent, *, _unsafe=False):
+        return super()._unmount_(element, parent, _unsafe=True)
 
     def mount(self):
         styles = {Raw(): '{__VARS__}'} | self.styles
         parent = self.real_parent
 
         if self.options['global']:  # TODO: add example
             self._content = dict_to_css(styles, parent._tag_name_)
```

### Comparing `beepy_web-0.8.9/beepy/tags.py` & `beepy_web-0.9.0/beepy/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,15 @@
 class option(html_tag, name='option'):
     value = html_attr()
     label = html_attr('')
     defaultSelected = html_attr(default=False)
     selected = html_attr(default=False)
 
 
+# TODO: fix bug with <select>    (click "Selector", then click "Admin panel" and see Group selection...)
 class select(html_tag, name='select'):
     value = html_attr(model='change')
 
     children = [
         options := Children(),
     ]
 
@@ -205,15 +206,15 @@
 
 
 class StandaloneTag(html_tag, _root=True):
     def __init__(self, *args, **kwargs):
         kwargs['_load_children'] = True
         super().__init__(*args, **kwargs)
 
-    def __mount__(self, element, parent: Tag, index=None):
+    def _mount_(self, element, parent: Tag, index=None):  # noqa: ARG002 - unused `index`
         # too many copy-paste?
         self.parent = parent
         self.mount_parent = element
         self.pre_mount()
 
     def clone(self, parent=None):  # noqa: ARG002 - arguments for overriding
         return self
```

### Comparing `beepy_web-0.8.9/beepy/trackable.py` & `beepy_web-0.9.0/beepy/trackable.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/types.py` & `beepy_web-0.9.0/beepy/types.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/modules/context_menu.py` & `beepy_web-0.9.0/beepy/modules/context_menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,19 +79,19 @@
         if y + el.offsetHeight > js.innerHeight:
             y -= el.offsetHeight
 
         self.pos_x = x
         self.pos_y = y
         self.show()
 
-    def __mount__(self, element, parent, index=None):
-        super().__mount__(Body.mount_element, Body)
+    def _mount_(self, element, parent, index=None):  # noqa: ARG002 - unused arguments
+        super()._mount_(Body.mount_element, Body)
 
-    def __unmount__(self, element, parent, *, _unsafe=False):
-        return super().__unmount__(element, parent, _unsafe=True)
+    def _unmount_(self, element, parent, *, _unsafe=False):
+        return super()._unmount_(element, parent, _unsafe=True)
 
 
 class ContextMenuHandler(div):
     menu: ContextMenu
 
     default_style = Style(
         position='absolute',
```

### Comparing `beepy_web-0.8.9/beepy/modules/local_storage.py` & `beepy_web-0.9.0/beepy/modules/local_storage.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/modules/modal.py` & `beepy_web-0.9.0/beepy/modules/modal.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,19 +50,19 @@
     @on('keyup.esc')
     @button_close.on('click')
     def close(self):
         self.visible = False
         if self.on_close:
             self.on_close()
 
-    def __mount__(self, element, parent, index=None):
-        super().__mount__(Body.mount_element, Body)
+    def _mount_(self, element, parent, index=None):  # noqa: ARG002 - unused arguments
+        super()._mount_(Body.mount_element, Body)
 
-    def __unmount__(self, element, parent, *, _unsafe=False):
-        return super().__unmount__(element, parent, _unsafe=True)
+    def _unmount_(self, element, parent, *, _unsafe=False):
+        return super()._unmount_(element, parent, _unsafe=True)
 
 
 class ModalHandler(div, content_tag=div()):
     modal: Modal
 
     default_style = Style()
```

### Comparing `beepy_web-0.8.9/beepy/modules/table.py` & `beepy_web-0.9.0/beepy/modules/table.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/modules/tabs.py` & `beepy_web-0.9.0/beepy/modules/tabs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/utils/api.py` & `beepy_web-0.9.0/beepy/utils/api.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/utils/asyncio.py` & `beepy_web-0.9.0/beepy/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/utils/common.py` & `beepy_web-0.9.0/beepy/utils/common.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/utils/dev.py` & `beepy_web-0.9.0/beepy/utils/dev.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/utils/import_hooks.py` & `beepy_web-0.9.0/beepy/utils/import_hooks.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/utils/internal.py` & `beepy_web-0.9.0/beepy/utils/internal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/beepy/utils/js.py` & `beepy_web-0.9.0/beepy/utils/js.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,33 +2,35 @@
 This file is partly mock of JS API, created to make possible run and debug BeePy apps using console
 """
 
 from __future__ import annotations
 
 import time
 from collections import defaultdict
+from collections.abc import Callable
 from threading import Thread
 from typing import TYPE_CHECKING, Self
 
 try:
     from pyodide.ffi import IN_BROWSER, create_once_callable, create_proxy
 except ImportError:
     from pyodide import IN_BROWSER, create_once_callable, create_proxy
 
 
 class HTMLElement:
     __PYTHON_TAG__: Tag
 
-    def __init__(self, tag_name):
+    def __init__(self, tag_name, *, _parent=None):
         self.attributes = {}
         self.data = []
         self.listeners = defaultdict(list)
         self.tagName = tag_name
         self.shadowRoot = None
         self.clientWidth = self.clientHeight = self.scrollWidth = self.scrollHeight = 1
+        self.parentElement = _parent
 
     def getAttribute(self, name):
         return self.attributes.get(name)
 
     def setAttribute(self, name, value):
         self.attributes[name] = value
 
@@ -40,14 +42,17 @@
         print(self)
 
     def appendChild(self, el: HTMLElement):
         self.data.append(el)
         print(self)
 
     def insertChild(self, el: HTMLElement | str, index: int = None):
+        if not isinstance(el, str):
+            el.parentElement = self
+
         if index is None:
             self.data.append(el)
         else:
             self.data.insert(index, el)
         print(self)
 
     def removeChild(self, child: HTMLElement):
@@ -267,54 +272,53 @@
     from beepy.framework import Tag
 
 
 class BeePyModule:
     config = {}
 
     def addElement(self, mount_point, element_name, **options):
-        return HTMLElement(element_name)
+        return HTMLElement(element_name, _parent=mount_point)
 
     def startLoading(self, *a, **kw):
         return
 
     def stopLoading(self):
         return
 
     def addAsyncListener(self, el, eventName, method, modifiers, **options):
         return
 
     class files:
         _lastLoadedFile = ''
 
-        def getPathWithCurrentPathAndOrigin(self, path):
+        @staticmethod
+        def getPathWithCurrentPathAndOrigin(path):
             return path
 
     class dev_server:
         started = True
 
 
 beepy = BeePyModule()
 _locals = {}
 window = self = globalThis = Self
 
 
+# Mock of pyodide functions, but without `.destroy()`
+# For testing outside of browser
+
 #################
 #       .       #
 #       .       #
 # . . . . . . . #
 #       .       #
 #       .       #
 #################
 
 
-class Destroyable:
-    def destroy(self):
-        pass
-
-
 EVENT_LISTENERS = {}
 
 
 def add_event_listener(elt, event, listener):
     """Wrapper for JavaScript's addEventListener() which automatically manages the lifetime
     of a JsProxy corresponding to the listener param.
     """
@@ -323,20 +327,18 @@
     elt.addEventListener(event, proxy)
 
 
 def remove_event_listener(elt, event, listener):
     """Wrapper for JavaScript's removeEventListener() which automatically manages the lifetime
     of a JsProxy corresponding to the listener param.
     """
-    proxy = EVENT_LISTENERS.pop((elt.js_id, event, listener))
-    elt.removeEventListener(event, proxy)
-    proxy.destroy()
+    elt.removeEventListener(event, EVENT_LISTENERS.pop((elt.js_id, event, listener)))
 
 
-TIMEOUTS: dict[int, Destroyable] = {}
+TIMEOUTS: dict[int, Callable] = {}
 
 
 def set_timeout(callback, timeout):
     """Wrapper for JavaScript's setTimeout() which automatically manages the lifetime
     of a JsProxy corresponding to the callback param.
     """
     id = -1
@@ -347,33 +349,23 @@
 
     callable = create_once_callable(wrapper)
     id = setTimeout(callable, timeout)
     TIMEOUTS[id] = callable
     return id
 
 
-# An object with a no-op destroy method so we can do
-#
-# TIMEOUTS.pop(id, DUMMY_DESTROYABLE).destroy()
-#
-# and either it gets a real object and calls the real destroy method or it gets
-# the fake which does nothing. This is to handle the case where clear_timeout is
-# called after the timeout executes.
-DUMMY_DESTROYABLE = Destroyable()
-
-
 def clear_timeout(id):
     """Wrapper for JavaScript's clearTimeout() which automatically manages the lifetime
     of a JsProxy corresponding to the callback param.
     """
     clearTimeout(id)
-    TIMEOUTS.pop(id, DUMMY_DESTROYABLE).destroy()
+    TIMEOUTS.pop(id, None)
 
 
-INTERVAL_CALLBACKS: dict[int, Destroyable] = {}
+INTERVAL_CALLBACKS: dict[int, Callable] = {}
 
 
 def set_interval(callback, interval):
     """Wrapper for JavaScript's setInterval() which automatically manages the lifetime
     of a JsProxy corresponding to the callback param.
     """
     proxy = create_proxy(callback)
@@ -383,8 +375,8 @@
 
 
 def clear_interval(id):
     """Wrapper for JavaScript's clearInterval() which automatically manages the lifetime
     of a JsProxy corresponding to the callback param.
     """
     clearInterval(id)
-    INTERVAL_CALLBACKS.pop(id, DUMMY_DESTROYABLE).destroy()
+    INTERVAL_CALLBACKS.pop(id, None)
```

### Comparing `beepy_web-0.8.9/beepy/utils/js_py.py` & `beepy_web-0.9.0/beepy/utils/js_py.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,26 @@
 except ModuleNotFoundError:
     from . import js
 
     js.window = js.self = js.globalThis = js
 
 from pyodide.ffi import IN_BROWSER, create_once_callable, create_proxy
 from pyodide.ffi import to_js as pyodide_to_js
-from pyodide.ffi.wrappers import (
-    add_event_listener,
-    clear_interval,
-    clear_timeout,
-    remove_event_listener,
-    set_interval,
-    set_timeout,
-)
+
+if IN_BROWSER:
+    from pyodide.ffi.wrappers import (
+        add_event_listener,
+        clear_interval,
+        clear_timeout,
+        remove_event_listener,
+        set_interval,
+        set_timeout,
+    )
+else:
+    from .js import add_event_listener, clear_interval, clear_timeout, remove_event_listener, set_interval, set_timeout
 
 log = js.console
 
 
 class Interval:
     __slots__ = ('_id',)
```

### Comparing `beepy_web-0.8.9/web/package-lock.json` & `beepy_web-0.9.0/web/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899982970027248%*

 * *Differences: {"'packages'": "{'': {'version': '0.8.10'}}", "'version'": "'0.8.10'"}*

```diff
@@ -12,15 +12,15 @@
                 "webpack": "^5.89.0",
                 "webpack-cli": "^5.1.4",
                 "webpack-dev-server": "^4.15.1",
                 "webpack-merge": "^5.10.0"
             },
             "license": "MIT",
             "name": "@kor0p/beepy",
-            "version": "0.8.9"
+            "version": "0.8.10"
         },
         "node_modules/@discoveryjs/json-ext": {
             "dev": true,
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==",
@@ -4174,9 +4174,9 @@
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         }
     },
     "requires": true,
-    "version": "0.8.9"
+    "version": "0.8.10"
 }
```

### Comparing `beepy_web-0.8.9/web/package.json` & `beepy_web-0.9.0/web/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.8.10'"}*

```diff
@@ -32,9 +32,9 @@
     "scripts": {
         "build": "webpack --config webpack.prod.js",
         "publish-2": "cp ../README.md . && npm publish --access=public && rm README.md",
         "start": "webpack serve --config webpack.dev.js",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch"
     },
-    "version": "0.8.9"
+    "version": "0.8.10"
 }
```

### Comparing `beepy_web-0.8.9/web/webpack.prod.js` & `beepy_web-0.9.0/web/webpack.prod.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/web/src/beepy.js` & `beepy_web-0.9.0/web/src/beepy.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,15 @@
 const _script = document.currentScript
 let localConfig = {}
 if (!!window.beepy) {
     localConfig = window.beepy
 }
 
 class BeePy {
-    __version__ = '0.8.9'
+    __version__ = '0.9.0'
 
     pyodideIndexURL = null
     globals = null
     dev_server = dev_server
     dev_path = ''
     python_api = python
```

### Comparing `beepy_web-0.8.9/web/src/dev-server.js` & `beepy_web-0.9.0/web/src/dev-server.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/web/src/files.js` & `beepy_web-0.9.0/web/src/files.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/web/src/main.css` & `beepy_web-0.9.0/web/src/main.css`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/web/src/python.js` & `beepy_web-0.9.0/web/src/python.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/web/src/utils.js` & `beepy_web-0.9.0/web/src/utils.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/.gitignore` & `beepy_web-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/LICENSE` & `beepy_web-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beepy_web-0.8.9/README.md` & `beepy_web-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # 🐝 BeePy
 
 [![NPM Package](https://img.shields.io/npm/v/@kor0p/beepy)](https://www.npmjs.com/package/@kor0p/beepy)
-[![Documentation](https://readthedocs.org/projects/bee-py/badge/?version=latest)](https://bee-py.readthedocs.io/en/latest/)
+[![PyPI Package](https://img.shields.io/pypi/v/beepy-web.svg)](https://pypi.org/project/beepy-web/)
+[![Documentation](https://cdn.jsdelivr.net/gh/Andre601/devins-badges@v3.x-mkdocs-material/assets/compact-minimal/built-with/mkdocs-material_vector.svg)](https://kor0p.github.io/BeePy/)
 
 ## The _frontend_ web framework for python
 ### Thanks for [Pyodide](https://pyodide.org/) - port of Python to [Emscripten](https://emscripten.org/), based on [WASM](https://webassembly.org/).
 ### Use Python in browser to build modern frontend via BeePy!
 
-## Try it out! [CodeSandBox](https://codesandbox.io/s/beepy-two-synced-counters-k5sm9j) and [BeePy Sandbox](https://kor0p.github.io/BeePy/examples/sandbox/)
+## Try it out! [CodeSandBox](https://codesandbox.io/s/beepy-two-synced-counters-k5sm9j) and [BeePy Sandbox](https://kor0p.github.io/BeePy-examples/sandbox)
 
 ## Join our community at [Telegram chat](https://t.me/bee_py/)
 
 ## Local development:
-### Firstly, install BeePy
+### Install BeePy
 ### `pip install -U beepy-web[dev]`
-### Then, add `index.html` and `__init__.py` to root of project
-### and start local server at same directory
-### `python -m beepy.dev`
-### That's it!
+### Then just start local server
+### `python -m beepy.dev --create`
+### And that's it!
+
 ### Now, click on link in console to visit your server
 ### and change code to see updates in browser in no time!
 
 Code (custom_url.py from examples):
 ```python
 from beepy import Tag, mount, state, on
 
@@ -57,8 +58,8 @@
 - [Modal](https://beepy-web-ba63e5a12994.herokuapp.com/e/modal)
 - [Context Menu](https://beepy-web-ba63e5a12994.herokuapp.com/e/context-menu)
 - [Dynamic URL](https://beepy-web-ba63e5a12994.herokuapp.com/e/dynamic-url)
 - [Timer](https://beepy-web-ba63e5a12994.herokuapp.com/e/timer)
 - [Input's model](https://beepy-web-ba63e5a12994.herokuapp.com/e/text-sync)
 - [Multiple apps on one page](https://beepy-web-ba63e5a12994.herokuapp.com/multiple-apps)
 - [Just the other one example](https://beepy-web-ba63e5a12994.herokuapp.com/e/custom_url)
-- [BeePy Sandbox](https://kor0p.github.io/BeePy/examples/sandbox/)
+- [BeePy Sandbox](https://kor0p.github.io/BeePy-examples/sandbox)
```

### Comparing `beepy_web-0.8.9/pyproject.toml` & `beepy_web-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 requires-python = ">=3.10.10"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "pyodide-py==0.24.1", # Pyodide package
+    "pyodide-py==0.25.1", # Pyodide package
     "python-dotenv==1.0.0", # .env file to os.environ
     "boltons==23.1.1", # Better builtins
 ]
 
 [project.urls]
 "Homepage" = "https://bit.ly/beepy"
 "Repository" = "https://github.com/kor0p/BeePy"
-"Docs" = "https://bee-py.readthedocs.io/en/latest/"
+"Docs" = "https://kor0p.github.io/BeePy/"
 
 [project.optional-dependencies]
 dev = [
     "micropip==0.3.0", # A lightweight Python package installer for the web
     "watchdog==3.0.0", # watcher for files that changes for Hot reload
     "websockets==11.0.3", # Hot reload is working using simple WebSockets server
     "requests==2.31.0", # HTTP synchronous requests lib
@@ -38,16 +38,16 @@
 [tool.hatch.version]
 path = "beepy/framework.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
     "/.github",
     "/.idea",
+    "mkdocs.yml",
     "/docs",
-    ".readthedocs.yaml",
     "/backend",
     "/examples",
     "app.json",
     "Procfile",
 ]
 
 [tool.hatch.build.targets.wheel]
```

### Comparing `beepy_web-0.8.9/PKG-INFO` & `beepy_web-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 Metadata-Version: 2.1
 Name: beepy-web
-Version: 0.8.9
+Version: 0.9.0
 Summary: The modern frontend web framework for Python
 Project-URL: Homepage, https://bit.ly/beepy
 Project-URL: Repository, https://github.com/kor0p/BeePy
-Project-URL: Docs, https://bee-py.readthedocs.io/en/latest/
+Project-URL: Docs, https://kor0p.github.io/BeePy/
 Author-email: kor0p <3.kor0p@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.10
 Requires-Dist: boltons==23.1.1
-Requires-Dist: pyodide-py==0.24.1
+Requires-Dist: pyodide-py==0.25.1
 Requires-Dist: python-dotenv==1.0.0
 Provides-Extra: contributing
 Requires-Dist: pre-commit; extra == 'contributing'
 Provides-Extra: dev
 Requires-Dist: micropip==0.3.0; extra == 'dev'
 Requires-Dist: requests==2.31.0; extra == 'dev'
 Requires-Dist: watchdog==3.0.0; extra == 'dev'
 Requires-Dist: websockets==11.0.3; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # 🐝 BeePy
 
 [![NPM Package](https://img.shields.io/npm/v/@kor0p/beepy)](https://www.npmjs.com/package/@kor0p/beepy)
-[![Documentation](https://readthedocs.org/projects/bee-py/badge/?version=latest)](https://bee-py.readthedocs.io/en/latest/)
+[![PyPI Package](https://img.shields.io/pypi/v/beepy-web.svg)](https://pypi.org/project/beepy-web/)
+[![Documentation](https://cdn.jsdelivr.net/gh/Andre601/devins-badges@v3.x-mkdocs-material/assets/compact-minimal/built-with/mkdocs-material_vector.svg)](https://kor0p.github.io/BeePy/)
 
 ## The _frontend_ web framework for python
 ### Thanks for [Pyodide](https://pyodide.org/) - port of Python to [Emscripten](https://emscripten.org/), based on [WASM](https://webassembly.org/).
 ### Use Python in browser to build modern frontend via BeePy!
 
-## Try it out! [CodeSandBox](https://codesandbox.io/s/beepy-two-synced-counters-k5sm9j) and [BeePy Sandbox](https://kor0p.github.io/BeePy/examples/sandbox/)
+## Try it out! [CodeSandBox](https://codesandbox.io/s/beepy-two-synced-counters-k5sm9j) and [BeePy Sandbox](https://kor0p.github.io/BeePy-examples/sandbox)
 
 ## Join our community at [Telegram chat](https://t.me/bee_py/)
 
 ## Local development:
-### Firstly, install BeePy
+### Install BeePy
 ### `pip install -U beepy-web[dev]`
-### Then, add `index.html` and `__init__.py` to root of project
-### and start local server at same directory
-### `python -m beepy.dev`
-### That's it!
+### Then just start local server
+### `python -m beepy.dev --create`
+### And that's it!
+
 ### Now, click on link in console to visit your server
 ### and change code to see updates in browser in no time!
 
 Code (custom_url.py from examples):
 ```python
 from beepy import Tag, mount, state, on
 
@@ -81,8 +82,8 @@
 - [Modal](https://beepy-web-ba63e5a12994.herokuapp.com/e/modal)
 - [Context Menu](https://beepy-web-ba63e5a12994.herokuapp.com/e/context-menu)
 - [Dynamic URL](https://beepy-web-ba63e5a12994.herokuapp.com/e/dynamic-url)
 - [Timer](https://beepy-web-ba63e5a12994.herokuapp.com/e/timer)
 - [Input's model](https://beepy-web-ba63e5a12994.herokuapp.com/e/text-sync)
 - [Multiple apps on one page](https://beepy-web-ba63e5a12994.herokuapp.com/multiple-apps)
 - [Just the other one example](https://beepy-web-ba63e5a12994.herokuapp.com/e/custom_url)
-- [BeePy Sandbox](https://kor0p.github.io/BeePy/examples/sandbox/)
+- [BeePy Sandbox](https://kor0p.github.io/BeePy-examples/sandbox)
```

