# Comparing `tmp/python_injection-0.8.1.post0.tar.gz` & `tmp/python_injection-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_injection-0.8.1.post0.tar", max compression
+gzip compressed data, was "python_injection-0.8.2.tar", max compression
```

## Comparing `python_injection-0.8.1.post0.tar` & `python_injection-0.8.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     3049 2024-04-03 18:32:39.943349 python_injection-0.8.1.post0/documentation/basic-usage.md
--rw-r--r--   0        0        0       20 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/__init__.py
--rw-r--r--   0        0        0      647 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/_pkg.py
--rw-r--r--   0        0        0     5327 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/_pkg.pyi
--rw-r--r--   0        0        0        0 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/__init__.py
--rw-r--r--   0        0        0     1316 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/event.py
--rw-r--r--   0        0        0      558 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/invertible.py
--rw-r--r--   0        0        0     1401 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/lazy.py
--rw-r--r--   0        0        0     1443 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/queue.py
--rw-r--r--   0        0        0        0 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/tools/__init__.py
--rw-r--r--   0        0        0      271 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/tools/threading.py
--rw-r--r--   0        0        0     1276 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/common/tools/type.py
--rw-r--r--   0        0        0       22 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/core/__init__.py
--rw-r--r--   0        0        0    18952 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/core/module.py
--rw-r--r--   0        0        0      653 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/integrations/__init__.py
--rw-r--r--   0        0        0      723 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/integrations/blacksheep.py
--rw-r--r--   0        0        0      676 2024-04-03 18:32:39.947349 python_injection-0.8.1.post0/injection/utils.py
--rw-r--r--   0        0        0     1212 2024-04-03 18:33:44.384278 python_injection-0.8.1.post0/pyproject.toml
--rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 python_injection-0.8.1.post0/PKG-INFO
+-rw-r--r--   0        0        0     3047 2024-04-11 08:00:09.618740 python_injection-0.8.2/documentation/basic-usage.md
+-rw-r--r--   0        0        0      609 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/__init__.py
+-rw-r--r--   0        0        0     5395 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/__init__.py
+-rw-r--r--   0        0        0     1316 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/event.py
+-rw-r--r--   0        0        0      558 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/invertible.py
+-rw-r--r--   0        0        0     1401 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/lazy.py
+-rw-r--r--   0        0        0     1443 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/queue.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/tools/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/tools/threading.py
+-rw-r--r--   0        0        0     1276 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/common/tools/type.py
+-rw-r--r--   0        0        0       22 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/core/__init__.py
+-rw-r--r--   0        0        0    19663 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/core/module.py
+-rw-r--r--   0        0        0      653 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/integrations/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/integrations/blacksheep.py
+-rw-r--r--   0        0        0      676 2024-04-11 08:00:09.622740 python_injection-0.8.2/injection/utils.py
+-rw-r--r--   0        0        0     1206 2024-04-11 08:00:32.710757 python_injection-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 python_injection-0.8.2/PKG-INFO
```

### Comparing `python_injection-0.8.1.post0/documentation/basic-usage.md` & `python_injection-0.8.2/documentation/basic-usage.md`

 * *Files 2% similar despite different names*

```diff
@@ -115,24 +115,24 @@
     ...
 
 @injectable(on=(AbstractService, ConcreteService))
 class ConcreteServiceOverload(ConcreteService):
     ...
 ```
 
-If a class is registered in a package and you want to override it, there is the `override` parameter:
+If a class is registered in a package and you want to override it, there is the `mode` parameter:
 
 ```python
 @injectable
 class InaccessibleService:
     ...
 
 # ...
 
-@injectable(on=InaccessibleService, override=True)
+@injectable(on=InaccessibleService, mode="override")
 class ServiceOverload(InaccessibleService):
     ...
 ```
 
 ## Recipes
 
 A recipe is a function that tells the injector how to construct the instance to be injected. It is important to specify
```

