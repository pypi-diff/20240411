# Comparing `tmp/bigdata_client-0.0.4.tar.gz` & `tmp/bigdata_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigdata_client-0.0.4.tar", max compression
+gzip compressed data, was "bigdata_client-0.0.5.tar", max compression
```

## Comparing `bigdata_client-0.0.4.tar` & `bigdata_client-0.0.5.tar`

### file list

```diff
@@ -1,45 +1,49 @@
--rw-r--r--   0        0        0      761 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/README.md
--rw-r--r--   0        0        0      155 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/api/__init__.py
--rw-r--r--   0        0        0     7747 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/api/search.py
--rw-r--r--   0        0        0     2880 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/auth.py
--rw-r--r--   0        0        0        0 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/clerk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/clerk/authenticators/__init__.py
--rw-r--r--   0        0        0     2256 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/clerk/authenticators/base_instance.py
--rw-r--r--   0        0        0     4166 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/clerk/authenticators/dev_instance.py
--rw-r--r--   0        0        0     3650 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/clerk/authenticators/production_instance.py
--rw-r--r--   0        0        0      853 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/clerk/exceptions.py
--rw-r--r--   0        0        0      245 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/clerk/models.py
--rw-r--r--   0        0        0        0 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/clerk/sign_in_strategies/__init__.py
--rw-r--r--   0        0        0      243 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/clerk/sign_in_strategies/base.py
--rw-r--r--   0        0        0     1008 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/clerk/sign_in_strategies/password.py
--rw-r--r--   0        0        0     2510 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/clerk/token_manager.py
--rw-r--r--   0        0        0     2040 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/clerk/token_manager_factory.py
--rw-r--r--   0        0        0     4550 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/connection.py
--rw-r--r--   0        0        0      154 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/constants.py
--rw-r--r--   0        0        0     2352 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/daterange.py
--rw-r--r--   0        0        0     1234 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/entity_types.py
--rw-r--r--   0        0        0      664 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/enum_utils.py
--rw-r--r--   0        0        0       82 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/errors.py
--rw-r--r--   0        0        0      513 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/jwt.py
--rw-r--r--   0        0        0        0 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/models/__init__.py
--rw-r--r--   0        0        0     1181 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/models/comentions.py
--rw-r--r--   0        0        0     4797 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/models/entities.py
--rw-r--r--   0        0        0      326 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/models/languages.py
--rw-r--r--   0        0        0     2925 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/models/parse.py
--rw-r--r--   0        0        0     1920 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/models/search.py
--rw-r--r--   0        0        0      694 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/models/sources.py
--rw-r--r--   0        0        0      872 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/models/story.py
--rw-r--r--   0        0        0      735 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/models/topics.py
--rw-r--r--   0        0        0     1390 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/models/uploads.py
--rw-r--r--   0        0        0      329 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/models/watchlists.py
--rw-r--r--   0        0        0     4633 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/old_auth.py
--rw-r--r--   0        0        0      251 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/query_type.py
--rw-r--r--   0        0        0     7068 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/search.py
--rw-r--r--   0        0        0     6879 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/services.py
--rw-r--r--   0        0        0      839 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/settings.py
--rw-r--r--   0        0        0    12020 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/simple_search_query.py
--rw-r--r--   0        0        0     1893 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/story.py
--rw-r--r--   0        0        0      465 2024-03-22 18:09:40.716759 bigdata_client-0.0.4/bigdata/user_agent.py
--rw-r--r--   0        0        0     1410 2024-03-22 18:09:40.720759 bigdata_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 bigdata_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      358 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/README.md
+-rw-r--r--   0        0        0      155 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/__init__.py
+-rw-r--r--   0        0        0     6526 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/advanced_search_query.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/api/__init__.py
+-rw-r--r--   0        0        0     1045 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/api/autosuggest.py
+-rw-r--r--   0        0        0     8160 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/api/search.py
+-rw-r--r--   0        0        0     6237 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/auth.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/clerk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/clerk/authenticators/__init__.py
+-rw-r--r--   0        0        0     2256 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/clerk/authenticators/base_instance.py
+-rw-r--r--   0        0        0     4166 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/clerk/authenticators/dev_instance.py
+-rw-r--r--   0        0        0     3650 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/clerk/authenticators/production_instance.py
+-rw-r--r--   0        0        0      853 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/clerk/exceptions.py
+-rw-r--r--   0        0        0      245 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/clerk/models.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/clerk/sign_in_strategies/__init__.py
+-rw-r--r--   0        0        0      243 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/clerk/sign_in_strategies/base.py
+-rw-r--r--   0        0        0     1008 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/clerk/sign_in_strategies/password.py
+-rw-r--r--   0        0        0     2510 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/clerk/token_manager.py
+-rw-r--r--   0        0        0     2040 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/clerk/token_manager_factory.py
+-rw-r--r--   0        0        0     6778 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/connection.py
+-rw-r--r--   0        0        0      154 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/constants.py
+-rw-r--r--   0        0        0     3626 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/daterange.py
+-rw-r--r--   0        0        0     1234 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/entity_types.py
+-rw-r--r--   0        0        0      664 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/enum_utils.py
+-rw-r--r--   0        0        0       82 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/errors.py
+-rw-r--r--   0        0        0      513 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/jwt.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/models/__init__.py
+-rw-r--r--   0        0        0    21160 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/models/advanced_search_query.py
+-rw-r--r--   0        0        0     1181 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/models/comentions.py
+-rw-r--r--   0        0        0     5988 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/models/entities.py
+-rw-r--r--   0        0        0     1094 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/models/languages.py
+-rw-r--r--   0        0        0     3443 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/models/parse.py
+-rw-r--r--   0        0        0     1710 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/models/search.py
+-rw-r--r--   0        0        0     2280 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/models/sources.py
+-rw-r--r--   0        0        0      978 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/models/story.py
+-rw-r--r--   0        0        0     2180 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/models/topics.py
+-rw-r--r--   0        0        0     1390 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/models/uploads.py
+-rw-r--r--   0        0        0     1084 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/models/watchlists.py
+-rw-r--r--   0        0        0     4633 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/old_auth.py
+-rw-r--r--   0        0        0      970 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/query.py
+-rw-r--r--   0        0        0      251 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/query_type.py
+-rw-r--r--   0        0        0     7873 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/search.py
+-rw-r--r--   0        0        0     9021 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/services.py
+-rw-r--r--   0        0        0     1020 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/settings.py
+-rw-r--r--   0        0        0    12157 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/simple_search_query.py
+-rw-r--r--   0        0        0     2022 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/story.py
+-rw-r--r--   0        0        0      465 2024-04-11 14:42:10.293227 bigdata_client-0.0.5/bigdata/user_agent.py
+-rw-r--r--   0        0        0     1429 2024-04-11 14:42:10.297227 bigdata_client-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 bigdata_client-0.0.5/PKG-INFO
```

### Comparing `bigdata_client-0.0.4/bigdata/api/search.py` & `bigdata_client-0.0.5/bigdata/api/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,27 +29,30 @@
     SearchPagination,
     SortBy,
 )
 from bigdata.models.sources import Source
 from bigdata.models.story import StoryType
 from bigdata.models.topics import Topic
 from bigdata.query_type import QueryType
