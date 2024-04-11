# Comparing `tmp/tweets_to_topic_network-0.1.0.tar.gz` & `tmp/tweets_to_topic_network-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweets_to_topic_network-0.1.0.tar", max compression
+gzip compressed data, was "tweets_to_topic_network-0.1.1.tar", max compression
```

## Comparing `tweets_to_topic_network-0.1.0.tar` & `tweets_to_topic_network-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2024-04-04 12:55:52.691295 tweets_to_topic_network-0.1.0/LICENSE
--rw-r--r--   0        0        0     9754 2024-04-10 15:06:30.536170 tweets_to_topic_network-0.1.0/README.md
--rw-r--r--   0        0        0     2343 2024-04-08 15:12:50.920582 tweets_to_topic_network-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 12:55:52.693650 tweets_to_topic_network-0.1.0/tweets_to_topic_network/__init__.py
--rw-r--r--   0        0        0     7915 2024-04-09 11:34:58.569613 tweets_to_topic_network-0.1.0/tweets_to_topic_network/data.py
--rw-r--r--   0        0        0    10831 2024-04-10 13:10:56.947375 tweets_to_topic_network-0.1.0/tweets_to_topic_network/network.py
--rw-r--r--   0        0        0     8394 2024-04-11 09:00:06.252820 tweets_to_topic_network-0.1.0/tweets_to_topic_network/topic.py
--rw-r--r--   0        0        0    13589 1970-01-01 00:00:00.000000 tweets_to_topic_network-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-11 12:12:13.477841 tweets_to_topic_network-0.1.1/LICENSE
+-rw-r--r--   0        0        0     9801 2024-04-11 12:12:13.478046 tweets_to_topic_network-0.1.1/README.md
+-rw-r--r--   0        0        0      717 2024-04-11 12:53:46.938254 tweets_to_topic_network-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 12:12:13.484112 tweets_to_topic_network-0.1.1/tweets_to_topic_network/__init__.py
+-rw-r--r--   0        0        0     7915 2024-04-11 12:12:13.484388 tweets_to_topic_network-0.1.1/tweets_to_topic_network/data.py
+-rw-r--r--   0        0        0    10831 2024-04-11 12:12:13.484495 tweets_to_topic_network-0.1.1/tweets_to_topic_network/network.py
+-rw-r--r--   0        0        0     8441 2024-04-11 12:36:59.087972 tweets_to_topic_network-0.1.1/tweets_to_topic_network/topic.py
+-rw-r--r--   0        0        0    10683 1970-01-01 00:00:00.000000 tweets_to_topic_network-0.1.1/PKG-INFO
```

### Comparing `tweets_to_topic_network-0.1.0/LICENSE` & `tweets_to_topic_network-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tweets_to_topic_network-0.1.0/README.md` & `tweets_to_topic_network-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # tweets-to-network
-
+```bash
+pip install tweets-to-topic-network
+```
 
 This repository contains the code to 
 - create networks from a set of tweets in json format (as they come from the API (RIP))
 - label each tweet with a topic using BERTopic
 
 from a set of tweets it is possibile to generate multiple networks:
 - *retweet network*:  a network where the nodes are the users and the edges are the retweets
```

### Comparing `tweets_to_topic_network-0.1.0/tweets_to_topic_network/data.py` & `tweets_to_topic_network-0.1.1/tweets_to_topic_network/data.py`

 * *Files identical despite different names*

### Comparing `tweets_to_topic_network-0.1.0/tweets_to_topic_network/network.py` & `tweets_to_topic_network-0.1.1/tweets_to_topic_network/network.py`

 * *Files identical despite different names*

### Comparing `tweets_to_topic_network-0.1.0/tweets_to_topic_network/topic.py` & `tweets_to_topic_network-0.1.1/tweets_to_topic_network/topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
         except(Exception) as e:
             print(e)
             print('error in saving vectors in qdrant')
 
     def _save_files(self):
         self.df.to_pickle(self.df_labeled_path)
-        self.model.save(self.model_path)
+        self.model.save(self.model_path, serialization="safetensors", save_ctfidf=True)
 
     def label_topics(self):
         llm = OpenAI(temperature=0.3)
 
         template = """I want you to act as a tweet labeler, you are given representative words
             from a topic and three representative tweets, give more attention to the words, all the tweets are related to climate change, and COP, no need to mention it, detect subtopics.
             start with "label:" and avoid hashtags,
```