### Comparing `python_injection-0.8.1.post0/injection/_pkg.py` & `python_injection-0.8.2/injection/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from .core import Injectable, Module, ModulePriority
+from .core import Injectable, Module
 
 __all__ = (
     "Injectable",
     "Module",
-    "ModulePriority",
     "default_module",
     "get_instance",
     "get_lazy_instance",
     "inject",
     "injectable",
     "set_constant",
     "should_be_injectable",
```

### Comparing `python_injection-0.8.1.post0/injection/_pkg.pyi` & `python_injection-0.8.2/injection/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from abc import abstractmethod
 from collections.abc import Callable, Iterable
 from contextlib import ContextDecorator
-from enum import Enum
 from types import UnionType
 from typing import (
     Any,
     ContextManager,
     Final,
+    Literal,
     Protocol,
     TypeVar,
     final,
     runtime_checkable,
 )
 
-from injection.common.invertible import Invertible
+from .common.invertible import Invertible
 
 _T = TypeVar("_T")
 
 default_module: Final[Module] = ...
 
 get_instance = default_module.get_instance
 get_lazy_instance = default_module.get_lazy_instance
@@ -50,30 +50,30 @@
         self,
         wrapped: Callable[..., Any] = ...,
         /,
         *,
         cls: type[Injectable] = ...,
         inject: bool = ...,
         on: type | Iterable[type] | UnionType = ...,
-        override: bool = ...,
+        mode: Literal["fallback", "normal", "override"] = ...,
     ):
         """
         Decorator applicable to a class or function. It is used to indicate how the
         injectable will be constructed. At injection time, a new instance will be
         injected each time.
         """
 
     def singleton(
         self,
         wrapped: Callable[..., Any] = ...,
         /,
         *,
         inject: bool = ...,
         on: type | Iterable[type] | UnionType = ...,
-        override: bool = ...,
+        mode: Literal["fallback", "normal", "override"] = ...,
     ):
         """
         Decorator applicable to a class or function. It is used to indicate how the
         singleton will be constructed. At injection time, the injected instance will
         always be the same.
         """
 
