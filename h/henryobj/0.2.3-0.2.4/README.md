# Comparing `tmp/henryobj-0.2.3.tar.gz` & `tmp/henryobj-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henryobj-0.2.3.tar", last modified: Wed Apr 10 09:35:51 2024, max compression
+gzip compressed data, was "henryobj-0.2.4.tar", last modified: Thu Apr 11 08:34:22 2024, max compression
```

## Comparing `henryobj-0.2.3.tar` & `henryobj-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-10 09:35:51.446456 henryobj-0.2.3/
--rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-10 09:35:51.446309 henryobj-0.2.3/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)     2976 2024-01-24 08:03:39.000000 henryobj-0.2.3/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-10 09:35:51.445292 henryobj-0.2.3/henryobj/
--rw-r--r--   0 henry      (501) staff       (20)      224 2024-04-09 07:08:41.000000 henryobj-0.2.3/henryobj/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)    22625 2024-04-10 09:35:29.000000 henryobj-0.2.3/henryobj/base.py
--rw-r--r--   0 henry      (501) staff       (20)     1543 2024-04-10 09:35:13.000000 henryobj-0.2.3/henryobj/config.py
--rw-r--r--   0 henry      (501) staff       (20)    15087 2024-03-30 15:15:07.000000 henryobj-0.2.3/henryobj/gpt.py
--rw-r--r--   0 henry      (501) staff       (20)    28883 2024-04-09 16:04:06.000000 henryobj-0.2.3/henryobj/oai.py
--rw-r--r--   0 henry      (501) staff       (20)    14268 2024-03-30 15:59:40.000000 henryobj-0.2.3/henryobj/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-10 09:35:51.446083 henryobj-0.2.3/henryobj.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-10 09:35:51.000000 henryobj-0.2.3/henryobj.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      282 2024-04-10 09:35:51.000000 henryobj-0.2.3/henryobj.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-04-10 09:35:51.000000 henryobj-0.2.3/henryobj.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       60 2024-04-10 09:35:51.000000 henryobj-0.2.3/henryobj.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)        9 2024-04-10 09:35:51.000000 henryobj-0.2.3/henryobj.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-04-10 09:35:51.446520 henryobj-0.2.3/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      574 2024-04-10 09:35:42.000000 henryobj-0.2.3/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-11 08:34:22.203877 henryobj-0.2.4/
+-rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-11 08:34:22.203737 henryobj-0.2.4/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)     2976 2024-01-24 08:03:39.000000 henryobj-0.2.4/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-11 08:34:22.202944 henryobj-0.2.4/henryobj/
+-rw-r--r--   0 henry      (501) staff       (20)      224 2024-04-09 07:08:41.000000 henryobj-0.2.4/henryobj/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)    22625 2024-04-11 08:30:24.000000 henryobj-0.2.4/henryobj/base.py
+-rw-r--r--   0 henry      (501) staff       (20)     1543 2024-04-10 09:35:13.000000 henryobj-0.2.4/henryobj/config.py
+-rw-r--r--   0 henry      (501) staff       (20)    13971 2024-04-11 08:30:55.000000 henryobj-0.2.4/henryobj/gpt.py
+-rw-r--r--   0 henry      (501) staff       (20)    29571 2024-04-11 08:29:52.000000 henryobj-0.2.4/henryobj/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)    14268 2024-04-11 08:33:40.000000 henryobj-0.2.4/henryobj/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-11 08:34:22.203559 henryobj-0.2.4/henryobj.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-11 08:34:22.000000 henryobj-0.2.4/henryobj.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      282 2024-04-11 08:34:22.000000 henryobj-0.2.4/henryobj.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-04-11 08:34:22.000000 henryobj-0.2.4/henryobj.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       60 2024-04-11 08:34:22.000000 henryobj-0.2.4/henryobj.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)        9 2024-04-11 08:34:22.000000 henryobj-0.2.4/henryobj.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-04-11 08:34:22.203919 henryobj-0.2.4/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      574 2024-04-11 08:30:11.000000 henryobj-0.2.4/setup.py
```

### Comparing `henryobj-0.2.3/PKG-INFO` & `henryobj-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henryobj
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/HenryObj/mypip
 Description-Content-Type: text/markdown
 
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
```

### Comparing `henryobj-0.2.3/README.md` & `henryobj-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.3/henryobj/base.py` & `henryobj-0.2.4/henryobj/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import os
 import re
 
 
 # *************************************** General Utilities ***************************************
 
 def check_co() -> bool:
