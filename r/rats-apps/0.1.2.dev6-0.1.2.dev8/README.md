# Comparing `tmp/rats_apps-0.1.2.dev6-py3-none-any.whl.zip` & `tmp/rats_apps-0.1.2.dev8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6677 bytes, number of entries: 13
+Zip file size: 6696 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      857 b- defN 80-Jan-01 00:00 rats/apps/__init__.py
--rw-r--r--  2.0 unx     5110 b- defN 80-Jan-01 00:00 rats/apps/_annotations.py
--rw-r--r--  2.0 unx      539 b- defN 80-Jan-01 00:00 rats/apps/_composite_container.py
--rw-r--r--  2.0 unx     3089 b- defN 80-Jan-01 00:00 rats/apps/_container.py
+-rw-r--r--  2.0 unx     5124 b- defN 80-Jan-01 00:00 rats/apps/_annotations.py
+-rw-r--r--  2.0 unx      553 b- defN 80-Jan-01 00:00 rats/apps/_composite_container.py
+-rw-r--r--  2.0 unx     3131 b- defN 80-Jan-01 00:00 rats/apps/_container.py
 -rw-r--r--  2.0 unx      457 b- defN 80-Jan-01 00:00 rats/apps/_ids.py
 -rw-r--r--  2.0 unx      188 b- defN 80-Jan-01 00:00 rats/apps/_namespaces.py
--rw-r--r--  2.0 unx      839 b- defN 80-Jan-01 00:00 rats/apps/_plugin_container.py
+-rw-r--r--  2.0 unx      853 b- defN 80-Jan-01 00:00 rats/apps/_plugin_container.py
 -rw-r--r--  2.0 unx     1304 b- defN 80-Jan-01 00:00 rats/apps/_scoping.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 rats/apps/py.typed
--rw-r--r--  2.0 unx      716 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev6.dist-info/WHEEL
--rw-r--r--  2.0 unx       86 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev6.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1045 b- defN 16-Jan-01 00:00 rats_apps-0.1.2.dev6.dist-info/RECORD
-13 files, 14318 bytes uncompressed, 4925 bytes compressed:  65.6%
+-rw-r--r--  2.0 unx      716 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       86 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev8.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1045 b- defN 16-Jan-01 00:00 rats_apps-0.1.2.dev8.dist-info/RECORD
+13 files, 14402 bytes uncompressed, 4944 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: rats/apps/_scoping.py
 Comment: 
 
 Filename: rats/apps/py.typed
 Comment: 
 
-Filename: rats_apps-0.1.2.dev6.dist-info/METADATA
+Filename: rats_apps-0.1.2.dev8.dist-info/METADATA
 Comment: 
 
-Filename: rats_apps-0.1.2.dev6.dist-info/WHEEL
+Filename: rats_apps-0.1.2.dev8.dist-info/WHEEL
 Comment: 
 
-Filename: rats_apps-0.1.2.dev6.dist-info/entry_points.txt
+Filename: rats_apps-0.1.2.dev8.dist-info/entry_points.txt
 Comment: 
 
-Filename: rats_apps-0.1.2.dev6.dist-info/RECORD
+Filename: rats_apps-0.1.2.dev8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rats/apps/_annotations.py

```diff
@@ -62,29 +62,29 @@
                 for namespace, services in self._service_ids.items()
             ]
         )
 
 
 class AnnotatedContainer(Container):
 
-    def get_namespace(
+    def get_namespaced_group(
         self,
         namespace: str,
         group_id: ServiceId[T_ServiceType],
     ) -> Iterator[T_ServiceType]:
         annotations = _extract_class_annotations(type(self))
         containers = annotations.with_namespace(ProviderNamespaces.CONTAINERS)
         groups = annotations.group_in_namespace(namespace, group_id)
 
         for annotation in groups:
             yield getattr(self, annotation.name)()
 
         for container in containers:
             c = getattr(self, container.name)()
-            yield from c.get_namespace(namespace, group_id)
+            yield from c.get_namespaced_group(namespace, group_id)
 
 
 def service(
     service_id: ServiceId[T_ServiceType],
 ) -> Callable[..., Callable[..., T_ServiceType]]:
     return fn_annotation_decorator(ProviderNamespaces.SERVICES, service_id)
```

## rats/apps/_composite_container.py

```diff
@@ -6,14 +6,14 @@
 
 class CompositeContainer(Container):
     _contailers: tuple[Container, ...]
 
     def __init__(self, *containers: Container) -> None:
         self._containers = containers
 
-    def get_namespace(
+    def get_namespaced_group(
         self,
         namespace: str,
         group_id: ServiceId[T_ServiceType],
     ) -> Iterator[T_ServiceType]:
         for container in self._containers:
-            yield from container.get_namespace(namespace, group_id)
+            yield from container.get_namespaced_group(namespace, group_id)
```

## rats/apps/_container.py