@@ -85,83 +85,80 @@
         """
 
     def set_constant(
         self,
         instance: _T,
         on: type | Iterable[type] | UnionType = ...,
         *,
-        override: bool = ...,
+        mode: Literal["fallback", "normal", "override"] = ...,
     ) -> _T:
         """
         Function for registering a specific instance to be injected. This is useful for
         registering global variables. The difference with the singleton decorator is
         that no dependencies are resolved, so the module doesn't need to be locked.
         """
 
-    def get_instance(self, cls: type[_T], none: bool = ...) -> _T | None:
+    def get_instance(self, cls: type[_T], *, none: bool = ...) -> _T | None:
         """
         Function used to retrieve an instance associated with the type passed in
         parameter or return `None` but if `none` parameter is `False` an exception
         will be raised.
         """
 
     def get_lazy_instance(
         self,
         cls: type[_T],
+        *,
         cache: bool = ...,
     ) -> Invertible[_T | None]:
         """
         Function used to retrieve an instance associated with the type passed in
         parameter or `None`. Return a `Invertible` object. To access the instance
         contained in an invertible object, simply use a wavy line (~).
         With `cache=True`, the instance retrieved will always be the same.
 
         Example: instance = ~lazy_instance
         """
 
-    def use(self, module: Module, priority: ModulePriority = ...):
+    def use(self, module: Module, *, priority: Literal["low", "high"] = ...):
         """
         Function for using another module. Using another module replaces the module's
         dependencies with those of the module used. If the dependency is not found, it
         will be searched for in the module's dependency container.
         """
 
     def stop_using(self, module: Module):
         """
         Function to remove a module in use.
         """
 
     def use_temporarily(
         self,
         module: Module,
-        priority: ModulePriority = ...,
+        *,
+        priority: Literal["low", "high"] = ...,
     ) -> ContextManager | ContextDecorator:
         """
         Context manager or decorator for temporary use of a module.
         """
 
-    def change_priority(self, module: Module, priority: ModulePriority):
+    def change_priority(self, module: Module, priority: Literal["low", "high"]):
         """
         Function for changing the priority of a module in use.
         There are two priority values:
 
         * **LOW**: The module concerned becomes the least important of the modules used.
         * **HIGH**: The module concerned becomes the most important of the modules used.
         """
 
     def unlock(self):
         """
         Function to unlock the module by deleting cached instances of singletons.
         """
 
-@final
-class ModulePriority(Enum):
-    HIGH = ...
-    LOW = ...
-
 @runtime_checkable
 class Injectable(Protocol[_T]):
     def __init__(self, factory: Callable[[], _T] = ..., /): ...
     @property
     def is_locked(self) -> bool: ...
     def unlock(self): ...
     @abstractmethod
```

### Comparing `python_injection-0.8.1.post0/injection/common/event.py` & `python_injection-0.8.2/injection/common/event.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1.post0/injection/common/invertible.py` & `python_injection-0.8.2/injection/common/invertible.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1.post0/injection/common/lazy.py` & `python_injection-0.8.2/injection/common/lazy.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1.post0/injection/common/queue.py` & `python_injection-0.8.2/injection/common/queue.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1.post0/injection/common/tools/type.py` & `python_injection-0.8.2/injection/common/tools/type.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1.post0/injection/core/module.py` & `python_injection-0.8.2/injection/core/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 from collections.abc import (
     Callable,
     Collection,
     Iterable,
     Iterator,
     Mapping,
     MutableMapping,
-    Set,
 )
 from contextlib import ContextDecorator, contextmanager, suppress
 from dataclasses import dataclass, field
-from enum import Enum, auto
 from functools import partialmethod, singledispatchmethod, update_wrapper
 from inspect import Signature, isclass
 from types import MethodType, UnionType
 from typing import (
     Any,
     ClassVar,
     ContextManager,
+    Literal,
     NamedTuple,
     NoReturn,
     Protocol,
     TypeVar,
     cast,
+    get_args,
     runtime_checkable,
 )
 
 from injection.common.event import Event, EventChannel, EventListener
 from injection.common.invertible import Invertible, SimpleInvertible
 from injection.common.lazy import Lazy, LazyMapping
 from injection.common.queue import LimitedQueue
@@ -41,20 +41,29 @@
     InjectionError,
     ModuleError,
     ModuleLockError,
     ModuleNotUsedError,
     NoInjectable,
 )
 
-__all__ = ("Injectable", "Module", "ModulePriority")
+__all__ = ("Injectable", "Module")
 
 _logger = logging.getLogger(__name__)
 
 _T = TypeVar("_T")
-Types = Iterable[type] | UnionType
+_Types = Iterable[type] | UnionType
+
+
+"""
+Literal types
+"""
+
+
+_Mode = Literal["fallback", "normal", "override"]
+_Priority = Literal["low", "high"]
 
 
 """
 Events
 """
 
 
@@ -62,15 +71,15 @@
 class ContainerEvent(Event, ABC):
     on_container: Container
 
 
 @dataclass(frozen=True, slots=True)
 class ContainerDependenciesUpdated(ContainerEvent):
     classes: Collection[type]
-    override: bool
+    mode: _Mode
 
     def __str__(self) -> str:
         length = len(self.classes)
         formatted_classes = ", ".join(f"`{format_type(cls)}`" for cls in self.classes)
         return (
             f"{length} container dependenc{'ies' if length > 1 else 'y'} have been "
             f"updated{f': {formatted_classes}' if formatted_classes else ''}."
@@ -116,19 +125,19 @@
     def __str__(self) -> str:
         return f"`{self.on_module}` no longer uses `{self.module_removed}`."
 
 
 @dataclass(frozen=True, slots=True)
 class ModulePriorityUpdated(ModuleEvent):
     module_updated: Module
-    priority: ModulePriority
+    priority: _Priority
 
     def __str__(self) -> str:
         return (
-            f"In `{self.on_module}`, the priority `{self.priority.name}` "
+            f"In `{self.on_module}`, the priority `{self.priority}` "
             f"has been applied to `{self.module_updated}`."
         )
 
 
 """
 Injectables
 """
@@ -149,21 +158,14 @@
         pass
 
     @abstractmethod
     def get_instance(self) -> _T:
         raise NotImplementedError
 
 
-class FallbackInjectable(Injectable[_T], ABC):
-    __slots__ = ()
-
-    def __bool__(self) -> bool:
-        return False
-
-
 @dataclass(repr=False, frozen=True, slots=True)
 class BaseInjectable(Injectable[_T], ABC):
     factory: Callable[[], _T]
 
 
 class NewInjectable(BaseInjectable[_T]):
     __slots__ = ()
@@ -196,15 +198,15 @@
             instance = self.factory()
             self.cache[self.__INSTANCE_KEY] = instance
 
         return instance
 
 
 @dataclass(repr=False, frozen=True, slots=True)
-class ShouldBeInjectable(FallbackInjectable[_T]):
+class ShouldBeInjectable(Injectable[_T]):
     cls: type[_T]
 
     def get_instance(self) -> NoReturn:
         raise InjectionError(f"`{format_type(self.cls)}` should be an injectable.")
 
 
 """
