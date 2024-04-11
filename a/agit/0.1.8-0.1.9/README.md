# Comparing `tmp/agit-0.1.8.tar.gz` & `tmp/agit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agit-0.1.8.tar", last modified: Fri Nov 10 04:47:12 2023, max compression
+gzip compressed data, was "agit-0.1.9.tar", last modified: Fri Nov 10 05:10:04 2023, max compression
```

## Comparing `agit-0.1.8.tar` & `agit-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2023-11-10 04:47:12.130090 agit-0.1.8/
--rw-r--r--   0 chenhao    (501) staff       (20)      212 2023-11-10 04:47:12.129820 agit-0.1.8/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)      111 2023-10-09 10:38:53.000000 agit-0.1.8/README.md
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2023-11-10 04:47:12.125563 agit-0.1.8/agit/
--rw-r--r--   0 chenhao    (501) staff       (20)      859 2023-10-19 03:44:24.000000 agit-0.1.8/agit/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     6131 2023-11-07 10:53:08.000000 agit-0.1.8/agit/assistant.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2023-11-10 04:47:12.126959 agit-0.1.8/agit/backend/
--rw-r--r--   0 chenhao    (501) staff       (20)      448 2023-11-01 07:40:57.000000 agit-0.1.8/agit/backend/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2107 2023-11-06 08:48:46.000000 agit-0.1.8/agit/backend/openai_bk.py
--rw-r--r--   0 chenhao    (501) staff       (20)     5323 2023-11-06 08:57:20.000000 agit-0.1.8/agit/backend/zhipuai_bk.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1933 2023-10-18 08:15:13.000000 agit-0.1.8/agit/cls.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4396 2023-11-10 04:44:09.000000 agit-0.1.8/agit/eval.py
--rw-r--r--   0 chenhao    (501) staff       (20)     5780 2023-10-19 04:02:00.000000 agit-0.1.8/agit/kb.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2023-11-10 04:47:12.128450 agit-0.1.8/agit/langchain/
--rw-r--r--   0 chenhao    (501) staff       (20)      190 2023-09-21 09:13:23.000000 agit-0.1.8/agit/langchain/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1994 2023-09-25 06:18:14.000000 agit-0.1.8/agit/langchain/document_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1064 2023-10-19 03:55:16.000000 agit-0.1.8/agit/langchain/embedding.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2184 2023-09-21 09:29:58.000000 agit-0.1.8/agit/langchain/text_splitter.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1249 2023-11-07 10:48:23.000000 agit-0.1.8/agit/tool.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2186 2023-11-06 08:55:33.000000 agit-0.1.8/agit/utils.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2023-11-10 04:47:12.129602 agit-0.1.8/agit.egg-info/
--rw-r--r--   0 chenhao    (501) staff       (20)      212 2023-11-10 04:47:12.000000 agit-0.1.8/agit.egg-info/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)      505 2023-11-10 04:47:12.000000 agit-0.1.8/agit.egg-info/SOURCES.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2023-11-10 04:47:12.000000 agit-0.1.8/agit.egg-info/dependency_links.txt
--rw-r--r--   0 chenhao    (501) staff       (20)      138 2023-11-10 04:47:12.000000 agit-0.1.8/agit.egg-info/requires.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        5 2023-11-10 04:47:12.000000 agit-0.1.8/agit.egg-info/top_level.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2023-11-10 04:47:12.000000 agit-0.1.8/agit.egg-info/zip-safe
--rw-r--r--   0 chenhao    (501) staff       (20)       38 2023-11-10 04:47:12.130140 agit-0.1.8/setup.cfg
--rwxr-xr-x   0 chenhao    (501) staff       (20)     1399 2023-10-16 09:35:21.000000 agit-0.1.8/setup.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2023-11-10 05:10:04.921302 agit-0.1.9/
+-rw-r--r--   0 chenhao    (501) staff       (20)      212 2023-11-10 05:10:04.921065 agit-0.1.9/PKG-INFO
+-rw-r--r--   0 chenhao    (501) staff       (20)      111 2023-10-09 10:38:53.000000 agit-0.1.9/README.md
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2023-11-10 05:10:04.917241 agit-0.1.9/agit/
+-rw-r--r--   0 chenhao    (501) staff       (20)      859 2023-10-19 03:44:24.000000 agit-0.1.9/agit/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     6131 2023-11-07 10:53:08.000000 agit-0.1.9/agit/assistant.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2023-11-10 05:10:04.918370 agit-0.1.9/agit/backend/
+-rw-r--r--   0 chenhao    (501) staff       (20)      448 2023-11-01 07:40:57.000000 agit-0.1.9/agit/backend/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2107 2023-11-06 08:48:46.000000 agit-0.1.9/agit/backend/openai_bk.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     5323 2023-11-06 08:57:20.000000 agit-0.1.9/agit/backend/zhipuai_bk.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1933 2023-10-18 08:15:13.000000 agit-0.1.9/agit/cls.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4604 2023-11-10 05:09:25.000000 agit-0.1.9/agit/eval.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     5780 2023-10-19 04:02:00.000000 agit-0.1.9/agit/kb.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2023-11-10 05:10:04.919743 agit-0.1.9/agit/langchain/
+-rw-r--r--   0 chenhao    (501) staff       (20)      190 2023-09-21 09:13:23.000000 agit-0.1.9/agit/langchain/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1994 2023-09-25 06:18:14.000000 agit-0.1.9/agit/langchain/document_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1064 2023-10-19 03:55:16.000000 agit-0.1.9/agit/langchain/embedding.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2184 2023-09-21 09:29:58.000000 agit-0.1.9/agit/langchain/text_splitter.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1249 2023-11-07 10:48:23.000000 agit-0.1.9/agit/tool.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2186 2023-11-06 08:55:33.000000 agit-0.1.9/agit/utils.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2023-11-10 05:10:04.920873 agit-0.1.9/agit.egg-info/
+-rw-r--r--   0 chenhao    (501) staff       (20)      212 2023-11-10 05:10:04.000000 agit-0.1.9/agit.egg-info/PKG-INFO
+-rw-r--r--   0 chenhao    (501) staff       (20)      505 2023-11-10 05:10:04.000000 agit-0.1.9/agit.egg-info/SOURCES.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        1 2023-11-10 05:10:04.000000 agit-0.1.9/agit.egg-info/dependency_links.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)      138 2023-11-10 05:10:04.000000 agit-0.1.9/agit.egg-info/requires.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        5 2023-11-10 05:10:04.000000 agit-0.1.9/agit.egg-info/top_level.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        1 2023-11-10 05:10:04.000000 agit-0.1.9/agit.egg-info/zip-safe
+-rw-r--r--   0 chenhao    (501) staff       (20)       38 2023-11-10 05:10:04.921349 agit-0.1.9/setup.cfg
+-rwxr-xr-x   0 chenhao    (501) staff       (20)     1399 2023-10-16 09:35:21.000000 agit-0.1.9/setup.py
```

### Comparing `agit-0.1.8/agit/__init__.py` & `agit-0.1.9/agit/__init__.py`

 * *Files identical despite different names*

### Comparing `agit-0.1.8/agit/assistant.py` & `agit-0.1.9/agit/assistant.py`

 * *Files identical despite different names*

### Comparing `agit-0.1.8/agit/backend/openai_bk.py` & `agit-0.1.9/agit/backend/openai_bk.py`

 * *Files identical despite different names*

### Comparing `agit-0.1.8/agit/backend/zhipuai_bk.py` & `agit-0.1.9/agit/backend/zhipuai_bk.py`

 * *Files identical despite different names*

### Comparing `agit-0.1.8/agit/cls.py` & `agit-0.1.9/agit/cls.py`

 * *Files identical despite different names*

### Comparing `agit-0.1.8/agit/eval.py` & `agit-0.1.9/agit/eval.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 '''
 @Time    :   2023/11/10 12:30:19
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 from agit.utils import getlog
 from agit import AGIT_ENV
+import re
 import requests
 
 
 logger = getlog(AGIT_ENV, __file__)
 
 
 PREFIX_PROMPT_WITH_REF = "[Instruction]\nPlease act as an impartial judge and evaluate the quality of the response provided by an AI assistant to the user question displayed below. Your evaluation should consider factors such as the helpfulness, relevance, accuracy, depth, creativity, and level of detail of the response. Begin your evaluation by providing a short explanation. You will be given a high-quality reference answer and the assistant's answer. Be as objective as possible. You should first provide your explanation IN CHINESE, then you must rate the response on a scale of 1 to 10 by STRICTLY following the below MAPPING for the relation between the scores and response quality:\n1) The score 1~2 stands for very chaotic or absence of answer, and the AI assissant completely failed to address the instructions. Serious mathematical, logical and factual errors might also be included in this term. The gap between the AI assistant's answer and the high-quality reference answer is huge and insuperable.\n2) The score 3~4 indicates fragment-like responses from AI assistant's answer. It did not provide answers in proper grammar, fluency, or accuracy. There are obvious gaps between the high-quality reference answer and the AI assistant's response.\n3) The score 5~6 indicates for existence of minute disadvantage from the AI assistant's answer compared to the high-quality reference answer. Yet the AI assistant did provide an average answer. The AI assistant either did not fully satisfy instructions, or was somewhat short of helpfulness, relevance, depth, creativity, or detailedness. The disadvantages from the AI assistant's answer overwhelm its advantages.\n4) The score 7~8 indicates the AI assistant provided a good answer as well as the high-quality reference answer, satisfying the instruction, while addressing good helpfulness, relevance, accuracy, depth, creativity, and level of detail of the response. The AI assistant might have flaws compared to the reference answer, but that does not overwhelm the above advantages.\n5) The score 9~10 indicates the AI assistant responsed better than the provided reference answer in most aspects, fully achieved the instruction goal, and have unique advantages to the reference answer.\nYou should give scores around 7 if you do not find obvious advantages or disadvantages. You should seriously consider the above guide before give lowest and highest scores such as 1 or 10, and avoid such situation if you do not have sound explanations.\nAvoid any positional biases and ensure that the order in which the responses were presented does not influence your decision. Do not allow the length of the responses to influence your evaluation. Do not favor certain names of the assistants. AND again, VERY IMPORTANTLY, after you provide your explanation IN CHINESE, you must rate the response strictly following this format: \"[[rating]]\", for example: \"Rating: [[5]]\"."
@@ -33,17 +34,22 @@
     }
     header = {
         "Host": "api-research-score-32b-0926.glm.ai"
     }
     resp = requests.post(url="https://117.161.233.25:8443/v1/completions", verify=False, headers=header, json=data)
     resp.raise_for_status()
     text = resp.json()["choices"][0]["text"]
-    logger.info(text)
+    # logger.info(text)
     idx = text.index("评分")
     reason = text[:idx].strip()
-    score = eval(text[idx + 3:])[0][0]
+    pattern = "\[\[(.*?)\]\]"
+    score = re.findall(pattern, text[idx + 3:])
+    score = eval(score[0])
+
+    # score = eval(text[idx + 3:])[0][0]
     return {"reason": reason, "score": score}
 
 
 if __name__ == "__main__":
+    print(eval_by_ref(question="中国人口有多少", reference="", answer="1亿"))
 
-    print(eval_by_ref(question="贵州茅台营收是多少", reference="100亿", answer="10000000000"))
+    # print(eval_by_ref(question="贵州茅台营收是多少", reference="100亿", answer="10000000000"))
```

### Comparing `agit-0.1.8/agit/kb.py` & `agit-0.1.9/agit/kb.py`

 * *Files identical despite different names*

### Comparing `agit-0.1.8/agit/langchain/document_loader.py` & `agit-0.1.9/agit/langchain/document_loader.py`

 * *Files identical despite different names*

### Comparing `agit-0.1.8/agit/langchain/embedding.py` & `agit-0.1.9/agit/langchain/embedding.py`

 * *Files identical despite different names*

### Comparing `agit-0.1.8/agit/langchain/text_splitter.py` & `agit-0.1.9/agit/langchain/text_splitter.py`

 * *Files identical despite different names*

### Comparing `agit-0.1.8/agit/tool.py` & `agit-0.1.9/agit/tool.py`

 * *Files identical despite different names*

### Comparing `agit-0.1.8/agit/utils.py` & `agit-0.1.9/agit/utils.py`

 * *Files identical despite different names*

### Comparing `agit-0.1.8/setup.py` & `agit-0.1.9/setup.py`

 * *Files identical despite different names*

