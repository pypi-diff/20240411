# Comparing `tmp/phub-4.5.7.tar.gz` & `tmp/phub-4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phub-4.5.7.tar", last modified: Mon Mar 25 15:14:28 2024, max compression
+gzip compressed data, was "phub-4.6.tar", last modified: Thu Apr 11 17:33:43 2024, max compression
```

## Comparing `phub-4.5.7.tar` & `phub-4.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:14:28.653027 phub-4.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-25 15:14:19.000000 phub-4.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41940 2024-03-25 15:14:28.653027 phub-4.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-03-25 15:14:19.000000 phub-4.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-25 15:14:19.000000 phub-4.5.7/pypi.md
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-25 15:14:19.000000 phub-4.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 15:14:28.653027 phub-4.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-25 15:14:19.000000 phub-4.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:14:28.645027 phub-4.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:14:28.649027 phub-4.5.7/src/phub/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/literals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:14:28.649027 phub-4.5.7/src/phub/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/modules/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/modules/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/modules/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/modules/rss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:14:28.653027 phub-4.5.7/src/phub/objects/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/objects/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/objects/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/objects/feed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/objects/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/objects/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/objects/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/objects/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    18750 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/objects/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:14:28.653027 phub-4.5.7/src/phub/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/tests/test_playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/tests/test_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-03-25 15:14:19.000000 phub-4.5.7/src/phub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:14:28.653027 phub-4.5.7/src/phub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41940 2024-03-25 15:14:28.000000 phub-4.5.7/src/phub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-25 15:14:28.000000 phub-4.5.7/src/phub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 15:14:28.000000 phub-4.5.7/src/phub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-25 15:14:28.000000 phub-4.5.7/src/phub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-25 15:14:28.000000 phub-4.5.7/src/phub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.902743 phub-4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 17:33:39.000000 phub-4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41938 2024-04-11 17:33:43.902743 phub-4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-11 17:33:39.000000 phub-4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-11 17:33:39.000000 phub-4.6/pypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-11 17:33:39.000000 phub-4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:33:43.902743 phub-4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 17:33:39.000000 phub-4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.894743 phub-4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.898743 phub-4.6/src/phub/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-11 17:33:39.000000 phub-4.6/src/phub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-11 17:33:39.000000 phub-4.6/src/phub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-04-11 17:33:39.000000 phub-4.6/src/phub/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16579 2024-04-11 17:33:39.000000 phub-4.6/src/phub/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-11 17:33:39.000000 phub-4.6/src/phub/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-04-11 17:33:39.000000 phub-4.6/src/phub/literals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.898743 phub-4.6/src/phub/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-11 17:33:39.000000 phub-4.6/src/phub/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-11 17:33:39.000000 phub-4.6/src/phub/modules/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-11 17:33:39.000000 phub-4.6/src/phub/modules/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-11 17:33:39.000000 phub-4.6/src/phub/modules/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-11 17:33:39.000000 phub-4.6/src/phub/modules/rss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.898743 phub-4.6/src/phub/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18719 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.902743 phub-4.6/src/phub/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:39.000000 phub-4.6/src/phub/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-11 17:33:39.000000 phub-4.6/src/phub/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-11 17:33:39.000000 phub-4.6/src/phub/tests/test_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-11 17:33:39.000000 phub-4.6/src/phub/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-11 17:33:39.000000 phub-4.6/src/phub/tests/test_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-11 17:33:39.000000 phub-4.6/src/phub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.902743 phub-4.6/src/phub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41938 2024-04-11 17:33:43.000000 phub-4.6/src/phub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-11 17:33:43.000000 phub-4.6/src/phub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:33:43.000000 phub-4.6/src/phub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 17:33:43.000000 phub-4.6/src/phub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 17:33:43.000000 phub-4.6/src/phub.egg-info/top_level.txt
```

### Comparing `phub-4.5.7/LICENSE` & `phub-4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/PKG-INFO` & `phub-4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 4.5.7
+Version: 4.6
 Summary: An API for Pornhub
 Author-email: Egsagon <egsagon12@gmail.com>, EchterAlsFake <EchterAlsFake@proton.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `phub-4.5.7/README.md` & `phub-4.6/README.md`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/pypi.md` & `phub-4.6/pypi.md`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/pyproject.toml` & `phub-4.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phub"
-version = "4.5.7"
+version = "4.6"
 description = "An API for Pornhub"
 authors = [
   {name = 'Egsagon', email = "egsagon12@gmail.com"},
   {name = "EchterAlsFake", email = "EchterAlsFake@proton.me"}
 ]
 license = {file = "LICENSE"}
 readme = {file = "pypi.md", content-type = "text/markdown"}
```