@@ -235,57 +237,58 @@
 
 
 """
 Container
 """
 
 
+class Record(NamedTuple):
+    injectable: Injectable
+    mode: _Mode
+
+
 @dataclass(repr=False, frozen=True, slots=True)
 class Container(Broker):
-    __data: dict[type, Injectable] = field(default_factory=dict, init=False)
+    __data: dict[type, Record] = field(default_factory=dict, init=False)
     __channel: EventChannel = field(default_factory=EventChannel, init=False)
 
     def __getitem__(self, cls: type[_T] | UnionType, /) -> Injectable[_T]:
-        for origin in get_origins(cls):
-            with suppress(KeyError):
-                return self.__data[origin]
+        for cls in get_origins(cls):
+            try:
+                injectable, _ = self.__data[cls]
+            except KeyError:
+                continue
+
+            return injectable
 
         raise NoInjectable(cls)
 
     def __contains__(self, cls: type | UnionType, /) -> bool:
-        return any(origin in self.__data for origin in get_origins(cls))
+        return any(cls in self.__data for cls in get_origins(cls))
 
     @property
     def is_locked(self) -> bool:
         return any(injectable.is_locked for injectable in self.__injectables)
 
     @property
-    def __classes(self) -> frozenset[type]:
-        return frozenset(self.__data)
-
-    @property
     def __injectables(self) -> frozenset[Injectable]:
-        return frozenset(self.__data.values())
+        return frozenset(injectable for injectable, _ in self.__data.values())
 
     @synchronized()
-    def update(self, classes: Iterable[type], injectable: Injectable, override: bool):
-        classes = frozenset(get_origins(*classes))
-
-        if not injectable:
-            classes -= self.__classes
-            override = True
+    def update(self, classes: Iterable[type], injectable: Injectable, mode: _Mode):
+        records = {
+            cls: Record(injectable, mode)
+            for cls in self.__filter_classes(classes, mode)
+        }
 
-        if classes:
-            event = ContainerDependenciesUpdated(self, classes, override)
+        if records:
+            event = ContainerDependenciesUpdated(self, records.keys(), mode)
 
             with self.notify(event):
-                if not override:
-                    self.__check_if_exists(classes)
-
-                self.__data.update((cls, injectable) for cls in classes)
+                self.__data.update(records)
 
         return self
 
     @synchronized()
     def unlock(self):
         for injectable in self.__injectables:
             injectable.unlock()
@@ -295,36 +298,40 @@
     def add_listener(self, listener: EventListener):
         self.__channel.add_listener(listener)
         return self
 
     def notify(self, event: Event) -> ContextManager | ContextDecorator:
         return self.__channel.dispatch(event)
 
-    def __check_if_exists(self, classes: Set[type]):
-        intersection = classes & self.__classes
+    def __filter_classes(self, classes: Iterable[type], mode: _Mode) -> Iterator[type]:
+        modes = get_args(_Mode)
+        rank = modes.index(mode)
 
-        for cls in intersection:
-            if self.__data[cls]:
-                raise RuntimeError(
-                    f"An injectable already exists for the class `{format_type(cls)}`."
-                )
+        for cls in frozenset(get_origins(*classes)):
+            try:
+                _, current_mode = self.__data[cls]
 
+            except KeyError:
+                pass
 