+from bigdata.settings import settings
 
 # Save a search
 
 
 class SaveSearchQueryRequest(BaseModel):
     """Model to represent the "query" attribute of a request to save a search"""
 
     expression: Expression
     scope: FileType = Field(default=FileType.ALL)
     sort: SortBy = Field(default=SortBy.RELEVANCE)
-    ranking: Ranking = Field(default=Ranking.STABLE)
+    ranking: Ranking = Field(default=settings.LLM.RANKING)
     search_chain: Optional[SearchChain] = Field(alias="searchChain", default=None)
-    hybrid: bool = False
+    hybrid: bool = settings.LLM.USE_HYBRID
+    # The date expression neds a type=ExpressionTypes.DATE
+    # the value is coming from date_range.to_expression()
     date: Optional[list[Expression]] = None
 
 
 class SaveSearchRequest(BaseModel):
     """Model to represent the request to create a search"""
 
     name: str
@@ -72,17 +75,17 @@
     Model to represent the "query" attribute of a response from getting a saved
     search.
     """
 
     expression: Expression
     scope: FileType = Field(default=FileType.ALL)
     sort: SortBy = Field(default=SortBy.RELEVANCE)
-    ranking: Ranking = Field(default=Ranking.STABLE)
+    ranking: Ranking = Field(default=settings.LLM.RANKING)
     search_chain: Optional[SearchChain] = Field(alias="searchChain", default=None)
-    hybrid: bool = False
+    hybrid: bool = settings.LLM.USE_HYBRID
     date: Optional[list[Expression]] = None
 
 
 class SavedSearchResponse(BaseModel):
     """Model to represent the response from getting a saved search"""
 
     id: str
@@ -124,34 +127,34 @@
 
 class QueryClustersRequest(BaseModel):
     """Model to represent a request to run a search"""
 
     expression: Expression
     scope: FileType = Field(default=FileType.ALL)
     sort: SortBy = Field(default=SortBy.RELEVANCE)
-    ranking: Ranking = Field(default=Ranking.STABLE)
+    ranking: Ranking = Field(default=settings.LLM.RANKING)
     pagination: SearchPagination = Field(
         default=SearchPagination(limit=SEARCH_PAGE_SIZE, cursor=1)
     )
     search_chain: Optional[SearchChain] = Field(alias="searchChain", default=None)
-    hybrid: bool = False
+    hybrid: bool = settings.LLM.USE_HYBRID
 
 
 class QueryChunksRequest(BaseModel):
     """Model to represent a request to run a search"""
 
     expression: Expression
     scope: FileType = Field(default=FileType.ALL)
     sort: SortBy = Field(default=SortBy.RELEVANCE)
-    ranking: Ranking = Field(default=Ranking.STABLE)
+    ranking: Ranking = Field(default=settings.LLM.RANKING)
     pagination: SearchPagination = Field(
         default=SearchPagination(limit=SEARCH_PAGE_SIZE, cursor=1)
     )
     search_chain: Optional[SearchChain] = Field(alias="searchChain", default=None)
-    hybrid: bool = False
+    hybrid: bool = settings.LLM.USE_HYBRID
 
 
 class ClusteredStoryResponse(BaseModel):
     """
     Helper class to parse the response from the API.
     It should be used only internally to parse the JSON response from the API,
     and not passed around.