### Comparing `phub-4.5.7/src/phub/__init__.py` & `phub-4.6/src/phub/__init__.py`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/src/phub/__main__.py` & `phub-4.6/src/phub/__main__.py`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/src/phub/consts.py` & `phub-4.6/src/phub/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 FFMPEG_EXECUTABLE = 'ffmpeg' # Use from PATH by default
 FFMPEG_COMMAND = FFMPEG_EXECUTABLE + ' -i "{input}" -bsf:a aac_adtstoasc -y -c copy {output}'
 
 IFRAME = '<iframe src="https://www.pornhub.com/embed/{key}" frameborder="0" width="{width}" height="{height}" scrolling="no" allowfullscreen></iframe>'
 
 # Supported languages
-LANGUAGES = [ 'cn', 'de', 'fr', 'it', 'pt', 'pl', 'rt', 'nl', 'cz', 'jp' ]
+LANGUAGES = [ 'en', 'cn', 'de', 'fr', 'it', 'pt', 'pl', 'rt', 'nl', 'cz', 'jp' ]
 
 FEED_CLASS_TO_CONST = {
     'stream_videos_uploaded': 'Section.VIDEO',
     'stream_favourites_videos': 'Section.FAVORITE',
     'stream_grouped_comments_videos': 'Section.COMMENT',
     # TODO - More options
 }
@@ -207,17 +207,17 @@
     get_token                = find(                             r'token *?= \"(.*?)\",'                                                       ) # Get authentification token
     video_channel            = find(                             r'href=\"(.*?)\" data-event=\"Video Underplayer\".*?bolded\">(.*?)<'          ) # Get video author, if channel
     video_model              = find(                             r'n class=\"usernameBadgesWrapper.*? href=\"(.*?)\"  class=\"bolded\">(.*?)<' ) # Get video author, if model
     get_feed_type            = find(                             r'data-table="(.*?)"'                                                         ) # Get feed section type
     get_user_type            = find(                             r'\/(model|pornstar|channels|user|users)\/.*?'                                ) # Get a user type
     get_thumb_id             = find(                             r'\/([a-z0-9]+?)\/(?=original|thumb)'                                         ) # Get video id from its thumbnail 
     remove_host              = subc(                             _raw_root, ''                                                                 ) # Remove the HOST root from a URL
-    is_favorite              = find(                             r'<div class=\".*?js-favoriteBtn.*?active\"'                                  ) # Check if is favorite
-    eval_video               = find( engine.DOTALL,              r'id=\"(.*?)\".*?-vkey=\"(.*?)\".*?title=\"(.*?)\".*?src=\"(.'
-                                                                 r'*?)\".*?-mediabook=\"(.*?)\".*?marker-overlays.*?>(.*?)</div'               ) # Parse video data
+    is_favorite              = find(                             r'<div class=\".*?js-favoriteBtn.*?active\"'                                  ) # Check if is favorite    
+    eval_video               = find( engine.DOTALL,              r'id=\"(.*?)\".*?-vkey=\"(.*?)\".*?title=\"(.*?)\".*?src=\"(.*?)\".*?</div'   ) # Parse video data
+    eval_public_video        = find( engine.DOTALL,              r'-mediabook=\"(.*?)\".*?marker-overlays.*?>(.*?)'                            ) # Parse public-only video data
     user_avatar              = find( engine.DOTALL,              r'previewAvatarPicture\">.*?src=\"(.*?)\"'                                    ) # get the user avatar
     query_counter            = find( engine.DOTALL,              r'showing(?:Counter|Info).*?\">.*?(\d+)\s*<\/'                                ) # Get a query's video amount
     user_bio                 = find( engine.DOTALL,              r'\"aboutMeSection.*?\"title.*?<div>\s*(.*?)\s*<\/'                           ) # Get the user bio
     container                = find( engine.DOTALL,              r'class=\"container(.*)'                                                      ) # Get the page container
     document                 = find( engine.DOTALL,              r'.*'                                                                         ) # Match a whole document
     get_playlist_unavailable = find( engine.DOTALL,              r': (\d+)</h5'                                                                ) # Get playlist unavailable videos amount
     playlist_data            = find( engine.DOTALL,              r'id=\"playlistWrapper(.*?)playlistSectionWrapper\"'                          ) # Get playlist data container
```

### Comparing `phub-4.5.7/src/phub/core.py` & `phub-4.6/src/phub/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,153 +24,167 @@
 class Client:
     '''
     Represents a client capable of handling requests
     with Pornhub.
     '''
     
     def __init__(self,
-                 username: str = None,
+                 email: str = None,
                  password: str = None,
                  *,
-                 language: str = 'en,en-US',
-                 delay: int = 0,
+                 language: literals.language = 'en,en-US',
+                 delay: int | float = 0,
                  proxies: dict = None,
                  login: bool = True) -> None:
         '''
-        Initialise a new client.
+        Initialises a new client.
         
         Args:
-            username (str): Optional account username/address to connect to.
-            password (str): Optional account password to connect to.
-            language (str): Language locale (fr, en, ru, etc.)
-            delay  (float): Minimum delay between requests.
+            email (str): Account email address.
+            password (str): Account password.
+            language (str): Client language (fr, en, ru, etc.)
+            delay (int | float): Minimum delay between requests.
             proxies (dict): Dictionary of proxies for the requests.
-            login   (bool): Whether to automatically log in after initialization.
+            login (bool): Whether to directly log in after initialization.
+        
+        Raises:
+            LoginFailed: If Pornhub refuses the authentification.
+                The reason will be passed as the error body.
         '''
         
         logger.debug('Initialised new Client %s', self)
         
         # Initialise session
         self.reset()
         
         self.proxies = proxies
         self.language = {'Accept-Language': language}
