# Comparing `tmp/telugu_words_numbers-0.0.6.tar.gz` & `tmp/telugu_words_numbers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telugu_words_numbers-0.0.6.tar", last modified: Tue Apr  9 18:31:49 2024, max compression
+gzip compressed data, was "dist\telugu_words_numbers-0.0.7.tar", last modified: Thu Apr 11 18:39:25 2024, max compression
```

## Comparing `telugu_words_numbers-0.0.6.tar` & `telugu_words_numbers-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 18:31:49.119846 telugu_words_numbers-0.0.6/
--rw-rw-rw-   0        0        0     1091 2024-04-09 15:10:22.000000 telugu_words_numbers-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3372 2024-04-09 18:31:49.119846 telugu_words_numbers-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2695 2024-04-09 18:04:30.000000 telugu_words_numbers-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 18:31:49.119846 telugu_words_numbers-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1373 2024-04-09 18:31:41.000000 telugu_words_numbers-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:31:49.104223 telugu_words_numbers-0.0.6/telugu_words_numbers/
--rw-rw-rw-   0        0        0      122 2024-04-09 17:46:35.000000 telugu_words_numbers-0.0.6/telugu_words_numbers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:31:49.119846 telugu_words_numbers-0.0.6/telugu_words_numbers/json_files/
--rw-rw-rw-   0        0        0      214 2024-04-09 14:21:45.000000 telugu_words_numbers-0.0.6/telugu_words_numbers/json_files/telugu_currency_units.json
--rw-rw-rw-   0        0        0    11500 2024-04-09 14:21:45.000000 telugu_words_numbers-0.0.6/telugu_words_numbers/json_files/telugu_numbers.json
--rw-rw-rw-   0        0        0     7806 2024-04-09 18:28:11.000000 telugu_words_numbers-0.0.6/telugu_words_numbers/telugu_word_to_number.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:31:49.104223 telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/
--rw-rw-rw-   0        0        0     3372 2024-04-09 18:31:48.000000 telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2024-04-09 18:31:48.000000 telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 18:31:48.000000 telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-09 18:31:48.000000 telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-09 18:31:48.000000 telugu_words_numbers-0.0.6/telugu_words_numbers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 18:39:25.834853 telugu_words_numbers-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2024-04-09 15:10:22.000000 telugu_words_numbers-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5753 2024-04-11 18:39:25.819232 telugu_words_numbers-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5292 2024-04-11 18:31:57.000000 telugu_words_numbers-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 18:39:25.834853 telugu_words_numbers-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2024-04-11 18:35:25.000000 telugu_words_numbers-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 18:39:25.819232 telugu_words_numbers-0.0.7/telugu_words_numbers/
+-rw-rw-rw-   0        0        0      122 2024-04-09 17:46:35.000000 telugu_words_numbers-0.0.7/telugu_words_numbers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 18:39:25.819232 telugu_words_numbers-0.0.7/telugu_words_numbers/json_files/
+-rw-rw-rw-   0        0        0    11500 2024-04-09 14:21:45.000000 telugu_words_numbers-0.0.7/telugu_words_numbers/json_files/telugu_numbers.json
+-rw-rw-rw-   0        0        0     5880 2024-04-11 18:28:46.000000 telugu_words_numbers-0.0.7/telugu_words_numbers/telugu_word_to_number.py
+drwxrwxrwx   0        0        0        0 2024-04-11 18:39:25.819232 telugu_words_numbers-0.0.7/telugu_words_numbers.egg-info/
+-rw-rw-rw-   0        0        0     5753 2024-04-11 18:39:24.000000 telugu_words_numbers-0.0.7/telugu_words_numbers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-04-11 18:39:24.000000 telugu_words_numbers-0.0.7/telugu_words_numbers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 18:39:24.000000 telugu_words_numbers-0.0.7/telugu_words_numbers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-11 18:39:24.000000 telugu_words_numbers-0.0.7/telugu_words_numbers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-11 18:39:24.000000 telugu_words_numbers-0.0.7/telugu_words_numbers.egg-info/top_level.txt
```

### Comparing `telugu_words_numbers-0.0.6/LICENSE` & `telugu_words_numbers-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `telugu_words_numbers-0.0.6/setup.py` & `telugu_words_numbers-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-with codecs.open(os.path.join(here, "README.srt"), encoding="utf-8") as fh:
+with codecs.open(os.path.join(here, "DESCRIPTION.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 # Setting up
 setup(
     name="telugu_words_numbers",
     packages=find_packages(),
     package_data={'telugu_words_numbers': ['json_files/*.json']},
-    version='0.0.6',
+    version='0.0.7',
     license='MIT',
     author="Sandeep Panchal",
     author_email="sandeep.panchal545@gmail.com",
     description='Telugu words to numbers conversion',
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/Sandeep-Panchal/telugu-word-to-number-conversion/tree/main",
```

