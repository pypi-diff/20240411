# Comparing `tmp/pluto_rt-0.6.0.tar.gz` & `tmp/pluto_rt-0.7.0.tar.gz`

## Comparing `pluto_rt-0.6.0.tar` & `pluto_rt-0.7.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/MANIFEST.in
--rw-r--r--   0        0        0   625891 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/pluto_rt.gif
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/Dockerfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/asgi.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/compose.yaml
--rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/manage.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/requirements.txt
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/settings.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/tasks.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/urls.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/views.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/wsgi.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/templates/demo/demo_index.html
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/templates/demo/demo_list.html
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/templates/demo/demo_messages.html
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/templates/demo/demo_progress.html
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/templates/pluto_rt/list_item.html
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/templates/pluto_rt/progress_item.html
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/demo/templates/pluto_rt/toast_item.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt/apps.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt/ops.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt/urls.py
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt/views.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt/templates/pluto_rt/polling.html
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt/templates/pluto_rt/sse.html
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt/templates/pluto_rt/table.html
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt/templates/pluto_rt/table_item.html
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt.egg-info/PKG-INFO
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/src/pluto_rt.egg-info/top_level.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/tests/tests.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/.gitignore
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/LICENSE
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/README.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 pluto_rt-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/MANIFEST.in
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/Dockerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/asgi.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/compose.yaml
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/manage.py
+-rw-r--r--   0        0        0  2281154 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/pluto_rt_demo.gif
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/requirements.txt
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/settings.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/tasks.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/urls.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/views.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/wsgi.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/demo/demo_index.html
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/demo/demo_list.html
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/demo/demo_messages.html
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/demo/demo_progress.html
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/pluto_rt/list_item.html
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/pluto_rt/progress_item.html
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/demo/templates/pluto_rt/toast_item.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/apps.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/ops.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/urls.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/views.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/templates/pluto_rt/polling.html
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/templates/pluto_rt/sse.html
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/templates/pluto_rt/table.html
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt/templates/pluto_rt/table_item.html
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/src/pluto_rt.egg-info/top_level.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/tests/tests.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/.gitignore
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/README.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 pluto_rt-0.7.0/PKG-INFO
```

### Comparing `pluto_rt-0.6.0/demo/compose.yaml` & `pluto_rt-0.7.0/demo/compose.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     volumes:
       - ../src:/code
       - .:/code/demo
     depends_on:
       - cache
     ports:
       - ${ES_PORT:-8000}:8000
-    command: granian --reload --interface asgi --host 0.0.0.0 --port 8000 demo.asgi:application
+    command: granian --reload --interface asginl --host 0.0.0.0 --port 8000 demo.asgi:application
     environment:
       - REDIS_URL=redis://cache:6379/0
       - DJANGO_SETTINGS_MODULE=demo.settings
       - DEBUG=true
       - TEMPLATE_DEBUG=true
       - LOG_LEVEL=DEBUG
       - PYTHONDONTWRITEBYTECODE=1
```

### Comparing `pluto_rt-0.6.0/demo/manage.py` & `pluto_rt-0.7.0/demo/manage.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.6.0/demo/settings.py` & `pluto_rt-0.7.0/demo/settings.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.6.0/demo/tasks.py` & `pluto_rt-0.7.0/demo/tasks.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.6.0/demo/views.py` & `pluto_rt-0.7.0/demo/views.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.6.0/demo/templates/demo/demo_index.html` & `pluto_rt-0.7.0/demo/templates/demo/demo_index.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.6.0/demo/templates/demo/demo_list.html` & `pluto_rt-0.7.0/demo/templates/demo/demo_list.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.6.0/demo/templates/demo/demo_messages.html` & `pluto_rt-0.7.0/demo/templates/demo/demo_messages.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.6.0/demo/templates/demo/demo_progress.html` & `pluto_rt-0.7.0/demo/templates/demo/demo_progress.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.6.0/src/pluto_rt/urls.py` & `pluto_rt-0.7.0/src/pluto_rt/urls.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.6.0/src/pluto_rt/views.py` & `pluto_rt-0.7.0/src/pluto_rt/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,31 +16,35 @@
 
 
 async def rt_sse_content(
     request: HttpRequest, queue_name: str, item_template: str
 ) -> AsyncGenerator[str, None]:
     """Deliver event stream of formatted messages from the item template."""
     mqueue = get_rt_queue_handle(queue_name)