-        self.credentials = {'username': username,
+        self.credentials = {'email': email,
                             'password': password}
         
         self.delay = delay
         self.start_delay = False
+        self.last_request_time = None
         
         # Connect account
         self.logged = False
         self.account = Account(self)
         logger.debug('Connected account to client %s', self.account)
         
         # Automatic login
         if login and self.account:
-            logger.debug('Automatic login triggered')
             self.login()
     
     def reset(self) -> None:
         '''
         Reset the client requests session.
+        This is useful if you are keeping the client running
+        for a long time and can help with Pornhub rate limit.
         '''
         
         # Initialise session
         self.session = requests.Session()
         self._clear_granted_token()
         
         # Insert cookies
         self.session.cookies.update(consts.COOKIES)
-        
+
     def call(self,
              func: str,
              method: str = 'GET',
              data: dict = None,
              headers: dict = {},
              timeout: float = consts.CALL_TIMEOUT,
              throw: bool = True,
              silent: bool = False) -> requests.Response:
         '''
-        Send a request.
-        
+        Used internally to send a request or an API call.
+
         Args:
-            func      (str): URL or PH function to call.
-            method    (str): Request method.
-            data     (dict): Optional data to send to the server.
-            headers  (dict): Request optional headers.
+            func (str): URL or PH function to fetch or call.
+            method (str): Request method (GET, POST, PUT, ...).
+            data (dict): Optional data to send to the server.
+            headers (dict): Additional request headers.
             timeout (float): Request maximum response time.
-            throw    (bool): Whether to raise an error when a request explicitly fails.
-            silent   (bool): Make the call logging one level deeper.
-        
+            throw (bool): Whether to raise an error when a request explicitly fails.
+            silent (bool): Whether to supress this call from logs.
+
         Returns:
-            requests.Response: The fetched response.
-        '''
+            Response: The fetched response.
         
-        logger.log(logging.DEBUG if silent else logging.INFO, 'Making call %s', func or '/')
-        
-        # Delay
-        if self.start_delay:
-            time.sleep(self.delay)
-        else:
-            self.start_delay = True
+        Raises:
+            ConnectionError: If the request was blocked by Pornhub.
+            HTTPError: If the request failed, for any reason.
+        '''
+
+        logger.log(logging.DEBUG if silent else logging.INFO, 'Fetching %s', func or '/')
+
+        # Delay mechanism
+        if self.last_request_time:
+            elapsed_time = time.time() - self.last_request_time
+            if elapsed_time < self.delay:
+                time.sleep(self.delay - elapsed_time)
+
+        self.last_request_time = time.time()  # Update the time of the last request
 
         url = func if 'http' in func else utils.concat(consts.HOST, func)
-        
+
         for i in range(consts.MAX_CALL_RETRIES):
-            
             try:
-                # Send request
                 response = self.session.request(
                     method = method,
                     url = url,
-                    headers = consts.HEADERS | headers | self.language,
+                    headers = headers,
                     data = data,
                     timeout = timeout,
-                    proxies = self.proxies
                 )
-                
+
                 # Silent 429 errors
                 if b'429</title>' in response.content:
                     raise ConnectionError('Pornhub raised error 429: too many requests')
-                
+
                 # Attempt to resolve the challenge if needed
                 if challenge := consts.re.get_challenge(response.text, False):
-                    logger.info('\n\nChallenge found, attempting to resolve\n\n')
+                    logger.info('Challenge found, attempting to resolve')
                     parser.challenge(self, *challenge)
-                    logging.info(f"Sleeping for {consts.CHALLENGE_TIMEOUT} seconds")
+                    
+                    logger.info(f"Sleeping for {consts.CHALLENGE_TIMEOUT} seconds")
                     time.sleep(consts.CHALLENGE_TIMEOUT)
-                    continue # Reload page
-                
+                    continue  # Reload page
+
                 break
-            
+
             except Exception as err:
                 logger.log(logging.DEBUG if silent else logging.WARNING,
                            f'Call failed: {repr(err)}. Retrying (attempt {i + 1}/{consts.MAX_CALL_RETRIES})')
                 time.sleep(consts.MAX_CALL_TIMEOUT)
                 continue
-        
+
         else:
             raise ConnectionError(f'Call failed after {i + 1} retries. Aborting.')
 
         if throw: response.raise_for_status()
         return response
-    
+
     def login(self,
               force: bool = False,
               throw: bool = True) -> bool:
         '''
         Attempt to log in.
         
         Args:
             force (bool): Whether to force the login (used to reconnect).
             throw (bool): Whether to raise an error if this fails.
         
         Returns:
             bool: Whether the login was successful.
+            
+        Raises:
+            ClientAlreadyLogged: If ``force`` was False and client was already logged.
+            LoginFailed: If the login failed, for a reason passed in the error body.
         '''
         
         logger.debug('Attempting login')
         
         if not force and self.logged:
             logger.error('Client is already logged in')
             raise errors.ClientAlreadyLogged()
@@ -198,18 +212,18 @@
         # Update account data
         self.account.connect(data)
         self.logged = bool(success)
         return self.logged
     
     def get(self, video: str | Video) -> Video:
         '''
-        Fetch a Pornhub video.
+        Get a Pornhub video.
         
         Args:
-            video (str): Video full URL, partial URL or viewkey.
+            video (str | Video): Video URL or viewkey.
         
         Returns:
             Video: The corresponding video object.
         '''
         
         logger.debug('Fetching video at', video)
 
@@ -233,18 +247,18 @@
             
             url = utils.concat(consts.HOST, 'view_video.php?viewkey=' + key)
         
         return Video(self, url)
 
     def get_user(self, user: str | User) -> User:
         '''
-        Get a specific user.
+        Get a Pornhub user.
         
         Args:
-            user (str): user URL or name.
+            user (str | User): user URL or name.
         
         Returns:
             User: The corresponding user object.
         '''
         
         if isinstance(user, User):
             user = user.url
@@ -260,21 +274,24 @@
                sort: literals.ht_sort = None,
                period: literals.ht_period = None) -> Query:
         '''
         Perform searching on Pornhub using the HubTraffic API.
         It is condidered to be much faster but has less filters.
         
         Args:
-            query    (str): The query to search.
-            category (str): A category the video is in. 
-            sort     (str): Sorting type.
-            period   (str): When using sort, specify the search period.
+            query (str): The query to search.
+            category (str): A category the video is in.
+            sort (str): Sorting type.
+            period (str): When using sort, specify the search period.
         
         Returns:
-            Query: Initialised query.
+            Query: Initialised query response.
+        
+        Raises:
+            AssertionError: If one or more filters don't match their literals.
         '''
         
         literals.ass('category', category, literals.category)
         literals.ass('sort'    , sort    , literals.ht_sort)
         literals.ass('period'  , period  , literals.ht_period)
     
         return queries.JSONQuery(
@@ -299,24 +316,28 @@
                hd: bool = None,
                sort: literals.sort = None,
                period: literals.period = None) -> Query:
         '''
         Performs searching on Pornhub.
         
         Args:
-            query                   (str): The query to search.
-            production              (str): Production type.
-            category                (str): A category the video is in. 
+            query (str): The query to search.
+            production (str): Production type.
+            category (str): A category the video is in. 
             exclude_category (str | list): One or more categories to exclude.
-            hd                     (bool): Whether to search only HD videos.
-            sort                    (str): Sorting type.
-            period                  (str): When using sort, specify the search period.
+            hd (bool): Whether to search only HD videos.
+            sort (str): Sorting type.
+            period (str): When using sort, specify the search period.
         
         Returns:
             Query: Initialised query.
+        
+        Raises:
+            AssertioneError: If the query is empty.
+            AssertioneError: If one or more filters don't match their literals.
         '''
         
         query = query.strip()
         
         assert query, 'Query must be a non-empty string'
         
         literals.ass('production'      , production      , literals.production)
@@ -336,57 +357,71 @@
                 'o': literals.map.sort.get(sort),
                 't': literals.map.period.get(period),
                 'hd': literals._craft_boolean(hd)
             },
             query_repr = query
         )
     
-    def get_playlist(self, pl: str | int | Playlist) -> Playlist:
+    def get_playlist(self, playlist: str | int | Playlist) -> Playlist:
         '''
-        Initializes a Playlist object.
+        Get a Pornhub playlist.
 
         Args:
-            pl (str | int | Playlist): The playlist url or id
+            playlist (str | int | Playlist): The playlist url or id
 
         Returns:
-            Playlist object
+            Playlist: The corresponding playlist object.
+        
+        Raises:
+            TypeError: If the playlist argument is invalid.
         '''
         
-        assert isinstance(pl, str | int | Playlist), 'Invalid type'
+        if not isinstance(playlist, str | int | Playlist):
+            raise TypeError(f'Invalid type: {type(playlist)} should be str, int or Playlist.')
         
-        if isinstance(pl, Playlist):
-            pl = pl.url
+        if isinstance(playlist, Playlist):
+            playlist = playlist.url
         
-        if isinstance(pl, str) and 'playlist' in pl:
-            pl = pl.split('/')[-1]
+        if isinstance(playlist, str) and 'playlist' in playlist:
+            playlist = playlist.split('/')[-1]
 
-        return Playlist(self, pl)
+        return Playlist(self, playlist)
 
     def search_user(self,
-                    username: str = None,
-                    country: str = None,
-                    city: str = None,
-                    min_age: int = None,
-                    max_age: int = None,
-                    gender: literals.gender = None,
-                    orientation: literals.orientation = None,
-                    offers: literals.offers = None,
-                    relation: literals.relation = None,
-                    sort: literals.sort_user = None,
-                    is_online: bool = None,
-                    is_model: bool = None,
-                    is_staff: bool = None,
-                    has_avatar: bool = None,
-                    has_videos: bool = None,
-                    has_photos: bool = None,
-                    has_playlists: bool = None    
-                    ) -> queries.UserQuery:
+                    username: str = None,                     country: str = None,
+                    city: str = None,                         min_age: int = None,
+                    max_age: int = None,                      gender: literals.gender = None,
+                    orientation: literals.orientation = None, offers: literals.offers = None,
+                    relation: literals.relation = None,       sort: literals.sort_user = None,
+                    is_online: bool = None,                   is_model: bool = None,
+                    is_staff: bool = None,                    has_avatar: bool = None,
+                    has_videos: bool = None,                  has_photos: bool = None,
+                    has_playlists: bool = None) -> queries.UserQuery:
         '''
         Search for users in the community.
         
+        Args:
+            username (str): Filters users with a name query.
+            country (str): Filter users with a country.
+            city (str): Filters users with a city.
+            min_age (int): Filters users with a minimal age.
+            max_age (int): Filters users with a maximal age.
+            gender (gender): Filters users with a gender.
+            orientation (orientation): Filters users with an orientation.
+            offers (offers): Filters users with what content they do on their channel.
+            relation (relation): Filters users with their relation.
+            sort (sort_user): Response sort type.
+            is_online (bool): Get only online or offline users.
+            is_model (bool): Get only model users.
+            is_staff (bool): Get only Pornhub staff members.
+            has_avatar (bool): Get only users with a custom avatar.
+            has_videos (bool): Get only users that have posted videos.
+            has_photos (bool): Get only users that have posted photos.
+            has_playlists (bool): Get only users that have posted playlists.
+        
         Returns:
             UserQuery: Initialised query.
         '''
         
         return queries.UserQuery(
             client = self,
             func = 'user/search',
@@ -409,27 +444,28 @@
                 'photos': literals._craft_boolean(has_photos),
                 'playlists': literals._craft_boolean(has_playlists),
             }
         )
 
     def _clear_granted_token(self) -> None:
         '''
-        Clear the granted token cache.
+        Removes the current granted token stored, if any.
         '''
         
         if '_granted_token' in self.__dict__:
             del self._granted_token
 
     @cached_property
     def _granted_token(self) -> str:
         '''
-        Get a granted token after having
-        authentified the account.
+        Get a granted token for the account. Used internally
+        for making API calls.
+        
+        Raises:
+            AssertionError: If the client is not logged in
         '''
         
         assert self.logged, 'Client must be logged in'
-        self._token_controller = True
-
         page = self.call('').text
         return consts.re.get_token(page)
 
 # EOF
```

### Comparing `phub-4.5.7/src/phub/errors.py` & `phub-4.6/src/phub/errors.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,55 @@
 '''
 PHUB errors types.
 '''
 
 class ClientAlreadyLogged(Exception):
     '''
-    The Client already has initiated
-    a login call which was successful.
+    The Client is already logged in.
     '''
 
 class LoginFailed(Exception):
     '''
     The Client failed to connect.
-    Given credentials might be wrong.
+    Input credentials might be wrong.
     '''
 
 class RegexError(Exception):
     '''
     A regex failed to execute.
     '''
 
 class URLError(Exception):
     '''
-    Provided URL is invalid.
+    The provided URL is invalid.
     '''
 
 class ParsingError(Exception):
     '''
-    The parser failed to properly
-    fetch data.
+    The parser failed to properly fetch data.
     '''
 
 class MaxRetriesExceeded(Exception):
     '''
-    A module failed its job after too
-    many retries. You might want to
-    try again after a little time.
+    A process failed after too many retries.
     
-    You can also use: attr:`Client.delay`
-    to slow down requests.
+    Note: You can use: attr:`Client.delay` to slow down requests.
     '''
 
 class UserNotFound(Exception):
     '''
-    User wasn't found. This either happens
-    because the user does not exist, or
-    its name or URL is wrong.
+    User could not be foundn either because
+    it does not exists, or its name/URL is wrong.
     '''
 
 class NoResult(Exception):
     '''
     A query failed to retrieve an item
     at a specific index. Most of the time,
-    this is raised when you go too far in
-    a fetching loop:
-    
-    .. code-block:: python
-    
-        query = ...
-        for i in range(1000):
-            print(query[i])
-    
-    Instead, use:
-    
-    .. code-block:: python
-    
-        query = ...
-        for item in query[:1000]:
-            print(item)
-    
+    this is the equivalent of a StopIteration signal.
     '''
 
 class InvalidCategory(Exception):
     '''
     The category is invalid. This happens
     while trying to make Temporary
     categories behave like normal categories.
@@ -84,11 +62,11 @@
     
     '''
 
 class VideoError(Exception):
     '''
     Pornhub refused to serve video data because
     of some internal error (mostly because the video
-    is not available anymore).
+    is not available).
     '''
 
 # EOF
```

### Comparing `phub-4.5.7/src/phub/literals.py` & `phub-4.6/src/phub/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 '''
 PHUB Literals.
 '''
 
 from typing import Literal, Iterable, Type
 
+# Language locales
+language = Literal['en', 'cn', 'de', 'fr', 'it', 'pt', 'pl', 'rt', 'nl', 'cz', 'jp']
+
 # Production type
 production = Literal['homemade', 'professional']
 
 # Sortings for videos
 sort = Literal['recent', 'views', 'rated', 'longuest']
 ht_sort = Literal['recent', 'views', 'rated', 'featured']
 
@@ -75,15 +78,15 @@
     'female-orgasm', 'muscular-men', 'romantic', 'scissoring', 'strap-on', 'tattooed-men-gay', 'tattooed-women',
     'trans-with-girl', 'trans-with-guy', 'fingering', 'trans-male', '360', '180', '2d', '3d', 'voyeur',
     'pov', 'uncensored', 'verified-amateurs-gay', 'closed-captions', 'closed-captions-gay'
 ]
 
 class map:
     '''