```diff
@@ -33,24 +33,24 @@
         try:
             return next(self.get_group(group_id)) is not None
         except StopIteration:
             return False
 
     def has_namespace(self, namespace: str, group_id: ServiceId[T_ServiceType]) -> bool:
         try:
-            return next(self.get_namespace(namespace, group_id)) is not None
+            return next(self.get_namespaced_group(namespace, group_id)) is not None
         except StopIteration:
             return False
 
     def get(self, service_id: ServiceId[T_ServiceType]) -> T_ServiceType:
         """Retrieve a service instance by its id."""
-        services = list(self.get_namespace(ProviderNamespaces.SERVICES, service_id))
+        services = list(self.get_namespaced_group(ProviderNamespaces.SERVICES, service_id))
         if len(services) == 0:
             services.extend(
-                list(self.get_namespace(ProviderNamespaces.FALLBACK_SERVICES, service_id)),
+                list(self.get_namespaced_group(ProviderNamespaces.FALLBACK_SERVICES, service_id)),
             )
 
         if len(services) > 1:
             raise DuplicateServiceError(service_id)
         elif len(services) == 0:
             raise ServiceNotFoundError(service_id)
         else:
@@ -58,20 +58,20 @@
 
     def get_group(
         self,
         group_id: ServiceId[T_ServiceType],
     ) -> Iterator[T_ServiceType]:
         """Retrieve a service group by its id."""
         if not self.has_namespace(ProviderNamespaces.GROUPS, group_id):
-            yield from self.get_namespace(ProviderNamespaces.FALLBACK_GROUPS, group_id)
+            yield from self.get_namespaced_group(ProviderNamespaces.FALLBACK_GROUPS, group_id)
 
-        yield from self.get_namespace(ProviderNamespaces.GROUPS, group_id)
+        yield from self.get_namespaced_group(ProviderNamespaces.GROUPS, group_id)
 
     @abstractmethod
-    def get_namespace(
+    def get_namespaced_group(
         self,
         namespace: str,
         group_id: ServiceId[T_ServiceType],
     ) -> Iterator[T_ServiceType]:
         """Retrieve a service group by its id, within a given service namespace."""
```

## rats/apps/_plugin_container.py

```diff
@@ -10,19 +10,19 @@
     _app: Container
     _group: str
 
     def __init__(self, app: Container, group: str) -> None:
         self._app = app
         self._group = group
 
-    def get_namespace(
+    def get_namespaced_group(
         self,
         namespace: str,
         group_id: ServiceId[T_ServiceType],
     ) -> Iterator[T_ServiceType]:
         for container in self._load_containers():
-            yield from container.get_namespace(namespace, group_id)
+            yield from container.get_namespaced_group(namespace, group_id)
 
     @cache  # noqa: B019
     def _load_containers(self) -> Iterable[Container]:
         entries = entry_points(group=self._group)
         return tuple(entry.load()(self._app) for entry in entries)
```

## Comparing `rats_apps-0.1.2.dev6.dist-info/METADATA` & `rats_apps-0.1.2.dev8.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rats-apps
-Version: 0.1.2.dev6
+Version: 0.1.2.dev8
 Summary: research analysis tools for building applications
 Home-page: https://github.com/microsoft/rats/
 License: MIT
 Keywords: pipelines,machine learning,research
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `rats_apps-0.1.2.dev6.dist-info/RECORD` & `rats_apps-0.1.2.dev8.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 rats/apps/__init__.py,sha256=EHza57K66uM7w8pFBJBqMWaJ7Xn_7E4hn0xA7k8Ag5U,857
-rats/apps/_annotations.py,sha256=QXx78Qbiikn_4uV09J9N0c2aNK6bj-RtUcbgCy3Q718,5110
-rats/apps/_composite_container.py,sha256=-o942CbRgczz2GXDN1gABF8vLTKDOXGddOpob1tZaNw,539
-rats/apps/_container.py,sha256=dm1wRAuPWM0hV2BtNyBmfZ-cybId55w7oua4rvKuiis,3089
+rats/apps/_annotations.py,sha256=V6sNsvh66VGB6ciog0AwPgXwTjBrtlIZXT-ZZx_LpdY,5124
+rats/apps/_composite_container.py,sha256=wSWVQWPin2xxIlEoSgk_D1rlc3N2gpTxQ2y9UFdqXy0,553
+rats/apps/_container.py,sha256=JSmO4x0JcnM9gQP0ki9JcGzYqbjmgAj79lZw5YfBrqI,3131
 rats/apps/_ids.py,sha256=dxWCPMpMA_vpaTDJEKNByIBJaX97Db203XqWLhaOezo,457
 rats/apps/_namespaces.py,sha256=THUV_Xj5PtweC23Ob-zsSpk8exC4fT-qRwjpQ6IDm0U,188
-rats/apps/_plugin_container.py,sha256=jKD1ft5Ph-DJU7fw2NKC7_FKwSqhWTvZoJTd7lHt6_s,839
+rats/apps/_plugin_container.py,sha256=W_xQD2btc0N2dEb3c5tXM-ZZ4A4diMpkCjbOZdlXYuI,853
 rats/apps/_scoping.py,sha256=-5hl0RoOdQGkxWLIn42hthMUyX8_84sV8H3u40y-gIU,1304
 rats/apps/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rats_apps-0.1.2.dev6.dist-info/METADATA,sha256=N7hlG8xu1DhseCv2Krrt2-g5-5QoQw_8T4XDEY03OzA,716
-rats_apps-0.1.2.dev6.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-rats_apps-0.1.2.dev6.dist-info/entry_points.txt,sha256=Vu1IgAPQvL4xMJzW_OG2JSPFac7HalCHyXiRr0-OfCI,86
-rats_apps-0.1.2.dev6.dist-info/RECORD,,
+rats_apps-0.1.2.dev8.dist-info/METADATA,sha256=498TKmvfbSS_0mgTQ_vDntHzvo1uL1g7jcJIVQGwflA,716
+rats_apps-0.1.2.dev8.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+rats_apps-0.1.2.dev8.dist-info/entry_points.txt,sha256=Vu1IgAPQvL4xMJzW_OG2JSPFac7HalCHyXiRr0-OfCI,86
+rats_apps-0.1.2.dev8.dist-info/RECORD,,
```

