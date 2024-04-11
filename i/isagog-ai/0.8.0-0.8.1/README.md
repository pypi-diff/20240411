# Comparing `tmp/isagog_ai-0.8.0.tar.gz` & `tmp/isagog_ai-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isagog_ai-0.8.0.tar", max compression
+gzip compressed data, was "isagog_ai-0.8.1.tar", max compression
```

## Comparing `isagog_ai-0.8.0.tar` & `isagog_ai-0.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.8.0/isagog/__init__.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.8.0/isagog/client/__init__.py
--rw-r--r--   0        0        0     8560 2024-03-29 14:48:01.626394 isagog_ai-0.8.0/isagog/client/kg_client.py
--rw-r--r--   0        0        0     5928 2024-03-29 14:48:01.665081 isagog_ai-0.8.0/isagog/client/nlp_client.py
--rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.8.0/isagog/generator/__init__.py
--rw-r--r--   0        0        0     5647 2024-03-29 14:48:01.711776 isagog_ai-0.8.0/isagog/generator/sparql_generator.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.8.0/isagog/model/__init__.py
--rw-r--r--   0        0        0    13646 2024-03-29 14:48:01.643535 isagog_ai-0.8.0/isagog/model/kg_model.py
--rw-r--r--   0        0        0    26876 2024-03-29 14:48:01.680285 isagog_ai-0.8.0/isagog/model/kg_query.py
--rw-r--r--   0        0        0      443 2024-03-29 14:48:01.725437 isagog_ai-0.8.0/isagog/model/nlp_model.py
--rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.8.0/LICENSE
--rw-r--r--   0        0        0      569 2024-03-29 11:45:02.491727 isagog_ai-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.8.0/README.md
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 isagog_ai-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.8.1/isagog/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.8.1/isagog/client/__init__.py
+-rw-r--r--   0        0        0     9032 2024-04-10 13:38:15.982049 isagog_ai-0.8.1/isagog/client/kg_client.py
+-rw-r--r--   0        0        0     5971 2024-04-09 14:40:57.250758 isagog_ai-0.8.1/isagog/client/nlp_client.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.8.1/isagog/generator/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-10 08:27:28.933122 isagog_ai-0.8.1/isagog/generator/sparql_generator.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.8.1/isagog/model/__init__.py
+-rw-r--r--   0        0        0    14592 2024-04-10 14:14:03.090951 isagog_ai-0.8.1/isagog/model/kg_model.py
+-rw-r--r--   0        0        0    27390 2024-04-10 09:06:24.629297 isagog_ai-0.8.1/isagog/model/kg_query.py
+-rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.8.1/isagog/model/nlp_model.py
+-rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.8.1/LICENSE
+-rw-r--r--   0        0        0      588 2024-04-09 14:31:16.952983 isagog_ai-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.8.1/README.md
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.8.1/PKG-INFO
```

### Comparing `isagog_ai-0.8.0/isagog/client/kg_client.py` & `isagog_ai-0.8.1/isagog/client/kg_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 (c) Isagog S.r.l. 2024, MIT License
 """
 import logging
 import os
 import time
 from typing import Type, TypeVar
 
-import requests
+# import requests
+import httpx
 from dotenv import load_dotenv
 
 from isagog.model.kg_model import Individual, Entity, Assertion, Ontology, Attribute, Concept, Relation, ID
 from isagog.model.kg_query import UnarySelectQuery, DisjunctiveClause, AtomicClause, Comparison, Value
 
 load_dotenv()
 
@@ -44,15 +45,15 @@
         self.dataset = dataset
         self.ontology = ontology
         self.version = version if version else "latest"
         self.logger = logger if logger else logging.getLogger()
         self.logger.info("Isagog KG client (%s) initialized on route %s", hex(id(self)), route)
 
     def get_entity(self,
-                   _id: str,
+                   _id: ID,
                    expand: bool = True,
                    entity_type: Type[E] = Entity
                    ) -> E | None:
         """
         Gets the entity by its identifier
         :param _id: the entity identifier
         :param expand: whether to return entity attributes