-    Map literals values to Pornhub arg representation.
+    This object maps PHUB literals to their Pornhub URL value.
     '''
 
     sort = {
         'recent': 'mr',
         'views': 'mv',
         'rated': 'tr',
         'longuest': 'lg'
@@ -175,36 +178,56 @@
     
     ht_period = {
         'all': 'alltime',
         'week': 'weekly',
         'month': 'monthly'
     }
 
-def _craft_list(args: Iterable[category]) -> str:
+def _craft_list(args: Iterable[str]) -> str:
     '''
     Craft an item list list into a url-valid list.
+    
+    Args:
+        args (Iterable[str]): A list of items.
+    
+    Returns:
+        str: A dash separated URL-valid list. 
     '''
     
     if isinstance(args, str):
         return args
     
     if args:
         return '-'.join(list(args))
 
-def _craft_boolean(b: bool | None) -> str:
+def _craft_boolean(b: bool | None) -> int | None:
     '''
     Craft a boolean into a url-valid int.
+    
+    Args:
+        b (bool): Initial boolean value.
+    
+    Returns:
+        int: URL-valid representation of b.
     '''
     
     if b is not None:
         return int(bool(b))
 
 def ass(name: str, item: str | list[str], literal: Type) -> None:
     '''
     Assert one or multiple items are part of a literal.
