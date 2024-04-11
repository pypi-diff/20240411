# Comparing `tmp/xmlcord-1.0.8.tar.gz` & `tmp/xmlcord-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlcord-1.0.8.tar", last modified: Sun Sep  4 14:21:13 2022, max compression
+gzip compressed data, was "xmlcord-1.0.9.tar", last modified: Fri Sep  9 14:27:52 2022, max compression
```

## Comparing `xmlcord-1.0.8.tar` & `xmlcord-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 14:21:13.866414 xmlcord-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-04 14:21:13.866414 xmlcord-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-04 14:21:06.000000 xmlcord-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-04 14:21:13.866414 xmlcord-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-09-04 14:21:06.000000 xmlcord-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 14:21:13.862414 xmlcord-1.0.8/xmlcord/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5765 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/listener.py
--rw-r--r--   0 runner    (1001) docker     (121)     7497 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/safeval.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 14:21:13.866414 xmlcord-1.0.8/xmlcord/tags/
--rw-r--r--   0 runner    (1001) docker     (121)     4614 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/tags/action.py
--rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/tags/ansi.py
--rw-r--r--   0 runner    (1001) docker     (121)     5600 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/tags/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8986 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/tags/control.py
--rw-r--r--   0 runner    (1001) docker     (121)     7645 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/tags/discord_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/tags/root.py
--rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-09-04 14:21:06.000000 xmlcord-1.0.8/xmlcord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 14:21:13.866414 xmlcord-1.0.8/xmlcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-04 14:21:13.000000 xmlcord-1.0.8/xmlcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-04 14:21:13.000000 xmlcord-1.0.8/xmlcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 14:21:13.000000 xmlcord-1.0.8/xmlcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-04 14:21:13.000000 xmlcord-1.0.8/xmlcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-04 14:21:13.000000 xmlcord-1.0.8/xmlcord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 14:27:52.408966 xmlcord-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-09 14:27:52.408966 xmlcord-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 14:27:39.000000 xmlcord-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-09 14:27:52.408966 xmlcord-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-09-09 14:27:39.000000 xmlcord-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 14:27:52.404966 xmlcord-1.0.9/xmlcord/
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5765 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/listener.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7610 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/safeval.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 14:27:52.408966 xmlcord-1.0.9/xmlcord/tags/
+-rw-r--r--   0 runner    (1001) docker     (121)     4614 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/tags/action.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/tags/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5687 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/tags/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9501 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/tags/control.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7717 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/tags/discord_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/tags/root.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-09-09 14:27:39.000000 xmlcord-1.0.9/xmlcord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 14:27:52.404966 xmlcord-1.0.9/xmlcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-09 14:27:52.000000 xmlcord-1.0.9/xmlcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-09 14:27:52.000000 xmlcord-1.0.9/xmlcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 14:27:52.000000 xmlcord-1.0.9/xmlcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-09 14:27:52.000000 xmlcord-1.0.9/xmlcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-09 14:27:52.000000 xmlcord-1.0.9/xmlcord.egg-info/top_level.txt
```

### Comparing `xmlcord-1.0.8/setup.py` & `xmlcord-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xmlcord",
-    version="1.0.8",
+    version="1.0.9",
     author="Fliqqr",
     author_email="author@example.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Fliqqr/xmlcord",
     packages=setuptools.find_packages(),
```

### Comparing `xmlcord-1.0.8/xmlcord/hooks.py` & `xmlcord-1.0.9/xmlcord/hooks.py`

 * *Files identical despite different names*

### Comparing `xmlcord-1.0.8/xmlcord/interface.py` & `xmlcord-1.0.9/xmlcord/interface.py`

 * *Files identical despite different names*

### Comparing `xmlcord-1.0.8/xmlcord/listener.py` & `xmlcord-1.0.9/xmlcord/listener.py`

 * *Files identical despite different names*

### Comparing `xmlcord-1.0.8/xmlcord/renderer.py` & `xmlcord-1.0.9/xmlcord/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,28 +30,29 @@
         # return root.message_tags()
 
     def get_message_ids(self) -> [int]:
         return [message.id for message in self.messages]
 
     async def update_reactions(self, message, reactions):
         # check if reactions need updating