+    queue_index = 0
+    count = 100
 
     while True:
-        item = await sync_to_async(mqueue.pop)()
-        if not item:
+        items = await sync_to_async(mqueue.range)(queue_index, queue_index + count)
+        if not items:
             await asyncio.sleep(0.1)
             continue
-        if item == mqueue.QUEUE_EXHAUSTED:
-            yield SSE_CLOSE
-            return
-        try:
-            lines = loader.render_to_string(item_template, {"item": item}).strip().split("\n")
-            formatted_data = "\n".join(f"data: {line}" for line in lines)
-            yield f"event: message\n{formatted_data}\n\n"
-        except TemplateDoesNotExist:
-            yield "data: template not found\n\n"
-            yield SSE_CLOSE
-            return
+        queue_index += len(items)
+        for item in items:
+            if item == mqueue.QUEUE_EXHAUSTED:
+                yield SSE_CLOSE
+                return
+            try:
+                lines = loader.render_to_string(item_template, {"item": item}).strip().split("\n")
+                formatted_data = "\n".join(f"data: {line}" for line in lines)
+                yield f"event: message\n{formatted_data}\n\n"
+            except TemplateDoesNotExist:
+                yield "data: template not found\n\n"
+                yield SSE_CLOSE
+                return
 
 
 def rt_sse(request: HttpRequest, queue_name: str, item_template: str) -> HttpResponseBase:
     return StreamingHttpResponse(
         streaming_content=rt_sse_content(request, queue_name, item_template),
         content_type="text/event-stream",
     )
@@ -56,49 +60,49 @@
     this view will return http 286, which tells htmx to stop polling.
 
     Args:
         queue_name: Required queue name
         item_template: optional template file location for rendering each row item
     Query params:
         count: Optional number of messages to retrieve "per gulp"