@@ -210,15 +213,21 @@
             key: str
             start: int
             end: int
             queryType: QueryType
 
         entities: list[StoryResponseEntity]
 
-    sentences: list[ChunkedStoryResponseSentence]
+        class StoryResponseSentence(BaseModel):
+            pnum: int
+            snum: int
+
+        sentences: list[StoryResponseSentence]
+
+    chunks: list[ChunkedStoryResponseSentence]
 
 
 class QueryClustersResponse(BaseModel):
     """Model to represent the response from running a search"""
 
     count: int
     document_count: int = Field(alias="documentCount")
@@ -244,17 +253,17 @@
 
 class DiscoveryPanelRequest(BaseModel):
     """Model to represent a request to get comentions"""
 
     expression: Expression
     scope: FileType = Field(default=FileType.ALL)
     sort: SortBy = Field(default=SortBy.RELEVANCE)
-    ranking: Ranking = Field(default=Ranking.STABLE)
+    ranking: Ranking = Field(default=settings.LLM.RANKING)
     search_chain: Optional[SearchChain] = Field(alias="searchChain", default=None)
-    hybrid: bool = False
+    hybrid: bool = settings.LLM.USE_HYBRID
 
 
 class DiscoveryPanelResponse(BaseModel):
     """Model to represent the response from getting comentions"""
 
     companies: list[Company]
     concepts: list[Concept]
```

### Comparing `bigdata_client-0.0.4/bigdata/clerk/authenticators/base_instance.py` & `bigdata_client-0.0.5/bigdata/clerk/authenticators/base_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/clerk/authenticators/dev_instance.py` & `bigdata_client-0.0.5/bigdata/clerk/authenticators/dev_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/clerk/authenticators/production_instance.py` & `bigdata_client-0.0.5/bigdata/clerk/authenticators/production_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/clerk/exceptions.py` & `bigdata_client-0.0.5/bigdata/clerk/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/clerk/sign_in_strategies/password.py` & `bigdata_client-0.0.5/bigdata/clerk/sign_in_strategies/password.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/clerk/token_manager.py` & `bigdata_client-0.0.5/bigdata/clerk/token_manager.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/clerk/token_manager_factory.py` & `bigdata_client-0.0.5/bigdata/clerk/token_manager_factory.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/entity_types.py` & `bigdata_client-0.0.5/bigdata/entity_types.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/enum_utils.py` & `bigdata_client-0.0.5/bigdata/enum_utils.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/jwt.py` & `bigdata_client-0.0.5/bigdata/jwt.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/models/comentions.py` & `bigdata_client-0.0.5/bigdata/models/comentions.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/models/parse.py` & `bigdata_client-0.0.5/bigdata/models/parse.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,74 @@
-from typing import Annotated, Any, Optional, Union
+from typing import Annotated, Any, Literal, Optional, Union
 
-from pydantic import BaseModel, Discriminator, Tag, ValidationError
+from pydantic import BaseModel, ConfigDict, Discriminator, Field, Tag, ValidationError
 
 from bigdata.models.entities import (
     Company,
     Concept,
     Facility,
     Landmark,
+    MacroEntity,
     Organization,
     OrganizationType,
     Person,
     Place,
     Product,
     ProductType,
 )
 from bigdata.models.languages import Language
-from bigdata.models.search import AutosuggestedSearch
 from bigdata.models.sources import Source
 from bigdata.models.topics import Topic
 from bigdata.models.watchlists import Watchlist
 
 
-def get_discriminator_domain_value(v: Any) -> Optional[str]:
+def get_discriminator_knowledge_graph_value(v: Any) -> Optional[str]:
     if isinstance(v, dict):
         return v.get(
             "entityType", v.get("entity_type", v.get("queryType", v.get("query_type")))
         )
     return getattr(v, "entity_type", getattr(v, "query_type", None))
 
 
+class AutosuggestedSavedSearch(BaseModel):
+    """Class used only to parse the output from the Autosuggestion"""
+
+    model_config = ConfigDict(populate_by_name=True)
+    id: Optional[str] = Field(validation_alias="key", default=None)
+    name: Optional[str] = Field(default=None)
+    query_type: Literal["savedSearch"] = Field(
+        default="savedSearch", validation_alias="queryType"
+    )
+
+
 EntityTypes = Union[
     Company,
     Facility,
     Landmark,
     Organization,
     OrganizationType,
     Person,
     Place,
     Product,
     ProductType,
     Concept,
 ]
 