@@ -69,24 +70,24 @@
         expand = "true" if expand else "false"
 
         params = f"id={_id}&expand={expand}"
 
         if self.dataset:
             params += f"&dataset={self.dataset}"
 
-        res = requests.get(
+        res = httpx.get(
             url=self.route,
             params=params,
             headers={"Accept": "application/json"},
         )
-        if res.ok:
+        if res.status_code == 200:
             self.logger.debug("Fetched %s", _id)
             return entity_type(_id, **res.json())
         else:
-            self.logger.error("Couldn't fetch %s due to %s", _id, res.reason)
+            self.logger.error("Couldn't fetch %s due to %s", _id, res.text)
             return None
 
     def query_assertions(self,
                          subject: Individual,
                          properties: list[Attribute | Relation],
                          timeout=KG_DEFAULT_TIMEOUT
                          ) -> list[Assertion]:
@@ -96,31 +97,37 @@
         :param timeout:
         :param subject:
         :param properties: the queried properties
         :return: a list of dictionaries { property: values }
         """
         assert (subject and properties)
 
-        self.logger.debug("Querying assertions for %s", subject.id)
+        if not isinstance(subject, Individual):
+            raise ValueError(f"{subject} not an Individual")
 
-        query = UnarySelectQuery(subject=subject)
+        if not all(isinstance(prop, (Attribute, Relation)) for prop in properties):
+            raise ValueError(f"{properties} not all Attributes or Relations")
+
+        self.logger.debug("Querying assertions for %s", subject)
+
+        query = UnarySelectQuery(subject=subject.id)
 
         for prop in properties:
-            query.add_fetch_clause(predicate=str(prop))
+            query.add_fetch_clause(predicate=str(prop.id))
 
         query_dict = query.to_dict(self.version)
 
-        res = requests.post(
+        res = httpx.post(
             url=self.route,
             json=query_dict,
             headers={"Accept": "application/json"},
             timeout=timeout
         )
 
-        if res.ok:
+        if res.status_code == 200:
             res_list = res.json()
             if len(res_list) == 0:
                 self.logger.warning("Void attribute query")
                 return []
             else:
                 res_attrib_list = res_list[0].get('attributes', OSError("malformed response"))
 
@@ -129,15 +136,15 @@
                         record = next(item for item in res_attrib_list if item['id'] == _prop)
                         return record.get('values', OSError("malformed response"))
                     except StopIteration:
                         raise OSError("incomplete response: %s not found", _prop)
 
                 return [Assertion(predicate=prop, values=__get_values(prop)) for prop in properties]
         else:
-            self.logger.warning("Query of entity %s failed due to %s", subject, res.reason)
+            self.logger.warning("Query of entity %s failed due to %s", subject, res.text)
             return []
 
     def search_individuals(self,
                            kinds: list[Concept] = None,
                            constraints: dict[Attribute, Value] = None,
                            timeout=KG_DEFAULT_TIMEOUT
                            ) -> list[Individual]:
@@ -158,27 +165,27 @@
             attribute, value = next(iter(constraints.items()))
             search_clause = AtomicClause(property=attribute, argument=value, method=Comparison.REGEX)
         else:
             search_clause = DisjunctiveClause()
             for attribute, value in constraints.items():
                 search_clause.add_atom(property=attribute, argument=value, method=Comparison.REGEX)
 
-        query.clause(search_clause)
+        query.add(search_clause)
 
-        res = requests.post(
+        res = httpx.post(
             url=self.route,
             json=query.to_dict(self.version),
             headers={"Accept": "application/json"},
             timeout=timeout
         )
 
-        if res.ok:
+        if res.status_code == 200:
             entities.extend([Individual(r.get('id'), **r) for r in res.json()])
         else:
-            self.logger.error("Search individuals failed: code %d, reason %s", res.status_code, res.reason)
+            self.logger.error("Search individuals failed: code %d, reason %s", res.status_code, res.text)
 
         return entities
 
     def query_individuals(self,
                           query: UnarySelectQuery,
                           kind: Type[E] = Individual,
                           timeout=KG_DEFAULT_TIMEOUT
@@ -193,60 +200,63 @@
         start_time = time.time()
 
         req = query.to_dict(self.version)
 
         if self.dataset and (self.version == "latest" or self.version > "v1.0.0"):
             req['dataset'] = self.dataset
 
-        res = requests.post(
+        res = httpx.post(
             url=self.route,
             json=req,
             headers={"Accept": "application/json"},
             timeout=timeout
         )
 
-        if res.ok:
-            self.logger.debug("Query individuals successful in %d seconds", time.time() - start_time)
+        if res.status_code == 200:
+            self.logger.debug("Query individuals done in %d seconds", time.time() - start_time)
             return [kind(r.get('id'), **r) for r in res.json()]
         elif res.status_code < 500:
-            self.logger.warning("query individuals return code %d, reason %s", res.status_code, res.reason)
+            self.logger.warning("query individuals return code %d, reason %s", res.status_code, res.text)
         else:
-            self.logger.error("query individuals return code code %d, reason %s", res.status_code, res.reason)
+            self.logger.error("query individuals return code code %d, reason %s", res.status_code, res.text)
         return []
 
-    def upsert_individual(self, individual: Individual, auth_token=None) -> bool:
+    def upsert_individual(self, individual: ID, assetions: list[Assertion], auth_token=None) -> bool:
         """
         Updates an individual or insert it if not present; existing properties are preserved
 
         :param individual: the individual
+        :param assetions: assertions to be updated
         :param auth_token:
         :return:
         """
-        self.logger.debug("Updating individual %s", individual.id)
-        params = {
-            'id': individual.id
-        }
+        self.logger.debug("Updating individual %s", individual)
 
-        if self.dataset and (self.version == "latest" or self.version > "v1.0.0"):
+        params = {'id': individual}
+        if self.dataset:
             params['dataset'] = self.dataset
 
-        req = individual.to_dict()
+        req = [ass.to_dict() for ass in assetions]
 
         headers = {"Accept": "application/json"}
 
         if auth_token:
             headers["Authorization"] = f'Bearer {auth_token}'
 
-        res = requests.patch(
-            url=self.route,
-            params=params,
-            json=req,
-            headers=headers
-        )
+        try:
+            res = httpx.patch(
+                url=self.route,
+                params=params,
+                json=req,
+                headers=headers
+            )
 
-        if res.ok:
-            return True
-        else:
-            raise OSError(f"upsert failed {res.status_code}")
+            if res.status_code == 200:
+                return True
+            else:
+                print(f"upsert failed {res.status_code}")
+                return False
+        except Exception as e:
+            raise e
 
     def delete_individual(self, _id: ID, auth_key=None):
         pass
```

### Comparing `isagog_ai-0.8.0/isagog/client/nlp_client.py` & `isagog_ai-0.8.1/isagog/client/nlp_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Client for Isagog NLP service
 (c) Isagog S.r.l. 2024, MIT License
 """
 import logging
 import os
 import time
+import httpx
+
 
-import requests
 from dotenv import load_dotenv
 
 from isagog.model.nlp_model import Word, NamedEntity
 
 load_dotenv()
 
 NLP_DEFAULT_TIMEOUT = int(os.getenv('NLP_DEFAULT_TIMEOUT', 60))
@@ -62,55 +63,55 @@
         """
         start = time.time()
         req = {
             "target": target,
             "candidates": candidates,
         }
 
-        res = requests.post(
+        res = httpx.post(
             url=self.route + "/rank",
             json=req,
             timeout=timeout
         )
 
-        if res.ok:
+        if res.status_code == 200:
             self.logger.debug("Ranked %s in %d seconds", truncate(target), time.time() - start)
             return [(rank[0], rank[1]) for rank in res.json()]
         else:
-            self.logger.error("similarity ranking failed: code=%d, reason=%s", res.status_code, res.reason)
+            self.logger.error("similarity ranking failed: code=%d, reason=%s", res.status_code, res.text)
             return []
 
     def extract_keywords_from(self,
                               text: str,
                               number=5,
                               timeout=NLP_DEFAULT_TIMEOUT) -> list[str]:
         """
         Extract the main N words (keywords) from the supplied text
         :param timeout:
         :param text:
         :param number:
         :return:
         """
         self.logger.debug("Extracting %d keywords from %s", number, truncate(text))
-        res = requests.post(
+        res = httpx.post(
             url=self.route + "/analyze",
             json={
                 "text": text,
                 "tasks": ["keyword"],
                 "keyword_number": number
             },
             headers={"Accept": "application/json"},
             timeout=timeout
         )
-        if res.ok:
+        if res.status_code == 200:
             res_dict = res.json()
             words = [kwr[0] for kwr in res_dict["keyword"]]
             return words
         else:
-            self.logger.error("fail to extract from '%s': code=%d, reason=%s", text, res.status_code, res.reason)
+            self.logger.error("fail to extract from '%s': code=%d, reason=%s", text, res.status_code, res.text)
             return []
 
     def extract_words(self,
                       text: str,
                       filter_pos=None,
                       timeout=NLP_DEFAULT_TIMEOUT) -> list[str]:
         """
@@ -120,29 +121,29 @@
         :param filter_pos: part of speech list
         :return:
         """
         self.logger.debug("Extracting words from %s", truncate(text))
         if not filter_pos:
             filter_pos = DEFAULT_LEXICAL_POS
 
-        res = requests.post(
+        res = httpx.post(
             url=self.route + "/analyze",
             json={
                 "text": text,
                 "tasks": ["word"]
             },
             headers={"Accept": "application/json"},
             timeout=timeout
         )
-        if res.ok:
+        if res.status_code == 200:
             res_dict = res.json()
             words = [Word(**{k: v for k, v in r.items() if k in Word._fields}) for r in res_dict["words"]]
             return [w.text for w in words if w.pos in filter_pos]
         else:
-            self.logger.error("fail to extract from '%s': code=%d, reason=%s", text, res.status_code, res.reason)
+            self.logger.error("fail to extract from '%s': code=%d, reason=%s", text, res.status_code, res.text)
             return []
 
     def extract_words_entities(self,
                                text: str,
                                filter_pos=None,
                                timeout=NLP_DEFAULT_TIMEOUT) -> (list[Word], list[NamedEntity]):
         """
@@ -152,28 +153,28 @@
         :param timeout:
         :return:
         """
         self.logger.debug("Extracting words and entities from %s", truncate(text))
         if not filter_pos:
             filter_pos = DEFAULT_LEXICAL_POS
 
-        res = requests.post(
+        res = httpx.post(
             url=self.route + "/analyze",
             json={
                 "text": text,
                 "tasks": ["word", "entity"]
             },
             headers={"Accept": "application/json"},
             timeout=timeout
         )
 
-        if res.ok:
+        if res.status_code == 200:
             res_dict = res.json()
             words = list(filter(lambda w: w.pos in filter_pos,
                                 [Word(**{k: v for k, v in r.items() if k in Word._fields}) for r in res_dict["words"]]))
             entities = [NamedEntity(**{k: v for k, v in r.items() if k in NamedEntity._fields}) for r in
                         res_dict["entities"]]
             return words, entities
 
         else:
-            self.logger.error("fail to extract from '%s': code=%d, reason=%s", text, res.status_code, res.reason)
+            self.logger.error("fail to extract from '%s': code=%d, reason=%s", text, res.status_code, res.text)
             return [], []
```

### Comparing `isagog_ai-0.8.0/isagog/generator/sparql_generator.py` & `isagog_ai-0.8.1/isagog/generator/sparql_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 SPARQL query generator
 (c) Isagog S.r.l. 2024, MIT License
 """
 from io import StringIO
 
+from isagog.model.kg_model import Assertion
 from isagog.model.kg_query import UnarySelectQuery, AtomicClause, Comparison, Variable, \
     ConjunctiveClause, DisjunctiveClause, _SCOREVAR, SelectQuery
 from isagog.model.kg_query import Generator, Clause
 
 
 class SPARQLGenerator(Generator):
     """
@@ -89,14 +90,20 @@
         else:
             raise ValueError("Unsupported clause type")
 
     def __init__(self):
         super().__init__("SPARQL")
 
     def generate_query(self, query: SelectQuery, **kwargs) -> str:
+        """
+        Generates a SPARQL query from a SelectQuery
+        :param query:
+        :param kwargs:
+        :return:
+        """
 
         if not isinstance(query, UnarySelectQuery):
             raise TypeError("Can only generate_query from UnarySelectQuery")
 
         strio = StringIO()
         for (name, uri) in query.prefixes:
             strio.write(f"PREFIX {name}: <{uri}#>\n")
@@ -131,8 +138,9 @@
             strio.write(f"ORDER BY DESC(?{_SCOREVAR})\n")
         if query.limit > 0:
             strio.write(f"LIMIT {query.limit}\n")
 
         return strio.getvalue()
 
 
+
 _SPARQLGEN = SPARQLGenerator()
```

### Comparing `isagog_ai-0.8.0/isagog/model/kg_model.py` & `isagog_ai-0.8.1/isagog/model/kg_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,18 +163,28 @@
         """
 
         :param predicate:
         :param subject:
         :param values:
         """
         assert predicate
-        self.property = str(predicate).strip("<>")
+        self.predicate = str(predicate).strip("<>")
         self.subject = str(subject).strip("<>") if subject else None
         self.values = values if values else []
 
+    def n3(self) -> list[str]:
+        """Convert to n3"""
+        rt = []
+        for value in self.values:
+            rt.append(f"<{self.subject}> <{self.predicate}> {value}")
+        return rt
+
+    def to_dict(self) -> dict:
+        return _todict(self)
+
 
 class Ontology(Graph):
     """
     In-memory, read-only RDF representation of an ontology.
     Manages basic reasoning on declared inclusion dependencies (RDFS.subClassOf).
     Also, it manages classes annotated as 'category' in the ontology. Categories
     are 'rigid' concepts,
@@ -259,22 +269,32 @@
                         break
                 break
         return found
 
 
 class AttributeInstance(Assertion):
     """
-    Attribute instance, as defined in
-    isagog_api/openapi/isagog_kg.openapi.yaml
+    Attributive assertion
     """
 
-    def __init__(self, **kwargs):
-        predicate = kwargs.get('property', kwargs.get('id', KeyError("missing relation property")))
-        values = kwargs.get('values', [])
+    def __init__(self, predicate: ID = None,
+                 subject: ID = None,
+                 values: list = None, **kwargs):
+        """
+        :param subject: the asserted subject
+        :param predicate: the asserted property
+        :param values: the asserted values
+        :param kwargs:
+        """
+        if predicate is None:
+            predicate = kwargs.get('property', kwargs.get('id', KeyError("missing relation property")))
+        if values is None:
+            values = kwargs.get('values', [])
         super().__init__(predicate=predicate,
+                         subject=subject,
                          values=values)
         self.value_type = kwargs.get('type', "string")
 
     def all_values_as_string(self) -> str:
         match len(self.values):
             case 0:
                 return ""
@@ -292,36 +312,45 @@
         else:
             return default
 
     def is_empty(self) -> bool:
         return len(self.values) == 0 or self.values[0] == "None"
 
 
-VOID_ATTRIBUTE = AttributeInstance(id='http://isagog.com/attribute#void')
+VOID_ATTRIBUTE = AttributeInstance(predicate='http://isagog.com/attribute#void')
 
 
 class RelationInstance(Assertion):
     """
-    Relational assertion, as defined in
-    isagog_api/openapi/isagog_kg.openapi.yaml
+    Relational assertion
     """
 
-    def __init__(self, **kwargs):
-        predicate = kwargs.get('property', kwargs.get('id', KeyError("missing relation property")))
-        values = kwargs.get('values', [])
+    def __init__(self, predicate: ID = None, subject: ID = None, values: list = None, **kwargs):
+        """
+
+        :param property: the asserted property
+        :param subject: the assertion's subject
+        :param values: the asserted values
+        :param kwargs:
+        """
+        if predicate is None:
+            predicate = kwargs.get('property', kwargs.get('id', KeyError("missing relation property")))
+        if values is None:
+            values = kwargs.get('values', [])
         if values:
             specimen = values[0]
             if isinstance(specimen, Individual):
                 pass
             elif isinstance(specimen, dict):
                 inst_values = [Individual(_id=r_data.get('id'), **r_data) for r_data in values]
                 values = inst_values
             else:
                 raise ValueError("bad values for relation instance")
         super().__init__(predicate=predicate,
+                         subject=subject,
                          values=values)
 
     def all_values(self, only_id=True) -> list:
         """
         Returns all values of the relation instance
         :param only_id:
         :return:
@@ -358,20 +387,24 @@
 
 
 VOID_RELATION = RelationInstance(predicate='http://isagog.com/relation#void')
 
 
 class Individual(Entity):
     """
-    Individual entity as defined in
-    isagog_api/openapi/isagog_kg.openapi.yaml
-    (Individual)
+    Individual entity
+
     """
 
     def __init__(self, _id: ID, **kwargs):
+        """
+
+        :param _id: the individual identifier
+        :param kwargs:
+        """
         super().__init__(_id, **kwargs)
         self.__owl__ = OWL.NamedIndividual
         self.label = kwargs.get('label', _uri_label(self.id))
         self.kind = kwargs.get('kind', kwargs.get('kinds', [OWL.Thing]))  # back compatibility w 0.7
         self.comment = kwargs.get('comment', '')
         self.attributes = [AttributeInstance(**a_data) for a_data in
                            kwargs.get('attributes', list[AttributeInstance]())]
@@ -388,45 +421,45 @@
 
     def has_attribute(self, attribute_id: ID) -> bool:
         """
         Checks if the individual has a given ontology defined attribute
         :param attribute_id:
         :return:
         """
-        found = next(filter(lambda x: x.property == attribute_id, self.attributes), None)
+        found = next(filter(lambda x: x.predicate == attribute_id, self.attributes), None)
         return found and not found.is_empty()
 
     def get_attribute(self, attribute_id: ID) -> AttributeInstance | Any:
         """
         Gets the ontology defined attribute instance of the individual
         :param attribute_id:
         :return:
         """
-        found = next(filter(lambda x: x.property == attribute_id, self.attributes), None)
+        found = next(filter(lambda x: x.predicate == attribute_id, self.attributes), None)
         if found and not found.is_empty():
             return found
         else:
             return VOID_ATTRIBUTE
 
     def has_relation(self, relation_id: ID) -> bool:
         """
         Checks if the individual has a given ontology defined relation
         :param relation_id:
         :return:
         """
-        found = next(filter(lambda x: x.property == relation_id, self.relations), None)
+        found = next(filter(lambda x: x.predicate == relation_id, self.relations), None)
         return found and not found.is_empty()
 
     def get_relation(self, relation_id: ID) -> RelationInstance | Any:
         """
         Gets the ontology defined relation instance of the individual
         :param relation_id:
         :return:
         """
-        found = next(filter(lambda x: x.property == relation_id, self.relations), None)
+        found = next(filter(lambda x: x.predicate == relation_id, self.relations), None)
         if found and not found.is_empty():
             return found
         else:
             return VOID_RELATION
 
     def set_score(self, score: float):
         self.score = score
```

### Comparing `isagog_ai-0.8.0/isagog/model/kg_query.py` & `isagog_ai-0.8.1/isagog/model/kg_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,38 @@
 """
 from __future__ import annotations
 import logging
 import random
 import re
 from enum import Enum
 from typing import Protocol
-
+from urllib.parse import urlparse
 from rdflib import RDF, RDFS, OWL, URIRef
 
+from isagog.model.kg_model import Assertion
+
 DEFAULT_PREFIXES = [("rdf", "http://www.w3.org/2000/01/rdf-schema"),
                     ("rdfs", "http://www.w3.org/2001/XMLSchema"),
                     ("text", "http://jena.apache.org/text")]
 
 # don't change this for the sake of back compatibility
 _SUBJVAR = 'i'
 _KINDVAR = 'k'
 _SCOREVAR = 'score'
 
 
+def is_uri(string: str) -> bool:
+    parsed = urlparse(string)
+    return bool(parsed.scheme) and bool(parsed.netloc)
+
+
+def is_variable(string: str) -> bool:
+    return string.startswith('?')
+
+
 class Comparison(Enum):
     EXACT = "exact_match"
     KEYWORD = "keyword_search"
     REGEX = "regex"
     SIMILARITY = "similarity"
     GREATER = "greater_than"
     LESSER = "lesser_than"
@@ -37,15 +48,15 @@
     Must be an uri string, possibly prefixed
 
     """
 
     @staticmethod
     def is_valid_id(id_string):
         try:
-            if id_string.startswith('?'):
+            if is_variable(id_string):
                 return False
             URIRef(id_string)
             return True
         except Exception:
             return False
 
     def __new__(cls, _id: str | URIRef):
@@ -74,15 +85,15 @@
         try:
             Variable(var_string)
             return True
         except ValueError:
             return False
 
     @staticmethod
-    def is_valid_variable_id(var_string):
+    def is_valid_variable_id(var_string: str):
         return var_string.startswith('?')
 
     def __new__(cls, value=None):
 
         if not value:
             value = random.randint(0, 1000000)  # assume that conflicts are negligible
         if not (isinstance(value, str) or isinstance(value, int)):
@@ -106,26 +117,27 @@
 
 class Value(str):
     """
     Can be a string or a number
     """
 
     def __init__(self, value: str | int | float):
-        if isinstance(value, str) and ((value.startswith("<") and value.endswith(">")) or value.startswith("?")):
+        if isinstance(value, str) and (is_uri(value) or value.startswith("?")):
             raise ValueError(f"Bad value string {value}")
         self.value = value
 
     def __str__(self) -> str:
         return str(self.value)
 
 
 class Clause(object):
     """
     A selection clause
     """
+
     def __init__(self,
                  subject: Identifier | Variable | str = None,
                  optional=False):
         self.subject = subject
         self.optional = optional
 
     def to_dict(self, **kwargs) -> dict:
@@ -158,15 +170,15 @@
 
     @staticmethod
     def _instantiate_argument(arg) -> Value | Identifier | Variable:
         if isinstance(arg, Variable) or isinstance(arg, Identifier) or isinstance(arg, Value):
             return arg
         elif isinstance(arg, URIRef):
             return Identifier(arg)
-        elif isinstance(arg, int) or isinstance(arg, float) or isinstance(arg, str):
+        elif isinstance(arg, int) or isinstance(arg, float):
             return Value(arg)
         else:
             arg = str(arg)
             if arg.startswith('?'):
                 return Variable(arg)
             elif arg.startswith('<') or ':' in arg[:8]:
                 return Identifier(arg)
@@ -206,20 +218,23 @@
         :param property:
         :param argument:
         :param variable:
         :param method:
         :param project:
         :param optional:
         """
-
+        if subject and not isinstance(subject, Identifier) and not isinstance(subject, str):
+            raise ValueError("Invalid subject")
+        if property and not isinstance(property, Identifier) and not isinstance(property, str):
+            raise ValueError("Invalid property")
         super().__init__(subject=subject, optional=optional)
 
         self.subject = subject
         if self.subject and isinstance(subject, str):
-            self.subject = Variable(subject) if subject.startswith("?") else Identifier(subject)
+            self.subject = Variable(subject) if is_variable(subject) else Identifier(subject)
         self.property = property if property and isinstance(property, Identifier) \
             else Identifier(property) if property \
             else None
         self.argument = self._instantiate_argument(argument) if argument else None
         self.variable = self._instantiate_variable(variable) if variable else None
         self.method = method
         self.project = project
```

### Comparing `isagog_ai-0.8.0/LICENSE` & `isagog_ai-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.0/pyproject.toml` & `isagog_ai-0.8.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2269 7361 676f 672d 6169  ame = "isagog-ai
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 302e  "..version = "0.
-00000030: 382e 3022 0d0a 6465 7363 7269 7074 696f  8.0"..descriptio
+00000030: 382e 3122 0d0a 6465 7363 7269 7074 696f  8.1"..descriptio
 00000040: 6e20 3d20 2263 6c69 656e 7420 666f 7220  n = "client for 
 00000050: 6973 6167 6f67 2061 6920 7365 7276 6963  isagog ai servic
 00000060: 6573 220d 0a61 7574 686f 7273 203d 205b  es"..authors = [
 00000070: 2247 7569 646f 2056 6574 6572 6520 3c67  "Guido Vetere <g
 00000080: 2e76 6574 6572 6540 6973 6167 6f67 2e63  .vetere@isagog.c
 00000090: 6f6d 3e22 5d0d 0a72 6561 646d 6520 3d20  om>"]..readme = 
 000000a0: 2252 4541 444d 452e 6d64 220d 0a70 6163  "README.md"..pac
@@ -23,14 +23,15 @@
 00000160: 0d0a 7264 666c 6962 203d 2022 5e37 2e30  ..rdflib = "^7.0
 00000170: 2e30 220d 0a72 6571 7565 7374 7320 3d20  .0"..requests = 
 00000180: 225e 322e 3238 2e32 220d 0a75 726c 6c69  "^2.28.2"..urlli
 00000190: 6233 203d 2022 5e32 2e30 2e36 220d 0a74  b3 = "^2.0.6"..t
 000001a0: 6f6d 6c20 3d20 225e 302e 3130 2e32 220d  oml = "^0.10.2".
 000001b0: 0a70 7974 6573 7420 3d20 225e 382e 312e  .pytest = "^8.1.
 000001c0: 3122 0d0a 7079 7468 6f6e 2d64 6f74 656e  1"..python-doten
-000001d0: 7620 3d20 225e 312e 302e 3022 0d0a 0d0a  v = "^1.0.0"....
-000001e0: 0d0a 5b62 7569 6c64 2d73 7973 7465 6d5d  ..[build-system]
-000001f0: 0d0a 7265 7175 6972 6573 203d 205b 2270  ..requires = ["p
-00000200: 6f65 7472 792d 636f 7265 225d 0d0a 6275  oetry-core"]..bu
-00000210: 696c 642d 6261 636b 656e 6420 3d20 2270  ild-backend = "p
-00000220: 6f65 7472 792e 636f 7265 2e6d 6173 6f6e  oetry.core.mason
-00000230: 7279 2e61 7069 220d 0a                   ry.api"..
+000001d0: 7620 3d20 225e 312e 302e 3022 0d0a 6874  v = "^1.0.0"..ht
+000001e0: 7470 7820 3d20 225e 302e 3237 2e30 220d  tpx = "^0.27.0".
+000001f0: 0a0d 0a0d 0a5b 6275 696c 642d 7379 7374  .....[build-syst
+00000200: 656d 5d0d 0a72 6571 7569 7265 7320 3d20  em]..requires = 
+00000210: 5b22 706f 6574 7279 2d63 6f72 6522 5d0d  ["poetry-core"].
+00000220: 0a62 7569 6c64 2d62 6163 6b65 6e64 203d  .build-backend =
+00000230: 2022 706f 6574 7279 2e63 6f72 652e 6d61   "poetry.core.ma
+00000240: 736f 6e72 792e 6170 6922 0d0a            sonry.api"..
```

### Comparing `isagog_ai-0.8.0/PKG-INFO` & `isagog_ai-0.8.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: isagog-ai
-Version: 0.8.0
+Version: 0.8.1
 Summary: client for isagog ai services
 Author: Guido Vetere
 Author-email: g.vetere@isagog.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rdflib (>=7.0.0,<8.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: urllib3 (>=2.0.6,<3.0.0)
 Description-Content-Type: text/markdown
```