-    '''
+    """
     Returns true if we have an internet connection. False otherwise.
-    '''
+    """
     try:
         requests.head("http://google.com")
         return True
     except Exception:
         return False
 
 def check__if_password_safe(password: str) -> bool:
```

### Comparing `henryobj-0.2.3/henryobj/config.py` & `henryobj-0.2.4/henryobj/config.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.3/henryobj/gpt.py` & `henryobj-0.2.4/henryobj/gpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -288,27 +288,8 @@
     4. Do not give general comments, ONLY specific issues with the way to resolve them in Markdown format. If you don't find any issue, simply say "No issue found".
     """)
 
 # *************************************************************************************************
 # *************************************************************************************************
     
 if __name__ == "__main__":
-    pass
-   
-# WIP for future functions
-'''
-# Example of Request
-REQUEST_WRITE_TEST = """
-Write all the tests functions to ensure that the endpoints are correctly working. 
-The tests must be broken down into smaller functions. If data is added to the DB, the data should then be removed from the DB if possible (ex: using the /delete endpoint).
-print() statements must be used extensively to log on the console the various step and results of those tests.
-Below is an example for the endpoints /training. Obviously, you need to do something more complete that this example and test ALL endpoints by calling one main functions which itself calls many smaller functions.
-Provide a perfect code, ready to use, with all typing hints and simple docstrings.
-"""
-
-# Example of Request
-REQUEST_REFACTOR = """
-The file assistant.py is poorly made. It composes code snippets, some are useful, others are not. 
-What we want is to refactor all this code to have all functions written as cleanly as oai_upload_file.
-Write all functions needed to achieve the above results. Only return the code with the typing hint for each one.
-"""
-'''
+    pass
```

### Comparing `henryobj-0.2.3/henryobj/oai.py` & `henryobj-0.2.4/henryobj/oai.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,28 +138,43 @@
     # Updated pattern to include "as a large language model" and remove less specific phrases.
     pattern = r'\b(as an ai|as a large language model|as a chatbot|as a virtual assistant|'\
               r'as a bot|as an artificial intelligence|as an automated|'\
               r'Assistant:|GPT-?\d+|OpenAI)\b'
     # re.IGNORECASE makes the search case-insensitive.
     return bool(re.search(pattern, text, re.IGNORECASE))
 
-def check_if_gptconv_format(conversation: list[dict[str, str]]) -> bool:
+def check_if_gptconv_format(conversation: list[dict[str, str]]) -> Optional[bool]:
     """
     Checks if the structure of the list matches the GPT conversation format.
     
     Returns:
     - bool: True if valid, False otherwise.
     """
+    allowed_roles = {'user', 'assistant', 'system'}
     for entry in conversation:
-        if not set(entry.keys()) == {'role', 'content'}:
-            return False
-        if not isinstance(entry['role'], str) or not isinstance(entry['content'], str):
-            return False
+        if not set(entry.keys()) == {'role', 'content'}: return
+        if not isinstance(entry['role'], str) or not isinstance(entry['content'], str): return
+        if entry['role'] not in allowed_roles: return
     return True
 
+def check_valid_gpt_conversation(possible_gpt_conv) -> Optional[bool]:
+    """
+    Returns True / False depending on whether it is a valid GPT conv.
+    
+    Args:
+        Can be a string or list, it doesn't matter. It will check that the internal elements match the GPT format.
+    """
+    try:
+        gpt_conv = possible_gpt_conv if isinstance(possible_gpt_conv, list) else json.loads(possible_gpt_conv)
+        if not isinstance(gpt_conv, list): return
+        if not all([isinstance(elem, dict) for elem in gpt_conv]): return
+        return check_if_gptconv_format(gpt_conv)
+    except:
+        return
+
 def new_chunk_text(text: str, target_token: int = 200) -> list[str]:
     """
     Much simpler function to chunk the text in blocks by spliting by sentence. The last chunk might be small.
     """
     tok_text = calculate_token(text)
     if tok_text < 1.1 * target_token:
         return [text]
```

### Comparing `henryobj-0.2.3/henryobj/web.py` & `henryobj-0.2.4/henryobj/web.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 import requests
 import random
 import time
 import re
 
 # ****** SET UP SESSION OBJECT FOR SCRAPPING *******
 
-'''
+"""
     500: Internal Server Error, which indicates that the server encountered an error while processing the request.
     502: Bad Gateway, which indicates that the server, while acting as a gateway or proxy, received an invalid response from the upstream server it accessed in attempting to fulfill the request.
     504: Gateway Timeout, which indicates that the server, while acting as a gateway or proxy, did not receive a timely response from the upstream server.
     These status codes are chosen because they represent temporary issues that may be resolved on subsequent requests.
-'''
+"""
 
 def create_session(max_retries: int = 3, backoff_factor: float = 0.3, status_forcelist: tuple = (500, 502, 504)) -> requests.Session:
     """
     Create and configure a requests.Session object.
     """
     session = requests.Session()
     retry = Retry(
@@ -121,18 +121,18 @@
     """
     parsed_url = urlparse(url)
     domain = parsed_url.netloc.replace('www.', '')
     path = parsed_url.path.strip('/')
     return f"{domain}/{path}"
 
 def content_type_is_text(content_type):
