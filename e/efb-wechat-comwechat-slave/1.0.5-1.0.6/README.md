# Comparing `tmp/efb-wechat-comwechat-slave-1.0.5.tar.gz` & `tmp/efb-wechat-comwechat-slave-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efb-wechat-comwechat-slave-1.0.5.tar", last modified: Thu Feb 23 13:26:00 2023, max compression
+gzip compressed data, was "efb-wechat-comwechat-slave-1.0.6.tar", last modified: Thu Apr 11 13:58:18 2024, max compression
```

## Comparing `efb-wechat-comwechat-slave-1.0.5.tar` & `efb-wechat-comwechat-slave-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:26:00.477036 efb-wechat-comwechat-slave-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-23 13:26:00.477036 efb-wechat-comwechat-slave-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-23 13:25:47.000000 efb-wechat-comwechat-slave-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:26:00.477036 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-02-23 13:25:47.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/ChatMgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    26654 2023-02-23 13:25:47.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/ComWechat.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-23 13:25:47.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/CustomTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25908 2023-02-23 13:25:47.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/MsgDeco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-02-23 13:25:47.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/MsgProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-02-23 13:25:47.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-23 13:25:47.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-23 13:25:47.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 13:26:00.477036 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-23 13:26:00.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-23 13:26:00.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 13:26:00.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-23 13:26:00.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-23 13:26:00.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-23 13:26:00.000000 efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 13:26:00.477036 efb-wechat-comwechat-slave-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-02-23 13:25:47.000000 efb-wechat-comwechat-slave-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:58:18.553969 efb-wechat-comwechat-slave-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-11 13:58:18.553969 efb-wechat-comwechat-slave-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-11 13:58:14.000000 efb-wechat-comwechat-slave-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:58:18.549969 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-11 13:58:14.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/ChatMgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26929 2024-04-11 13:58:14.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/ComWechat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-11 13:58:14.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/CustomTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25621 2024-04-11 13:58:14.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/MsgDeco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-11 13:58:14.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/MsgProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-11 13:58:14.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-11 13:58:14.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 13:58:14.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:58:18.549969 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-11 13:58:18.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-11 13:58:18.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:58:18.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-11 13:58:18.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-11 13:58:18.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 13:58:18.000000 efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:58:18.553969 efb-wechat-comwechat-slave-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-11 13:58:14.000000 efb-wechat-comwechat-slave-1.0.6/setup.py
```

### Comparing `efb-wechat-comwechat-slave-1.0.5/README.md` & `efb-wechat-comwechat-slave-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/ChatMgr.py` & `efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/ChatMgr.py`

 * *Files identical despite different names*

### Comparing `efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/ComWechat.py` & `efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/ComWechat.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     config : Dict = {}
 
     friends : EFBPrivateChat = []
     groups : EFBGroupChat    = []
 
     contacts : Dict = {}            # {wxid : {alias : str , remark : str, nickname : str , type : int}} -> {wxid : name(after handle)}
     group_members : Dict = {}       # {"group_id" : { "wxID" : "displayName"}}
-    
+
     time_out : int = 120
     cache =  TTLCache(maxsize=200, ttl= time_out)  # 缓存发送过的消息ID
     file_msg : Dict = {}                           # 存储待修改的文件类消息 {path : msg}
     delete_file : Dict = {}                        # 存储待删除的消息 {path : time}
 
     __version__ = version.__version__
     logger: logging.Logger = logging.getLogger("comwechat")
@@ -95,15 +95,15 @@
                 author = chat.self
 
             self.handle_msg(msg , author , chat)
 
         @self.bot.on("friend_msg")
         def on_friend_msg(msg : Dict):
             self.logger.debug(f"friend_msg:{msg}")
-            
+
             sender = msg['sender']
 
             if msg["type"] == "eventnotify":
                 return
 
             name = self.get_name_by_wxid(sender)
 
@@ -112,23 +112,23 @@
                     name= name,
             ))
             if sender.startswith('gh_'):
                 chat.vendor_specific = {'is_mp' : True}
                 self.logger.debug(f'modified_chat:{chat}')
             author = chat.other
             self.handle_msg(msg, author, chat)
-            
+
         @self.bot.on("group_msg")
         def on_group_msg(msg : Dict):
             self.logger.debug(f"group_msg:{msg}")
             sender = msg["sender"]
