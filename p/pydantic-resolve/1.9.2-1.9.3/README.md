# Comparing `tmp/pydantic_resolve-1.9.2.tar.gz` & `tmp/pydantic_resolve-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.9.2.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.9.3.tar", max compression
```

## Comparing `pydantic_resolve-1.9.2.tar` & `pydantic_resolve-1.9.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-12-14 06:50:45.409397 pydantic_resolve-1.9.2/LICENSE
--rw-r--r--   0        0        0     6865 2024-02-03 06:20:58.552638 pydantic_resolve-1.9.2/README.md
--rw-r--r--   0        0        0      742 2024-02-03 06:19:05.722638 pydantic_resolve-1.9.2/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0      363 2023-12-16 06:34:32.433696 pydantic_resolve-1.9.2/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     4317 2024-02-02 12:38:58.769790 pydantic_resolve-1.9.2/pydantic_resolve/core.py
--rw-r--r--   0        0        0      280 2024-02-02 15:20:40.489790 pydantic_resolve-1.9.2/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0    11248 2024-02-02 15:20:40.489790 pydantic_resolve-1.9.2/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0    12435 2024-02-04 03:58:04.989628 pydantic_resolve-1.9.2/pydantic_resolve/util.py
--rw-r--r--   0        0        0      765 2024-02-04 09:19:14.039628 pydantic_resolve-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     7749 1970-01-01 00:00:00.000000 pydantic_resolve-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-09-03 07:50:45.886654 pydantic_resolve-1.9.3/LICENSE
+-rw-r--r--   0        0        0     6267 2024-03-11 15:31:38.450483 pydantic_resolve-1.9.3/README.md
+-rw-r--r--   0        0        0      742 2024-02-20 13:14:31.276755 pydantic_resolve-1.9.3/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0      363 2024-01-22 11:38:04.481964 pydantic_resolve-1.9.3/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     4317 2024-01-22 11:38:04.482138 pydantic_resolve-1.9.3/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      280 2024-01-22 13:02:58.040788 pydantic_resolve-1.9.3/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0    11931 2024-03-07 15:14:42.661415 pydantic_resolve-1.9.3/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0    12433 2024-03-07 13:53:54.988565 pydantic_resolve-1.9.3/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      849 2024-03-12 12:14:33.745121 pydantic_resolve-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0     7100 1970-01-01 00:00:00.000000 pydantic_resolve-1.9.3/PKG-INFO
```

### Comparing `pydantic_resolve-1.9.2/LICENSE` & `pydantic_resolve-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.9.2/README.md` & `pydantic_resolve-1.9.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,216 +1,258 @@
+Metadata-Version: 2.1
+Name: pydantic-resolve
+Version: 1.9.3
+Summary: create nested data structure easily
+Home-page: https://github.com/allmonday/pydantic_resolve
+License: MIT
+Keywords: pydantic,fastapi
+Author: tangkikodo
+Author-email: allmonday@126.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiodataloader (>=0.4.0,<0.5.0)
+Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Project-URL: Repository, https://github.com/allmonday/pydantic_resolve
+Description-Content-Type: text/markdown
+
 [![pypi](https://img.shields.io/pypi/v/pydantic-resolve.svg)](https://pypi.python.org/pypi/pydantic-resolve)
 [![Downloads](https://static.pepy.tech/personalized-badge/pydantic-resolve?period=month&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pydantic-resolve)
 ![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
 ![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
 [![CI](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml/badge.svg)](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml)
 
 ![img](doc/imgs/resolver.png)
 
-**If you are using pydantic v2, please use pydantic2-resolve instead.**
+A hierarchical solution for data fetching and processing
 
-A small yet powerful tool to extend your pydantic schema, and then resolve all **descendants** automatically.
+1. use declaretive way to define view data, easy to maintain and develop
+2. use main query and loader query to break down complex queries, and better reuse
+3. provide various tools to precisely construct view data, no overhead
 
-It's also the key to the realm of composition-oriented-development-pattern (wip)
 
-> What is composable pattarn? https://github.com/allmonday/composable-development-pattern
+> If you are using pydantic v2, please use [pydantic2-resolve](https://github.com/allmonday/pydantic2-resolve) instead.
 
-[Change Logs](./changelog.md)
+> It is the key to composition-oriented-development-pattern (wip) 
+> https://github.com/allmonday/composition-oriented-development-pattern
 
-[discord](https://discord.com/channels/1197929379951558797/1197929379951558800)
+[Discord](https://discord.com/channels/1197929379951558797/1197929379951558800)
+
+[Change Logs](./changelog.md)
 
 ## Install
 
 ```shell
 pip install pydantic-resolve
 ```
 
-## Code snippets
+## Concept
+
+It taks 5 steps to convert from root data into view data.
+
+1. define schema of root data and descdants & load root data
+2. forward-resolve all descdants data
+3. backward-process the data
+4. tree shake the data marked as exclude=True
+5. get the output
+
+![](./doc/imgs/concept.jpeg)
+
+How resolve works, level by level:
+
+![](./doc/imgs/forward.jpeg)
+
+
+## Quick start
+
+Basic usage, resolve your fields.  (`N+1` query will happens in batch scenario)
+
+Let's build a blog site with blogs and comments.
 
-1. basic usage, resolve your fields.
+[0_demo.py](./examples/0_demo.py)
 
 ```python
 import asyncio
 from pydantic import BaseModel
 from pydantic_resolve import Resolver
 
-async def query_age(name):
-    print(f'query {name}')
-    await asyncio.sleep(1)
-    _map = {
-        'kikodo': 21,
-        'John': 14,
-        '老王': 40,
-    }
-    return _map.get(name)
+comments_table = [
+    dict(id=1, blog_id=1, content='its interesting'),
+    dict(id=2, blog_id=1, content='i dont understand'),
+    dict(id=3, blog_id=2, content='why? how?'),
+    dict(id=4, blog_id=2, content='wow!')]
+
+async def query_comments(blog_id: int):
+    print(f'run query - {blog_id}')
+    return [c for c in comments_table if c['blog_id'] == blog_id]
+
+async def get_blogs():
+    return [
+        dict(id=1, title='what is pydantic-resolve'),
+        dict(id=2, title='what is composition oriented development pattarn'),
+    ]
+
+class Comment(BaseModel):
+    id: int
+    content: str
+
+class Blog(BaseModel):
+    id: int
+    title: str
+
+    comments: list[Comment] = []
+    async def resolve_comments(self):
+        return await query_comments(self.id)
+
+    comment_count: int = 0
+    def post_comment_count(self):
+        return len(self.comments)
 
-class Person(BaseModel):
+
+class MyBlogSite(BaseModel):
     name: str
 
-    age: int = 0
-    async def resolve_age(self):
-        return await query_age(self.name)
-
-    is_adult: bool = False
-    def post_is_adult(self):
-        return self.age > 18
-
-async def simple():
-    p = Person(name='kikodo')
-    p = await Resolver().resolve(p)
-    print(p)
-    # query kikodo
-    # Person(name='kikodo', age=21, is_adult=True)
-
-    people = [Person(name=n) for n in ['kikodo', 'John', '老王']]
-    people = await Resolver().resolve(people)
-    print(people)
-    # Oops!! the issue of N+1 query happens
-    # query kikodo
-    # query John
-    # query 老王
-    # [Person(name='kikodo', age=21, is_adult=True), Person(name='John', age=14, is_adult=False), Person(name='老王', age=40, is_adult=True)]
+    blogs: list[Blog] = []
+    async def resolve_blogs(self):
+        return await get_blogs()
+
+    comment_count: int = 0
+    def post_comment_count(self):
+        return sum([b.comment_count for b in self.blogs])
+
+async def single():
+    blog = Blog(id=1, title='what is pydantic-resolve')
+    blog = await Resolver().resolve(blog)
+    print(blog)
+
+async def batch():
+    my_blog_site = MyBlogSite(name: "tangkikodo's blog")
+    my_blog_site = await Resolver().resolve(my_blog_site)
+    print(my_blog_site.json(indent=4))
+
+
+async def main():
+    await single()
+    # query_comments():
+    # >> run query - 1
+
+    await batch()
+    # query_comments(): Ooops!, N+1 happens
+    # >> run query - 1
+    # >> run query - 2
+
+asyncio.run(main())
+```
 
-asyncio.run(simple())
+output of my_blog_site:
+```json
+{
+    "name": "tangkikodo's blog",
+    "blogs": [
+        {
+            "id": 1,
+            "title": "what is pydantic-resolve",
+            "comments": [
+                {
+                    "id": 1,
+                    "content": "its interesting"
+                },
+                {
+                    "id": 2,
+                    "content": "i dont understand"
+                }
+            ]
+        },
+        {
+            "id": 2,
+            "title": "what is composition oriented development pattarn",
+            "comments": [
+                {
+                    "id": 3,
+                    "content": "why? how?"
+                },
+                {
+                    "id": 4,
+                    "content": "wow!"
+                }
+            ]
+        }
+    ]
+}
 ```
 
-2. optimize `N+1` with dataloader
+Optimize `N+1` with dataloader
+
+[0_demo_loader.py](./examples/0_demo_loader.py)
+
+- change `query_comments` to `blog_to_comments_loader` (loader function)
+- user loader in `resolve_comments`
 
 ```python
-import asyncio
-from typing import List
-from pydantic import BaseModel
-from pydantic_resolve import Resolver, LoaderDepend as LD
+from pydantic_resolve import LoaderDepend
 
-async def batch_person_age_loader(names: List[str]):
-    print(names)
-    _map = {
-        'kikodo': 21,
-        'John': 14,
-        '老王': 40,
-    }
-    return [_map.get(n) for n in names]
+async def blog_to_comments_loader(blog_ids: list[int]):
+    print(blog_ids)
+    return build_list(comments_table, blog_ids, lambda c: c['blog_id'])
 
-class Person(BaseModel):
-    name: str
+class Blog(BaseModel):
+    id: int
+    title: str
 
-    age: int = 0
-    def resolve_age(self, loader=LD(batch_person_age_loader)):
-        return loader.load(self.name)
+    comments: list[Comment] = []
+    def resolve_comments(self, loader=LoaderDepend(blog_to_comments_loader)):
+        return loader.load(self.id)
 
-    is_adult: bool = False
-    def post_is_adult(self):
-        return self.age > 18
+    comment_count: int = 0
+    def post_comment_count(self):
+        return len(self.comments)
 
-async def simple():
-    people = [Person(name=n) for n in ['kikodo', 'John', '老王']]
-    people = await Resolver().resolve(people)
-    print(people)
 
-    # query query kikodo,John,老王 (N+1 query fixed)
-    # [Person(name='kikodo', age=21, is_adult=True), Person(name='John', age=14, is_adult=False), Person(name='老王', age=40, is_adult=True)]
+# run main again
+async def main():
+    await batch()
+    # blog_to_comments_loader():
+    # >> [1, 2]
+    # N+1 fixed
 
-asyncio.run(simple())
+asyncio.run(main())
 ```
 
-## More examples:
+## Simple demo:
+
+[Introduction](./examples/readme_demo/readme.md)
 
 ```shell
 cd examples
 
 python -m readme_demo.0_basic
 python -m readme_demo.1_filter
 python -m readme_demo.2_post_methods
 python -m readme_demo.3_context
 python -m readme_demo.4_loader_instance
 python -m readme_demo.5_subset
 python -m readme_demo.6_mapper
 python -m readme_demo.7_single
 ```
 
-## API
-
-### Resolver(loader_filters, global_loader_filter, loader_instances, context)
-
-- loader_filters: `dict`
-
-  provide extra query filters along with loader key.
-
-  reference: [6_sqlalchemy_loaderdepend_global_filter.py](examples/6_sqlalchemy_loaderdepend_global_filter.py) L55, L59
 
-- global_loader_filter: `dict`
+## Advanced demo:
 
-  provide global filter config for all dataloader instances
+https://github.com/allmonday/composition-oriented-development-pattern
 
-  it will raise exception if some fields are duplicated with specific loader filter config in `loader_filters`
 
-  reference: [test_33_global_loader_filter.py](tests/resolver/test_33_global_loader_filter.py) L47, L49
+## API Reference
 
-- loader_instances: `dict`
+https://allmonday.github.io/pydantic-resolve/reference_api/
 
-  provide pre-created loader instance, with can `prime` data into loader cache.
-
-  reference: [test_20_loader_instance.py](tests/resolver/test_20_loader_instance.py), L62, L63
-
-- context: `dict`
-
-  context can carry setting into each single resolver methods.
-
-  ```python
-  class Earth(BaseModel):
-      humans: List[Human] = []
-      def resolve_humans(self, context):
-          return [dict(name=f'man-{i}') for i in range(context['count'])]
-
-  earth = await Resolver(context={'count': 10}).resolve(earth)
-  ```
-
-### LoaderDepend(loader_fn)
-
-- loader_fn: `subclass of DataLoader or batch_load_fn`. [detail](https://github.com/syrusakbary/aiodataloader#dataloaderbatch_load_fn-options)
-
-  declare dataloader dependency, `pydantic-resolve` will take the care of lifecycle of dataloader.
-
-### build_list(rows, keys, fn), build_object(rows, keys, fn)
-
-- rows: `list`, query result
-- keys: `list`, batch_load_fn:keys
-- fn: `lambda`, define the way to get primary key
-
-  helper function to generate return value required by `batch_load_fn`. read the code for details.
-
-  reference: [test_utils.py](tests/utils/test_utils.py), L32
-
-### mapper(param)
-
-- param: `class of pydantic or dataclass, or a lambda`
-
-  `pydantic-resolve` will trigger the fn in `mapper` after inner future is resolved. it exposes an interface to change return schema even from the same dataloader.
-  if param is a class, it will try to automatically transform it.
-
-  reference: [test_16_mapper.py](tests/resolver/test_16_mapper.py)
-
-  > you may need it if there has some reuseable transforming params.
-
-### ensure_subset(target_model)
-
-- target_model: `class`
-
-  it will raise exception if fields of decorated class has field not existed in `base_class`.
-
-  this provide a validation to ensure your schema's field is a subset of targe schema.
-
-  reference: [test_2_ensure_subset.py](tests/utils/test_2_ensure_subset.py)
-
-### model_config(hidden_fields: list[str], default_required: bool) (new in v1.9.1)
-
-- hidden_fields: list the field names you don't want to expose.
-- default_required: if True, fields with default values will also in schema['required']
-
-  reference: [test_schema_config.py](tests/utils/test_schema_config.py)
 
 ## Run FastAPI example
 
 ```shell
 poetry shell
 cd examples
 uvicorn fastapi_demo.main:app
@@ -227,7 +269,8 @@
 
 ## Coverage
 
 ```shell
 poetry run coverage run -m pytest
 poetry run coverage report -m
 ```
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydantic_resolve-1.9.2/pydantic_resolve/__init__.py` & `pydantic_resolve-1.9.3/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.9.2/pydantic_resolve/core.py` & `pydantic_resolve-1.9.3/pydantic_resolve/core.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.9.2/pydantic_resolve/resolver.py` & `pydantic_resolve-1.9.3/pydantic_resolve/resolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 from collections import defaultdict
 import contextvars
 import inspect
+import warnings
 from inspect import iscoroutine
 from typing import TypeVar, Dict
 from .exceptions import ResolverTargetAttrNotFound, LoaderFieldNotProvidedError, MissingAnnotationError
 from .util import get_kls_full_path
 from typing import Any, Callable, Optional
 from pydantic_resolve import core
 from aiodataloader import DataLoader
@@ -31,30 +32,40 @@
 
 class Resolver:
     """
     Entrypoint of a resolve action
     """
     def __init__(
             self,
-            loader_filters: Optional[Dict[Any, Dict[str, Any]]] = None,
-            global_loader_filter: Optional[Dict[str, Any]] = None,
+            loader_filters: Optional[Dict[Any, Dict[str, Any]]] = None,  # deprecated
+            loader_params: Optional[Dict[Any, Dict[str, Any]]] = None,
+            global_loader_filter: Optional[Dict[str, Any]] = None,  # deprecated
+            global_loader_param: Optional[Dict[str, Any]] = None,
             loader_instances: Optional[Dict[Any, Any]] = None,
             ensure_type=False,
             context: Optional[Dict[str, Any]] = None):
         self.loader_instance_cache = {}
 
         self.ancestor_vars = {}
         self.ancestor_vars_checker = defaultdict(set)  # expose_field_name: set(kls fullpath) if len > 1, raise error
 
         # for dataloader which has class attributes, you can assign the value at here
-        self.loader_filters = loader_filters or {}
+        if loader_filters:
+            warnings.warn('loader_filters is deprecated, use loader_params instead.', DeprecationWarning)
+            self.loader_params = loader_filters
+        else:
+            self.loader_params = loader_params or {}
 
         # keys in global_loader_filter are mutually exclusive with key-value pairs in loader_filters
         # eg: Resolver(global_loader_filter={'key_a': 1}, loader_filters={'key_a': 1}) will raise exception
-        self.global_loader_filter = global_loader_filter or {}
+        if global_loader_filter:
+            warnings.warn('global_loader_filter is deprecated, use global_loader_param instead.', DeprecationWarning)
+            self.global_loader_param = global_loader_filter or {}
+        else:
+            self.global_loader_param = global_loader_param or {}
 
         # now you can pass your loader instance, Resolver will check `isinstance``
         if loader_instances and self._validate_loader_instance(loader_instances):
             self.loader_instances = loader_instances
         else:
             self.loader_instances = None
 
@@ -106,15 +117,15 @@
         return True
 
     def _execute_resolver_method(self, method):
         """
         1. inspect method, atttach context if declared in method
         2. if params includes LoaderDepend, create instance and cache it.
             2.1 create from DataLoader class
-                2.1.1 apply loader_filters into dataloader instance
+                2.1.1 apply loader_params into dataloader instance
             2.2 ceate from batch_load_fn
         3. execute method
         """
 
         # >>> 1
         signature = inspect.signature(method)
         params = {}
@@ -150,30 +161,30 @@
                 else:
                     # >>> 2.1
                     # create loader instance 
                     if isclass(Loader):
                         # if extra transform provides
                         loader = Loader()
 
-                        filter_config = util.merge_dicts(
-                            self.global_loader_filter,
-                            self.loader_filters.get(Loader, {}))
+                        param_config = util.merge_dicts(
+                            self.global_loader_param,
+                            self.loader_params.get(Loader, {}))
 
                         for field in util.get_class_field_annotations(Loader):
-                        # >>> 2.1.1
-                        # class ExampleLoader(DataLoader):
-                        #     filtar_x: bool  <--------------- set this field
+                            # >>> 2.1.1
+                            # class ExampleLoader(DataLoader):
+                            #     param_a: bool  <-- set this field
                             try:
-                                value = filter_config[field]
+                                value = param_config[field]
                                 setattr(loader, field, value)
                             except KeyError:
                                 raise LoaderFieldNotProvidedError(f'{cache_key}.{field} not found in Resolver()')
 
                     # >>> 2.2
-                    # build loader from batch_load_fn, filters config is impossible
+                    # build loader from batch_load_fn, params config is impossible
                     else:
                         loader = DataLoader(batch_load_fn=Loader)  # type:ignore
 
                     self.loader_instance_cache[cache_key] = loader
                 params[k] = loader
 
         # 3
@@ -188,15 +199,16 @@
                 raise AttributeError('Post.context is missing')
             params['context'] = self.context
 
         if signature.parameters.get('ancestor_context'):
             if self.ancestor_vars is None:
                 raise AttributeError(f'there is not class has {const.EXPOSE_TO_DESCENDANT} configed')
             params['ancestor_context'] = self._build_ancestor_context()
-        return method(**params)
+        ret_val = method(**params)
+        return ret_val
 
     async def _resolve_obj_field(self, target, target_field, attr):
         """
         resolve each single object field
 
         1. validate the target field of resolver method existed.
         2. exec methods
@@ -218,14 +230,15 @@
         val = self._execute_resolver_method(attr)
         while iscoroutine(val) or asyncio.isfuture(val):
             val = await val
 
         # >>> 3
         if not getattr(attr, const.HAS_MAPPER_FUNCTION, False):  # defined in util.mapper
             val = util.try_parse_data_to_target_field_type(target, target_attr_name, val)
+            # else: it will be handled by mapper func
 
         val = await self._resolve(val)
 
         # >>> 4
         setattr(target, target_attr_name, val)
 
     async def _resolve(self, target: T) -> T:
```

### Comparing `pydantic_resolve-1.9.2/pydantic_resolve/util.py` & `pydantic_resolve-1.9.3/pydantic_resolve/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 T = TypeVar("T")
 V = TypeVar("V")
 
 def merge_dicts(a: Dict[str, Any], b: Dict[str, Any]):
     overlap = set(a.keys()) & set(b.keys())
     if overlap:
-        raise GlobalLoaderFieldOverlappedError(f'loader_filters and global_loader_filter have duplicated key(s): {",".join(overlap)}')
+        raise GlobalLoaderFieldOverlappedError(f'loader_params and global_loader_param have duplicated key(s): {",".join(overlap)}')
     else:
         return {**a, **b}
 
 def build_object(items: Sequence[T], keys: List[V], get_pk: Callable[[T], V]) -> Iterator[Optional[T]]:
     """
     helper function to build return object data required by aiodataloader
     """
```

### Comparing `pydantic_resolve-1.9.2/pyproject.toml` & `pydantic_resolve-1.9.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.9.2"
+version = "1.9.3"
 description = "create nested data structure easily"
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
@@ -20,11 +20,17 @@
 pytest-cov = "^4.0.0"
 coverage = "^7.2.1"
 aiosqlite = "^0.18.0"
 sqlalchemy = {extras = ["asyncio"], version = "^2.0.7"}
 pytest-asyncio = "^0.21.0"
 fastapi = "^0.96.0"
 uvicorn = "^0.22.0"
+mkdocs-material = "9.*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+filterwarnings = [
+    "error",
+]
```