-DomainTypes = Union[
-    EntityTypes, Topic, Source, Language, AutosuggestedSearch, Watchlist
+KnowledgeGraphTypes = Union[
+    MacroEntity,
+    Topic,
+    Source,
+    Language,
+    Watchlist,
+    AutosuggestedSavedSearch,
+    EntityTypes,
 ]
 
 
-class Domain(BaseModel):
+class KnowledgeGraphAnnotated(BaseModel):
     root: Annotated[
         Union[
             Annotated[Company, Tag(Company.model_fields["entity_type"].default)],
             Annotated[Facility, Tag(Facility.model_fields["entity_type"].default)],
             Annotated[Landmark, Tag(Landmark.model_fields["entity_type"].default)],
             Annotated[
                 Organization, Tag(Organization.model_fields["entity_type"].default)
@@ -66,25 +83,25 @@
             Annotated[
                 ProductType, Tag(ProductType.model_fields["entity_type"].default)
             ],
             Annotated[Source, Tag(Source.model_fields["entity_type"].default)],
             Annotated[Topic, Tag(Topic.model_fields["entity_type"].default)],
             Annotated[Language, Tag(Language.model_fields["query_type"].default)],
             Annotated[
-                AutosuggestedSearch,
-                Tag(AutosuggestedSearch.model_fields["query_type"].default),
+                AutosuggestedSavedSearch,
+                Tag(AutosuggestedSavedSearch.model_fields["query_type"].default),
             ],
             Annotated[Watchlist, Tag(Watchlist.model_fields["query_type"].default)],
         ],
-        Discriminator(get_discriminator_domain_value),
+        Discriminator(get_discriminator_knowledge_graph_value),
     ]
 
 
-def parse_domain_object(domain_obj: dict) -> DomainTypes:
+def parse_knowledge_graph_object(domain_obj: dict) -> KnowledgeGraphTypes:
     try:
-        return Domain.model_validate({"root": domain_obj}).root
+        return KnowledgeGraphAnnotated.model_validate({"root": domain_obj}).root
     except ValidationError:
         return Concept.model_validate(domain_obj)
 
 
 # TODO: could somehow unify domain_types and Annotated[Union] in a single list?
 # we have mypy to help. `poetry run task pre-commit`
```

### Comparing `bigdata_client-0.0.4/bigdata/models/search.py` & `bigdata_client-0.0.5/bigdata/models/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,41 @@
-from typing import Literal, Optional, Union
+from typing import Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel, Field
 
 from bigdata.enum_utils import StrEnum
 
 
-class AutosuggestedSearch(BaseModel):
-    """Class used only to parse the output from the Autosuggestion"""
-
-    # TODO: Move this to bigdata.api.autosuggest?
-
-    model_config = ConfigDict(populate_by_name=True)
-    id: Optional[str] = Field(validation_alias="key", default=None)
-    name: Optional[str] = Field(default=None)
-    query_type: Literal["savedSearch"] = Field(
-        default="savedSearch", validation_alias="queryType"
-    )
-
-
 class ExpressionOperation(StrEnum):
     IN = "in"
+    ALL = "all"
+    GREATER_THAN = "greater-than"
+    LOWER_THAN = "lower-than"
+    BETWEEN = "between"
 
 
 class ExpressionTypes(StrEnum):
     AND = "and"
+    OR = "or"
+    NOT = "not"
     KEYWORD = "keyword"
+    SIMILARITY = "similarity"
     ENTITY = "entity"
     SOURCE = "source"
     TOPIC = "rp_topic"
     LANGUAGE = "language"
     WATCHLIST = "watchlist"
     DATE = "date"
+    CONTENT_TYPE = "content_type"
+    SENTIMENT = "sentiment"
 
 
 class Expression(BaseModel):
     type: ExpressionTypes
-    value: Union[list[Union[str, "Expression"]], str]
+    value: Union[list[Union[str, float, "Expression"]], str, float, "Expression"]
     operation: Optional[ExpressionOperation] = None
 
     @classmethod
     def new(cls, etype: ExpressionTypes, values: Optional[list[str]]) -> "Expression":
         if not values:
             return None
         return cls(type=etype, operation=ExpressionOperation.IN, value=values)
```

### Comparing `bigdata_client-0.0.4/bigdata/models/story.py` & `bigdata_client-0.0.5/bigdata/models/story.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,7 +52,14 @@
     """
     A sentence in a story
     """
 
     text: str
     chunk: int
     entities: list[StorySentenceEntity]
+    sentences: list[StorySentence]
+
+
+@dataclass
+class StorySentence:
+    paragraph: int
+    sentence: int
```

### Comparing `bigdata_client-0.0.4/bigdata/models/uploads.py` & `bigdata_client-0.0.5/bigdata/models/uploads.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/old_auth.py` & `bigdata_client-0.0.5/bigdata/old_auth.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.4/bigdata/search.py` & `bigdata_client-0.0.5/bigdata/search.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from dataclasses import dataclass
 from typing import Iterable, Iterator, Optional, Union
 
+from bigdata.advanced_search_query import AdvancedSearchQuery
 from bigdata.api.search import (
     QueryChunksResponse,
     QueryClustersResponse,
     SavedSearchResponse,
     SaveSearchRequest,
     UpdateSearchRequest,
 )
 from bigdata.connection import BigdataConnection
 from bigdata.constants import MAX_SEARCH_PAGES
 from bigdata.daterange import AbsoluteDateRange, RollingDateRange
+from bigdata.models.advanced_search_query import QueryComponent
 from bigdata.models.comentions import Comentions
-from bigdata.models.search import SortBy
+from bigdata.models.search import FileType, SortBy
 from bigdata.simple_search_query import SimpleSearchQuery
 from bigdata.story import Story
 
 
 class Search:
     """
     Class representing a search, saved or not.
     It allows you to perform searches.
     """
 
     def __init__(
         self,
         api: BigdataConnection,
+        # TODO: Change the type of this to something more generic
         query: "SimpleSearchQuery",
         id: Optional[str] = None,
         name: str = "",
     ):
         self.api: BigdataConnection = api
         self.id: Optional[str] = id
         self.name: str = name
@@ -43,25 +46,42 @@
         keywords: Optional[list[str]] = None,
         entities: Optional[list[str]] = None,
         sources: Optional[list[str]] = None,
         topics: Optional[list[str]] = None,
         languages: Optional[list[str]] = None,
         watchlists: Optional[list[str]] = None,
         sortby: SortBy = SortBy.RELEVANCE,
+        scope: FileType = FileType.ALL,
     ) -> "Search":
         """Create a simplified search with just a set of filters"""
         rpx_query = SimpleSearchQuery(
             date_range=date_range,
             keywords=keywords,
             entities=entities,
             sources=sources,
             topics=topics,
             languages=languages,
             watchlists=watchlists,
             sortby=sortby,
+            scope=scope,
+        )
+        return cls(api=api, query=rpx_query)
+
+    @classmethod
+    def from_query(
+        cls,
+        api: "BigdataConnection",
+        query: QueryComponent,
+        date_range: Optional[Union[AbsoluteDateRange, RollingDateRange]] = None,
+        sortby: SortBy = SortBy.RELEVANCE,
+        scope: FileType = FileType.ALL,
+    ) -> "Search":
+        """Create a simplified search with just a set of filters"""
+        rpx_query = AdvancedSearchQuery(
+            date_range=date_range, query=query, sortby=sortby, scope=scope
         )
         return cls(api=api, query=rpx_query)
 
     @classmethod
     def from_saved_search_response(
         cls, api: BigdataConnection, response: SavedSearchResponse
     ):
```

### Comparing `bigdata_client-0.0.4/bigdata/services.py` & `bigdata_client-0.0.5/bigdata/services.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 import os
 from typing import Optional, Union
 
 from bigdata import old_auth
+from bigdata.api.autosuggest import (
+    AutosuggestRequests,
+    AutosuggestResponse,
+    ByIdsRequest,
+)
 from bigdata.auth import Auth
 from bigdata.connection import BigdataConnection
 from bigdata.daterange import AbsoluteDateRange, RollingDateRange
+from bigdata.models.advanced_search_query import QueryComponent
+from bigdata.models.entities import MacroEntity
 from bigdata.models.languages import Language
-from bigdata.models.parse import DomainTypes, EntityTypes, parse_domain_object
-from bigdata.models.search import SortBy
+from bigdata.models.parse import (
+    AutosuggestedSavedSearch,
+    EntityTypes,
+    KnowledgeGraphTypes,
+)
+from bigdata.models.search import FileType, SortBy
 from bigdata.models.sources import Source
 from bigdata.models.topics import Topic
 from bigdata.models.uploads import Document, UploadQuota
 from bigdata.models.watchlists import Watchlist
+from bigdata.query_type import QueryType
 from bigdata.search import Search
 from bigdata.settings import BigdataAuthType, settings
 
+CONCURRENT_AUTOSUGGEST_REQUESTS_LIMIT = 10
+
 
 class Bigdata:
     """
     Represents a connection to RavenPack's Bigdata API.
 
-    :ivar domain: Proxy for the domain search functionality.
+    :ivar knowledge_graph: Proxy for the domain search functionality.
     :ivar content_search: Proxy object for the content search functionality.
     :ivar watchlists: Proxy object for the watchlist functionality.
     :ivar uploads: Proxy object for the internal content functionality.
     """
 
     def __init__(
         self,
@@ -39,52 +53,88 @@
             username = os.environ.get("BIGDATA_USER")
         if username is None or password is None:
             raise ValueError("Username and password must be provided")
         if auth_type is None:
             auth_type = settings.BIGDATA_AUTH_TYPE
         if auth_type == BigdataAuthType.CLERK:
             auth = Auth.from_username_and_password(username, password)
-        else:  # FIXME OLD AUTH
+        else:
             auth = old_auth.Auth.from_username_and_password(username, password)
 
-        if api_url is None:  # FIXME OLD AUTH
+        if api_url is None:
             api_url = str(settings.BIGDATA_API_URL)
         self.api = BigdataConnection(auth, api_url)
-        self.domain = Domain(self.api)
+        self.knowledge_graph = KnowledgeGraph(self.api)
         self.content_search = ContentSearch(self.api)
         self.watchlists = Watchlists(self.api)
         self.uploads = Uploads(self.api)
 
 
-class Domain:
+class KnowledgeGraph:
     """For finding entities, sources and topics"""
 
     def __init__(self, api_connection: BigdataConnection):
         self.api = api_connection
 
-    def find(self, value: str, /) -> [DomainTypes]:
+    def autosuggest(
+        self, values: list[str], /, limit=20
+    ) -> dict[str, list[KnowledgeGraphTypes]]:
         """
         Searches for entities, sources, topics, searches and watchlists
-        TODO: To be renamed to autosuggest
         """
-        api_response = self.api.autosuggest(value)
-        # TODO: should we expand it with cqs/by-ids response?
-        return [parse_domain_object(s) for s in api_response]
+
+        # TODO update response model returned to dict[str, list[KnowledgeGraphTypes]]
+        api_response = self.api.autosuggest(
+            AutosuggestRequests(root=values), limit=limit
+        )
+
+        # Exclude macros and saved searches from response
+        api_response = self._exclude_macros_and_saved_searches(api_response)
+
+        return {key: results.root for key, results in api_response.root.items()}
+
+    @staticmethod
+    def _exclude_macros_and_saved_searches(
+        api_response: AutosuggestResponse,
+    ) -> AutosuggestResponse:
+        filtered_response = {}
+        for key, key_results in api_response.root.items():
+            filtered_response[key] = list(
+                filter(
+                    lambda result: not isinstance(
+                        result, (MacroEntity, AutosuggestedSavedSearch)
+                    ),
+                    key_results.root,
+                )
+            )
+        return AutosuggestResponse(root=filtered_response)
 
     def get_entities(self, ids: list[str], /) -> list[EntityTypes]:
         """Retrieve a list of entities by their ids."""
+        return self._get_by_ids(ids, QueryType.ENTITY)
 
     def get_sources(self, ids: list[str], /) -> list[Source]:
         """Retrieve a list of sources by its ids."""
+        return self._get_by_ids(ids, QueryType.SOURCE)
 
     def get_topics(self, ids: list[str], /) -> list[Topic]:
         """Retrieve a list of topics by its ids."""
+        return self._get_by_ids(ids, QueryType.TOPIC)
 
     def get_languages(self, ids: list[str], /) -> list[Language]:
         """Retrieve a list of languages by its ids."""
+        return self._get_by_ids(ids, QueryType.LANGUAGE)
+
+    def _get_by_ids(self, ids: list[str], query_type: QueryType) -> list:
+        api_response = self.api.by_ids(
+            ByIdsRequest.model_validate(
+                [{"key": id_, "queryType": query_type} for id_ in ids]
+            )
+        )
+        return [api_response.root.get(id_) for id_ in ids]
 
 
 class Watchlists:
     def __init__(self, api_connection: BigdataConnection):
         self.api = api_connection
 
     def get(self, id_, /) -> Watchlist:
@@ -113,14 +163,15 @@
         keywords: Optional[list[str]] = None,
         entities: Optional[list[str]] = None,
         sources: Optional[list[str]] = None,
         topics: Optional[list[str]] = None,
         languages: Optional[list[str]] = None,
         watchlists: Optional[list[str]] = None,
         sortby: Optional[SortBy] = SortBy.RELEVANCE,
+        scope: FileType = FileType.ALL,
     ) -> Search:
         """
         Creates a new search object that allows you to perform a search on
         keywords and entity_ids.
 
         Example usage:
 
@@ -140,14 +191,26 @@
             keywords=keywords,
             entities=entities,
             sources=sources,
             topics=topics,
             languages=languages,
             watchlists=watchlists,
             sortby=sortby,
+            scope=scope,
+        )
+
+    def new_from_query(
+        self,
+        query: QueryComponent,
+        date_range: Optional[Union[AbsoluteDateRange, RollingDateRange]] = None,
+        sortby: SortBy = SortBy.RELEVANCE,
+        scope: FileType = FileType.ALL,
+    ) -> Search:
+        return Search.from_query(
+            self.api, query, date_range=date_range, sortby=sortby, scope=scope
         )
 
     def get(self, id_, /) -> Search:
         """Retrieve a saved search by its id."""
         response = self.api.get_search(id_)
         return Search.from_saved_search_response(self.api, response)
```

### Comparing `bigdata_client-0.0.4/bigdata/settings.py` & `bigdata_client-0.0.5/bigdata/settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from enum import Enum
 
 from pydantic import HttpUrl
 from pydantic_settings import BaseSettings
 
+from bigdata.models.search import Ranking
+
 
 class ClerkInstanceType(str, Enum):
     DEV = "DEV"
     PROD = "PROD"
 
 
 class BigdataAuthType(str, Enum):
     CLERK = "CLERK"
     OLD = "OLD"
 
 
+class LLMSettings(BaseSettings):
+    USE_HYBRID: bool = True
+    RANKING: Ranking = Ranking.STABLE
+
+
 class Settings(
     BaseSettings
 ):  # FIXME OLD AUTH remove Clerk config when old auth is removed
     PACKAGE_NAME: str = "bigdata-client"  # The name of the python package
     BIGDATA_API_URL: HttpUrl = "https://api.bigdata.com"
     BIGDATA_AUTH_TYPE: BigdataAuthType = BigdataAuthType.CLERK
     CLERK_INSTANCE_TYPE: ClerkInstanceType = ClerkInstanceType.PROD
     # TODO: Change to another endpoint as we need the refresh token
     AUTH_LOGIN_FORM_ENDPOINT: HttpUrl = "https://auth.ravenpack.com/2.0/login"
     CLERK_FRONTEND_URL: HttpUrl = "https://clerk.bigdata.com/v1"
+    LLM: LLMSettings = LLMSettings()
 
 
 settings = Settings()
```

### Comparing `bigdata_client-0.0.4/bigdata/simple_search_query.py` & `bigdata_client-0.0.5/bigdata/simple_search_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 from dataclasses import dataclass
 from typing import Optional, Union
 
 from bigdata.api.search import (
     DiscoveryPanelRequest,
     QueryChunksRequest,
     QueryClustersRequest,
-    SavedSearchResponse,
+    SavedSearchQueryResponse,
     SaveSearchQueryRequest,
 )
 from bigdata.constants import SEARCH_PAGE_SIZE
 from bigdata.daterange import AbsoluteDateRange, RollingDateRange
 from bigdata.models.search import (
     Expression,
     ExpressionTypes,
     FileType,
-    Ranking,
     SearchPagination,
     SortBy,
 )
+from bigdata.settings import settings
 
 
 @dataclass
 class SimpleSearchQuery:
     """
     A class to hold the simplified search filters.
     For internal use only
@@ -35,25 +35,27 @@
     keywords: Optional[list[str]] = None
     entities: Optional[list[str]] = None
     sources: Optional[list[str]] = None
     topics: Optional[list[str]] = None
     languages: Optional[list[str]] = None
     watchlists: Optional[list[str]] = None
     sortby: SortBy = SortBy.RELEVANCE
+    scope: FileType = FileType.ALL
 
-    def make_copy(self):
+    def make_copy(self) -> "SimpleSearchQuery":
         return SimpleSearchQuery(
             date_range=self.date_range,
             keywords=list(self.keywords) if self.keywords else None,
             entities=list(self.entities) if self.entities else None,
             sources=list(self.sources) if self.sources else None,
             topics=list(self.topics) if self.topics else None,
             languages=list(self.languages) if self.languages else None,
             watchlists=list(self.watchlists) if self.watchlists else None,
             sortby=self.sortby,
+            scope=self.scope,
         )
 
     def to_query_clusters_api_request(self, page: int) -> QueryClustersRequest:
         """
         Used when composing the request to perform a search using the
         /query-clusters endpoint.
         The difference between this method and to_save_search_request is that
@@ -66,18 +68,18 @@
             sources=self.sources,
             topics=self.topics,
             languages=self.languages,
             watchlists=self.watchlists,
         )
         return QueryClustersRequest(
             sort=self.sortby,
-            scope=FileType.ALL,
-            ranking=Ranking.STABLE,
+            scope=self.scope,
+            ranking=settings.LLM.RANKING,
             pagination=SearchPagination(limit=SEARCH_PAGE_SIZE, cursor=page),
-            hybrid=True,
+            hybrid=settings.LLM.USE_HYBRID,
             expression=expression,
         )
 
     def to_query_chunks_api_request(self, page: int) -> QueryChunksRequest:
         """
         Used when composing the request to perform a search using the
         /query-chunks endpoint.
@@ -91,18 +93,18 @@
             sources=self.sources,
             topics=self.topics,
             languages=self.languages,
             watchlists=self.watchlists,
         )
         return QueryChunksRequest(
             sort=self.sortby,
-            scope=FileType.ALL,
-            ranking=Ranking.STABLE,
+            scope=self.scope,
+            ranking=settings.LLM.RANKING,
             pagination=SearchPagination(limit=SEARCH_PAGE_SIZE, cursor=page),
-            hybrid=True,
+            hybrid=settings.LLM.USE_HYBRID,
             expression=expression,
         )
 
     def to_discovery_panel_api_request(self) -> DiscoveryPanelRequest:
         """
         Used when composing the request to get comentions. Pretty much the same
         as to_query_chunks_api_request but without dates
@@ -115,17 +117,17 @@
             sources=self.sources,
             topics=self.topics,
             languages=self.languages,
             watchlists=self.watchlists,
         )
         return DiscoveryPanelRequest(
             sort=self.sortby,
-            scope=FileType.ALL,
-            ranking=Ranking.STABLE,
-            hybrid=True,
+            scope=self.scope,
+            ranking=settings.LLM.RANKING,
+            hybrid=settings.LLM.USE_HYBRID,
             expression=expression,
         )
 
     def to_save_search_request(self) -> SaveSearchQueryRequest:
         """
         Used when composing the request to create a search.
         The difference between this method and to_query_chunks_api_request is that