-            wxid  =  msg["wxid"] 
+            wxid  =  msg["wxid"]
 
             chatname = self.get_name_by_wxid(sender)
-                
+
             chat = ChatMgr.build_efb_chat_as_group(EFBGroupChat(
                 uid = sender,
                 name = chatname,
             ))
 
             try:
                 name = self.contacts[wxid]
@@ -143,15 +143,15 @@
             self.handle_msg(msg, author, chat)
 
         @self.bot.on("revoke_msg")
         def on_revoked_msg(msg : Dict):
             self.logger.debug(f"revoke_msg:{msg}")
             sender = msg["sender"]
             if "@chatroom" in sender:
-                wxid  =  msg["wxid"] 
+                wxid  =  msg["wxid"]
 
             name = self.get_name_by_wxid(sender)
 
             if "@chatroom" in sender:
                 chat = ChatMgr.build_efb_chat_as_group(EFBGroupChat(
                     uid = sender,
                     name = name,
@@ -283,48 +283,55 @@
             content["message"] = text
             content["name"] = name
             # if "v3" in username:
             #     content["commands"] = commands
             # 暂时屏蔽
             self.system_msg(content)
 
+    @staticmethod
+    def send_efb_msgs(efb_msgs: Union[Message, List[Message]], **kwargs):
+        if not efb_msgs:
+            return
+        efb_msgs = [efb_msgs] if isinstance(efb_msgs, Message) else efb_msgs
+        if 'deliver_to' not in kwargs:
+            kwargs['deliver_to'] = coordinator.master
+        for efb_msg in efb_msgs:
+            for k, v in kwargs.items():
+                setattr(efb_msg, k, v)
+            coordinator.send_message(efb_msg)
+            if efb_msg.file:
+                efb_msg.file.close()
+
     def system_msg(self, content : Dict):
         self.logger.debug(f"system_msg:{content}")
         msg = Message()
         sender = content["sender"]
         if "name" in content:
             name = content["name"]
         else:
-            name  = '\u2139 System' 
-        
+            name  = '\u2139 System'
+
         chat = ChatMgr.build_efb_chat_as_system_user(EFBSystemUser(
             uid = sender,
             name = name
         ))
-        
+
         try:
             author = chat.get_member(SystemChatMember.SYSTEM_ID)
         except KeyError:
             author = chat.add_system_member()
-        
+
         if "commands" in content:
             msg.commands = MessageCommands(content["commands"])
         if "message" in content:
             msg.text = content['message']
 
-        msg.uid = int(time.time())
-        msg.chat = chat
-        msg.author = author
-        msg.deliver_to = coordinator.master
-        msg.type = MsgType.Text
-        coordinator.send_message(msg)
+        self.send_efb_msgs(msg, uid=int(time.time()), chat=chat, author=author, type=MsgType.Text)
 
     def handle_msg(self , msg : Dict[str, Any] , author : 'ChatMember' , chat : 'Chat'):
-        efb_msgs = []
-
         emojiList = re.findall('\[[\w|！|!| ]+\]' , msg["message"])
         for emoji in emojiList:
             try:
                 msg["message"] = msg["message"].replace(emoji, WC_EMOTICON_CONVERSION[emoji])
             except:
                 pass
 
@@ -353,24 +360,15 @@
         if msg["type"] == "voice":
             file_path = re.search("clientmsgid=\"(.*?)\"", msg["message"]).group(1) + ".amr"
             msg["timestamp"] = int(time.time())
             msg["filepath"] = f'''{self.dir}{msg["self"]}/{file_path}'''
             self.file_msg[msg["filepath"]] = ( msg , author , chat )
             return
 
-        efb_msg = MsgProcess(msg , chat)
-        if not efb_msg:
-            return
-        efb_msg.author = author
-        efb_msg.chat = chat
-        efb_msg.uid = msg["msgid"]
-        efb_msg.deliver_to = coordinator.master
-        coordinator.send_message(efb_msg)
-        if efb_msg.file:
-            efb_msg.file.close()
+        self.send_efb_msgs(MsgProcess(msg, chat), author=author, chat=chat, uid=msg['msgid'])
 
     def handle_file_msg(self):
         while True:
             if len(self.file_msg) == 0:
                 time.sleep(1)
             else:
                 for path in list(self.file_msg.keys()):
@@ -391,44 +389,37 @@
                         if len(dbresult) == 2:
                             filebuffer = dbresult[1][0]
                             decoded = bytes(base64.b64decode(filebuffer))
                             with open(msg["filepath"], 'wb') as f:
                                 f.write(decoded)
                             f.close()
                             flag = True
-                    
+
                     if flag:
                         del self.file_msg[path]
-                        efb_msg = MsgProcess(msg , chat)
-                        efb_msg.author = author
-                        efb_msg.chat = chat
-                        efb_msg.uid = msg["msgid"]
-                        efb_msg.deliver_to = coordinator.master
-                        coordinator.send_message(efb_msg)
-                        if efb_msg.file:
-                            efb_msg.file.close()
+                        self.send_efb_msgs(MsgProcess(msg, chat), author=author, chat=chat, uid=msg['msgid'])
 
             if len(self.delete_file):
                 for k in list(self.delete_file.keys()):
                     file_path = k
                     begin_time = self.delete_file[k]
                     if  (int(time.time()) - begin_time) > self.time_out:
                         try:
                             os.remove(file_path)
                         except:
                             pass
-                        del self.delete_file[file_path]  
+                        del self.delete_file[file_path]
 
     def process_friend_request(self , v3 , v4):
         self.logger.debug(f"process_friend_request:{v3} {v4}")
         res = self.bot.VerifyApply(v3 = v3 , v4 = v4)
         if str(res['msg']) != "0":
             return "Success"
         else:
-            return "Failed" 
+            return "Failed"
 
     def process_transfer(self, transcationid , transferid , wxid):
         res = self.bot.GetTransfer(transcationid = transcationid , transferid = transferid , wxid = wxid)
         if str(res["msg"]) != "0":
             return "Success"
         else:
             return "Failed"
@@ -439,15 +430,15 @@
             return "Success"
         else:
             return "Failed"
 
     # 定时任务
     def scheduled_job(self):
         count = 1
-        while True: 
+        while True:
             time.sleep(1)
             if count % 1800 == 0:
                 self.GetGroupListBySql()
                 self.GetContactListBySql()
                 count = 1
             else:
                 count += 1
@@ -458,15 +449,15 @@
             self.GetContactListBySql()
         return self.groups + self.friends
 
     #获取联系人
     def get_chat(self, chat_uid: ChatID) -> 'Chat':
         if not self.friends and not self.groups:
             self.GetContactListBySql()
-        
+
         if "@chatroom" in chat_uid:
             for group in self.groups:
                 if group.uid == chat_uid:
                     return group
         else:
             for friend in self.friends:
                 if friend.uid == chat_uid:
@@ -482,15 +473,15 @@
         if msg.type == MsgType.Voice:
             f = tempfile.NamedTemporaryFile(prefix='voice_message_', suffix=".mp3")
             AudioSegment.from_ogg(msg.file.name).export(f, format="mp3")
             msg.file = f
             msg.file.name = "语音留言.mp3"
             msg.type = MsgType.Video
             msg.filename = f.name.split("/")[-1]
-        
+
         if msg.type in [MsgType.Text]:
             if msg.text.startswith('/changename'):
                 newname = msg.text.strip('/changename ')
                 res = self.bot.SetChatroomName(chatroom_id = chat_uid , chatroom_name = newname)
             elif msg.text.startswith('/getmemberlist'):
                 memberlist = self.bot.GetChatroomMemberList(chatroom_id = chat_uid)
                 message = '群组成员包括：'
@@ -526,14 +517,16 @@
 
 /at - 后面跟wxid，多个用英文,隔开，最后可用空格隔开，带内容。
 
 /sendcard - 后面格式'wxid nickname'
 
 /changename - 修改群组名称
 
+/addfriend - 后面格式'wxid message'
+
 /getstaticinfo - 可获取friends, groups, contacts信息'''
                 self.system_msg({'sender':chat_uid, 'message':message})
             elif msg.text.startswith('/search'):
                 keyword = msg.text[8::]
                 message = 'result:'
                 for key, value in self.contacts.items():
                     if keyword in value:
@@ -558,14 +551,24 @@
                     user, nickname = user_nickname
                 else:
                     user, nickname = user_nickname[0], ''
                 if user != '':
                     res = self.bot.SendCard(receiver = chat_uid, share_wxid = user, nickname = nickname)
                 else:
                     self.bot.SendText(wxid = chat_uid , msg = msg.text)
+            elif msg.text.startswith('/addfriend'):
+                user_invite = msg.text[11::].split(' ', 1)
+                if len(user_invite) == 2:
+                    user, invite = user_invite
+                else:
+                    user, invite = user_invite[0], ''
+                if user != '':
+                    res = self.bot.AddContactByWxid(wxid = user, msg = invite)
+                else:
+                    self.bot.SendText(wxid = chat_uid , msg = msg.text)
             else:
                 res = self.bot.SendText(wxid = chat_uid , msg = msg.text)
         elif msg.type in [MsgType.Link]:
             self.bot.SendText(wxid = chat_uid , msg = msg.text)
         elif msg.type in [MsgType.Image , MsgType.Sticker]:
             name = msg.file.name.replace("/tmp/", "")
             local_path =f"{self.dir}{self.wxid}/{name}"
@@ -643,15 +646,15 @@
     def get_message_by_id(self, chat: 'Chat', msg_id: MessageID) -> Optional['Message']:
         ...
 
     def get_name_by_wxid(self, wxid):
         try:
             name = self.contacts[wxid]
             if name == "":
-                name = sender
+                name = wxid
         except:
             data = self.bot.GetContactBySql(wxid = wxid)
             if data:
                 name = data[3]
                 if name == "":
                     name = wxid
             else:
@@ -684,8 +687,8 @@
                 )
                 self.friends.append(ChatMgr.build_efb_chat_as_private(new_entity))
 
     def GetGroupListBySql(self):
         self.group_members = self.bot.GetAllGroupMembersBySql()
     #定时更新 End
 
-    
+
```

### Comparing `efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/MsgDeco.py` & `efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/MsgDeco.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Mapping, Tuple, Union, IO
+from typing import Mapping, Tuple, List, Union, IO
 import magic
 from lxml import etree
+from functools import partial
 from traceback import print_exc
 import re , json
 
 from ehforwarderbot import MsgType, Chat
 from ehforwarderbot.chat import ChatMember
 from ehforwarderbot.message import Substitutions, Message, LinkAttribute, LocationAttribute
 
@@ -20,21 +21,21 @@
         type=MsgType.Text,
         text=text
     )
     if ats:
         efb_msg.substitutions = Substitutions(ats)
     return efb_msg
 
-def efb_image_wrapper(file: IO, filename: str = None, text: str = None) -> Message:
+def efb_image_wrapper(file: IO, filename: str = None, text: str = None) -> Union[Message, List[Message]]:
     """
     A EFB message wrapper for images.
     :param file: The file handle
     :param filename: The actual filename
     :param text: The attached text
-    :return: EFB Message
+    :return: EFB Message or list of EFB Messages
     """
     efb_msg = Message()
     efb_msg.file = file
     mime = magic.from_file(file.name, mime=True)
     if isinstance(mime, bytes):
         mime = mime.decode()
 
@@ -102,14 +103,44 @@
         efb_msg.filename += '.' + str(mime).split('/')[1]  # Add extension suffix
     efb_msg.path = efb_msg.file.name
     efb_msg.mime = mime
     if text:
         efb_msg.text = text
     return efb_msg
 
+def efb_mp_post_wrapper(item: etree.Element, show_name: str = None) -> Message:
+    url = cover = None
+    title = digest = result_text = ''
+    try:
+        title = item.find('title').text
+        url = item.find('url').text
+        digest = item.find('digest').text
+        cover = item.find('cover').text
+    except Exception:
+        print_exc()
+
+    digest += f'\n- - - - from {show_name}' if show_name else ''
+    if title and url:
+        attribute = LinkAttribute(
+            title=title,
+            description=digest,
+            url=url,
+            image=cover,
+        )
+        return Message(
+            attributes=attribute,
+            type=MsgType.Link,
+            text=result_text,
+            vendor_specific={'is_mp': True},
+        )
+    # 部分公众号通知没有url信息
+    return Message(
+        type=MsgType.Text,
+        text=f'{title}\n  - - - - - - - - - - - - - - - \n{digest}' if digest else str(title),
+    )
 
 def efb_share_link_wrapper(text: str) -> Message:
     """
     处理msgType49消息 - 复合xml, xml 中 //appmsg/type 指示具体消息类型.
     /msg/appmsg/type
     已知：
     //appmsg/type = 1 : 百度网盘分享
@@ -124,26 +155,26 @@
     //appmsg/type = 21 : 微信运动
     //appmsg/type = 24 : 从收藏中分享的笔记
     //appmsg/type = 33 : 美团外卖
     //appmsg/type = 35 : 消息同步
     //appmsg/type = 36 : 京东农场，滴滴打车
     //appmsg/type = 51 : 视频（微信视频号分享）
     //appmsg/type = 53 : 转账过期退还通知
-    //appmsg/type = 57 : 引用(回复)消息，未细致研究哪个参数是被引用的消息 id 
+    //appmsg/type = 57 : 引用(回复)消息，未细致研究哪个参数是被引用的消息 id
     //appmsg/type = 63 : 直播（微信视频号分享）
     //appmsg/type = 74 : 文件 (收到文件的第一个提示)
     //appmsg/type = 87 : 群公告
     //appmsg/type = 2000 : 转账
     :param text: The content of the message
     :return: EFB Message
     """
 
     xml = etree.fromstring(text)
     result_text = ""
-    try: 
+    try:
         type = int(xml.xpath('/msg/appmsg/type/text()')[0])
         if type in [ 1 , 2 ]:
             title = xml.xpath('/msg/appmsg/title/text()')[0]
             des = xml.xpath('/msg/appmsg/des/text()')[0]
             efb_msg = Message(
                 type = MsgType.Text,
                 text = title if title==des else title+" :\n"+des,
@@ -239,46 +270,16 @@
                         attributes=attribute,
                         type=MsgType.Link,
                         text=result_text,
                         vendor_specific={ "is_mp": True }
                     )
             elif showtype == 1: # 公众号发的推送
                 items = xml.xpath('//item')
-                for item in items:
-                    title = url = digest = cover = None # 初始化
-                    try:
-                        title = item.find("title").text
-                        url = item.find("url").text
-                        digest = item.find("digest").text
-                        cover = item.find("cover").text
-                    except Exception as e:
-                        print_exc()
-                    
-                    if '@app' in text:
-                        name = xml.xpath('//publisher/nickname/text()')[0]
-                        digest += f"\n- - - - from {name}"
-                    if title and url:
-                        attribute = LinkAttribute(
-                            title=title,
-                            description=digest,
-                            url=url,
-                            image= cover,
-                        )
-                        efb_msg = Message(
-                            attributes=attribute,
-                            type=MsgType.Link,
-                            text=result_text,
-                            vendor_specific={ "is_mp": True }
-                        )
-                    else: # 部分公众号通知没有url信息
-                        result_text += f"{title}\n  - - - - - - - - - - - - - - - \n{digest}"
-                        efb_msg = Message(
-                            type=MsgType.Text,
-                            text=result_text
-                        )
+                show_name = xml.xpath('//publisher/nickname/text()')[0] if '@app' in text else ''
+                efb_msg = list(map(partial(efb_mp_post_wrapper, show_name=show_name), items))
         elif type == 8:
             efb_msg = Message(
                 type=MsgType.Unsupported,
                 text='未解密表情消息 ，请在手机端查看',
             )
         elif type == 17:
             msg_title = xml.xpath('/msg/appmsg/title/text()')[0]
@@ -342,15 +343,15 @@
                 vendor_specific={ "is_mp": True }
             )
         elif type == 35:
             efb_msg = Message(
                 type=MsgType.Text,
                 text= '系统消息 : 消息同步',
                 vendor_specific={ "is_mp": False }
-            )  
+            )
         elif type == 40: # 转发的转发消息
             title = xml.xpath('/msg/appmsg/title/text()')[0]
             desc = xml.xpath('/msg/appmsg/des/text()')[0]
             efb_msg = Message(
                 type=MsgType.Text,
                 text= f"{title}\n\n{desc}" ,
                 vendor_specific={ "is_forwarded": True }
@@ -606,15 +607,15 @@
                 efb_msg = efb_text_simple_wrapper(f"[{displayname} 进入扫码支付]")
             if str(status) == "1":
                 efb_msg = efb_text_simple_wrapper(f"[{displayname} 完成了扫码支付]")
             elif str(status) == "2":
                 efb_msg = efb_text_simple_wrapper(f"[{displayname} 取消了扫码支付]")
         if "待接收" in text and "转账" in text:
             efb_msg = efb_text_simple_wrapper("[你有一笔待接收的转账]")
-        
+
     elif msg_type == "carditemmsg":
         msg_type = xml.xpath('/sysmsg/carditemmsg/msg_type/text()')[0]
         if str(msg_type) == "15":
             title = xml.xpath('/sysmsg/carditemmsg/title/text()')[0]
             desc = xml.xpath('/sysmsg/carditemmsg/description/text()')[0]
             url = xml.xpath('/sysmsg/carditemmsg/logo_url/text()')[0]
             attribute = LinkAttribute(
```

### Comparing `efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/MsgProcess.py` & `efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/MsgProcess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from typing import Union, List
 import base64
 import tempfile
 import logging
 from .Utils import *
 from .MsgDeco import *
 import re
 import pydub
 import json
 from lxml import etree
 
 from ehforwarderbot import utils as efb_utils
 from ehforwarderbot.message import Message
 
-def MsgProcess(msg : dict , chat) -> Message:
+def MsgProcess(msg : dict , chat) -> Union[Message, List[Message]]:
 
     if msg["type"] == "text":
         at_list = {}
         try:
             if "<atuserlist>" in msg["extrainfo"]:
                 at_user = re.search("<atuserlist>(.*)<\/atuserlist>", msg["extrainfo"]).group(1)
                 if msg["self"] in at_user:
@@ -25,15 +26,15 @@
             ...
         if at_list:
             return efb_text_simple_wrapper(msg['message'] , at_list)
         return efb_text_simple_wrapper(msg['message'])
 
     elif msg["type"] == "sysmsg":
         if "<revokemsg>" in msg["message"]:  # 重复的撤回通知，不在此处处理
-            return                            
+            return
         return efb_text_simple_wrapper("[" + msg['message'] + "]")
 
     elif msg["type"] == "image":
         file = wechatimagedecode(msg["filepath"])
         return efb_image_wrapper(file)
 
     elif msg["type"] == "animatedsticker":
@@ -44,27 +45,27 @@
         except:
             return efb_text_simple_wrapper("Image received and download failed. Please check it on your phone.")
 
     elif msg["type"] == "share":
         if ("FileStorage" in msg["filepath"]) and ("Cache" not in msg["filepath"]):
             file = load_local_file_to_temp(msg["filepath"])
             return efb_file_wrapper(file , msg["filepath"].split("/")[-1])
-        return efb_share_link_wrapper(msg['message'])
+        return efb_share_link_wrapper(msg['message'])  # may return msgs in a list
 
     elif msg["type"] == "voice":
         file = convert_silk_to_mp3(load_local_file_to_temp(msg["filepath"]))
         return efb_voice_wrapper(file , file.name + ".ogg")
 
     elif msg["type"] == "video":
         file = load_local_file_to_temp(msg["filepath"])
         return efb_video_wrapper(file)
-    
+
     elif msg["type"] == "location":
         return efb_location_wrapper(msg["message"])
-    
+
     elif msg["type"] == "qqmail":
         return efb_qqmail_wrapper(msg["message"])
 
     elif msg["type"] == "voip":
         if "<status>1</status>" in msg["message"]:
             return efb_text_simple_wrapper("[语音/视频聊天]\n  - - - - - - - - - - - - - - - \n[语音邀请]")
         if "<status>2</status>" in msg["message"]:
```

### Comparing `efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave/Utils.py` & `efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave/Utils.py`

 * *Files identical despite different names*

### Comparing `efb-wechat-comwechat-slave-1.0.5/efb_wechat_comwechat_slave.egg-info/SOURCES.txt` & `efb-wechat-comwechat-slave-1.0.6/efb_wechat_comwechat_slave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efb-wechat-comwechat-slave-1.0.5/setup.py` & `efb-wechat-comwechat-slave-1.0.6/setup.py`

 * *Files identical despite different names*

