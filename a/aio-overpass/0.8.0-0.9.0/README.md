# Comparing `tmp/aio_overpass-0.8.0.tar.gz` & `tmp/aio_overpass-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_overpass-0.8.0.tar", max compression
+gzip compressed data, was "aio_overpass-0.9.0.tar", max compression
```

## Comparing `aio_overpass-0.8.0.tar` & `aio_overpass-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6516 2023-10-07 14:55:16.575943 aio_overpass-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-10-07 14:55:16.575943 aio_overpass-0.8.0/LICENSE
--rw-r--r--   0        0        0     8414 2023-10-07 14:55:16.575943 aio_overpass-0.8.0/README.md
--rwxr-xr-x   0        0        0      579 2023-10-07 14:55:16.575943 aio_overpass-0.8.0/aio_overpass/__init__.py
--rw-r--r--   0        0        0      977 2023-10-07 14:55:16.575943 aio_overpass-0.8.0/aio_overpass/_dist.py
--rwxr-xr-x   0        0        0    13548 2023-10-07 14:55:16.575943 aio_overpass-0.8.0/aio_overpass/client.py
--rwxr-xr-x   0        0        0    28105 2023-10-07 14:55:16.575943 aio_overpass-0.8.0/aio_overpass/element.py
--rwxr-xr-x   0        0        0    14947 2023-10-07 14:55:16.575943 aio_overpass-0.8.0/aio_overpass/error.py
--rwxr-xr-x   0        0        0    25348 2023-10-07 14:55:16.575943 aio_overpass-0.8.0/aio_overpass/pt.py
--rwxr-xr-x   0        0        0    22853 2023-10-07 14:55:16.575943 aio_overpass-0.8.0/aio_overpass/pt_ordered.py
--rwxr-xr-x   0        0        0     1362 2023-10-07 14:55:16.575943 aio_overpass-0.8.0/aio_overpass/ql.py
--rwxr-xr-x   0        0        0    24314 2023-10-07 14:55:16.575943 aio_overpass-0.8.0/aio_overpass/query.py
--rwxr-xr-x   0        0        0     3730 2023-10-07 14:55:16.599943 aio_overpass-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    10165 1970-01-01 00:00:00.000000 aio_overpass-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     8377 2023-10-20 01:42:44.577586 aio_overpass-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-10-20 01:42:44.577586 aio_overpass-0.9.0/LICENSE
+-rw-r--r--   0        0        0     8429 2023-10-20 01:42:44.577586 aio_overpass-0.9.0/README.md
+-rwxr-xr-x   0        0        0      584 2023-10-20 01:42:44.577586 aio_overpass-0.9.0/aio_overpass/__init__.py
+-rw-r--r--   0        0        0      977 2023-10-20 01:42:44.577586 aio_overpass-0.9.0/aio_overpass/_dist.py
+-rwxr-xr-x   0        0        0    16082 2023-10-20 01:42:44.577586 aio_overpass-0.9.0/aio_overpass/client.py
+-rwxr-xr-x   0        0        0    32667 2023-10-20 01:42:44.577586 aio_overpass-0.9.0/aio_overpass/element.py
+-rwxr-xr-x   0        0        0    15171 2023-10-20 01:42:44.577586 aio_overpass-0.9.0/aio_overpass/error.py
+-rwxr-xr-x   0        0        0    25479 2023-10-20 01:42:44.577586 aio_overpass-0.9.0/aio_overpass/pt.py
+-rwxr-xr-x   0        0        0    24055 2023-10-20 01:42:44.581586 aio_overpass-0.9.0/aio_overpass/pt_ordered.py
+-rwxr-xr-x   0        0        0     1362 2023-10-20 01:42:44.581586 aio_overpass-0.9.0/aio_overpass/ql.py
+-rwxr-xr-x   0        0        0    25877 2023-10-20 01:42:44.581586 aio_overpass-0.9.0/aio_overpass/query.py
+-rwxr-xr-x   0        0        0     3973 2023-10-20 01:42:44.609587 aio_overpass-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 aio_overpass-0.9.0/PKG-INFO
```

### Comparing `aio_overpass-0.8.0/LICENSE` & `aio_overpass-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.8.0/README.md` & `aio_overpass-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 A client for the [Overpass API], a read-only API that serves up custom selected
-parts of [OpenStreetMap] data. It is optimized for data consumers that need a few
-elements within a glimpse or up to roughly 10 million elements in some minutes,
-both selected by search criteria like location, type of objects, tag properties,
-proximity, or combinations of them. To make use of it, you should familiarize yourself
-with [Overpass QL], the query language used to select the elements that you want.
+parts of [OpenStreetMap] data.
+
+The Overpass API is optimized for data consumers that need a few elements within
+a glimpse or up to roughly 10 million elements in some minutes, both selected by
+search criteria like location, type of objects, tag properties, proximity, or
+combinations of them. To make use of it, you should familiarize yourself with
+[Overpass QL], the query language used to select the elements that you want.
 
 #### Contents
 - [Features](#features)
 - [Getting Started](#getting-started)
   - [Choosing Extras](#choosing-extras)
 - [Basic Usage](#basic-usage)
   - [Example](#example)
```

### Comparing `aio_overpass-0.8.0/aio_overpass/__init__.py` & `aio_overpass-0.9.0/aio_overpass/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Async client for the Overpass API."""
 import importlib.metadata
 
 
-__version__ = importlib.metadata.version("aio-overpass")
+__version__: str = importlib.metadata.version("aio-overpass")
 
 # we add this to all modules for pdoc;
 # see https://pdoc.dev/docs/pdoc.html#use-numpydoc-or-google-docstrings
 __docformat__ = "google"
 
 # we also use __all__ in all modules for pdoc; this lets us control the order
 __all__ = (
```

### Comparing `aio_overpass-0.8.0/aio_overpass/_dist.py` & `aio_overpass-0.9.0/aio_overpass/_dist.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.8.0/aio_overpass/client.py` & `aio_overpass-0.9.0/aio_overpass/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Interface for making API calls."""
 
 import asyncio
 import logging
 import re
 from contextlib import suppress
 from dataclasses import dataclass
-from typing import Optional, Union
 from urllib.parse import urljoin
 
 from aio_overpass import __version__
 from aio_overpass.error import (
     CallError,
     CallTimeoutError,
     ClientError,
@@ -33,36 +32,46 @@
     "Status",
     "DEFAULT_INSTANCE",
     "DEFAULT_USER_AGENT",
 )
 
 
 DEFAULT_INSTANCE = "https://overpass-api.de/api/"
+"""Main Overpass API instance."""
+
 DEFAULT_USER_AGENT = f"aio-overpass/{__version__} (https://github.com/timwie/aio-overpass)"
+"""User agent that points to the ``aio-overpass`` repo."""
 
 
-@dataclass
+@dataclass(slots=True)
 class Status:
     """
     Information about the API server's rate limit.
 
     Attributes:
         slots: The maximum number of concurrent queries per IP
                (or ``None`` if there is no rate limit).
         free_slots: The number of slots open for this IP
                     (or ``None`` if there is no rate limit).
         cooldown_secs: The number of seconds until a slot opens for this IP
                        (or 0 if there is a free slot).
         concurrency: Maximum concurrent queries configured for this client.
+        endpoint: Announced endpoint. For example, there are two distinct servers
+                  that both can be reached by the main Overpass API instance.
+                  Depending on server load, a query may be sent to either of them.
+                  This value is the server name, f.e. ``"gall.openstreetmap.de/"``.
+        nb_running_queries: Number of currently running queries for this IP.
     """
 
-    slots: Optional[int]
-    free_slots: Optional[int]
+    slots: int | None
+    free_slots: int | None
     cooldown_secs: int
     concurrency: int
+    endpoint: str | None
+    nb_running_queries: int
 
     def __repr__(self) -> str:
         f, s, c = self.free_slots, self.slots, self.cooldown_secs
 
         if self.slots:
             return f"{type(self).__name__}(slots={f}/{s}, cooldown={c}s)"
 
@@ -91,46 +100,56 @@
         runner: You can provide another query runner if you want to implement your own retry
                 strategy.
 
     References:
         - https://wiki.openstreetmap.org/wiki/Overpass_API#Public_Overpass_API_instances
     """
 
+    __slots__ = (
+        "_concurrency",
+        "_maybe_any_status",
+        "_maybe_sem",
+        "_maybe_session",
+        "_runner",
+        "_url",
+        "_user_agent",
+    )
+
     def __init__(
         self,
         url: str = DEFAULT_INSTANCE,
         user_agent: str = DEFAULT_USER_AGENT,
         concurrency: int = 32,
-        runner: Optional[QueryRunner] = None,
+        runner: QueryRunner | None = None,
     ) -> None:
         if concurrency <= 0:
             msg = "'concurrency' must be > 0"
             raise ValueError(msg)
 
         self._url = url
         self._user_agent = user_agent
         self._concurrency = concurrency
         self._runner = runner or DefaultQueryRunner()
 
-        self._maybe_session: Optional[aiohttp.ClientSession] = None
-        self._maybe_any_status: Optional[Status] = None
-        self._maybe_sem: Optional[asyncio.BoundedSemaphore] = None
+        self._maybe_session: aiohttp.ClientSession | None = None
+        self._maybe_any_status: Status | None = None
+        self._maybe_sem: asyncio.BoundedSemaphore | None = None
 
     def _session(self) -> aiohttp.ClientSession:
         """The session used for all requests of this client."""
         if not self._maybe_session or self._maybe_session.closed:
             headers = {"User-Agent": self._user_agent}
             connector = aiohttp.TCPConnector(limit=0)  # we limit concurrency ourselves
             self._maybe_session = aiohttp.ClientSession(headers=headers, connector=connector)
 
         return self._maybe_session
 
     async def _rate_limiter(
         self,
-        timeout: Union[ClientTimeout, object] = sentinel,
+        timeout: ClientTimeout | object = sentinel,
     ) -> asyncio.BoundedSemaphore:
         """
         A rate-limiting semaphore for queries.
 
         This semaphore can be acquired as many times as there are query slots at the API instance.
         If all slots are acquired, further queries need to wait until a slot is released.
         """
@@ -154,36 +173,47 @@
 
             # is raised when there are still active queries. that's ok
             with suppress(aiohttp.ServerDisconnectedError):
                 await self._maybe_session.close()
 
     async def _status(
         self,
-        timeout: Union[ClientTimeout, object] = sentinel,
+        timeout: ClientTimeout | object = sentinel,
     ) -> "Status":
         try:
             async with self._session().get(
                 url=urljoin(self._url, "status"), timeout=timeout
             ) as response:
                 text = await response.text()
         except aiohttp.ClientError as err:
             raise _to_client_error(err) from err
 
-        slots = 0
+        slots: int | None = 0
         free_slots = None
         cooldown_secs = 0
         concurrency = self._concurrency
+        endpoint = None
+        nb_running_queries = 0
 
         try:
-            match_slots_overall = re.findall("Rate limit: (\\d+)", text)
-            match_slots_available = re.findall("(\\d+) slots available now", text)
-            match_cooldowns = re.findall("Slot available after: .+, in (\\d+) seconds", text)
+            match_slots_overall = re.findall(r"Rate limit: (\d+)", text)
+            match_slots_available = re.findall(r"(\d+) slots available now", text)
+            match_cooldowns = re.findall(r"Slot available after: .+, in (\d+) seconds", text)
+            match_endpoint = re.findall(r"Announced endpoint: (.+)", text)
+            match_running_queries = re.findall(
+                r"\d+\t\d+\t\d+\t\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}Z", text
+            )
+
+            (slots_str,) = match_slots_overall
+            slots = int(slots_str) or None
+
+            endpoint = match_endpoint[0] if match_endpoint else None
+            endpoint = None if endpoint == "none" else endpoint
 
-            (slots,) = match_slots_overall
-            slots = int(slots) or None
+            nb_running_queries = len(match_running_queries)
 
             if slots:
                 cooldowns = [int(secs) for secs in match_cooldowns]
 
                 if match_slots_available:
                     free_slots = int(match_slots_available[0])
                 else:
@@ -198,14 +228,16 @@
             raise _to_client_error(response) from err
 
         self._maybe_any_status = Status(
             slots=slots,
             free_slots=free_slots,
             cooldown_secs=cooldown_secs,
             concurrency=concurrency,
+            endpoint=endpoint,
+            nb_running_queries=nb_running_queries,
         )
         return self._maybe_any_status
 
     async def status(self) -> Status:
         """
         Check the current API status.
 
@@ -232,52 +264,61 @@
             async with session.get(endpoint) as response:
                 body = await response.text()
                 killed_pids = re.findall("\\(pid (\\d+)\\)", body)
                 return len(set(killed_pids))
         except aiohttp.ClientError as err:
             raise _to_client_error(err) from err
 
-    async def run_query(self, query: Query) -> None:
+    async def run_query(self, query: Query, raise_on_failure: bool = True) -> None:
         """
         Send a query to the API, and await its completion.
 
         "Running" the query entails acquiring a connection from the pool, waiting for a slot
         to open up, the query requests themselves (which may be retried), status requests
         when the server is busy, and cooldown periods.
 
-        The query runner is invoked before every try.
+        The query runner is invoked before every try, and once after the last try.
 
         To run multiple queries concurrently, wrap the returned coroutines in an ``asyncio`` task,
         f.e. with ``asyncio.create_task()`` and subsequent ``asyncio.gather()``.
 
         Args:
             query: the query to run on this API instance
+            raise_on_failure: if ``True``, raises ``query.error`` if the query failed
 
         Raises:
             ClientError: when query or status requests fail. If the query was retried, the error
                          of the last try will be raised. The same exception is also captured in
-                         ``query.error``.
+                         ``query.error``. Raising can be prevented by setting ``raise_on_failure``
+                         to ``False``.
+            RunnerError: when a call to the query runner raises. This exception is raised
+                         even if ``raise_on_failure` is ``False``, since it is likely an error
+                         that is not just specific to this query.
         """
         if query.done:
             return  # nothing to do
 
         if query.nb_tries > 0:
             query.reset()  # reset failed queries
 
         while True:
-            await self._invoke_runner(query)
+            await self._invoke_runner(query, raise_on_failure=raise_on_failure)
             if query.done:
                 return
             await self._run_query_once(query)
 
-    async def _invoke_runner(self, query: Query) -> None:
+    async def _invoke_runner(self, query: Query, raise_on_failure: bool) -> None:
         try:
             await self._runner(query)
-        except ClientError:
-            raise
+        except ClientError as err:
+            if err is not query.error:
+                msg = "query runner raised a ClientError other than 'query.error'"
+                raise ValueError(msg) from err
+            if raise_on_failure:
+                raise
         except BaseException as err:
             raise RunnerError(err) from err
 
     async def _run_query_once(self, query: Query) -> None:
         logger = query.logger or logging.getLogger(f"{type(self).__module__}.{type(self).__name__}")
 
         if query.done:
@@ -285,16 +326,21 @@
 
         query_mut = query._mutator()
 
         query_mut.begin_try()
 
         acquired_slot = False
 
+        if query.request_timeout.total_without_query_secs is not None:
+            total = float(query.timeout_secs) + query.request_timeout.total_without_query_secs
+        else:
+            total = None
+
         req_timeout = aiohttp.ClientTimeout(
-            total=float(query.timeout_secs) + query.request_timeout.total_without_query_secs,
+            total=total,
             connect=None,
             sock_connect=query.request_timeout.sock_connect_secs,
             sock_read=query.request_timeout.each_sock_read_secs,
         )
 
         try:
             await self._wait_for_slot(query)
@@ -314,31 +360,38 @@
                     response_bytes=response.content.total_bytes,
                 )
 
         except aiohttp.ClientError as err:
             query_mut.fail_try(_to_client_error(err))
 
         except asyncio.TimeoutError as err:
+            query_err: ClientError
+
             if query.run_timeout_elapsed:
+                assert query.run_duration_secs is not None
                 query_err = GiveupError(kwargs=query.kwargs, after_secs=query.run_duration_secs)
             else:
                 assert not query.run_timeout_secs or acquired_slot
+                assert req_timeout.total
                 query_err = CallTimeoutError(cause=err, after_secs=req_timeout.total)
+
             query_mut.fail_try(query_err)
 
         except ClientError as err:
             query_mut.fail_try(err)
 
         finally:
             query_mut.end_try()
             if acquired_slot:
+                assert self._maybe_sem is not None
                 self._maybe_sem.release()
 
     async def _wait_for_slot(self, query: Query) -> None:
         def next_timeout() -> aiohttp.ClientTimeout:
+            assert query.run_duration_secs is not None
             if query.run_timeout_secs:
                 remaining = query.run_timeout_secs - query.run_duration_secs
                 if remaining <= 0.0:
                     raise asyncio.TimeoutError()  # no point delaying the inevitable
             else:
                 remaining = None  # no limit
 
@@ -354,15 +407,20 @@
         if check_cooldown:
             # If this client is running too many queries, we can check the status for a
             # cooldown period. This request failing is a bit of an edge case.
             # 'query.error' will be overwritten, which means we will not check for a
             # cooldown in the next iteration.
             status = await self._status(timeout=next_timeout())
 
-            if (timeout := next_timeout()) and status.cooldown_secs > timeout.total:
+            if (
+                (timeout := next_timeout())
+                and timeout.total is not None
+                and status.cooldown_secs > timeout.total
+            ):
+                assert query.run_duration_secs
                 raise GiveupError(kwargs=query.kwargs, after_secs=query.run_duration_secs)
 
             logger.info(f"{query} has cooldown for {status.cooldown_secs:.1f}s")
             await asyncio.sleep(status.cooldown_secs)
 
         # This requests an API status if we haven't done so already.
         rate_limiter = await self._rate_limiter(timeout=next_timeout())
```

### Comparing `aio_overpass-0.8.0/aio_overpass/element.py` & `aio_overpass-0.9.0/aio_overpass/element.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 """Typed result set members."""
 import math
 import re
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from collections.abc import Iterable, Iterator
 from dataclasses import dataclass
-from typing import Any, Optional, Union, cast
+from typing import Any, Generic, TypeAlias, TypeVar, cast
 
 from aio_overpass import Query
 
 import shapely.geometry
 import shapely.ops
 from shapely.geometry import LinearRing, LineString, MultiPolygon, Point, Polygon
 from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 
 
 __docformat__ = "google"
 __all__ = (
-    "GeoJsonDict",
-    "OverpassDict",
-    "Bbox",
+    "collect_elements",
     "Spatial",
     "Element",
     "Node",
     "Way",
     "Relation",
     "Relationship",
+    "GeometryDetails",
     "Metadata",
-    "collect_elements",
+    "Bbox",
+    "GeoJsonDict",
+    "OverpassDict",
 )
 
-GeoJsonDict = dict[str, Any]
+GeoJsonDict: TypeAlias = dict[str, Any]
 """
 A dictionary representing a GeoJSON object.
 """
 
-OverpassDict = dict[str, Any]
+OverpassDict: TypeAlias = dict[str, Any]
 """
 A dictionary representing a JSON object returned by the Overpass API.
 """
 
-Bbox = tuple[float, float, float, float]
+Bbox: TypeAlias = tuple[float, float, float, float]
 """
 The bounding box of a spatial object.
 
 This tuple can be understood as any of
     - ``(s, w, n, e)``
     - ``(minlat, minlon, maxlat, maxlon)``
     - ``(minx, miny, maxx, maxy)``
@@ -55,23 +56,25 @@
     """
     Base class for (groups of) geospatial objects.
 
     Classes that represent spatial features extend this class and implement the
     ``geojson`` property. Exporting objects in the GeoJSON format should make it possible
     to integrate them with other tools for visualization, or further analysis.
 
-    Objects of this class have the ``__geo_interface__`` property to follow a protocol proposed
-    by Sean Gillies, which can make it easier to use spatial data in other Python software
-    (https://gist.github.com/sgillies/2217756). An example of this is the ``shape()`` function
-    that builds Shapely geometries from any object with the ``__geo_interface__`` property.
+    Objects of this class have the ``__geo_interface__`` property to follow a protocol
+    [proposed](https://gist.github.com/sgillies/2217756) by Sean Gillies, which can make
+    it easier to use spatial data in other Python software . An example of this is the ``shape()``
+    function that builds Shapely geometries from any object with the ``__geo_interface__`` property.
 
     The ability to re-import the exported GeoJSON structures as ``Spatial`` objects is not
     considered here.
     """
 
+    __slots__ = ("__validated__",)  # we use that field in tests
+
     @property
     @abstractmethod
     def geojson(self) -> GeoJsonDict:
         """
         A mapping of this object, using the GeoJSON format.
 
         The coordinate reference system for all GeoJSON coordinates is ``CRS:84``,
@@ -87,15 +90,15 @@
 
     @property
     def __geo_interface__(self) -> GeoJsonDict:
         """See ``geojson``."""
         return self.geojson
 
 
-@dataclass(repr=False)
+@dataclass(slots=True)
 class Metadata:
     """
     Metadata concerning the most recent edit of an OSM element.
 
     Attributes:
         version: The version number of the element
         timestamp: Timestamp (ISO 8601) of the most recent change of this element
@@ -107,14 +110,55 @@
     version: int
     timestamp: str
     changeset: int
     user_name: str
     user_id: int
 
 
+G = TypeVar("G", bound=BaseGeometry)
+
+
+@dataclass(slots=True)
+class GeometryDetails(Generic[G]):
+    """
+    Element geometry with more info on its validity.
+
+    Shapely validity is based on an [OGC standard](https://www.ogc.org/standard/sfa/).
+
+    For MultiPolygons, one assertion is that its elements may only touch at a finite number
+    of Points, which means they may not share an edge on their exteriors. In terms of
+    OSM multipolygons, it makes sense to lift this requirement, and such geometries
+    end up in the ``accepted`` field.
+
+    For invalid MultiPolygon and Polygons, we use Shapely's ``make_valid()``. If and only if
+    the amount of polygons stays the same before and after making them valid,
+    they will end up in the ``valid`` field.
+
+    Attributes:
+        valid: if set, this is the original valid geometry
+        accepted: if set, this is the original geometry that is invalid by Shapely standards,
+                  but accepted by us
+        fixed: if set, this is the geometry fixed by ``make_valid()``
+        invalid: if set, this is the original invalid geometry
+        invalid_reason: if the original geometry is invalid by Shapely standards,
+                        this message states why
+    """
+
+    valid: G | None = None
+    accepted: G | None = None
+    fixed: G | None = None
+    invalid: G | None = None
+    invalid_reason: str | None = None
+
+    @property
+    def best(self) -> G | None:
+        """The "best" geometry, prioritizing ``fixed`` over ``invalid``."""
+        return self.valid or self.accepted or self.fixed or self.invalid
+
+
 @dataclass(repr=False, eq=False)
 class Element(Spatial):
     """
     Elements are the basic components of OpenStreetMap's data.
 
     A query's result set is made up of these elements.
 
@@ -159,21 +203,23 @@
     References:
         - https://wiki.openstreetmap.org/wiki/Elements
         - https://wiki.openstreetmap.org/wiki/Map_features
         - https://wiki.openstreetmap.org/wiki/Overpass_API/Overpass_QL#out
         - https://wiki.openstreetmap.org/wiki/Overpass_API/Permanent_ID
     """
 
+    __slots__ = ()
+
     id: int
-    tags: Optional[OverpassDict]
-    bounds: Optional[Bbox]
-    center: Optional[Point]
-    meta: Optional[Metadata]
+    tags: OverpassDict | None
+    bounds: Bbox | None
+    center: Point | None
+    meta: Metadata | None
     relations: list["Relationship"]
-    geometry: Optional[BaseGeometry]
+    geometry: BaseGeometry | None
 
     def tag(self, key: str, default: Any = None) -> Any:
         """
         Get the tag value for the given key.
 
         Returns ``default`` if there is no ``key`` tag.
 
@@ -183,29 +229,31 @@
         if not self.tags:
             return default
         return self.tags.get(key, default)
 
     @property
     def type(self) -> str:
         """The element's type: "node", "way", or "relation"."""
-        if isinstance(self, Node):
-            return "node"
-        if isinstance(self, Way):
-            return "way"
-        if isinstance(self, Relation):
-            return "relation"
-        raise ValueError()
+        match self:
+            case Node():
+                return "node"
+            case Way():
+                return "way"
+            case Relation():
+                return "relation"
+            case _:
+                raise AssertionError
 
     @property
     def link(self) -> str:
         """This element on openstreetmap.org."""
         return f"https://www.openstreetmap.org/{self.type}/{self.id}"
 
     @property
-    def wikidata_id(self) -> Optional[str]:
+    def wikidata_id(self) -> str | None:
         """
         [Wikidata](https://www.wikidata.org) item ID of this element.
 
         This is "perhaps, the most stable and reliable manner to obtain Permanent ID
         of relevant spatial features".
 
         References:
@@ -219,28 +267,28 @@
         """
         # since tag values are not enforced, use a regex to filter out bad IDs
         if self.tags and "wikidata" in self.tags and _WIKIDATA_Q_ID.match(self.tags["wikidata"]):
             return self.tags["wikidata"]
         return None
 
     @property
-    def wikidata_link(self) -> Optional[str]:
+    def wikidata_link(self) -> str | None:
         """This element on wikidata.org."""
         if self.wikidata_id:
             return f"https://www.wikidata.org/wiki/{self.wikidata_id}"
         return None
 
     @property
     def geojson(self) -> GeoJsonDict:
         """
         A mapping of this object, using the GeoJSON format.
 
         Objects are mapped as the following:
          - ``Node`` -> ``Feature`` with optional ``Point`` geometry
-         - ``Way`` -> ``Feature`` with optional ``LineString`` or `Polygon`` geometry
+         - ``Way`` -> ``Feature`` with optional ``LineString`` or ``Polygon`` geometry
          - ``Relation`` with geometry -> ``Feature`` with ``Polygon`` or ``MultiPolygon`` geometry
          - ``Relation`` -> ``FeatureCollection`` (nested ``Relations`` are mapped to unlocated
            ``Features``)
 
         ``Feature`` properties contain all the following keys if they are present for the element:
         ``id``, ``type``, ``role``, ``tags``, ``nodes``, ``bounds``, ``center``, ``timestamp``,
         ``version``, ``changeset``, ``user``, ``uid``.
@@ -262,108 +310,33 @@
 
         return _geojson_feature(self)
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.id})"
 
 
-_WIKIDATA_Q_ID = re.compile(r"^Q\d+$")
-
-
-def _geojson_properties(obj: Union[Element, "Relationship"]) -> GeoJsonDict:
-    elem = obj if isinstance(obj, Element) else obj.member
-
-    properties = {
-        "id": elem.id,
-        "type": elem.type,
-        "tags": elem.tags,
-        "bounds": elem.bounds,
-        "center": elem.center.coords[0] if elem.center else None,
-        "timestamp": elem.meta.timestamp if elem.meta else None,
-        "version": elem.meta.version if elem.meta else None,
-        "changeset": elem.meta.changeset if elem.meta else None,
-        "user": elem.meta.user_name if elem.meta else None,
-        "uid": elem.meta.user_id if elem.meta else None,
-        "nodes": getattr(elem, "nodes", None),
-    }
-
-    properties = {k: v for k, v in properties.items() if v is not None}
-
-    if isinstance(obj, Relationship):
-        properties["role"] = obj.role or ""
-        properties["__rel__"] = _geojson_properties(obj.relation)
-
-    return properties
-
-
-def _geojson_geometry(obj: Union[Element, "Relationship"]) -> Optional[GeoJsonDict]:
-    elem = obj if isinstance(obj, Element) else obj.member
-
-    geom = elem.geometry
-    if not geom:
-        return None
-
-    # Flip coordinates for GeoJSON compliance.
-    geom = shapely.ops.transform(lambda lat, lon: (lon, lat), geom)
-
-    mapping = shapely.geometry.mapping(geom)
-    if mapping["type"] == "LinearRing":  # this geometry does not exist in GeoJSON
-        mapping["type"] = "LineString"
-
-    return mapping
-
-
-def _geojson_bbox(obj: Union[Element, "Relationship"]) -> Optional[Bbox]:
-    elem = obj if isinstance(obj, Element) else obj.member
-
-    geom = elem.geometry
-    if not geom:
-        return None
-
-    bounds = geom.bounds  # can be (nan, nan, nan, nan)
-    if not any(math.isnan(c) for c in bounds):
-        (minlat, minlon, maxlat, maxlon) = bounds
-        return minlon, minlat, maxlon, maxlat
-
-    return None
-
-
-def _geojson_feature(obj: Union[Element, "Relationship"]) -> GeoJsonDict:
-    feature = {
-        "type": "Feature",
-        "geometry": _geojson_geometry(obj),
-        "properties": _geojson_properties(obj),
-    }
-
-    bbox = _geojson_bbox(obj)
-    if bbox:
-        feature["bbox"] = bbox  # type: ignore
-
-    return feature
-
-
-@dataclass(repr=False, eq=False)
+@dataclass(slots=True, repr=False, eq=False)
 class Node(Element):
     """
     A point in space, at a specific coordinate.
 
     Nodes are used to define standalone point features (e.g. a bench),
     or to define the shape or "path" of a way.
 
     Attributes:
         geometry: A Point or ``None`` if the coordinate is not included in the query's result set.
 
     References:
         - https://wiki.openstreetmap.org/wiki/Node
     """
 
-    geometry: Optional[Point]
+    geometry: Point | None
 
 
-@dataclass(repr=False, eq=False)
+@dataclass(slots=True, repr=False, eq=False)
 class Way(Element):
     """
     A way is an ordered list of nodes.
 
     An open way is a way whose first node is not its last node (e.g. a railway line).
     A closed way is a way whose first node is also its last node, and may be interpreted either
     as a closed polyline (e.g. a roundabout), an area (e.g. a patch of grass), or both
@@ -371,24 +344,26 @@
 
     Attributes:
         node_ids: The IDs of the nodes that make up this way, or ``None`` if they are not included
                   in the query's result set.
         geometry: A Linestring if the way is open, a LinearRing if the way is closed,
                   a Polygon if the way is closed and its tags indicate that it represents an area,
                   or ``None`` if the geometry is not included in the query's result set.
+        geometry_details: More info on the validity of ``geometry``.
 
     References:
         - https://wiki.openstreetmap.org/wiki/Way
     """
 
-    node_ids: Optional[list[int]]
-    geometry: Union[LineString, LinearRing, Polygon, None]
+    node_ids: list[int] | None
+    geometry: LineString | LinearRing | Polygon | None
+    geometry_details: GeometryDetails[LineString | LinearRing | Polygon] | None
 
 
-@dataclass(repr=False, eq=False)
+@dataclass(slots=True, repr=False, eq=False)
 class Relation(Element):
     """
     A relation is a group of nodes and ways that have a logical or geographic relationship.
 
     This relationship is described through its tags.
 
     A relation may define an area geometry, which may have boundaries made up of several
@@ -406,30 +381,32 @@
         members: Ordered member elements of this relation, with an optional role
         geometry: If this relation is deemed to represent an area, these are the complex polygons
                   whose boundaries and holes are made up of the ways inside the relation. Members
                   that are not ways, or are not part of any polygon boundary, are not part of the
                   result geometry. This is ``None`` if the geometry of the relation members is not
                   included in the query's result set, or if the relation is not deemed to represent
                   an area.
+        geometry_details: More info on the validity of ``geometry``.
 
     References:
         - https://wiki.openstreetmap.org/wiki/Relation
         - https://wiki.openstreetmap.org/wiki/Relation:multipolygon
         - https://wiki.openstreetmap.org/wiki/Relation:boundary
     """
 
     members: list["Relationship"]
-    geometry: Union[Polygon, MultiPolygon, None]
+    geometry: Polygon | MultiPolygon | None
+    geometry_details: GeometryDetails[Polygon | MultiPolygon] | None
 
-    def __iter__(self) -> Iterator[tuple[Optional[str], Element]]:
+    def __iter__(self) -> Iterator[tuple[str | None, Element]]:
         for relship in self.members:
             yield relship.role, relship.member
 
 
-@dataclass(repr=False)
+@dataclass(slots=True, repr=False)
 class Relationship(Spatial):
     """
     The relationship of an element that is part of a relation, with an optional role.
 
     Attributes:
         member:     any element
         relation:   a relation that the member is a part of
@@ -437,15 +414,15 @@
 
     References:
         - https://wiki.openstreetmap.org/wiki/Relation#Roles
     """
 
     member: Element
     relation: Relation
-    role: Optional[str]
+    role: str | None
 
     @property
     def geojson(self) -> GeoJsonDict:
         """
         A mapping of ``member``.
 
         This is ``member.geojson``, with the added properties ``role`` and ``__rel__``.
@@ -453,51 +430,62 @@
         return _geojson_feature(self)
 
     def __repr__(self) -> str:
         role = f" as '{self.role}'" if self.role else " "
         return f"{type(self).__name__}({self.member}{role} in {self.relation})"
 
 
-_KNOWN_ELEMENTS = {"node", "way", "relation", "area"}
+_KNOWN_ELEMENTS = {"node", "way", "relation"}
 
 
-_ElementKey = tuple[str, int]
+_ElementKey: TypeAlias = tuple[str, int]
 """Elements are uniquely identified by the tuple (type, id)."""
 
-_MemberKey = tuple[_ElementKey, str]
+_MemberKey: TypeAlias = tuple[_ElementKey, str]
 """Relation members are identified by their element key and role."""
 
 
 class _ElementCollector:
+    __slots__ = (
+        "member_dict",
+        "result_set",
+        "typed_dict",
+        "untyped_dict",
+    )
+
     def __init__(self) -> None:
         self.result_set: list[_ElementKey] = []
         self.typed_dict: dict[_ElementKey, Element] = {}
         self.untyped_dict: dict[_ElementKey, OverpassDict] = defaultdict(dict)
         self.member_dict: dict[int, list[_MemberKey]] = defaultdict(list)
 
 
 def collect_elements(query: Query) -> list[Element]:
     """
     Produce typed elements from the result set of a query.
 
-    This function collects elements that are of type "node", "way", "relation", or "area".
-    Derived elements with other types - f.e. produced by ``make`` and ``convert`` statements
-    or when using ``out count`` - are ignored. An exception is made for areas, which are so
-    closely derived from ways and relations that it makes sense to represent them as such.
-    If you need to work with other derived elements, you should not use this function.
+    This function exclusively collects elements that are of type "node", "way", or "relation".
 
     Element data is "conflated", which means that if elements appear more than once in a
     result set, their data is merged. This is useful f.e. when querying tags for relation members:
     using ``rel(...); out tags;`` will only print tags for relation itself, not its members.
     For those you will have to recurse down from the relation, which means members will show
     up twice in the result set: once untagged as a member of the relation, and once tagged at
     the top level. This function will have these two occurrences point to the same, single object.
 
     The order of elements and relation members is retained.
 
+    If you want to query Overpass' "area" elements, you should use the `way(pivot)` or `rel(pivot)`
+    filter to select the element of the chosen type that defines the outline of the given area.
+    Otherwise, they will be ignored.
+
+    Derived elements with other types - f.e. produced by ``make`` and ``convert`` statements
+    or when using ``out count`` - are ignored. If you need to work with other derived elements,
+    you should not use this function.
+
     Args:
         query: a finished query
 
     Returns:
         the result set as a list of typed elements
 
     Raises:
@@ -513,15 +501,15 @@
     _collect_untyped(query, collector)
     _collect_typed(collector)
     _collect_relationships(collector)
     return [collector.typed_dict[elem_key] for elem_key in collector.result_set]
 
 
 def _collect_untyped(query: Query, collector: _ElementCollector) -> None:
-    if not query.result_set:
+    if query.result_set is None:
         raise AssertionError
 
     # Here we populate 'untyped_dict' with both top level elements, and
     # relation members, while conflating their data if they appear as both.
     # We also populate 'member_dict'.
     for elem_dict in query.result_set:
         if elem_dict.get("type") not in _KNOWN_ELEMENTS:
@@ -541,14 +529,16 @@
             collector.member_dict[elem_dict["id"]].append((key, mem.get("role")))
 
 
 def _collect_typed(collector: _ElementCollector) -> None:
     for elem_key, elem_dict in collector.untyped_dict.items():
         (elem_type, elem_id) = elem_key
 
+        geometry = _geometry(elem_dict)
+
         args = dict(
             id=elem_id,
             tags=elem_dict.get("tags"),
             bounds=tuple(elem_dict["bounds"].values()) if "bounds" in elem_dict else None,
             center=Point(elem_dict["center"].values()) if "center" in elem_dict else None,
             meta=Metadata(
                 timestamp=elem_dict["timestamp"],
@@ -556,46 +546,97 @@
                 changeset=elem_dict["changeset"],
                 user_name=elem_dict["user"],
                 user_id=elem_dict["uid"],
             )
             if "timestamp" in elem_dict
             else None,
             relations=[],  # add later
-            geometry=_geometry(elem_dict),
+            geometry=geometry,
         )
 
         cls: type[Element]
 
-        if elem_type == "node":
-            cls = Node
-        elif elem_type == "way":
-            cls = Way
-            args["node_ids"] = elem_dict.get("nodes")
-        elif elem_type == "relation":
-            cls = Relation
-            args["members"] = []  # add later
-        else:
-            raise AssertionError()
+        match elem_type:
+            case "node":
+                cls = Node
+                assert geometry is None or geometry.is_valid
+            case "way":
+                cls = Way
+                args["node_ids"] = elem_dict.get("nodes")
+                args["geometry_details"] = None
+                if geometry and (geometry_details := _try_validate_geometry(geometry)) is not None:
+                    args["geometry_details"] = geometry_details
+                    args["geometry"] = geometry_details.best
+            case "relation":
+                cls = Relation
+                args["members"] = []  # add later
+                args["geometry_details"] = None
+                if geometry and (geometry_details := _try_validate_geometry(geometry)) is not None:
+                    args["geometry_details"] = geometry_details
+                    args["geometry"] = geometry_details.best
+            case _:
+                raise AssertionError
 
-        elem = cls(**args)
+        elem = cls(**args)  # pyright: ignore[reportGeneralTypeIssues]
         collector.typed_dict[elem_key] = elem
 
 
 def _collect_relationships(collector: _ElementCollector) -> None:
     for rel_id, mem_roles in collector.member_dict.items():
         rel = cast(Relation, collector.typed_dict[("relation", rel_id)])
 
         for mem_key, mem_role in mem_roles:
             mem = collector.typed_dict[mem_key]
             relship = Relationship(member=mem, relation=rel, role=mem_role or None)
             mem.relations.append(relship)
             rel.members.append(relship)
 
 
-def _geometry(raw_elem: OverpassDict) -> Optional[BaseGeometry]:
+def _try_validate_geometry(geom: G) -> GeometryDetails[G]:
+    if geom.is_valid:
+        return GeometryDetails(valid=geom)
+
+    invalid_reason = shapely.is_valid_reason(geom)
+
+    if invalid_reason.startswith("Self-intersection") and isinstance(geom, MultiPolygon):
+        # we allow self-intersecting multi-polygons, if
+        # (1) the intersection is just lines or points, and
+        # (2) all the polygons inside are valid
+        intersection = shapely.intersection_all(geom.geoms)
+        accept = not isinstance(intersection, Polygon | MultiPolygon) and all(
+            poly.is_valid for poly in geom.geoms
+        )
+
+        if accept:
+            return GeometryDetails(accepted=geom, invalid_reason=invalid_reason)
+
+        return GeometryDetails(invalid=geom, invalid_reason=invalid_reason)
+
+    if isinstance(geom, Polygon):
+        valid_polygons = [g for g in _flatten(shapely.make_valid(geom)) if isinstance(g, Polygon)]
+        if len(valid_polygons) == 1:
+            return GeometryDetails(
+                fixed=valid_polygons[0],
+                invalid=geom,
+                invalid_reason=invalid_reason,
+            )
+
+    if isinstance(geom, MultiPolygon):
+        valid_polygons = [g for g in _flatten(shapely.make_valid(geom)) if isinstance(g, Polygon)]
+        if len(valid_polygons) == len(geom.geoms):
+            return GeometryDetails(
+                fixed=MultiPolygon(valid_polygons),
+                invalid=geom,
+                invalid_reason=invalid_reason,
+            )
+
+    return GeometryDetails(invalid=geom, invalid_reason=invalid_reason)
+
+
+def _geometry(raw_elem: OverpassDict) -> BaseGeometry | None:
     """
     Construct the geometry a given OSM element makes up.
 
     Args:
         raw_elem: an element from a query's result set
 
     Returns:
@@ -654,15 +695,15 @@
             return polys[0]
 
         return MultiPolygon(polys)
 
     return None
 
 
-def _line(way: OverpassDict) -> Union[LineString, LinearRing, None]:
+def _line(way: OverpassDict) -> LineString | LinearRing | None:
     """Returns the geometry of a way in the result set."""
     if "geometry" not in way or len(way["geometry"]) < 2:
         return None
     is_ring = way["geometry"][0] == way["geometry"][-1]
     cls = LinearRing if is_ring else LineString
     return cls((c["lat"], c["lon"]) for c in way["geometry"])
 
@@ -764,7 +805,81 @@
 }
 
 _AREA_TAG_VALUES_NONE_OF = {
     "aeroway": {"no", "taxiway"},
     "man_made": {"no", "cutline", "embankment", "pipeline"},
     "natural": {"no", "coastline", "cliff", "ridge", "arete", "tree_row"},
 }
+
+_WIKIDATA_Q_ID = re.compile(r"^Q\d+$")
+
+
+def _geojson_properties(obj: Element | Relationship) -> GeoJsonDict:
+    elem = obj if isinstance(obj, Element) else obj.member
+
+    properties = {
+        "id": elem.id,
+        "type": elem.type,
+        "tags": elem.tags,
+        "bounds": elem.bounds,
+        "center": elem.center.coords[0] if elem.center else None,
+        "timestamp": elem.meta.timestamp if elem.meta else None,
+        "version": elem.meta.version if elem.meta else None,
+        "changeset": elem.meta.changeset if elem.meta else None,
+        "user": elem.meta.user_name if elem.meta else None,
+        "uid": elem.meta.user_id if elem.meta else None,
+        "nodes": getattr(elem, "nodes", None),
+    }
+
+    properties = {k: v for k, v in properties.items() if v is not None}
+
+    if isinstance(obj, Relationship):
+        properties["role"] = obj.role or ""
+        properties["__rel__"] = _geojson_properties(obj.relation)
+
+    return properties
+
+
+def _geojson_geometry(obj: Element | Relationship) -> GeoJsonDict | None:
+    elem = obj if isinstance(obj, Element) else obj.member
+
+    geom = elem.geometry
+    if not geom:
+        return None
+
+    # Flip coordinates for GeoJSON compliance.
+    geom = shapely.ops.transform(lambda lat, lon: (lon, lat), geom)
+
+    mapping = shapely.geometry.mapping(geom)
+    if mapping["type"] == "LinearRing":  # this geometry does not exist in GeoJSON
+        mapping["type"] = "LineString"
+
+    return mapping
+
+
+def _geojson_bbox(obj: Element | Relationship) -> Bbox | None:
+    elem = obj if isinstance(obj, Element) else obj.member
+
+    geom = elem.geometry
+    if not geom:
+        return None
+
+    bounds = geom.bounds  # can be (nan, nan, nan, nan)
+    if not any(math.isnan(c) for c in bounds):
+        (minlat, minlon, maxlat, maxlon) = bounds
+        return minlon, minlat, maxlon, maxlat
+
+    return None
+
+
+def _geojson_feature(obj: Element | Relationship) -> GeoJsonDict:
+    feature = {
+        "type": "Feature",
+        "geometry": _geojson_geometry(obj),
+        "properties": _geojson_properties(obj),
+    }
+
+    bbox = _geojson_bbox(obj)
+    if bbox:
+        feature["bbox"] = bbox  # type: ignore
+
+    return feature
```

### Comparing `aio_overpass-0.8.0/aio_overpass/error.py` & `aio_overpass-0.9.0/aio_overpass/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 import asyncio
 import html
 import re
 from dataclasses import dataclass
 from enum import Enum, auto
 from json import JSONDecodeError
-from typing import Optional, Union, no_type_check
+from typing import no_type_check
 
 import aiohttp
 import aiohttp.typedefs
 
 
 __docformat__ = "google"
 __all__ = (
@@ -96,15 +96,15 @@
     An API request timed out.
 
     Attributes:
         cause: the exception that caused this error
         after_secs: the configured timeout for the request
     """
 
-    cause: asyncio.TimeoutError
+    cause: asyncio.TimeoutError  # type: ignore[assignment]
     after_secs: float
 
     def __post_init__(self) -> None:
         # imitate "raise CallError(...) from cause"
         self.__cause__ = self.cause
 
     def __str__(self) -> str:
@@ -120,23 +120,23 @@
     This may indicate a bug on our end, since the client is meant to process almost any
     response of an Overpass API instance.
 
     Attributes:
         request_info: Contains information about request.
         history: History from failed response.
         status: HTTP status code of response, e.g. ``400``.
-        message: Message of response, e.g. ``"OK"``.
+        message: Message of response, e.g. ``"Bad Request"``.
         headers: Headers in response, a list of pairs.
     """
 
     request_info: aiohttp.RequestInfo
     history: tuple[aiohttp.ClientResponse, ...]
     status: int
     message: str
-    headers: Optional[aiohttp.typedefs.LooseHeaders]
+    headers: aiohttp.typedefs.LooseHeaders | None
 
     @property
     def response(self) -> aiohttp.ClientResponse:
         """Client response returned by ``aiohttp.ClientSession.request()`` and family."""
         return self.history[-1]
 
     def __str__(self) -> str:
@@ -242,58 +242,63 @@
     its proposed ``[maxsize:*]``, and has been cancelled by the server.
 
     A higher ``[maxsize:*]`` value might allow the query run to completion, but also makes it
     more likely to be rejected by a server under heavy load, before executing it (see ``TOO_BUSY``).
     """
 
     def __str__(self) -> str:
-        if self == QueryRejectCause.TOO_BUSY:
-            return "server too busy"
-        if self == QueryRejectCause.TOO_MANY_QUERIES:
-            return "too many queries"
-        if self == QueryRejectCause.EXCEEDED_TIMEOUT:
-            return "exceeded 'timeout'"
-        if self == QueryRejectCause.EXCEEDED_MAXSIZE:
-            return "exceeded 'maxsize'"
-        raise AssertionError()
+        match self:
+            case QueryRejectCause.TOO_BUSY:
+                return "server too busy"
+            case QueryRejectCause.TOO_MANY_QUERIES:
+                return "too many queries"
+            case QueryRejectCause.EXCEEDED_TIMEOUT:
+                return "exceeded 'timeout'"
+            case QueryRejectCause.EXCEEDED_MAXSIZE:
+                return "exceeded 'maxsize'"
+            case _:
+                raise AssertionError
 
 
 @dataclass
 class QueryRejectError(QueryError):
     """
     A query was rejected or cancelled by the API server.
 
     Attributes:
         cause: why the query was rejected or cancelled
     """
 
     cause: QueryRejectCause
 
     def __str__(self) -> str:
-        if self.cause in (QueryRejectCause.TOO_BUSY, QueryRejectCause.TOO_MANY_QUERIES):
-            rejection = "query rejected"
-        else:
-            rejection = "query cancelled"
+        match self.cause:
+            case QueryRejectCause.TOO_BUSY | QueryRejectCause.TOO_MANY_QUERIES:
+                rejection = "query rejected"
+            case QueryRejectCause.EXCEEDED_TIMEOUT | QueryRejectCause.EXCEEDED_MAXSIZE:
+                rejection = "query cancelled"
+            case _:
+                raise AssertionError(self.cause)
 
         return f"{rejection}: {self.cause}"
 
 
 @no_type_check
 def _to_client_error(
-    obj: Union[aiohttp.ClientResponse, aiohttp.ClientError]
-) -> Union[CallError, ResponseError]:
+    obj: aiohttp.ClientResponse | aiohttp.ClientError,
+) -> CallError | ResponseError:
     """
     Build a ``ClientError`` from either an ``aiohttp`` client error or an unrecognized response.
 
     Returns:
         - ``CallError`` if ``obj`` is an ``aiohttp.ClientError``,
           but not an ``aiohttp.ClientResponseError``.
         - ``ResponseError`` if ``obj`` is a response or an ``aiohttp.ClientResponseError``.
     """
-    if not isinstance(obj, (aiohttp.ClientResponseError, aiohttp.ClientResponse)):
+    if not isinstance(obj, aiohttp.ClientResponseError | aiohttp.ClientResponse):
         return CallError(cause=obj)
 
     error = ResponseError(
         request_info=obj.request_info,
         history=obj.history,
         status=obj.status,
         message=obj.message if isinstance(obj, aiohttp.ClientResponseError) else obj.reason,
@@ -413,15 +418,15 @@
 
     if reject_causes:
         raise QueryRejectError(kwargs=query_kwargs, remarks=errors, cause=reject_causes[0])
 
     raise _query_response_error(kwargs=query_kwargs, remarks=errors, response=response)
 
 
-def _match_reject_cause(error_msg: str) -> Optional[QueryRejectCause]:
+def _match_reject_cause(error_msg: str) -> QueryRejectCause | None:
     """
     Check if the given error message indicates that a query was rejected or cancelled.
 
     AFAIK, neither the 'remarks' in JSON responses, nor the errors listed in HTML responses
     are neatly listed somewhere, but it seems matching a small subset of remarks is enough
     to identify recoverable errors.
```

### Comparing `aio_overpass-0.8.0/aio_overpass/pt.py` & `aio_overpass-0.9.0/aio_overpass/pt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Classes and queries specialized on public transportation routes."""
 
 from collections import Counter
 from collections.abc import Generator
 from dataclasses import dataclass
 from enum import Enum, auto
-from typing import Any, Optional, Union, cast
+from typing import Any, cast
 
 from aio_overpass._dist import fast_distance
 from aio_overpass.element import (
     Bbox,
     GeoJsonDict,
     Node,
     OverpassDict,
@@ -23,23 +23,23 @@
 
 import shapely.ops
 from shapely.geometry import GeometryCollection, Point, Polygon
 
 
 __docformat__ = "google"
 __all__ = (
+    "collect_routes",
+    "RouteQuery",
+    "SingleRouteQuery",
+    "RoutesWithinQuery",
     "Route",
+    "Vehicle",
     "Stop",
     "Connection",
-    "Vehicle",
     "RouteScheme",
-    "RouteQuery",
-    "SingleRouteQuery",
-    "RoutesWithinQuery",
-    "collect_routes",
 )
 
 
 class RouteQuery(Query):
     """
     Base class for queries that produce ``Route`` and ``RouteSegment`` objects.
 
@@ -99,15 +99,14 @@
             .routes <<;
             rel._[type=route_master]->.masters;
         """
 
         super().__init__(input_code, **kwargs)
 
 
-@dataclass
 class RoutesWithinQuery(RouteQuery):
     """
     A query that produces ``Route`` objects for any route within the exterior of a polygon.
 
     Args:
         polygon: Any route that has at least one member element within this shape
                  will be in the result set of this query. Note that the route members
@@ -115,17 +114,15 @@
                  be outside of it. This shape should be simplified, since a larger number
                  of coordinates on the exterior will slow down the query.
         vehicles: A list of transportation modes to filter by, or an empty list to include
                   routes of any type. A non-empty list will filter routes by the ``route``
                   key.
     """
 
-    def __init__(
-        self, polygon: Polygon, vehicles: Optional[list["Vehicle"]] = None, **kwargs
-    ) -> None:
+    def __init__(self, polygon: Polygon, vehicles: list["Vehicle"] | None = None, **kwargs) -> None:
         if not vehicles:
             vehicles = list(Vehicle)
 
         self.polygon = polygon
         self.vehicles = vehicles
 
         region_clause = poly_clause(self.polygon)
@@ -173,15 +170,15 @@
         """``True`` if you can exit at this stop on the route."""
         return self != Connection.ENTRY_ONLY
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}.{self.name}"
 
 
-@dataclass
+@dataclass(slots=True)
 class Stop(Spatial):
     """
     A stop on a public transportation route.
 
     Typically, a stop is modelled as two members in a relation: a stop_position node with the
     'stop' role, and a platform with the 'platform' role. These members may be grouped in
     a common stop_area.
@@ -192,20 +189,20 @@
         stop_position: the stop position node associated with this stop, if any
         stop_coords: a point that, compared to ``stop_position``, is guaranteed to be on the
                      track of the route whenever it is set. Only set if you are collecting
                      ``RouteSegments``.
     """
 
     idx: int
-    platform: Optional[Relationship]
-    stop_position: Optional[Relationship]
-    stop_coords: Union[Node, Point, None]
+    platform: Relationship | None
+    stop_position: Relationship | None
+    stop_coords: Node | Point | None
 
     @property
-    def name(self) -> Optional[str]:
+    def name(self) -> str | None:
         """
         This stop's name.
 
         If platform and stop position names are the same, that name will be returned.
         Otherwise, the most common name out of platform, stop position, and all related stop areas
         will be returned.
         """
@@ -249,15 +246,15 @@
     @property
     def geojson(self) -> GeoJsonDict:
         """A mapping of this object, using the GeoJSON format."""
         # TODO Stop geojson
         raise NotImplementedError
 
     @property
-    def _stop_point(self) -> Optional[Point]:
+    def _stop_point(self) -> Point | None:
         """This is set if we have a point that is on the track of the route."""
         if isinstance(self.stop_coords, Node):
             return self.stop_coords.geometry
         if isinstance(self.stop_coords, Point):
             return self.stop_coords
         return None
 
@@ -331,27 +328,31 @@
 
     ASSUME_V1 = auto()
     ASSUME_V2 = auto()
 
     OTHER = auto()
 
     @property
-    def version_number(self) -> Optional[int]:
+    def version_number(self) -> int | None:
         """Public transport tagging scheme."""
-        if self in (RouteScheme.EXPLICIT_V1, RouteScheme.ASSUME_V1):
-            return 1
-        if self in (RouteScheme.EXPLICIT_V2, RouteScheme.ASSUME_V2):
-            return 2
-        return None
+        match self:
+            case RouteScheme.EXPLICIT_V1 | RouteScheme.ASSUME_V1:
+                return 1
+            case RouteScheme.EXPLICIT_V2 | RouteScheme.ASSUME_V2:
+                return 2
+            case RouteScheme.OTHER:
+                return None
+            case _:
+                raise AssertionError
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}.{self.name}"
 
 
-@dataclass
+@dataclass(slots=True)
 class Route(Spatial):
     """
     A public transportation service route, e.g. a bus line.
 
     Instances of this class are meant to represent OSM routes using the
     'Public Transport Version 2' (PTv2) scheme. Compared to PTv1, this means f.e. that routes
     with multiple directions (forwards, backwards) are represented by multiple route elements.
@@ -443,52 +444,52 @@
         return [
             relship.relation
             for relship in self.relation.relations
             if relship.relation.tag("type") == "route_master"
         ]
 
     @property
-    def name_from(self) -> Optional[str]:
+    def name_from(self) -> str | None:
         """
         Name of the start station.
 
         This is either the value of the relation's ``from`` key, a name derived
         from the route's first stop (see ``Stop.name``), or ``None`` if neither
         is available.
         """
         return self.relation.tag(
             key="from",
             default=self.stops[0].name if self.stops else None,
         )
 
     @property
-    def name_to(self) -> Optional[str]:
+    def name_to(self) -> str | None:
         """
         Name of the end station.
 
         This is either the value of the relation's ``to`` key, a name derived
         from the route's last stop (see ``Stop.name``), or ``None`` if neither
         is available.
         """
         return self.relation.tag(
             key="to",
             default=self.stops[-1].name if len(self.stops) > 1 else None,
         )
 
     @property
-    def name_via(self) -> Optional[str]:
+    def name_via(self) -> str | None:
         """
         A name of an important station along the route.
 
         This is either the value of the relation's ``via`` key, or ``None`` if it is not set.
         """
         return self.relation.tag("via")
 
     @property
-    def name(self) -> Optional[str]:
+    def name(self) -> str | None:
         """
         The name of the route.
 
         This is either the value relation's ``name`` key, ``{from_} => {via} => {to}`` if at
         least ``from`` and ``to`` are set, or ``None`` otherwise.
         """
         name_tag = self.tag("name")
@@ -515,18 +516,18 @@
         This value corresponds with the value of the relation's ``route`` key.
         """
         if not self.relation.tags or "route" not in self.relation.tags:
             raise AssertionError
         return Vehicle[self.relation.tags["route"].upper()]
 
     @property
-    def bounds(self) -> Optional[Bbox]:
+    def bounds(self) -> Bbox | None:
         """The bounding box around all stops of this route."""
         geom = GeometryCollection([stop._geometry for stop in self.stops if stop._geometry])
-        return geom.bounds or None
+        return geom.bounds or None  # pyright: ignore[reportGeneralTypeIssues]
 
     @property
     def geojson(self) -> GeoJsonDict:
         """A mapping of this object, using the GeoJSON format."""
         # TODO Route geojson
         raise NotImplementedError
 
@@ -551,15 +552,15 @@
 in order to avoid duplication.
 
 References:
     - https://wiki.openstreetmap.org/wiki/Relation:route_master
 """
 
 
-def collect_routes(query: RouteQuery, perimeter: Optional[Polygon] = None) -> list[Route]:
+def collect_routes(query: RouteQuery, perimeter: Polygon | None = None) -> list[Route]:
     # TODO the way 'perimeter' works might be confusing
     """
     Consumes the result set of a query and produces ``Route`` objects.
 
     The order of elements is *not* retained.
 
     The result set in the input query will be empty after calling this function.
@@ -606,20 +607,22 @@
 
     return routes
 
 
 def _scheme(route: Relation) -> RouteScheme:
     """Try to identify a route's tagging scheme."""
     tagged_version = route.tag("public_transport:version")
-    if tagged_version == "1":
-        return RouteScheme.EXPLICIT_V1
-    if tagged_version == "2":
-        return RouteScheme.EXPLICIT_V2
-    if tagged_version:
-        return RouteScheme.OTHER
+
+    match tagged_version:
+        case "1":
+            return RouteScheme.EXPLICIT_V1
+        case "2":
+            return RouteScheme.EXPLICIT_V2
+        case _ if tagged_version:
+            return RouteScheme.OTHER
 
     # any directed and/or numbered tags like "forward:stop:1" indicate PTv1
     directions = {
         "forward:",
         "forward_",
         "backward:",
         "backward_",
@@ -661,15 +664,15 @@
     # Consider all route relation members that are tagged or given a role that makes them
     # relevant for public transportation.
     route_members = [
         relship for relship in route_relation.members if _role(relship) is not _RouteRole.NONE
     ]
 
     # no more than two elements per group (best case: roles "stop" & "platform")
-    prev: Optional[Relationship] = None
+    prev: Relationship | None = None
     for next_ in route_members:
         if not prev:  # case 1: no two members to compare yet
             prev = next_
             continue
 
         if not _at_same_stop(prev, next_):  # case 2: members are not part of same station
             yield to_stop(prev)
```

### Comparing `aio_overpass-0.8.0/aio_overpass/pt_ordered.py` & `aio_overpass-0.9.0/aio_overpass/pt_ordered.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 """Collect the routes of a ``RouteQuery`` with optimized geometry."""
 
 import itertools
-from collections.abc import Generator
+from collections.abc import Callable, Generator, Iterator
 from dataclasses import dataclass, replace
-from typing import Any, Callable, Optional, Union, cast
+from typing import Any, TypeAlias, cast
 
 from aio_overpass._dist import fast_distance
 from aio_overpass.element import GeoJsonDict, Node, Relation, Relationship, Spatial, Way
 
 import networkx as nx
 import shapely.ops
 from networkx import MultiDiGraph
 from shapely.geometry import (
     GeometryCollection,
+    LinearRing,
     LineString,
     MultiLineString,
     MultiPoint,
     Point,
     Polygon,
 )
 
 from .pt import _MAX_DISTANCE_TO_TRACK, Route, RouteQuery, Stop, collect_routes
 
 
 __docformat__ = "google"
 __all__ = (
+    "collect_ordered_routes",
+    "to_ordered_route",
+    "to_ordered_routes",
     "OrderedRouteView",
     "OrderedRouteViewNode",
-    "collect_ordered_routes",
 )
 
 
-@dataclass
+@dataclass(slots=True)
 class OrderedRouteViewNode:
     """
     A node on the path of a route.
 
     Attributes:
         lon: Node longitude.
         lat: Node latitude.
@@ -46,21 +49,21 @@
         n_seen_stops: The number of visited stops so far.
                       Increases on every stop (``1..=nb_stops``).
         distance: The approximate distance travelled so far, in meters.
     """
 
     lon: float
     lat: float
-    way_id: Optional[int]
+    way_id: int | None
     path_idx: int
     n_seen_stops: int
     distance: float
 
 
-@dataclass
+@dataclass(slots=True)
 class OrderedRouteView(Spatial):
     """
     A view of a public transportation route with simplified and directed path geometry.
 
     Views of a route can start at any stop, and end at a later stop.
     They are continouous if between every stop, there is a path of contigious ways.
     This is not the case for route relations that have a gap in their track.
@@ -108,22 +111,23 @@
         self, predicate: Callable[[OrderedRouteViewNode, OrderedRouteViewNode], bool]
     ) -> Generator["OrderedRouteView", None, None]:
         if len(self.ordering) < 2:
             return
 
         ordering: list[OrderedRouteViewNode] = []
 
-        for a, b in zip(self.ordering, self.ordering[1:]):
+        for a, b in zip(self.ordering, self.ordering[1:], strict=False):
             if predicate(a, b):
                 yield replace(self, ordering=ordering)
                 ordering = [a]
             else:
                 ordering.append(a)
 
-        ordering.append(b)
+        ordering.append(b)  # pyright: ignore[reportUnboundVariable]
+
         yield replace(self, ordering=ordering)
 
     def _group_by(self, key: Callable[[OrderedRouteViewNode], Any]) -> list["OrderedRouteView"]:
         return list(self._split(predicate=lambda a, b: key(a) != key(b)))
 
     def gap_split(self) -> list["OrderedRouteView"]:
         """Split this view wherever there's a gap in between stops."""
@@ -172,39 +176,39 @@
                 break
 
             ordering.extend(nodes)
 
         return replace(self, ordering=ordering)
 
     @property
-    def paths(self) -> list[Optional[LineString]]:
+    def paths(self) -> list[LineString | None]:
         """
         The simple paths between every pair of stops.
 
         These linestrings are the shortest paths, merged from contiguous ways in the route relation.
         Whenever there is no path between two stops, a `None` element will be inserted into the
         result list.
         """
         max_nb_paths = len(self.stops) - 1
 
         grouped = itertools.groupby(iterable=self.ordering, key=lambda node: node.path_idx)
 
-        lines: list[Optional[LineString]] = [None for _ in range(max_nb_paths)]
+        lines: list[LineString | None] = [None for _ in range(max_nb_paths)]
 
         for n, nodes_iter in grouped:
             nodes = [(node.lat, node.lon) for node in nodes_iter]
             if len(nodes) < 2:
                 continue
             line = LineString(nodes)
             lines[n] = line
 
         return lines
 
     @property
-    def path(self) -> Union[LineString, MultiLineString]:
+    def path(self) -> LineString | MultiLineString:
         """
         The geometry representing the path travelled on this view from the first to last stop.
 
         This is the result of ordering (a subset of) ways inside a route relation by the order of
         traversal, and concatenating them. The order is found by building shortest paths between
         stops. Whenever stops cannot be reached with the ways that are included in the relation,
         the geometry will be split up. This happens when there are "holes" in the relation.
@@ -214,28 +218,29 @@
         if not any(ls for ls in paths):
             return MultiLineString([])
 
         # group consecutive stretches of lines or None values
         stretches_grouped = itertools.groupby(iterable=paths, key=bool)
 
         # select all sets of consecutive lines to merge them
-        stretches = (line_strings for has_track, line_strings in stretches_grouped if has_track)
+        stretches: Iterator[Iterator[LineString]] = (
+            line_strings for has_track, line_strings in stretches_grouped if has_track
+        )
 
         merged_lines = []
 
         for line_strings in stretches:
             coords: list[list[float]] = []
 
             for line in line_strings:
                 if not coords:
                     coords.extend(line.coords)
                 else:
-                    coords.extend(
-                        line.coords[1:]
-                    )  # ignore first coord, it's equal to the previous one
+                    # ignore first coord, it's equal to the previous one
+                    coords.extend(line.coords[1:])
 
             merged_line = LineString(coords)
             merged_lines.append(merged_line)
 
         if len(merged_lines) == 1:
             return merged_lines[0]
 
@@ -245,20 +250,21 @@
     def geojson(self) -> GeoJsonDict:
         """A mapping of this object, using the GeoJSON format."""
         # TODO OrderedRouteView geojson
         raise NotImplementedError
 
 
 def collect_ordered_routes(
-    query: RouteQuery, perimeter: Optional[Polygon] = None, n_jobs: int = 1
+    query: RouteQuery, perimeter: Polygon | None = None, n_jobs: int = 1
 ) -> list[OrderedRouteView]:
+    # TODO the way 'perimeter' works might be confusing
     """
     Produce ``OrderedRouteViews`` objects from a result set.
 
-    Compare to ``collect_routes()``, this function tries to build the geometry representing the
+    Compared to ``collect_routes()``, this function tries to build the geometry representing the
     path travelled on every route from the first to last stop. If there are no holes in a route's
     relation, this can typically generate a single line string to represent the entire path of
     a route. Note that routes tagged with the PTv1 scheme will be ignored (in an effort to keep
     the implemenation as simple as possible).
 
     Since we cannot guarantee that relation members are ordered, we have to convert the route into
     a graph, and find the shortest paths between stops. The more complex the graph, and the more
@@ -283,19 +289,25 @@
     Raises:
         ValueError: if the input query has no result set
         ImportError: if ``n_jobs != 1`` and the ``joblib`` extra is missing
 
     Returns:
         all routes in the result set of the input query
     """
-    if n_jobs != 1:
-        import joblib
-
     routes = collect_routes(query, perimeter)
+    return to_ordered_routes(routes, n_jobs)
+
 
+def to_ordered_route(route: Route) -> OrderedRouteView:
+    """Like ``collect_ordered_routes()``, but for a single route."""
+    return next(iter(to_ordered_routes([route])))
+
+
+def to_ordered_routes(routes: list[Route], n_jobs: int = 1) -> list[OrderedRouteView]:
+    """Like ``collect_ordered_routes()``, but for a list of routes."""
     if not routes:
         return []
 
     if len(routes) == 1:
         n_jobs = 1
 
     views = []
@@ -323,30 +335,33 @@
             stop.stop_coords = _find_stop_coords(stop, track_graph, track_nodes, track_ways)
 
         views.append(seg)
         graphs.append(track_graph)
 
     # Try to find linestrings that connect all pairs of stops.
     if n_jobs == 1:
-        for seg, route, graph in zip(views, routes, graphs):
-            seg.ordering = _paths(graph, targets=[stop._stop_point for stop in route.stops])
+        for seg, route, graph in zip(views, routes, graphs, strict=False):
+            targets = [stop._stop_point for stop in route.stops]
+            seg.ordering = _paths(graph, targets=targets)
     else:
+        import joblib
+
         # Note: keep in mind that these objects have to be serialized to use in a seperate process,
         # which could take a while for large objects.
         parallel_args = [
             (graph, [stop._stop_point for stop in route.stops])
-            for route, graph in zip(views, graphs)
+            for route, graph in zip(views, graphs, strict=True)
         ]
 
         # TODO think about using joblib.Parallel's "return_as"
         #   => can produce a generator that yields the results as soon as they are available
         with joblib.parallel_backend(backend="loky", n_jobs=n_jobs):
             paths = joblib.Parallel()(joblib.delayed(_paths)(*args) for args in parallel_args)
 
-        for seg, path in zip(views, paths):
+        for seg, path in zip(views, paths, strict=True):
             seg.ordering = path
 
     return [*views, *views_empty]
 
 
 def _route_graph(rel: Relation) -> MultiDiGraph:
     """
@@ -361,14 +376,15 @@
     """
     graph = MultiDiGraph()
 
     track = [relship for relship in rel.members if _is_track(relship)]
 
     for relship in track:
         way = cast(Way, relship.member)
+        assert way.geometry is not None
 
         data = {_WAY_ID_KEY: way.id}
 
         if way.tag("oneway") == "no":
             is_oneway = False
         else:
             is_oneway = any((way.tag(k) in v for k, v in _PT_ONEWAY_TAGS.items()))
@@ -376,19 +392,20 @@
         if is_oneway:
             add_forward_edges = relship.role != "backward"
             add_backward_edges = not add_forward_edges
         else:
             add_forward_edges = add_backward_edges = True
 
         if isinstance(way.geometry, Polygon):
-            nodes = list(way.geometry.exterior.coords)
+            ext: LinearRing = way.geometry.exterior
+            nodes = list(ext.coords)
         else:
             nodes = list(way.geometry.coords)
 
-        for a, b in zip(nodes, nodes[1:]):
+        for a, b in itertools.pairwise(nodes):
             if add_forward_edges:
                 graph.add_edge(a, b, **data)
 
             if add_backward_edges:
                 graph.add_edge(b, a, **data)
 
     return graph
@@ -413,15 +430,15 @@
     return relship.member.type == "way" and (
         not relship.role or not relship.role.startswith("platform")
     )
 
 
 def _find_stop_coords(
     stop: Stop, track_graph: MultiDiGraph, track_nodes: MultiPoint, track_ways: MultiLineString
-) -> Union[Node, Point, None]:
+) -> Node | Point | None:
     """
     Find a node on the track that closesly represents the stop position.
 
     Args:
         stop: the stop to locate on the graph
         track_graph: the graph that represents the route's track
         track_nodes: a point for every node in the graph
@@ -432,27 +449,28 @@
      - Some Node if we found a stop position in either relation or a stop relation
      - Some Point if we found a close node on the track, that is *probably* close to the
        actual stop position
     """
     # (a) check if the route relation has a stop_position for this stop
     if stop.stop_position:
         stop_node = cast(Node, stop.stop_position.member)
+        assert stop_node.geometry is not None
         if stop_node.geometry.coords[0] in track_graph:
             return stop_node
 
     # (b) check if a related stop_area has a stop_position for this stop
     station_stop_positions = (
         cast(Node, member)
         for stop_area in stop.stop_areas
         for _, member in stop_area
         if member.tag("public_transport") == "stop_position"
     )
 
     stop_pos = next(
-        (el for el in station_stop_positions if el.geometry.coords[0] in track_graph), None
+        (el for el in station_stop_positions if el.geometry.coords[0] in track_graph), None  # type: ignore[union-attr]
     )
 
     if stop_pos:
         return stop_pos
 
     # (c) use a node on the graph, that is closest to one of the relation members
     station_geom = GeometryCollection(
@@ -477,26 +495,27 @@
     # This node is *probably* representative of the actual stop position for this stop.
     # It is possible though, that the node is actually close to more than one way
     # on the route's track, and that we choose a node that could be far from the
     # actual stop position.
     return a
 
 
-def _paths(route_graph: MultiDiGraph, targets: list[Optional[Point]]) -> list[OrderedRouteViewNode]:
+def _paths(route_graph: MultiDiGraph, targets: list[Point | None]) -> list[OrderedRouteViewNode]:
     """
     Find shortest paths in the directed route graph between every target stop.
 
     Edge weights are set to the metric distance between two nodes.
 
     Not every two stops can be connected, f.e. when they have no representative
     position on the route's track, or when that track has gaps.
 
     Args:
         route_graph: the unweighted, directed graph of the route's track
-        targets: the stop positions to connect
+        targets: the stop positions to connect - missing stop positions are
+                 represented by ``None``
     """
     # set edge weights to metric distance
     for u, v in route_graph.edges():
         if _WEIGHT_KEY in route_graph[u][v][0]:
             continue
 
         distance = fast_distance(*u, *v)  # meters
@@ -514,97 +533,107 @@
         targets_left=targets[1:],
         targets_visited=targets[:1],
         ordering=[],
         distance=0.0,
         path_idx=0,
     )
 
-    traversal = _traverse_graph(graph=route_graph, progress=traversal)
+    _traverse_graph(graph=route_graph, progress=traversal)
 
     return traversal.ordering
 
 
-_GraphNode = tuple[float, float]
+_GraphNode: TypeAlias = tuple[float, float]
 
 
-@dataclass
+@dataclass(slots=True, repr=False, eq=False, match_args=False)
 class _Traversal:
+    """
+    Route graph traversal.
+
+    Attributes:
+        ordering: nodes that make up the traversed path
+        targets_visited: visited targets - missing stop positions are represented by ``None``
+        targets_left: targets left to visit - missing stop positions are represented by ``None``
+        distance: travelled distance so far
+        path_idx: see ``OrderedRouteViewNode.path_idx``
+    """
+
     ordering: list[OrderedRouteViewNode]
-    targets_visited: list[Optional[Point]]
-    targets_left: list[Optional[Point]]
+    targets_visited: list[Point | None]
+    targets_left: list[Point | None]
     distance: float
     path_idx: int
 
 
-def _traverse_graph(graph: MultiDiGraph, progress: _Traversal) -> _Traversal:
+def _traverse_graph(graph: MultiDiGraph, progress: _Traversal) -> None:
     """Find shortest paths between targets, while discouraging edges to be traversed twice."""
     if len(progress.targets_left) == 0:
-        return progress
+        return
 
     a = progress.targets_visited[-1]
     b = progress.targets_left[0]
 
     u = a.coords[0] if a else None
     v = b.coords[0] if b else None
 
     if u != v:
         try:
             path_nodes = nx.shortest_path(graph, source=u, target=v, weight=_WEIGHT_KEY)
-            next_progress = _traverse_path(graph, progress, path_nodes)
-            return _traverse_graph(graph, next_progress)
+            _traverse_path(graph, progress, path_nodes)
+            return _traverse_graph(graph, progress)
         except nx.NetworkXNoPath:
             pass
 
-    next_progress = _Traversal(
-        ordering=[
-            *progress.ordering,
+    if u is not None and progress.ordering:
+        progress.ordering.append(
             OrderedRouteViewNode(
                 lon=u[1],
                 lat=u[0],
                 way_id=None,
                 path_idx=progress.path_idx,
                 n_seen_stops=len(progress.targets_visited),
                 distance=progress.distance,
-            ),
-        ],
-        targets_left=progress.targets_left[1:],
-        targets_visited=progress.targets_visited + progress.targets_left[:1],
-        distance=progress.distance,
-        path_idx=progress.path_idx + 1,
-    )
-    return _traverse_graph(graph, next_progress)
+            )
+        )
+
+    progress.targets_visited.append(progress.targets_left.pop(0))
+    progress.path_idx += 1
 
+    return _traverse_graph(graph, progress)
 
-def _traverse_path(
-    graph: MultiDiGraph, progress: _Traversal, path_nodes: list[_GraphNode]
-) -> _Traversal:
+
+def _traverse_path(graph: MultiDiGraph, progress: _Traversal, path_nodes: list[_GraphNode]) -> None:
     """
     Walk the path to visit the next stop, and collect path nodes along the way.
 
     Repeated traversal of the edge (u, v) is discouraged by setting a large, arbitrary weight.
     Implicitly, this discourages repeated traversal of ways in a route relation. Since the path
     members are supposed to be ordered, ways that are repeatedly traversed should appear more than
     once in the relation. But since we cannot guarantee that, flat-out removal of these edges/ways
     would be too drastic.
     """
     if not path_nodes:
         msg = "expected non-empty list of nodes"
         raise ValueError(msg)
 
-    edges = list(zip(path_nodes, path_nodes[1:]))
+    edges = itertools.pairwise(path_nodes)
     n_seen_stops = len(progress.targets_visited)
-    new_ordering = []
+
+    last_node: _GraphNode | None = None
+    last_way_id: int | None = None
+
+    skip_node: _GraphNode | None = None
+    if progress.ordering:
+        skip_node = (progress.ordering[-1].lat, progress.ordering[-1].lon)
 
     for u, v in edges:
         # don't duplicate last visited stop position node
-        if (
-            progress.ordering
-            and progress.ordering[-1].lat == u[0]
-            and progress.ordering[-1].lon == u[1]
-        ):
+        if skip_node is not None:
+            skip_node = None
             continue
 
         # The path does not specify exactly which edge was traversed, so we select
         # the parallel edge of (u, v) that has the smallest weight, and increase it.
         u, v, key, _ = min(
             graph.edges([u, v], keys=True, data=True), key=lambda t: t[3][_WEIGHT_KEY]
         )
@@ -615,43 +644,44 @@
         if graph.has_edge(v, u, key):
             graph[v][u][key][_WEIGHT_KEY] += _WEIGHT_MULTIPLIER
 
         way_id = graph[u][v][key][_WAY_ID_KEY]
 
         way_distance = graph[u][v][key][_WEIGHT_KEY] % _WEIGHT_MULTIPLIER
 
-        new_ordering.append(
+        progress.ordering.append(
             OrderedRouteViewNode(
                 lon=u[1],
                 lat=u[0],
                 way_id=way_id,
                 path_idx=progress.path_idx,
                 n_seen_stops=n_seen_stops,
                 distance=progress.distance,
             )
         )
 
         progress.distance += way_distance
 
-    new_ordering.append(
+        last_node = v
+        last_way_id = way_id
+
+    assert last_node is not None
+    assert last_way_id is not None
+
+    progress.ordering.append(
         OrderedRouteViewNode(
-            lon=v[1],
-            lat=v[0],
-            way_id=way_id,
+            lon=last_node[1],
+            lat=last_node[0],
+            way_id=last_way_id,
             path_idx=progress.path_idx,
             n_seen_stops=n_seen_stops + 1,
             distance=progress.distance,
         )
     )
 
-    return _Traversal(
-        ordering=progress.ordering + new_ordering,
-        targets_left=progress.targets_left[1:],
-        targets_visited=progress.targets_visited + progress.targets_left[:1],
-        distance=progress.distance,
-        path_idx=progress.path_idx + 1,
-    )
+    progress.targets_visited.append(progress.targets_left.pop(0))
+    progress.path_idx += 1
 
 
 _WEIGHT_MULTIPLIER: float = 1e10
 _WEIGHT_KEY = "weight"
 _WAY_ID_KEY = "way"
```

### Comparing `aio_overpass-0.8.0/aio_overpass/ql.py` & `aio_overpass-0.9.0/aio_overpass/ql.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.8.0/aio_overpass/query.py` & `aio_overpass-0.9.0/aio_overpass/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import logging
 import math
 import os
 import re
 import sys
 import tempfile
 import time
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
-from typing import Optional, Protocol
 
 from aio_overpass.error import (
     ClientError,
     GiveupError,
     QueryLanguageError,
     QueryRejectCause,
     QueryRejectError,
@@ -33,74 +33,91 @@
     "RequestTimeout",
     "DEFAULT_MAXSIZE",
     "DEFAULT_TIMEOUT",
 )
 
 
 DEFAULT_MAXSIZE = 512
-"""Default ``maxsize`` setting in mebibytes"""
+"""Default ``maxsize`` setting in mebibytes."""
 
 DEFAULT_TIMEOUT = 180
-"""Default ``timeout`` setting in seconds"""
+"""Default ``timeout`` setting in seconds."""
 
 _COPYRIGHT = "The data included in this document is from www.openstreetmap.org. The data is made available under ODbL."  # noqa: E501
 """This is the same copyright notice included in result sets"""
 
 _SETTING_PATTERN = re.compile(r"\[(\w+?):(.+?)]\s*;?")
 """A pattern to match setting declarations (not the entire settings statement)."""
 
 
 class Query:
     """
-    State of a query that is either pending, successful, or failed.
+    State of a query that is either pending, running, successful, or failed.
 
     Args:
         input_code: The input Overpass QL code. Note that some settings might be changed
                     by query runners, notably the 'timeout' and 'maxsize' settings.
         logger: The logger to use for all logging output related to this query.
         **kwargs: Additional keyword arguments that can be used to identify queries.
 
     References:
         - https://wiki.openstreetmap.org/wiki/Overpass_API/Overpass_QL
     """
 
-    def __init__(self, input_code: str, logger: Optional[logging.Logger] = None, **kwargs) -> None:
+    __slots__ = (
+        "_error",
+        "_input_code",
+        "_kwargs",
+        "_logger",
+        "_nb_tries",
+        "_request_timeout",
+        "_response",
+        "_response_bytes",
+        "_run_timeout_secs",
+        "_settings",
+        "_time_end_try",
+        "_time_start",
+        "_time_start_req",
+        "_time_start_try",
+    )
+
+    def __init__(self, input_code: str, logger: logging.Logger | None = None, **kwargs) -> None:
         self._input_code = input_code
         self._logger = logger
         self._kwargs = kwargs
 
         self._settings = dict(_SETTING_PATTERN.findall(input_code))
 
         self._settings["out"] = "json"
 
         if "maxsize" not in self._settings:
             self._settings["maxsize"] = DEFAULT_MAXSIZE * 1024 * 1024
 
         if "timeout" not in self._settings:
             self._settings["timeout"] = DEFAULT_TIMEOUT
 
-        self._run_timeout_secs: Optional[float] = None
+        self._run_timeout_secs: float | None = None
         self._request_timeout: RequestTimeout = RequestTimeout()
 
         # set by the client that executes this query
-        self._error: Optional[ClientError] = None
-        self._response: Optional[dict] = None
+        self._error: ClientError | None = None
+        self._response: dict | None = None
         self._response_bytes = 0.0
         self._nb_tries = 0
 
-        self._time_start: Optional[_Instant] = None
+        self._time_start: _Instant | None = None
         """time prior to executing the first try"""
 
-        self._time_start_try: Optional[_Instant] = None
+        self._time_start_try: _Instant | None = None
         """time prior to executing the most recent try"""
 
-        self._time_start_req: Optional[_Instant] = None
+        self._time_start_req: _Instant | None = None
         """time prior to executing the most recent try's query request"""
 
-        self._time_end_try: Optional[_Instant] = None
+        self._time_end_try: _Instant | None = None
         """time the most recent try finished"""
 
     def reset(self) -> None:
         """Reset the query to its initial state, ignoring previous tries."""
         Query.__init__(self, input_code=self._input_code, **self._kwargs)
 
     @property
@@ -114,73 +131,87 @@
         Keyword arguments that can be used to identify queries.
 
         The default query runner will log these values when a query is run.
         """
         return self._kwargs
 
     @property
-    def logger(self) -> Optional[logging.Logger]:
+    def logger(self) -> logging.Logger | None:
         """If set, this is the logger used for logging output related to this query."""
         return self._logger
 
     @property
     def nb_tries(self) -> int:
         """Current number of tries."""
         return self._nb_tries
 
     @property
-    def error(self) -> Optional[ClientError]:
+    def error(self) -> ClientError | None:
         """
         Error of the most recent try.
 
         Returns:
             an error or ``None`` if the query wasn't tried or hasn't failed
         """
         return self._error
 
     @property
-    def response(self) -> Optional[dict]:
-        """The entire JSON response of the query."""
+    def response(self) -> dict | None:
+        """
+        The entire JSON response of the query.
+
+        Returns:
+            the response, or ``None`` if the query has not successfully finished (yet)
+        """
         return self._response
 
     @property
-    def was_cached(self) -> Optional[bool]:
+    def was_cached(self) -> bool | None:
         """
         Indicates whether the query result was cached.
 
         Returns:
             ``None`` if the query has not been run yet.
             ``True`` if the query has a result set with zero tries.
             ``False`` otherwise.
         """
         if self._response is None:
             return None
         return self._nb_tries == 0
 
     @property
-    def result_set(self) -> Optional[list[dict]]:
+    def result_set(self) -> list[dict] | None:
         """
         The result set of the query.
 
         This is open data, licensed under the Open Data Commons Open Database License (ODbL).
         You are free to copy, distribute, transmit and adapt this data, as long as you credit
         OpenStreetMap and its contributors. If you alter or build upon this data, you may
         distribute the result only under the same licence.
 
+        Returns:
+            the elements of the result set, or ``None`` if the query has not successfully
+            finished (yet)
+
         References:
             - https://www.openstreetmap.org/copyright
             - https://opendatacommons.org/licenses/odbl/1-0/
         """
         if not self._response:
             return None
         return self._response["elements"]
 
     @property
-    def response_size_mib(self) -> Optional[float]:
-        """The size of the response in mebibytes."""
+    def response_size_mib(self) -> float | None:
+        """
+        The size of the response in mebibytes.
+
+        Returns:
+            the size, or ``None`` if the query has not successfully finished (yet)
+        """
         if self._response is None:
             return None
         return self._response_bytes / 1024.0 / 1024.0
 
     @property
     def maxsize_mib(self) -> float:
         """
@@ -215,41 +246,41 @@
     def timeout_secs(self, value: int) -> None:
         if value < 1:
             msg = "timeout_secs must be >= 1"
             raise ValueError(msg)
         self._settings["timeout"] = value
 
     @property
-    def run_timeout_secs(self) -> Optional[float]:
+    def run_timeout_secs(self) -> float | None:
         """
         A limit to ``run_duration_secs``, that cancels the query when exceeded.
 
         Defaults to no timeout.
 
         The client will raise a ``QueryCancelledError`` if the timeout is reached.
 
         Not to be confused with ``timeout_secs``, which is a setting for the Overpass API instance,
         that limits the query execution time. Instead, this value can be used to limit the total
         client-side time spent on this query (see ``Client.run_query``).
         """
         return self._run_timeout_secs
 
     @run_timeout_secs.setter
-    def run_timeout_secs(self, value: Optional[float]) -> None:
+    def run_timeout_secs(self, value: float | None) -> None:
         if value is not None and value <= 0.0:
             msg = "run_timeout_secs must be > 0"
             raise ValueError(msg)
         self._run_timeout_secs = value
 
     @property
     def run_timeout_elapsed(self) -> bool:
         """Returns ``True`` if ``run_timeout_secs`` is set and has elapsed."""
         return (
-            self.run_timeout_secs
-            and self.run_duration_secs
+            self.run_timeout_secs is not None
+            and self.run_duration_secs is not None
             and self.run_timeout_secs < self.run_duration_secs
         )
 
     @property
     def request_timeout(self) -> "RequestTimeout":
         """Request timeout settings for this query."""
         return self._request_timeout
@@ -264,15 +295,15 @@
         The Overpass QL source code of this query.
 
         This is different from ``input_code`` only when it comes to settings.
         """
         return self._code(without_dynamic_settings=False)
 
     def _code(self, without_dynamic_settings: bool) -> str:
-        settings_iter = self._settings.items()
+        settings_iter = iter(self._settings.items())
 
         if without_dynamic_settings:
             settings_iter = ((k, v) for k, v in settings_iter if k not in {"maxsize", "timeout"})
 
         settings = "".join((f"[{k}:{v}]" for k, v in settings_iter)) + ";"
 
         # Remove the original settings statement
@@ -293,82 +324,94 @@
 
     @property
     def done(self) -> bool:
         """Returns ``True`` if the result set was received."""
         return self._response is not None
 
     @property
-    def request_duration_secs(self) -> Optional[float]:
+    def request_duration_secs(self) -> float | None:
         """
         How long it took to fetch the result set in seconds.
 
         This is the duration starting with the API request, and ending once
         the result is written to this query object. Although it depends on how busy
         the API instance is, this can give some indication of how long a query takes.
 
-        This is ``None`` if there is no result set yet, or when it was cached.
+        Returns:
+            the duration or ``None`` if there is no result set yet, or when it was cached.
         """
         if self._response is None or self.was_cached:
             return None
 
+        assert self._time_end_try is not None
+        assert self._time_start_req is not None
+
         return self._time_end_try - self._time_start_req
 
     @property
-    def run_duration_secs(self) -> Optional[float]:
+    def run_duration_secs(self) -> float | None:
         """
         The total required time for this query in seconds (so far).
 
-        This is ``None`` if the query has not been run yet, or when its result was cached.
+        Returns:
+            the duration or ``None`` if there is no result set yet, or when it was cached.
         """
         if self._time_start is None:
             return None
 
         if self._time_end_try:
             return self._time_end_try - self._time_start
 
         return self._time_start.elapsed_secs_since
 
     @property
-    def api_version(self) -> Optional[str]:
+    def api_version(self) -> str | None:
         """
         The Overpass API version used by the queried instance.
 
         Returns:
-            f.e. ``"Overpass API 0.7.56.8 7d656e78"``.
+            f.e. ``"Overpass API 0.7.56.8 7d656e78"``, or ``None`` if the query
+            has not successfully finished (yet)
 
         References:
             - https://wiki.openstreetmap.org/wiki/Overpass_API/versions
         """
         if self._response is None:
             return None
 
         return self._response["generator"]
 
     @property
-    def timestamp_osm(self) -> Optional[datetime]:
+    def timestamp_osm(self) -> datetime | None:
         """
         All OSM edits that have been uploaded before this date are included.
 
         It can take a couple of minutes for changes to the database to show up in the
         Overpass API query results.
+
+        Returns:
+            the timestamp, or ``None`` if the query has not successfully finished (yet)
         """
         if self._response is None:
             return None
 
         date_str = self._response["osm3s"]["timestamp_osm_base"]
         return datetime.strptime(date_str, "%Y-%m-%dT%H:%M:%SZ")
 
     @property
-    def timestamp_areas(self) -> Optional[datetime]:
+    def timestamp_areas(self) -> datetime | None:
         """
         All area data edits that have been uploaded before this date are included.
 
         If the query involves area data processing, this is the date of the latest edit
         that has been considered in the most recent batch run of the area generation.
-        Otherwise, it is set to ``None``.
+
+        Returns:
+            the timestamp, or ``None`` if the query has not successfully finished (yet), or
+            if it does not involve area data processing.
         """
         if self._response is None:
             return None
 
         date_str = self._response["osm3s"].get("timestamp_areas_base")
         if not date_str:
             return None
@@ -431,25 +474,26 @@
         return f"{cls_name}({details_str})"
 
     def _mutator(self) -> "_QueryMutator":
         return _QueryMutator(self)
 
 
 class _QueryMutator:
+    __slots__ = ("_query",)
+
     def __init__(self, query: Query) -> None:
         self._query = query
 
     def begin_try(self) -> None:
         if self._query._time_start is None:
             self._query._time_start = _Instant.now()
 
         self._query._time_start_try = _Instant.now()
         self._query._time_start_req = None
         self._query._time_end_try = None
-        self._query.try_timeout_secs = None
 
     def begin_request(self) -> None:
         self._query._time_start_req = _Instant.now()
 
     def succeed_try(self, response: dict, response_bytes: int) -> None:
         self._query._time_end_try = _Instant.now()
         self._query._response = response
@@ -459,15 +503,15 @@
     def fail_try(self, err: ClientError) -> None:
         self._query._error = err
 
     def end_try(self) -> None:
         self._query._nb_tries += 1
 
 
-@dataclass(frozen=True, repr=False, order=True)
+@dataclass(slots=True, frozen=True, repr=False, order=True)
 class _Instant:
     """
     Measurement of a monotonic clock.
 
     Attributes:
         when: the current time, according to the event loop's internal monotonic clock
               (details are unspecified and may differ per event loop).
@@ -493,15 +537,15 @@
             raise ValueError(msg)
         return self.when - earlier.when
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.when:.02f})"
 
 
-@dataclass
+@dataclass(slots=True)
 class RequestTimeout:
     """
     Request timeout settings.
 
     Attributes:
         total_without_query_secs: If set, the sum of this duration and the query's ``[timeout:*]``
                                   setting is used as timeout duration of the entire request,
@@ -510,17 +554,17 @@
                                   Defaults to 20 seconds.
         sock_connect_secs: The maximum number of seconds allowed for pure socket connection
                            establishment (same as ``aiohttp.ClientTimeout.sock_connect``).
         each_sock_read_secs: The maximum number of seconds allowed for the period between reading
                              a new chunk of data (same as ``aiohttp.ClientTimeout.sock_read``).
     """
 
-    total_without_query_secs: Optional[float] = 20.0
-    sock_connect_secs: Optional[float] = None
-    each_sock_read_secs: Optional[float] = None
+    total_without_query_secs: float | None = 20.0
+    sock_connect_secs: float | None = None
+    each_sock_read_secs: float | None = None
 
     def __post_init__(self) -> None:
         if self.total_without_query_secs is not None and self.total_without_query_secs <= 0.0:
             msg = "'total_without_query_secs' has to be > 0"
             raise ValueError(msg)
 
         if self.sock_connect_secs is not None and self.sock_connect_secs <= 0.0:
@@ -528,25 +572,31 @@
             raise ValueError(msg)
 
         if self.each_sock_read_secs is not None and self.each_sock_read_secs <= 0.0:
             msg = "'each_sock_read_secs' has to be > 0"
             raise ValueError(msg)
 
 
-class QueryRunner(Protocol):
+class QueryRunner(ABC):
     """
     A query runner is an async function that is called before a client makes an API request.
 
-    Query runners can be used to
-     - retry queries when they fail
-     - modify queries, f.e. to lower/increase their maxsize/timeout
-     - log query results & errors
-     - implement caching
+    Query runners can be used to…
+     - …retry queries when they fail
+     - …modify queries, f.e. to lower/increase their maxsize/timeout
+     - …log query results & errors
+     - …implement caching
+
+    The absolute minimum a query runner function has to do is to simply return to (re)try
+    a query, or to raise ``query.error`` to stop trying.
     """
 
+    __slots__ = ()
+
+    @abstractmethod
     async def __call__(self, query: Query) -> None:
         """Called with the current query state before the client makes an API request."""
         pass
 
 
 class DefaultQueryRunner(QueryRunner):
     """
@@ -554,24 +604,27 @@
 
     This runner…
      - …retries with an increasing back-off period in between tries if the server is too busy
      - …retries and doubles timeout and maxsize settings if they were exceeded
      - …limits the number of tries
      - …optionally caches query results in temp files
 
-    This runner does *not*…
-     - …limit the total time a query runs, including retries
-     - …lower timeout and maxsize settings if the server rejected a query
+    This runner does *not* lower timeout and maxsize settings if the server rejected a query.
 
     Args:
         max_tries: The maximum number of times a query is tried. (5 by default)
         cache_ttl_secs: Amount of seconds a query's result set is cached for.
                         Set to zero to disable caching. (zero by default)
     """
 
+    __slots__ = (
+        "_max_tries",
+        "_cache_ttl_secs",
+    )
+
     def __init__(self, max_tries: int = 5, cache_ttl_secs: int = 0) -> None:
         if max_tries < 1:
             msg = "max_tries must be >= 1"
             raise ValueError(msg)
 
         if cache_ttl_secs < 0:
             msg = "cache_ttl_secs must be >= 0"
@@ -606,18 +659,19 @@
 
         if not file_path.exists():
             logger.info("result was not cached")
             logger.debug(f"checked for cache at {file_path}")
             return
 
         try:
-            with open(file_path) as file:
+            with open(file_path, mode="r", encoding="utf-8") as file:
                 response = json.load(file)
         except (OSError, json.JSONDecodeError):
             logger.exception(f"failed to read cached {query}")
+            return
 
         if response.get(_EXPIRATION_KEY, 0) <= now:
             logger.info(f"{query} cache expired")
             return
 
         query._response = response
         logger.info(f"{query} was cached")
@@ -625,47 +679,49 @@
     def _cache_write(self, query: Query) -> None:
         logger = DefaultQueryRunner._logger(query)
 
         if not self._cache_ttl_secs or self._force_disable_caching():
             return
 
         now = int(time.time())
+
+        assert query._response is not None
         query._response[_EXPIRATION_KEY] = now + self._cache_ttl_secs
 
         file_name = f"{query.cache_key}.json"
         file_path = Path(tempfile.gettempdir()) / file_name
 
         logger.debug(f"caching at {file_path}…")
 
         try:
-            with open(file_path, "w") as file:
+            with open(file_path, mode="w", encoding="utf-8") as file:
                 json.dump(query._response, file)
         except OSError:
             logger.exception(f"failed to cache {query}")
 
     async def __call__(self, query: Query) -> None:
         """Called with the current query state before the client makes an API request."""
         logger = DefaultQueryRunner._logger(query)
 
         # Check cache ahead of first try
         if query.nb_tries == 0:
-            self._cache_read(query)
+            await asyncio.to_thread(self._cache_read, query)
 
         # Success or cached
         if query.done:
             if not query.was_cached:
-                self._cache_write(query)
+                await asyncio.to_thread(self._cache_write, query)
             return
 
         err = query.error
 
         # Do not retry if we exhausted all tries, when a retry would not change the result,
         # or when the timeout was reached.
         failed = query.nb_tries == self._max_tries or isinstance(
-            err, (ResponseError, QueryLanguageError, GiveupError)
+            err, ResponseError | QueryLanguageError | GiveupError
         )
 
         # Exhausted all tries; do not retry.
         if err and failed:
             logger.error(f"give up on {query}", exc_info=err)
             raise err
 
@@ -716,14 +772,14 @@
 
 
 def __cache_expire(query: Query) -> None:
     """Clear a response cached by the default runner (only to be used in tests)."""
     file_name = f"{query.cache_key}.json"
     file_path = Path(tempfile.gettempdir()) / file_name
 
-    with open(file_path) as file:
+    with open(file_path, mode="r", encoding="utf-8") as file:
         response = json.load(file)
 
     response[_EXPIRATION_KEY] = 0
 
-    with open(file_path, "w") as file:
+    with open(file_path, mode="w", encoding="utf-8") as file:
         json.dump(response, file)
```

### Comparing `aio_overpass-0.8.0/pyproject.toml` & `aio_overpass-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-overpass"
-version = "0.8.0"
+version = "0.9.0"
 description = "Async client for the Overpass API"
 authors = ["Tim Wiechers <mail@timwie.dev>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/timwie/aio-overpass"
 documentation = "https://www.timwie.dev/aio-overpass/"
 packages = [{ include = "aio_overpass" }]
@@ -41,101 +41,110 @@
     "License :: OSI Approved :: MIT License",
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Internet :: WWW/HTTP",
     "Typing :: Typed",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    # TODO "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/timwie/aio-overpass/blob/main/CHANGELOG.md"
 "Coverage" = "https://codecov.io/gh/timwie/aio-overpass"
 
 [tool.poetry.dependencies]
-aiohttp = "~3.8"
+aiohttp = { version = "~3.9.0b0", extras = ["speedups"] }
 joblib = { version = "~1.3", optional = true }
 networkx = { version = ">=2.7", optional = true }
-python = "^3.9"
+python = "^3.10"
 shapely = { version = "~2.0", optional = true }
 
 [tool.poetry.extras]
 joblib = ["joblib"]
 networkx = ["networkx"]
 shapely = ["shapely"]
 
 [tool.poetry.group.dev.dependencies]
 aioresponses = "^0.7.4"
-black = "^23.9.1"
+black = "^23.10.0"
 codecov = "^2.1.13"
-geojson = { version = "^3.0.1", python = "<3.12" }
+geojson = [
+    # TODO "geojson" for 3.12 - https://github.com/jazzband/geojson/issues/221
+    { version = "^3.0.1", python = "<3.12" },
+    { git = "https://github.com/jazzband/geojson.git", python = ">=3.12" },
+]
 invoke = "^2.2.0"
 isort = "^5.12.0"
-mypy = "^1.5.1"
+mypy = "^1.6.1"
 pdoc = "^14.1.0"
+pyright = "^1.1.332"
 pytest = "^7.4.2"
 pytest-asyncio = "^0.21.1"
 pytest-cov = "^4.1.0"
-ruff = "^0.0.292"
+pytest-xdist = "^3.3.1"
+ruff = "^0.1.1"
+slotscheck = "^0.17.0"
 
 [tool.poetry.group.notebooks]
 optional = true
 
 [tool.poetry.group.notebooks.dependencies]
 folium = "^0.14.0"
-jupyterlab = "^4.0.6"
+jupyterlab = "^4.0.7"
 papermill = "^2.4.0"
 randomcolor = "^0.4.4.6"
-selenium = "^4.13.0"
+selenium = "^4.14.0"
 tabulate = "^0.9.0"
 
 [tool.ruff]
 # https://github.com/charliermarsh/ruff#configuration
 # https://beta.ruff.rs/docs/rules/
 line-length = 100
-target-version = "py39"
+target-version = "py310"
 select = [
     "F", "E", "W", "N", "D", "UP",
     "ANN", "S", "B", "C4", "EM", "SIM", "ARG",
     "PL", "TRY", "PERF", "RUF"
 ]
 ignore = [
     "S101",
     "D105", "D107", "D203", "D212",
     "ANN003", "ANN101", "ANN102", "ANN401",
     "C408",
     "PLR2004", "PLW2901",
     "TRY003",
+    "UP015",
 ]
 
-# TODO can we select "FIX" with warnings instead of errors?
-#   https://github.com/astral-sh/ruff/issues/1256
-
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.black]
 # https://github.com/psf/black#configuration
 line-length = 100
 
 [tool.isort]
 # https://pycqa.github.io/isort/docs/configuration/options.html
 profile = "black"
 line_length=100
 indent='    '
 multi_line_output=6
 lines_after_imports=2
-known_first_party="aio_overpass"
+known_first_party="aio_overpass,test"
 sections="STDLIB,FIRSTPARTY,THIRDPARTY,LOCALFOLDER"
 
 [tool.mypy]
 # https://mypy.readthedocs.io/en/stable/running_mypy.html#missing-library-stubs-or-py-typed-marker
 ignore_missing_imports = true
 
+[tool.pyright]
+# https://microsoft.github.io/pyright/#/configuration
+pythonVersion = "3.10"
+verboseOutput = true
+
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.7.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aio_overpass-0.8.0/PKG-INFO` & `aio_overpass-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 Metadata-Version: 2.1
 Name: aio-overpass
-Version: 0.8.0
+Version: 0.9.0
 Summary: Async client for the Overpass API
 Home-page: https://github.com/timwie/aio-overpass
 License: MIT
 Keywords: geojson,geospatial,gis,openstreetmap,osm,overpass-api,public-transport,spatial-analysis,spatial-data,shapely
 Author: Tim Wiechers
 Author-email: mail@timwie.dev
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: aiohttp
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: joblib
 Provides-Extra: networkx
 Provides-Extra: shapely
-Requires-Dist: aiohttp (>=3.8,<3.9)
+Requires-Dist: aiohttp[speedups] (>=3.9.0b0,<3.10.0)
 Requires-Dist: joblib (>=1.3,<1.4) ; extra == "joblib"
 Requires-Dist: networkx (>=2.7) ; extra == "networkx"
 Requires-Dist: shapely (>=2.0,<2.1) ; extra == "shapely"
 Project-URL: Changelog, https://github.com/timwie/aio-overpass/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://codecov.io/gh/timwie/aio-overpass
 Project-URL: Documentation, https://www.timwie.dev/aio-overpass/
 Project-URL: Repository, https://github.com/timwie/aio-overpass
 Description-Content-Type: text/markdown
 
 A client for the [Overpass API], a read-only API that serves up custom selected
-parts of [OpenStreetMap] data. It is optimized for data consumers that need a few
-elements within a glimpse or up to roughly 10 million elements in some minutes,
-both selected by search criteria like location, type of objects, tag properties,
-proximity, or combinations of them. To make use of it, you should familiarize yourself
-with [Overpass QL], the query language used to select the elements that you want.
+parts of [OpenStreetMap] data.
+
+The Overpass API is optimized for data consumers that need a few elements within
+a glimpse or up to roughly 10 million elements in some minutes, both selected by
+search criteria like location, type of objects, tag properties, proximity, or
+combinations of them. To make use of it, you should familiarize yourself with
+[Overpass QL], the query language used to select the elements that you want.
 
 #### Contents
 - [Features](#features)
 - [Getting Started](#getting-started)
   - [Choosing Extras](#choosing-extras)
 - [Basic Usage](#basic-usage)
   - [Example](#example)
```

