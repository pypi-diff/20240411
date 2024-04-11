# Comparing `tmp/sommify-0.8.3.tar.gz` & `tmp/sommify-0.8.4.tar.gz`

## Comparing `sommify-0.8.3.tar` & `sommify-0.8.4.tar`

### file list

```diff
@@ -1,51 +1,53 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sommify-0.8.3/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/__init__.py
--rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/regex.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/test.py
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/utils.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/countries/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/__init__.py
--rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/categories.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/constants.py
--rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/cuisine.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/embeddings.py
--rw-r--r--   0        0        0   356666 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredient_funnel.py
--rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredients.py
--rw-r--r--   0        0        0  5768681 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/mean_ing_embedding_per_tag.csv
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/meat.py
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/modifiers.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/vegetables.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/vulgar_fractions.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredient_categories/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredient_categories/cheeses.py
--rw-r--r--   0        0        0     8421 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredient_categories/drinks.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredient_categories/fruit.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredient_categories/herbs.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredient_categories/legumes.py
--rw-r--r--   0        0        0     7426 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredient_categories/meats.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredient_categories/nuts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredient_categories/pasta.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredient_categories/spices.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/data/ingredient_categories/vegetables.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/prompts/__init__.py
--rw-r--r--   0        0        0    47884 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/prompts/data/__init__.py
--rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/prompts/data/default.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/pygrape/__init__.py
--rw-r--r--   0        0        0   367143 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/pygrape/data.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/pyregion/__init__.py
--rw-r--r--   0        0        0    53240 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/pyregion/data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/recipes/__init__.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/recipes/elastic.py
--rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/recipes/reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/tests/__init__.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/tests/test_elastic.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/tests/test_prompts.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/tests/test_pygrape.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/tests/test_pyregion.py
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/tests/test_recipe_reader.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sommify-0.8.3/sommify/tests/test_tag_reader.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 sommify-0.8.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sommify-0.8.3/LICENSE
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sommify-0.8.3/README.md
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 sommify-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 sommify-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sommify-0.8.4/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/__init__.py
+-rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/regex.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/test.py
+-rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/utils.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/countries/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/__init__.py
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/categories.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/constants.py
+-rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/cuisine.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/embeddings.py
+-rw-r--r--   0        0        0   356666 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_funnel.py
+-rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredients.py
+-rw-r--r--   0        0        0  5768681 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/mean_ing_embedding_per_tag.csv
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/meat.py
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/modifiers.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/vegetables.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/vulgar_fractions.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/cheeses.py
+-rw-r--r--   0        0        0     8421 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/drinks.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/fruit.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/herbs.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/legumes.py
+-rw-r--r--   0        0        0     7426 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/meats.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/nuts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/pasta.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/spices.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/data/ingredient_categories/vegetables.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/prompts/__init__.py
+-rw-r--r--   0        0        0    47884 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/prompts/data/__init__.py
+-rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/prompts/data/default.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/pygrape/__init__.py
+-rw-r--r--   0        0        0   367143 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/pygrape/data.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/pynotesandhints/__init__.py
+-rw-r--r--   0        0        0    63339 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/pynotesandhints/data.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/pyregion/__init__.py
+-rw-r--r--   0        0        0    53240 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/pyregion/data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/recipes/__init__.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/recipes/elastic.py
+-rw-r--r--   0        0        0    15852 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/recipes/reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/test_elastic.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/test_prompts.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/test_pygrape.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/test_pyregion.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/test_recipe_reader.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sommify-0.8.4/sommify/tests/test_tag_reader.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 sommify-0.8.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sommify-0.8.4/LICENSE
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sommify-0.8.4/README.md
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 sommify-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 sommify-0.8.4/PKG-INFO
```