-        if reactions == self.reactions.get(message.id, []):
+        if reactions == (curr_reactions := self.reactions.get(message.id, [])):
             return
 
-        await message.clear_reactions()
+        if curr_reactions:
+            await message.clear_reactions()
         # manually keeping track of the reactions we are adding
         self.reactions[message.id] = reactions
 
         for emoji in reactions:
             await message.add_reaction(emoji)
 
     # creates and publishes a new message object while adding
     # it to the messages list
     async def new_message(self, tag) -> discord.Message:
-        message = await self.context.send(content=tag.message, embed=tag.embed)
+        message = await self.context.channel.send(content=tag.message, embed=tag.embed)
 
         self.messages.append(message)
 
         return message
 
     # retrieves message object from messages list
     def get_message(self, index) -> discord.Message:
@@ -197,14 +198,15 @@
             await self.context.author.create_dm()
 
         return self.context.author.dm_channel
 
     async def construct(self, root):
         # this is stupid
         if root.config.get('channel') == 'dm' and not self.swap:
+            # this is even stupider
             self.context.channel = await self.get_dm_channel()
 
         await self.display.construct(root)
 
         self.listener.add_renderer(self)
 
     # needs to be capable of swiching channels 
@@ -223,14 +225,15 @@
         else:
             await self.display.update(root)
 
     def swap_channel(self, channel_id):
         self.swap = True
         channel = self.context.guild.get_channel(int(channel_id))
 
+        # BAD, NO
         self.context.channel = channel
 
         self.display = TemplateDisplay(self.context)
 
     async def deactivate(self):
         self.listener.remove_renderer(self)
         await self.display.deactivate()
```

### Comparing `xmlcord-1.0.8/xmlcord/safeval.py` & `xmlcord-1.0.9/xmlcord/safeval.py`

 * *Files identical despite different names*

### Comparing `xmlcord-1.0.8/xmlcord/tags/__init__.py` & `xmlcord-1.0.9/xmlcord/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlcord-1.0.8/xmlcord/tags/action.py` & `xmlcord-1.0.9/xmlcord/tags/action.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,7 +42,23 @@
         name='cleanup',
         singleton=True
     )
 
     @on_render()
     async def render(self, args):
         self.ui.clean_up()
+
+
+class ForwardTag(Tag):
+
+    _config = TagConfig(
+        name="forward",
+        args={
+            "channel": int,
+            "mode":    Optional(str, "view")
+        },
+        singleton=True
+    )
+
+    @on_render()
+    async def render(self, args):
+        self.ui.forward(args.channel, args.mode)
```

### Comparing `xmlcord-1.0.8/xmlcord/tags/ansi.py` & `xmlcord-1.0.9/xmlcord/tags/ansi.py`

 * *Files identical despite different names*

### Comparing `xmlcord-1.0.8/xmlcord/tags/base.py` & `xmlcord-1.0.9/xmlcord/tags/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,18 +225,21 @@
         self._content = content[start:end]
 
     async def render_children(self) -> list:
         children_contents = []
 
         for child in self.children:
 
-            children_contents.append(
-                # without this we would have 'None' whenever
-                # a child does not return any content
-                await child.render() or ''
-            )
+            content = await child.render()
+
+            if not child.singleton:
+                children_contents.append(
+                    # without this we would have 'None' whenever
+                    # a child does not return any content
+                    content or ''
+                )
 
         return children_contents
 
     @abstractmethod
     async def render(self, *_):
         ...