+    
+    Args:
+        name (str): The literal name, used for error bodies.
+        item (str | list[str]): The object(s) to assert.
+        literal (Type): The literal that should match the item(s).
+    
+    Raises:
+        AssertionError: If the item is invalid.
     '''
     
     if not item: return
     
     if isinstance(item, str):
         item = [item]
```

### Comparing `phub-4.5.7/src/phub/modules/display.py` & `phub-4.6/src/phub/modules/display.py`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/src/phub/modules/download.py` & `phub-4.6/src/phub/modules/download.py`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/src/phub/modules/parser.py` & `phub-4.6/src/phub/modules/parser.py`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/src/phub/modules/rss.py` & `phub-4.6/src/phub/modules/rss.py`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/src/phub/objects/account.py` & `phub-4.6/src/phub/objects/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,14 @@
             client (Client): The client that initialized this.
         
         Returns:
             Self: The Account object or None, if login is not triggered.
         '''
         
         if all(client.credentials.values()):
-            logger.info('Creating new account object')
             return object.__new__(cls)
     
     def __init__(self, client: Client) -> None:
         '''
         Initialise a new account object.
         
         Args:
@@ -51,17 +50,15 @@
         self.avatar: Image = None
         self.is_premium: bool = None
         self.user: User = None
         
         # Save data keys so far, so we can make a difference with the
         # cached property ones.
         self.loaded_keys = list(self.__dict__.keys()) + ['loaded_keys']
-        
-        logger.info('Account object %s created', self)
-        
+            
     def __repr__(self) -> str:
         
         status = 'logged-out' if self.name is None else f'name={self.name}' 
         return f'phub.Account({status})'
 
     def connect(self, data: dict) -> None:
         '''