### Comparing `sommify-0.8.3/sommify/regex.py` & `sommify-0.8.4/sommify/regex.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/test.py` & `sommify-0.8.4/sommify/test.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/utils.py` & `sommify-0.8.4/sommify/utils.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/countries/__init__.py` & `sommify-0.8.4/sommify/countries/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/categories.py` & `sommify-0.8.4/sommify/data/categories.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/constants.py` & `sommify-0.8.4/sommify/data/constants.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/cuisine.py` & `sommify-0.8.4/sommify/data/cuisine.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/embeddings.py` & `sommify-0.8.4/sommify/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/ingredient_funnel.py` & `sommify-0.8.4/sommify/data/ingredient_funnel.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/ingredients.py` & `sommify-0.8.4/sommify/data/ingredients.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/mean_ing_embedding_per_tag.csv` & `sommify-0.8.4/sommify/data/mean_ing_embedding_per_tag.csv`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/meat.py` & `sommify-0.8.4/sommify/data/meat.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/modifiers.py` & `sommify-0.8.4/sommify/data/modifiers.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/vegetables.py` & `sommify-0.8.4/sommify/data/vegetables.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/ingredient_categories/__init__.py` & `sommify-0.8.4/sommify/data/ingredient_categories/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/ingredient_categories/drinks.py` & `sommify-0.8.4/sommify/data/ingredient_categories/drinks.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/ingredient_categories/fruit.py` & `sommify-0.8.4/sommify/data/ingredient_categories/fruit.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/ingredient_categories/herbs.py` & `sommify-0.8.4/sommify/data/ingredient_categories/herbs.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/ingredient_categories/meats.py` & `sommify-0.8.4/sommify/data/ingredient_categories/meats.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/ingredient_categories/nuts.py` & `sommify-0.8.4/sommify/data/ingredient_categories/nuts.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/ingredient_categories/spices.py` & `sommify-0.8.4/sommify/data/ingredient_categories/spices.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/data/ingredient_categories/vegetables.py` & `sommify-0.8.4/sommify/data/ingredient_categories/vegetables.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/prompts/__init__.py` & `sommify-0.8.4/sommify/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/prompts/data/__init__.py` & `sommify-0.8.4/sommify/prompts/data/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/prompts/data/default.py` & `sommify-0.8.4/sommify/prompts/data/default.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/pygrape/__init__.py` & `sommify-0.8.4/sommify/pygrape/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/pygrape/data.py` & `sommify-0.8.4/sommify/pygrape/data.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/pyregion/__init__.py` & `sommify-0.8.4/sommify/pyregion/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/pyregion/data.py` & `sommify-0.8.4/sommify/pyregion/data.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/recipes/elastic.py` & `sommify-0.8.4/sommify/recipes/elastic.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/sommify/recipes/reader.py` & `sommify-0.8.4/sommify/recipes/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from unidecode import unidecode
 
 try:
     spacy.load("en_core_web_sm")
 except OSError:
     print("Downloading language model for the spaCy")
     from spacy.cli import download
+
     download("en_core_web_sm")
     print("Download complete")
 
 
 from .. import regex as re_
 
 # from data.ingredient_funnel import dictionary as ing_funnel
@@ -341,15 +342,15 @@
 
     def read(
         self,
         title: str,
         phrases: list[str],
         steps: list[str] = list,
         ing_parsed: bool = False,
-        version: int = 'v1',
+        version: int = "v1",
     ) -> object:
         parsed_phrases = [self.read_phrase(p) for p in phrases]
         parsed_phrases = self.merge_ingredients([p for p in parsed_phrases if p])
 
         if ing_parsed:
             ingredients = phrases
         else:
@@ -363,16 +364,18 @@
         columns = sorted(set(ing_funnel.values()))
         if "niche" in categories:
             categories = ["niche"]
 
         _models = self.categories_to_models(categories)
 
         values = np.array([1 if c in ingredients else 0 for c in columns])