### Comparing `telugu_words_numbers-0.0.6/telugu_words_numbers/json_files/telugu_numbers.json` & `telugu_words_numbers-0.0.7/telugu_words_numbers/json_files/telugu_numbers.json`

 * *Files identical despite different names*

### Comparing `telugu_words_numbers-0.0.6/telugu_words_numbers/telugu_word_to_number.py` & `telugu_words_numbers-0.0.7/telugu_words_numbers/telugu_word_to_number.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 
         # creating an instance of the text2digit
         self.t2d = text2digits.Text2Digits()
 
         # get the json files path
         self.dir_name = os.path.dirname(__file__)
         self.tel_num_json = os.path.join(self.dir_name, "json_files", "telugu_numbers.json")
-        self.tel_cur_json = os.path.join(self.dir_name, "json_files", "telugu_currency_units.json")
         
         # load the json files
         self.num_word_dict = self.json_load_method(self.tel_num_json)["telugu_dict"]
-        self.currency_units_dict = self.json_load_method(self.tel_cur_json)["telugu_units"]
 
         # thresholds of unigram and bigram
         self.unigram_threshold, self.bigram_threshold = 0.8, 0.9
 
     # method to load json files
     def json_load_method(self,
                          filename: str
@@ -88,55 +86,14 @@
                 flag = True
 
         if flag and l:
             return sum(l)
         else:
             return None
 
-    # method logic for telugu rupees and paise
-    def rupees_paise_logic(self,
-                           text: str
-                        ) -> Union[int, float]:
-
-        # get the paise and rupees variations
-        paise_variations = self.currency_units_dict["paise_unit"]
-        rupees_variations = self.currency_units_dict["rupees_unit"]
-
-        if any(variation in text for variation in paise_variations):
-            try:
-                if any(variation in text for variation in rupees_variations):
-                    for variation in rupees_variations:
-                        if variation in text:
-                            parts = text.split(variation)
-                            paise_amount = self.t2d.convert(parts[1])
-                            paise_amount = float(re.sub(r"\D", "", paise_amount))
-
-                            rupees_amount = self.t2d.convert(parts[0])
-                            rupees_amount = float(re.sub(r"\D", "", rupees_amount))
-                            amt = rupees_amount + (paise_amount / 100)
-                else:
-                    txt_amt = self.t2d.convert(text)
-                    amt = self.handle_thousand_pattern(txt_amt)
-                    if amt:
-                        amt = amt / 100
-                    else:
-                        amt = float(re.sub(r"\D", "", txt_amt)) / 100
-            except:
-                amt = 0
-        else:
-            try:
-                txt_amt = self.t2d.convert(text)
-                amt = self.handle_thousand_pattern(txt_amt)
-                if not amt:
-                    amt = float(re.sub(r"\D", "", txt_amt))
-            except:
-                amt = 0
-
-        return amt
-
     # method for n-gram (uni-gram and bi-gram)
     def n_gram_method(self,
                       text_org: str
                     ) -> str:
 
         # calling create_num_dict to get number dictionaries
         tel_dict_1, tel_dict_2 = self.create_num_dict()
@@ -200,17 +157,16 @@
                     .replace("500", "5 100")
                     .replace("600", "6 100")
                     .replace("700", "7 100")
                     .replace("800", "8 100")
                     .replace("900", "9 100")
                 )
 
-            # calling telugu_paise_logic function for paise logic
-            num = self.rupees_paise_logic(text_org)
-
             # applying number logic with package text2digit
             converted_text = self.t2d.convert(text_org)
+            num = re.sub(r"\D", " ", converted_text)
+            num = re.sub(" +", " ", num).strip()
+            num = list(num.split())
             return num, converted_text
 
         except:
-            num = 0
-            return num, None
+            return None, None
```