```

### Comparing `xmlcord-1.0.8/xmlcord/tags/control.py` & `xmlcord-1.0.9/xmlcord/tags/control.py`

 * *Files 3% similar despite different names*

```diff
@@ -298,14 +298,39 @@
             {args.var: args.value}
         )
         # page flipping needs this to work but 
         # when outside conditional it causes infinte loop
         # self.root.double_render()
 
 
+class GetTag(Tag):
+
+    _config = TagConfig(
+        name="get",
+        args={
+            "var":     str,
+            "source":  list,
+            "key":     str,
+            "default": Optional(int, 0)
+        },
+        singleton=True
+    )
+
+    @on_render()
+    async def render(self, args):
+        for item in args.source:
+            if item[0] == args.key:
+                var = item[1:]
+                break
+        else:
+            var = args.default
+
+        self.root.update_state({args.var: var})
+
+
 class DecorTag(Tag):
 
     _config = TagConfig(
         name="decor",
         args={
             "exp": Optional(bool, False),
             "op":  str,
```

### Comparing `xmlcord-1.0.8/xmlcord/tags/discord_tags.py` & `xmlcord-1.0.9/xmlcord/tags/discord_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,16 @@
             except TypeError:
                 return ''
 
             context = self.ui.renderer.context
             member_info = []
 
             if fetchUsers := self.first_ancestor('fetchUsers'):
-
+                
+                # member is not guaranteed to exist here
                 member = fetchUsers.get_state(user_id)
                 # saves the member info in root for future use,
                 # in case the member leaves the server
                 self.root.update_state({
                     user_id: self.get_member_info(member)
                 })
 
@@ -294,15 +295,14 @@
 
             elif member := await context.guild.fetch_member(user_id):
                 member_info = self.get_member_info(member)
 
             elif member := self.root.get_state(user_id):
                 member_info = member
 
-
             if member_info:
                 self.update_state({
                     'name':       member_info[0],
                     'nick':       member_info[1] or member_info[0],
                     'roles':      member_info[2],
                     'avatar_url': member_info[3]
                 })
```

### Comparing `xmlcord-1.0.8/xmlcord/tags/root.py` & `xmlcord-1.0.9/xmlcord/tags/root.py`

 * *Files identical despite different names*

### Comparing `xmlcord-1.0.8/xmlcord/utils.py` & `xmlcord-1.0.9/xmlcord/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,33 +3,34 @@
     connections = []
     for character1 in sample1:
         for i, character2 in enumerate(sample2[::-1]):
             index = len(sample2) - i - 1
             if character1 == character2:
                 # finds the highest position within connection layers where index can be inserted
                 if connections:
-                    added = False
                     # goes through all the connection layers in a reverse order
                     for depth, layer in enumerate(connections[::-1]):
                         if min(layer) < index:
                             layer_index = len(connections) - depth
                             if layer_index < len(connections):
                                 if index not in connections[layer_index]:
                                     connections[layer_index].append(index)
                             else:
                                 connections.append([index])
-                            added = True
                             break
-                    if not added and index not in connections[0]:
-                        connections[0].append(index)
+                    else: 
+                        if index not in connections[0]:
+                            connections[0].append(index)
                 else:
                     # if connection list is empty create a new connection and insert first (lowest) found value
                     connections.append([index])
             # print(character1, character2)
             # print(connections)
+        
+    # print(connections)
 
     return (len(connections) / len(sample1)) / (len(sample1) + len(sample2) - 2 * len(connections) + 1)
 
 
 def find_item_in_array(string, array, threshold=0):
     value = 0
     out = None
@@ -38,10 +39,10 @@
         if (value == 0 or sim > value) and sim >= threshold:
             value = sim
             out = item
     return out
 
 
 if __name__ == '__main__':
-    s1 = "darkrider"
-    s2 = "dickrider"
-    similarity(s1, s2)
+    s1 = "Fliqqrrrr"
+    s2 = "Flqqrrrri"
+    print(similarity(s1, s2))
```