-"""
-Module
-"""
+            else:
+                if mode == current_mode:
+                    raise RuntimeError(
+                        f"An injectable already exists for the class `{format_type(cls)}`."
+                    )
 
+                elif rank < modes.index(current_mode):
+                    continue
 
-class ModulePriority(Enum):
-    HIGH = auto()
-    LOW = auto()
+            yield cls
 
-    @classmethod
-    def get_default(cls):
-        return cls.LOW
+
+"""
+Module
+"""
 
 
 @dataclass(repr=False, eq=False, frozen=True, slots=True)
 class Module(EventListener, Broker):
     name: str = field(default=None)
     __channel: EventChannel = field(default_factory=EventChannel, init=False)
     __container: Container = field(default_factory=Container, init=False)
@@ -364,48 +371,52 @@
     def injectable(
         self,
         wrapped: Callable[..., Any] = None,
         /,
         *,
         cls: type[Injectable] = NewInjectable,
         inject: bool = True,
-        on: type | Types = None,
-        override: bool = False,
+        on: type | _Types = None,
+        mode: _Mode = "normal",
     ):
         def decorator(wp):
             factory = self.inject(wp, return_factory=True) if inject else wp
             injectable = cls(factory)
             classes = find_types(wp, on)
-            self.update(classes, injectable, override)
+            self.update(classes, injectable, mode)
             return wp
 
         return decorator(wrapped) if wrapped else decorator
 
     singleton = partialmethod(injectable, cls=SingletonInjectable)
 
     def should_be_injectable(self, wrapped: type = None, /):
         def decorator(wp):
-            self[wp] = ShouldBeInjectable(wp)
+            self.update(
+                (wp,),
+                ShouldBeInjectable(wp),
+                mode="fallback",
+            )
             return wp
 
         return decorator(wrapped) if wrapped else decorator
 
     def set_constant(
         self,
         instance: _T,
-        on: type | Types = None,
+        on: type | _Types = None,
         *,
-        override: bool = False,
+        mode: _Mode = "normal",
     ) -> _T:
         cls = type(instance)
         self.injectable(
             lambda: instance,
             inject=False,
             on=(cls, on),
-            override=override,
+            mode=mode,
         )
         return instance
 
     def inject(
         self,
         wrapped: Callable[..., Any] = None,
         /,
@@ -424,52 +435,49 @@
                 function.update(self)
                 self.add_listener(function)
 
             return function
 
         return decorator(wrapped) if wrapped else decorator
 
-    def get_instance(self, cls: type[_T], none: bool = True) -> _T | None:
+    def get_instance(self, cls: type[_T], *, none: bool = True) -> _T | None:
         try:
             injectable = self[cls]
         except KeyError as exc:
             if none:
                 return None
 
             raise exc
 
         instance = injectable.get_instance()
         return cast(cls, instance)
 
     def get_lazy_instance(
         self,
         cls: type[_T],
+        *,
         cache: bool = False,
     ) -> Invertible[_T | None]:
         if cache:
             return Lazy(lambda: self.get_instance(cls))
 
         function = self.inject(lambda instance=None: instance)
         function.set_owner(cls)
         return SimpleInvertible(function)
 
     def update(
         self,
         classes: Iterable[type],
         injectable: Injectable,
-        override: bool = False,
+        mode: _Mode = "normal",
     ):
-        self.__container.update(classes, injectable, override)
+        self.__container.update(classes, injectable, mode)
         return self
 
-    def use(
-        self,
-        module: Module,
-        priority: ModulePriority = ModulePriority.get_default(),
-    ):
+    def use(self, module: Module, *, priority: _Priority = "low"):
         if module is self:
             raise ModuleError("Module can't be used by itself.")
 
         if module in self.__modules:
             raise ModuleError(f"`{self}` already uses `{module}`.")
 
         event = ModuleAdded(self, module)
@@ -491,21 +499,22 @@
 
         return self
 
     @contextmanager
     def use_temporarily(
         self,
         module: Module,
-        priority: ModulePriority = ModulePriority.get_default(),
+        *,
+        priority: _Priority = "low",
     ) -> ContextManager | ContextDecorator:
-        self.use(module, priority)
+        self.use(module, priority=priority)
         yield
         self.stop_using(module)
 
-    def change_priority(self, module: Module, priority: ModulePriority):
+    def change_priority(self, module: Module, priority: _Priority):
         event = ModulePriorityUpdated(self, module, priority)
 
         with self.notify(event):
             self.__move_module(module, priority)
 
         return self
 
@@ -536,16 +545,16 @@
             yield
             _logger.debug(event)
 
     def __check_locking(self):
         if self.is_locked:
             raise ModuleLockError(f"`{self}` is locked.")
 
-    def __move_module(self, module: Module, priority: ModulePriority):
-        last = priority == ModulePriority.LOW
+    def __move_module(self, module: Module, priority: _Priority):
+        last = priority != "high"
 
         try:
             self.__modules.move_to_end(module, last=last)
         except KeyError as exc:
             raise ModuleNotUsedError(
                 f"`{module}` can't be found in the modules used by `{self}`."
             ) from exc
@@ -633,15 +642,23 @@
         "__wrapped__",
         "__dependencies",
         "__owner",
         "__setup_queue",
     )
 
     def __init__(self, wrapped: Callable[..., Any], /):