@@ -137,63 +139,61 @@
             keywords=self.keywords,
             entities=self.entities,
             sources=self.sources,
             topics=self.topics,
             languages=self.languages,
             watchlists=self.watchlists,
         )
-        date_expression = self._date_range_to_date_experession(self.date_range)
+        date_expression = self._date_range_to_date_expression(self.date_range)
         date_expression = [date_expression] if date_expression is not None else None
         return SaveSearchQueryRequest(
             sort=self.sortby,
-            scope=FileType.ALL,
-            ranking=Ranking.STABLE,
-            hybrid=True,
+            scope=self.scope,
+            ranking=settings.LLM.RANKING,
+            hybrid=settings.LLM.USE_HYBRID,
             expression=expression,
             date=date_expression,
         )
 
     @classmethod
     def from_saved_search_response(
-        cls, search_query: SavedSearchResponse
+        cls, search_query: SavedSearchQueryResponse
     ) -> "SimpleSearchQuery":
         """
         Deserializes a request/response object into a SimpleSearchQuery object,
         if possible
         """
-        date_range_raw: Union[list, str] = cls._extract_field(
+        date_range_raw: Union[list, str] = cls._get_field(
             search_query, ExpressionTypes.DATE
         )
         date_range = cls._date_expression_to_date_range(date_range_raw)
         if date_range is None and search_query.date is not None:
             if len(search_query.date) != 1:
                 raise ValueError(
                     "Unexpected error. The date expression should have 1 value"
                 )
             expression = search_query.date[0]
             date_range_raw = [
                 e
-                for e in cls._extract_field_from_expression(
+                for e in cls._get_field_from_expression(
                     expression, ExpressionTypes.DATE
                 )
                 if e is not None
             ]
             if date_range_raw is not None and len(date_range_raw) == 1:
                 date_range = cls._date_expression_to_date_range(date_range_raw[0])
 
         return cls(
             date_range=date_range,
-            keywords=cls._extract_field(search_query, ExpressionTypes.KEYWORD),
-            entities=cls._extract_field(search_query, ExpressionTypes.ENTITY),
-            sources=cls._extract_field(search_query, ExpressionTypes.SOURCE),
-            topics=cls._extract_field(search_query, ExpressionTypes.TOPIC),
-            languages=cls._extract_field(search_query, ExpressionTypes.LANGUAGE),
-            watchlists=cls._extract_field_to_list(
-                search_query, ExpressionTypes.WATCHLIST
-            ),
+            keywords=cls._get_field(search_query, ExpressionTypes.KEYWORD),
+            entities=cls._get_field(search_query, ExpressionTypes.ENTITY),
+            sources=cls._get_field(search_query, ExpressionTypes.SOURCE),
+            topics=cls._get_field(search_query, ExpressionTypes.TOPIC),
+            languages=cls._get_field(search_query, ExpressionTypes.LANGUAGE),
+            watchlists=cls._get_field_to_list(search_query, ExpressionTypes.WATCHLIST),
             sortby=search_query.sort,
         )
 
     def _build_expression(
         self,
         date_range: Optional[Union[AbsoluteDateRange, RollingDateRange]],
         keywords: Optional[list[str]],
@@ -238,43 +238,43 @@
                 value=[start, end],
             )
         else:
             # This should never happen
             raise ValueError(f"Wrong type sent for date range '{date_range}'")
 
     @classmethod
-    def _extract_field(
-        cls, search_query: SavedSearchResponse, expression_type: ExpressionTypes
+    def _get_field(
+        cls, search_query: SavedSearchQueryResponse, expression_type: ExpressionTypes
     ):
-        fields = cls._extract_field_from_expression(
+        fields = cls._get_field_from_expression(
             search_query.expression, expression_type
         )
         fields = list(fields)
         if not fields:
             return None
         if len(fields) != 1:
             raise ValueError(
                 f"Unexpected error. The expression should have 1 value of {expression_type}, but it has {len(fields)}"
             )
         return fields[0]
 
     @classmethod
-    def _extract_field_to_list(
-        cls, search_query: SavedSearchResponse, expression_type: ExpressionTypes
+    def _get_field_to_list(
+        cls, search_query: SavedSearchQueryResponse, expression_type: ExpressionTypes
     ):
         """Used for cases like watchlists, which are expressed as multiple objects"""
-        fields = cls._extract_field_from_expression(
+        fields = cls._get_field_from_expression(
             search_query.expression, expression_type
         )
         if fields is None:
             return None
         return list(fields) or None
 
     @classmethod
-    def _extract_field_from_expression(
+    def _get_field_from_expression(
         cls, expression: Union[Expression, str], expression_type: ExpressionTypes
     ) -> Optional[Union[list, str]]:
         # It should always be a list, because it either comes from the
         # "expression" field or from the values of an AND
         if isinstance(expression, str):
             return None
 
@@ -283,15 +283,15 @@
 
         if expression.type != ExpressionTypes.AND:
             # We do not support or, not, nor any other type of expression
             # since this should be a simple search query
             return None
 
         for subexpression in expression.value:
-            values = cls._extract_field_from_expression(subexpression, expression_type)
+            values = cls._get_field_from_expression(subexpression, expression_type)
             for value in values:
                 if value is not None:
                     yield value
         return None
 
     @staticmethod
     def _date_expression_to_date_range(
@@ -306,15 +306,15 @@
                     f" but it has {len(expression)}"
                 )
             return AbsoluteDateRange(expression[0], expression[1])
         else:
             return RollingDateRange(expression)
 
     @staticmethod
-    def _date_range_to_date_experession(
+    def _date_range_to_date_expression(
         date_range: Optional[Union[AbsoluteDateRange, RollingDateRange]]
     ) -> Optional[Expression]:
         if date_range is None:
             return None
         if isinstance(date_range, AbsoluteDateRange):
             start, end = date_range.to_string_tuple()
             return Expression(type=ExpressionTypes.DATE, value=[start, end])
```

### Comparing `bigdata_client-0.0.4/pyproject.toml` & `bigdata_client-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "bigdata-client"
 packages = [
     { include = "bigdata" },
 ]
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = [
     "Iago Veloso <iago@ravenpack.com>",
     "Diego de Aguilar <ddeaguilar@ravenpack.com>",
     "Jose Ramon Cano <jcano@ravenpack.com>"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
 pydantic = "^2.5.3"
 pydantic-settings = "^2.1.0"
 pyjwt = "^2.8.0"
+aiohttp = "^3.9.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 isort = "^5.13.2"
 pytest-cov = "^4.1.0"
 taskipy = "^1.12.2"
 black = "^24.1.1"
```