```

### Comparing `phub-4.5.7/src/phub/objects/data.py` & `phub-4.6/src/phub/objects/data.py`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/src/phub/objects/feed.py` & `phub-4.6/src/phub/objects/feed.py`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/src/phub/objects/image.py` & `phub-4.6/src/phub/objects/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,18 @@
                  url: str,
                  servers: list[dict] = [],
                  name: str = 'image') -> None:
         '''
         Initialise a new image object.
         
         Args:
-            client    (Client): Parent client.
-            url          (str): The image URL.
+            client (Client): Parent client.
+            url (str): The image URL.
             sizes (list[dict]): Image sizes/resolutions/servers.
-            name         (str): Image name.
+            name (str): Image name.
         '''
 
         self.url = url
         self.name = name
         self.client = client
         self._servers = servers
```

### Comparing `phub-4.5.7/src/phub/objects/playlist.py` & `phub-4.6/src/phub/objects/playlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     
     def __init__(self, client: Client, pid: str) -> None:
         '''
         Initialise a new Playlist.
         
         Args:
             client (Client): Parent client to use.
-            pid       (str): The playlist id.
+            pid (str): The playlist id.
         '''
         
         # Initialise 
         super().__init__(client, func = None)
         
         # Define both playlist url (first page) and chunked (next pages)
         self.url = 'playlist/' + str(pid)