-        if version == 'v2':
-            values = np.append(values, [1 if m in _models else 0 for m in models.keys()])
+        if version == "v2":
+            values = np.append(
+                values, [1 if m in _models else 0 for m in models.keys()]
+            )
 
         return {
             "ingredients": ingredients,
             "ingredients_": parsed_phrases,
             "title": title,
             "categories": categories,
             "models": _models,
```

### Comparing `sommify-0.8.3/sommify/tests/test_elastic.py` & `sommify-0.8.4/sommify/tests/test_elastic.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,37 +3,38 @@
 from dotenv import load_dotenv
 
 from sommify.recipes import elastic
 from sommify.recipes.reader import RecipeReader
 
 load_dotenv()
 
-ELASTIC_URL=os.getenv("ELASTIC_URL")
+ELASTIC_URL = os.getenv("ELASTIC_URL")
 
-ELASTIC_PASSWORD=os.getenv("ELASTIC_PASSWORD")
-ELASTIC_CLOUD_ID=os.getenv("ELASTIC_CLOUD_ID")
+ELASTIC_PASSWORD = os.getenv("ELASTIC_PASSWORD")
+ELASTIC_CLOUD_ID = os.getenv("ELASTIC_CLOUD_ID")
+
+ELASTIC_PASSWORD = os.getenv("ELASTIC_PASSWORD")
+ELASTIC_USERNAME = os.getenv("ELASTIC_USERNAME")
+ELASTIC_PORT = os.getenv("ELASTIC_PORT")
 
-ELASTIC_PASSWORD=os.getenv("ELASTIC_PASSWORD")
-ELASTIC_USERNAME=os.getenv("ELASTIC_USERNAME")
-ELASTIC_PORT=os.getenv("ELASTIC_PORT")
 
 def test_elastic_search_by_query_term() -> bool:
     try:
         r = RecipeReader(ELASTIC_URL, ELASTIC_USERNAME, ELASTIC_PASSWORD)
         input_term = "reindeer"
         found_ings = r.extract_ingredients(input_term)
-        elastic.search_by_query_term(r.es,input_term,found_ings)[1]
+        elastic.search_by_query_term(r.es, input_term, found_ings)[1]
         assert True
     except Exception as e:
         print(e)
         raise AssertionError()
 
+
 def test_elastic_read_terms() -> bool:
     try:
         r = RecipeReader(ELASTIC_URL, ELASTIC_USERNAME, ELASTIC_PASSWORD)
         input_term = "reindeer"
         r.read_terms(input_term)
         assert True
     except Exception as e:
         print(e)
         raise AssertionError()
-
```

### Comparing `sommify-0.8.3/sommify/tests/test_prompts.py` & `sommify-0.8.4/sommify/tests/test_prompts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 from sommify.prompts import (
     country_entity_to_iso,
     extract_mentions_naive,
     region_entity_to_closest,
 )
 
-extract_mentions_naive("france", region_pool=["france"], subregion_pool=["bordeaux"], grape_pool=["pinot"])
+extract_mentions_naive(
+    "france", region_pool=["france"], subregion_pool=["bordeaux"], grape_pool=["pinot"]
+)
+
 
 def test_extract_mentions_naive() -> bool:
-    assert extract_mentions_naive("france", region_pool=["france"], subregion_pool=["bordeaux"], grape_pool=["pinot"])['regions'] == ['france']
+    assert extract_mentions_naive(
+        "france",
+        region_pool=["france"],
+        subregion_pool=["bordeaux"],
+        grape_pool=["pinot"],
+    )["regions"] == ["france"]
+
 
 def test_country_entity_to_iso() -> bool:
     assert country_entity_to_iso("slovakia") == "SK"
 
+
 def test_region_entity_to_closest() -> bool:
     assert region_entity_to_closest("bordeau") == "Bordeaux"
```

### Comparing `sommify-0.8.3/.gitignore` & `sommify-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/LICENSE` & `sommify-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sommify-0.8.3/pyproject.toml` & `sommify-0.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "sommify"
-version = "0.8.3"
+version = "0.8.4"
 authors = [
   { name="William Brach", email="william@sommify.ai" },
   { name="Tomas Bedej", email="tomas@sommify.ai" },
 ]
 description = "A package for recipe parsing"
 dependencies = [
   "inflect==7.0.0",
```

### Comparing `sommify-0.8.3/PKG-INFO` & `sommify-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sommify
-Version: 0.8.3
+Version: 0.8.4
 Summary: A package for recipe parsing
 Author-email: William Brach <william@sommify.ai>, Tomas Bedej <tomas@sommify.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