+        index: Starting point from the queue (i.e. how many messages retrieved so far)
 
     Returns:
         Last `n` messages in the queue formatted in an html snippet (each rendered by the item_template)
     """
-    count = request.GET.get("count")
-    count = int(count) if count else 5
+    mode = request.GET.get("mode", "")
+    start = int(request.GET.get("index", 0))
+    end = start + int(request.GET.get("count", 5))
+    if mode == "replace":
+        # get the last item only
+        start = end = -1
     mqueue = get_rt_queue_handle(queue_name)
 
     items = list()
     status_code = 200
-    for _ in range(count):
-        temp_obj = mqueue.pop()
-
-        if not temp_obj:  # nothing further to get
-            break
-
+    for temp_obj in mqueue.range(start, end):
         # If sender tells us the queue is done, return 286
         # which instructs htmx to stop polling
         if temp_obj == mqueue.QUEUE_EXHAUSTED:
             status_code = 286
+            # replace always replaces innerHTML, so make sure we've got at least one item
+            if mode == "replace" and not items:
+                # only one, but we're getting a list back
+                for last_val in mqueue.range(-2, -2):
+                    items.append(last_val)
             break
 
         if temp_obj:
             items.append(temp_obj)
 
-    if not items:
-        return HttpResponse("", status=204)  # no content
+    if not items and status_code == 200:
+        return HttpResponse("", status=204)  # no content, not exhausted
 
-    match request.GET.get("mode", ""):
-        case "reverse":
-            items.reverse()
-        case "replace":
-            del items[:-1]  # last item only]
-        case _:
-            pass
+    if mode == "reverse":
+        items.reverse()
 
     try:
         body = "".join(loader.render_to_string(item_template, {"item": item}) for item in items)
     except TemplateDoesNotExist:
         body = "template not found"
         status_code = 286
     return HttpResponse(body, status=status_code)
```

### Comparing `pluto_rt-0.6.0/src/pluto_rt/templates/pluto_rt/table.html` & `pluto_rt-0.7.0/src/pluto_rt/templates/pluto_rt/table.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.6.0/src/pluto_rt.egg-info/PKG-INFO` & `pluto_rt-0.7.0/src/pluto_rt.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.6.0/README.md` & `pluto_rt-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 then the user has no insight into what the background worker is doing.
 
 Pluto-RT solves that by using Redis as a message queuing service with a FIFO (first in, first out)
 queue. Messages can be placed on the queue by the background worker and when they are retrieved by
 the view, it returns the oldest ones first. It can work either by by polling with a WSGI server,
 or by using server-sent events (SSE) with ASGI.
 
-![](pluto_rt.gif)
+![Animated gif showing pluto-rt demo functionality](demo/pluto_rt_demo.gif)
 
 The overall strategy is this:
 
 1. Create a unique "queue name" which can be sent to a worker queue and passed into a "results" page.
 1. Invoke your background processor (worker) with that queue name. The worker places messages onto the queue as it progresses with the task.
 1. Display the results template, passing it the queue name, item template name and div target. The template generates htmx which retrieves messages associated with that queue.
 1. The server removes the oldest messages from the queue and delivers them to the client.
@@ -41,15 +41,15 @@
 .venv/bin/pip install -r demo/requirements.txt
 PYTHONDONTWRITEBYTECODE=1 PYTHONUNBUFFERED=1 PYTHONPATH=.:src DJANGO_SETTINGS_MODULE=demo.settings .venv/bin/celery -A demo.tasks worker --loglevel=INFO
 ```
 
 In a new terminal run:
 
 ```
-PYTHONDONTWRITEBYTECODE=1 PYTHONUNBUFFERED=1 PYTHONPATH=.:src .venv/bin/granian --reload --interface asgi --port 8000 demo.asgi:application
+PYTHONDONTWRITEBYTECODE=1 PYTHONUNBUFFERED=1 PYTHONPATH=.:src .venv/bin/granian --reload --interface asginl --port 8000 demo.asgi:application
 ```
 
 Then open your browser to http://localhost:8000/ to view the various demos.
 
 ## Prerequisites
 
 We assume you already have these installed and working
@@ -111,15 +111,15 @@
 
 <script src="/js/htmx.min.js"></script>
 <script src="/js/htmx-sse.min.js"></script>
 ```
 
 Create an "item" template in your template dirs:
 
-1. The path (directory or filename) of the item_template _must_ contain `pluto_rt`. The format of the template is up to you! However it must not contain additional newlines: the `spaceless` template tag can be very handy for longer item templates. The object delivered in the template is named "item", and will hold whatever was added in the long-running process. It is a regular django template item at this point, but it will turn into an HTML snippet before it is delivered to the client. It could be as simple as or as complex as you want, so long as it can be delivered as mime type html/text:
+1. The path (directory or filename) of the item_template _must_ contain `pluto_rt`. The format of the template is up to you! The object delivered in the template is named "item", and will hold whatever was added in the long-running process. It is a regular django template item at this point, but it will turn into an HTML snippet before it is delivered to the client. It could be as simple as or as complex as you want, so long as it can be delivered as mime type html/text:
 
 A very simple example:
 
 ```
 <div>{{ item }}</div>
 ```
 
@@ -169,8 +169,10 @@
 
 0.3.0 Dec 14, 2023: Added reverse option, complete() function, demo app.
 
 0.4.0 Feb 21, 2024: Server-sent events, more flexible templates
 
 0.5.0 Mar 3, 2024: Improved template inclusion, added demos
 
-0.6.0 Mar 9, 2024: Use modes, add replace
+0.6.0 Mar 9, 2024: Use modes, add replace
+
+0.7.0 Apr 9, 2024: Support multiple consumers
```

### Comparing `pluto_rt-0.6.0/pyproject.toml` & `pluto_rt-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pluto_rt"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
   { name="Scot Hacker", email="shacker@energy-solution.com" },
   { name="Rob Harvey", email="rharvey@energy-solution.com" },
 ]
 description = "A reusable Django app providing a kit for storing and displaying messages from a background processor into a web view in real time, as the processor works."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `pluto_rt-0.6.0/PKG-INFO` & `pluto_rt-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pluto_rt
-Version: 0.6.0
+Version: 0.7.0
 Summary: A reusable Django app providing a kit for storing and displaying messages from a background processor into a web view in real time, as the processor works.
 Project-URL: Homepage, https://github.com/energy-solution/pluto-rt
 Author-email: Scot Hacker <shacker@energy-solution.com>, Rob Harvey <rharvey@energy-solution.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 then the user has no insight into what the background worker is doing.
 
 Pluto-RT solves that by using Redis as a message queuing service with a FIFO (first in, first out)
 queue. Messages can be placed on the queue by the background worker and when they are retrieved by
 the view, it returns the oldest ones first. It can work either by by polling with a WSGI server,
 or by using server-sent events (SSE) with ASGI.
 
-![](pluto_rt.gif)
+![Animated gif showing pluto-rt demo functionality](demo/pluto_rt_demo.gif)
 
 The overall strategy is this:
 
 1. Create a unique "queue name" which can be sent to a worker queue and passed into a "results" page.
 1. Invoke your background processor (worker) with that queue name. The worker places messages onto the queue as it progresses with the task.
 1. Display the results template, passing it the queue name, item template name and div target. The template generates htmx which retrieves messages associated with that queue.
 1. The server removes the oldest messages from the queue and delivers them to the client.
@@ -54,15 +54,15 @@
 .venv/bin/pip install -r demo/requirements.txt
 PYTHONDONTWRITEBYTECODE=1 PYTHONUNBUFFERED=1 PYTHONPATH=.:src DJANGO_SETTINGS_MODULE=demo.settings .venv/bin/celery -A demo.tasks worker --loglevel=INFO
 ```
 
 In a new terminal run:
 
 ```
-PYTHONDONTWRITEBYTECODE=1 PYTHONUNBUFFERED=1 PYTHONPATH=.:src .venv/bin/granian --reload --interface asgi --port 8000 demo.asgi:application
+PYTHONDONTWRITEBYTECODE=1 PYTHONUNBUFFERED=1 PYTHONPATH=.:src .venv/bin/granian --reload --interface asginl --port 8000 demo.asgi:application
 ```
 
 Then open your browser to http://localhost:8000/ to view the various demos.
 
 ## Prerequisites
 
 We assume you already have these installed and working
@@ -124,15 +124,15 @@
 
 <script src="/js/htmx.min.js"></script>
 <script src="/js/htmx-sse.min.js"></script>
 ```
 
 Create an "item" template in your template dirs:
 
-1. The path (directory or filename) of the item_template _must_ contain `pluto_rt`. The format of the template is up to you! However it must not contain additional newlines: the `spaceless` template tag can be very handy for longer item templates. The object delivered in the template is named "item", and will hold whatever was added in the long-running process. It is a regular django template item at this point, but it will turn into an HTML snippet before it is delivered to the client. It could be as simple as or as complex as you want, so long as it can be delivered as mime type html/text:
+1. The path (directory or filename) of the item_template _must_ contain `pluto_rt`. The format of the template is up to you! The object delivered in the template is named "item", and will hold whatever was added in the long-running process. It is a regular django template item at this point, but it will turn into an HTML snippet before it is delivered to the client. It could be as simple as or as complex as you want, so long as it can be delivered as mime type html/text:
 
 A very simple example:
 
 ```
 <div>{{ item }}</div>
 ```
 
@@ -182,8 +182,10 @@
 
 0.3.0 Dec 14, 2023: Added reverse option, complete() function, demo app.
 
 0.4.0 Feb 21, 2024: Server-sent events, more flexible templates
 
 0.5.0 Mar 3, 2024: Improved template inclusion, added demos
 
-0.6.0 Mar 9, 2024: Use modes, add replace
+0.6.0 Mar 9, 2024: Use modes, add replace
+
+0.7.0 Apr 9, 2024: Support multiple consumers
```