```

### Comparing `phub-4.5.7/src/phub/objects/query.py` & `phub-4.6/src/phub/objects/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,19 +76,19 @@
                  args: dict[str] = {},
                  container_hint: consts.WrappedRegex | Callable = None,
                  query_repr: str = None) -> None:
         '''
         Initialise a new query.
         
         Args:
-            client           (Client): The parent client.
-            func                (str): The URL function.
-            args               (dict): Arguments.
+            client (Client): The parent client.
+            func (str): The URL function.
+            args (dict): Arguments.
             container_hint (Callable): An hint function to help determine where should the target container be.
-            query_repr          (str): Indication for the query representation.
+            query_repr (str): Indication for the query representation.
         '''
 
         self.client = client
         self.hint = container_hint
         self._query_repr = query_repr
         
         # Build URL
@@ -139,17 +139,17 @@
                filter: Callable[[QueryItem], bool] = None,
                watched: bool | None = None,
                free_premium: bool | None = None) -> Iterator[QueryItem]:
         '''
         Get a sample of the query.
         
         Args:
-            max           (int): Maximum amount of items to fetch.
-            filter   (Callable): A filter function that decides whether to keep each QueryItems.
-            watched      (bool): Whether videos should have been watched by the account or not.
+            max (int): Maximum amount of items to fetch.
+            filter (Callable): A filter function that decides whether to keep each QueryItems.
+            watched (bool): Whether videos should have been watched by the account or not.
             free_premium (bool): Whether videos should be free premium or not.
         
         Returns:
             Iterator: Response iterator containing QueryItems.
         '''
         
         i = 0
@@ -289,18 +289,21 @@
         
         BASE = consts.HOST
         
         def _eval_video(self, raw: str) -> dict:
             # Evaluate video data.
             # Can be used externally from this query
             
-            keys = ('id', 'key', 'title', 'image', 'preview', 'markers')
-            data = {k: v for k, v in zip(keys, consts.re.eval_video(raw))} | {'raw': raw}
+            html_entries = consts.re.eval_video(raw)
+            html_public_entries = consts.re.eval_public_video(raw, False) or ()
             
-            return data
+            data =        {k: v for v, k in zip(html_entries, ('id', 'key', 'title', 'image'))}
+            public_data = {k: v for v, k in zip(html_public_entries, ('preview', 'markers'))}
+            
+            return {'mediabook': None, 'markers': ''} | data | public_data | {'raw': raw}
         
         def _parse_item(self, raw: str) -> Video:
             
             # Parse data
             data = self._eval_video(raw)
             
             url = f'{consts.HOST}view_video.php?viewkey={data["key"]}'
@@ -312,15 +315,16 @@
             obj.data = {
                 # Property overrides
                 'page@video_title': data["title"],
                 'data@thumb': data["image"],
                 'page@id': id,
                 
                 # Custom query properties
-                'query@parent': self
+                'query@parent': self,
+                'query@watched': 'videos/recent' in self.url
             }
             
             return obj
         
         def _parse_page(self, raw: str) -> list:
             container = (self.hint or consts.re.container)(raw)
             return consts.re.get_videos(container)
```

### Comparing `phub-4.5.7/src/phub/objects/user.py` & `phub-4.6/src/phub/objects/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
     def __init__(self, client: Client, name: str, url: str, type: str = None) -> None:
         '''
         Initialize a new user object.
         
         Args:
             client (Client): The client parent.
-            name      (str): The username.
-            url       (str): The user page URL.
+            name (str): The username.
+            url (str): The user page URL.
         '''
         
         self.client = client
         self.name = name
         self.url = consts.re.remove_host(url)
         self.type = type or consts.re.get_user_type(url)
         
@@ -118,15 +118,15 @@
         Fetch a user knowing its name or URL.
         Note - Using only a username makes the fetch between
         1 and 3 times slower, you might prefer to use a direct
         URL.
         
         Args:
             client (Client): The parent client.
-            user      (str): Username or URL.
+            user (str): Username or URL.
         '''
         
         if consts.re.is_url(user):
             url = user
             user_type = (path := url.split('/'))[-2]
             name = path[-1]
```

### Comparing `phub-4.5.7/src/phub/objects/video.py` & `phub-4.6/src/phub/objects/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     
     def __init__(self, client: Client, url: str) -> None:
         '''
         Initialise a new video object.
         
         Args:
             client (Client): The parent client.