-    '''
+    """
     Used to skip if content_type.startswith("image") or content_type.startswith("application/pdf").
     Now, we skip if it's not text or xml.
-    '''
+    """
     if content_type.startswith("text") or content_type.startswith("application/xhtml+xml"):
         return True
     else:
         return False
 
 def crawl_handle_fetch_result(future, data_name, memory_store) -> None:
     """
@@ -220,18 +220,18 @@
         log_issue(e, fetch_content_url, f"SSL/TLS error for url {url}")
         return None
     except Exception as e:
         log_issue(e, fetch_content_url, f"For url {url}")
         return None
 
 def is_useful_link(tag):
-    '''
+    """
     Mini function to check if a link is surrounded with content, hence useful, or alone.
     Return True if useful, False otherwise.
-    '''
+    """
    # Check previous and next siblings
     prev_sibling = tag.previous_sibling
     next_sibling = tag.next_sibling
     if prev_sibling and prev_sibling.string and prev_sibling.string.strip() != '':
         return True
     if next_sibling and next_sibling.string and next_sibling.string.strip() != '':
         return True
@@ -240,18 +240,18 @@
     if parent:
         text_without_link = parent.get_text().replace(tag.get_text(), '').strip()
         if text_without_link:
             return True
     return False
 
 def fetch_domain_links(local_domain, url):
-    '''
+    """
     Returns the list of all unique urls of a given domain. Search start from a specific page (url).
     Doesn't return links that are not part of the domain.
-    '''
+    """
     clean_links = set()
     try:
         raw_links = fetch_hyperlinks(url)
         if raw_links is None:
             print("No hyperlink", fetch_domain_links, f"For {url} and {local_domain}")
             return []
         for link in set(raw_links):
@@ -306,46 +306,46 @@
     # Use regex to split text into sentences
     #re.split(r'(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?)\s', text)
     sentences = re.split('(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?)\s', text)
     cleaned_sentences = [sentence for sentence in sentences if len(sentence.split()) <= max_words]
     return ' '.join(cleaned_sentences)
 
 def remove_reviews(soup : BeautifulSoup) -> BeautifulSoup:
-    '''
+    """
     Slightly risky function which removes the reviews from a Shopify store.
-    '''
+    """
     pattern = re.compile(r'data-verified-.*|review.*')
     for div in soup.find_all('div'):
         if div.attrs is not None: 
             div_class = div.get('class')
             if div_class is not None and any(pattern.match(class_) for class_ in div_class):
                 div.decompose()
     return soup
 
 def wrap_handle_fetch_result(future, data_name, memory_store):
-    '''
+    """
     Wrapper to allow adding paramaters to the callback function.
-    '''
+    """
     crawl_handle_fetch_result(future, data_name, memory_store)
 
 def check_valid_url(url):
-    '''
+    """
     Function which takes a string and return True if the url is valid.
-    '''
+    """
     try:
         result = urlparse(url)
         if len(result.netloc) <= 1: return False # Checks if the user has put a local file
         return all([result.scheme, result.netloc])
     except ValueError:
         return False
 
 def clean_url(url):
-    '''
+    """
     User-submitted urls might not be perfectly fit to be processed by check_valid_url
-    '''
+    """
     url = url.strip()
     if not url.startswith('http'):
         url = 'https://' + url
     parsed_url = urlparse(url)
 
     # Clean the domain by removing any unwanted characters
     cleaned_netloc = re.sub(r'[^a-zA-Z0-9\.\-]', '', parsed_url.netloc)
@@ -354,18 +354,18 @@
     unquoted_path = unquote(parsed_url.path)
     quoted_path = quote(unquoted_path)
 
     cleaned_url = urlunparse(parsed_url._replace(netloc=cleaned_netloc, path=quoted_path))
     return cleaned_url
 
 def get_local_domain(from_url):
-    '''
+    """
     Get the local domain from a given URL.
     Will return the same domain for https://chat.openai.com/chat" and https://openai.com/chat".
-    '''
+    """
     try:
         netloc = urlparse(from_url).netloc
         parts = netloc.split(".")
         if len(parts) > 2:
             domain = parts[-2]
         else:
             domain = parts[0]
```

### Comparing `henryobj-0.2.3/henryobj.egg-info/PKG-INFO` & `henryobj-0.2.4/henryobj.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henryobj
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/HenryObj/mypip
 Description-Content-Type: text/markdown
 
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
```

### Comparing `henryobj-0.2.3/setup.py` & `henryobj-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="henryobj",
-    version="0.2.3", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.2.4", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/mypip',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