-        update_wrapper(self, wrapped)
+        try:
+            variables = vars(wrapped)
+        except TypeError:
+            pass
+        else:
+            self.__update_vars(variables)
+            del variables
+
+        update_wrapper(self, wrapped, updated=())
         self.__dependencies = Dependencies.empty()
         self.__owner = None
         self.__setup_queue = LimitedQueue[Callable[[], Any]]()
         self.on_setup(self.__set_signature)
 
     def __repr__(self) -> str:
         return repr(self.wrapped)
@@ -723,7 +740,19 @@
     def _(self, event: ModuleEvent, /) -> ContextManager:
         yield
         self.update(event.on_module)
 
     def __set_signature(self):
         self.__signature__ = inspect.signature(self.wrapped, eval_str=True)
         return self
+
+    def __update_vars(self, variables: Mapping[str, Any], /):
+        def is_dunder(var: str) -> bool:
+            return var.startswith("__") and var.endswith("__")
+
+        restricted_vars = frozenset(var for var in dir(self) if not is_dunder(var))
+        variables = (
+            (var, value)
+            for var, value in variables.items()
+            if var not in restricted_vars
+        )
+        vars(self).update(variables)
```

### Comparing `python_injection-0.8.1.post0/injection/exceptions.py` & `python_injection-0.8.2/injection/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1.post0/injection/integrations/blacksheep.py` & `python_injection-0.8.2/injection/integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1.post0/injection/utils.py` & `python_injection-0.8.2/injection/utils.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.8.1.post0/pyproject.toml` & `python_injection-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-injection"
-version = "0.8.1.post0"
+version = "0.8.2"
 description = "Fast and easy dependency injection framework."
 authors = ["remimd"]
 keywords = ["dependencies", "inject", "injection"]
 license = "MIT"
 packages = [{ include = "injection" }]
 readme = "documentation/basic-usage.md"
 repository = "https://github.com/100nm/python-injection"
```

### Comparing `python_injection-0.8.1.post0/PKG-INFO` & `python_injection-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-injection
-Version: 0.8.1.post0
+Version: 0.8.2
 Summary: Fast and easy dependency injection framework.
 Home-page: https://github.com/100nm/python-injection
 License: MIT
 Keywords: dependencies,inject,injection
 Author: remimd
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
@@ -132,24 +132,24 @@
     ...
 
 @injectable(on=(AbstractService, ConcreteService))
 class ConcreteServiceOverload(ConcreteService):
     ...
 ```
 
-If a class is registered in a package and you want to override it, there is the `override` parameter:
+If a class is registered in a package and you want to override it, there is the `mode` parameter:
 
 ```python
 @injectable
 class InaccessibleService:
     ...
 
 # ...
 
-@injectable(on=InaccessibleService, override=True)
+@injectable(on=InaccessibleService, mode="override")
 class ServiceOverload(InaccessibleService):
     ...
 ```
 
 ## Recipes
 
 A recipe is a function that tells the injector how to construct the instance to be injected. It is important to specify
```