-            url       (str): The video URL.
+            url (str): The video URL.
         '''
         
         if not consts.re.is_video_url(url):
             raise errors.URLError('Invalid video URL:', url)
         
         self.client = client
         
@@ -440,15 +440,15 @@
         url = self.data.get('page@image_url')
         
         if url:
             servers = None
         
         else:
             url = self.fetch('data@thumb')
-            servers = self.fetch('data@thumbs')
+            servers = self.data.get('data@thumbs') or [] # TODO - Use cache on prop Image.servers
         
         return Image(client = self.client,
                      url = url,
                      servers = servers,
                      name = f'thumb-{self.key}')
     
     @cached_property
@@ -617,25 +617,26 @@
     def watched(self) -> bool:
         '''
         Whether the video was viewed previously by the account.
         '''
         
         assert self.client.logged, 'Client must be logged in to use this property'
         
-        # If we fetched the video page while logged in, PH consider we have watched it
-        if self.page:
-            return True
-        
-        if 'watchedVideo' in self._as_query['markers']:
+        # Use query sortcut if possible
+        if self.data.get('query@watched'):
             return True
         
-        # For some reason the watched text is different in playlists
+        # Search in markers
         if 'class="watchedVideoText' in self._as_query['raw']:
             return True
         
+        # Evaluate on page (TODO)
+        if self.page:
+            ...
+        
         return False
     
     @property
     def is_favorite(self) -> bool:
         '''
         Whether the video has been set as favorite by the client.
         '''
```

### Comparing `phub-4.5.7/src/phub/tests/test_model.py` & `phub-4.6/src/phub/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/src/phub/tests/test_playlist.py` & `phub-4.6/src/phub/tests/test_playlist.py`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/src/phub/tests/test_search.py` & `phub-4.6/src/phub/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/src/phub/tests/test_video.py` & `phub-4.6/src/phub/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `phub-4.5.7/src/phub/utils.py` & `phub-4.6/src/phub/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def concat(*args) -> str:
     '''
     Concatenate multiple URL or file path parts.
 
     Args:
-        *args: A variable number of arguments, each can be a str or a pathlib.Path object.
+        args: A variable number of arguments, each can be a str or a pathlib.Path object.
 
     Returns:
         str: The concatenated path as a string.
     '''
 
     # Convert all arguments to strings first
     args = [str(arg).strip() for arg in args]
@@ -96,15 +96,15 @@
     return min(numbers, key = lambda x: abs(x - value))
 
 def serialize(object_: object, recursive: bool = False) -> object:
     '''
     Simple serializer for PHUB objects.
     
     Args:
-        object_    (Any): The object to serialize.
+        object_ (Any): The object to serialize.
         recursive (bool): Whether to allow serializing PHUB objects inside the object.
     
     Returns:
         Any: A JSON serializable object.
     '''
     
     # if an object is a built-in
@@ -136,18 +136,18 @@
             keys: str | list[str],
             all_: list[str],
             recursive: bool) -> dict:
     '''
     Dictify an object.
     
     Args:
-        object_     (Any): The object to serialize.
-        keys  (list[str]): A list of keys to dictify.
-        all_  (list[str]): The total list of serializeable object keys.
-        recursive  (bool): Whether to allow serializing PHUB objects inside the object.
+        object_ (Any): The object to serialize.
+        keys (list[str]): A list of keys to dictify.
+        all_ (list[str]): The total list of serializeable object keys.
+        recursive (bool): Whether to allow serializing PHUB objects inside the object.
     
     Returns:
         dict: The object dictified.
     '''
     
     if isinstance(keys, str): keys = [keys]
     if 'all' in keys: keys = all_
@@ -156,15 +156,15 @@
             for key in keys}
 
 def suppress(gen: Iterable, errs: Exception | tuple[Exception] = errors.VideoError) -> Iterator:
     '''
     Set up a generator to bypass items that throw errors.
     
     Args:
-        gen   (Iterable): The iterable to suppress.
+        gen (Iterable): The iterable to suppress.
         errs (Exception): The errors that fall under the suppression rule.
     
     Returns
         Iterator: The result iterator. 
     '''
     
     logger.info('Initialising suppressed generator')
@@ -224,15 +224,15 @@
 def head(client: object, url: str) -> str | bool:
     '''
     Performs a silent HEAD request to check if a page is available
     without fetching its content.
     
     Args:
         client (Client): A client containing an initialised session.
-        url       (str): The url of the request.
+        url (str): The url of the request.
     
     Returns:
         str | bool: The redirect URL if success, False otherwise.
     '''
     
     res = client.call(url, 'HEAD', throw = False, silent = True)
```

### Comparing `phub-4.5.7/src/phub.egg-info/PKG-INFO` & `phub-4.6/src/phub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 4.5.7
+Version: 4.6
 Summary: An API for Pornhub
 Author-email: Egsagon <egsagon12@gmail.com>, EchterAlsFake <EchterAlsFake@proton.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `phub-4.5.7/src/phub.egg-info/SOURCES.txt` & `phub-4.6/src/phub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

