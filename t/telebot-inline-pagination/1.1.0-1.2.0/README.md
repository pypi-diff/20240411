# Comparing `tmp/telebot_inline_pagination-1.1.0.tar.gz` & `tmp/telebot_inline_pagination-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebot_inline_pagination-1.1.0.tar", last modified: Wed Sep 27 12:12:05 2023, max compression
+gzip compressed data, was "telebot_inline_pagination-1.2.0.tar", last modified: Thu Apr 11 12:34:12 2024, max compression
```

## Comparing `telebot_inline_pagination-1.1.0.tar` & `telebot_inline_pagination-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-09-27 12:12:05.866021 telebot_inline_pagination-1.1.0/
--rw-rw-rw-   0        0        0     1087 2023-09-21 11:33:13.000000 telebot_inline_pagination-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     9984 2023-09-27 12:12:05.866563 telebot_inline_pagination-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     9605 2023-09-27 12:06:50.000000 telebot_inline_pagination-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-09-27 12:12:05.866563 telebot_inline_pagination-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      599 2023-09-27 12:10:22.000000 telebot_inline_pagination-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-27 12:12:05.861524 telebot_inline_pagination-1.1.0/telebot_inline_pagination/
--rw-rw-rw-   0        0        0     4109 2023-09-27 11:40:25.000000 telebot_inline_pagination-1.1.0/telebot_inline_pagination/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-27 12:12:05.864679 telebot_inline_pagination-1.1.0/telebot_inline_pagination.egg-info/
--rw-rw-rw-   0        0        0     9984 2023-09-27 12:12:05.000000 telebot_inline_pagination-1.1.0/telebot_inline_pagination.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-09-27 12:12:05.000000 telebot_inline_pagination-1.1.0/telebot_inline_pagination.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-27 12:12:05.000000 telebot_inline_pagination-1.1.0/telebot_inline_pagination.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-09-27 12:12:05.000000 telebot_inline_pagination-1.1.0/telebot_inline_pagination.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-09-27 12:12:05.000000 telebot_inline_pagination-1.1.0/telebot_inline_pagination.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 12:34:12.178770 telebot_inline_pagination-1.2.0/
+-rw-rw-rw-   0        0        0     1087 2023-09-21 11:33:13.000000 telebot_inline_pagination-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    10191 2024-04-11 12:34:12.178770 telebot_inline_pagination-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9790 2024-04-11 12:16:39.000000 telebot_inline_pagination-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 12:34:12.179768 telebot_inline_pagination-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      599 2024-04-11 12:32:22.000000 telebot_inline_pagination-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 12:34:12.171695 telebot_inline_pagination-1.2.0/telebot_inline_pagination/
+-rw-rw-rw-   0        0        0     7636 2024-04-11 12:05:12.000000 telebot_inline_pagination-1.2.0/telebot_inline_pagination/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 12:34:12.176765 telebot_inline_pagination-1.2.0/telebot_inline_pagination.egg-info/
+-rw-rw-rw-   0        0        0    10191 2024-04-11 12:34:12.000000 telebot_inline_pagination-1.2.0/telebot_inline_pagination.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-11 12:34:12.000000 telebot_inline_pagination-1.2.0/telebot_inline_pagination.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 12:34:12.000000 telebot_inline_pagination-1.2.0/telebot_inline_pagination.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-11 12:34:12.000000 telebot_inline_pagination-1.2.0/telebot_inline_pagination.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-11 12:34:12.000000 telebot_inline_pagination-1.2.0/telebot_inline_pagination.egg-info/top_level.txt
```

### Comparing `telebot_inline_pagination-1.1.0/LICENSE` & `telebot_inline_pagination-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `telebot_inline_pagination-1.1.0/PKG-INFO` & `telebot_inline_pagination-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: telebot_inline_pagination
-Version: 1.1.0
+Version: 1.2.0
 Summary: Pageable inline keyboard for pyTelegramBotAPI (telebot)
 Home-page: https://github.com/kremastra/telebot-inline-pagination
 Author: kremastra
 Author-email: fotisgrek@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: telebot
 
 # Pageable inline keyboard for [pyTelegramBotAPI](https://github.com/eternnoir/pyTelegramBotAPI/) (telebot)
 
 A library for pyTelegramBotAPI that allows you to display data in the format of a pageable inline keyboard.
 
 ## Installation
 You can use [pip](https://pip.pypa.io/en/stable/) to install this library.
@@ -53,14 +54,15 @@
             ('George Bush Intercontinental Airport', 'IAH/KIAH', 'Houston, Texas, United States')
         ]
 
 text_message = 'Demo'        
 ```
 
 ### Optional parameters
+**row_width**: The number of buttons per row (from 1 to 3, by default - 1).
 
 **rows_per_page**: The number of rows of buttons on one page, excluding the navigation bar (by default - 5).
 
 **text_index**: Column index - data source for button titles (by default - 0).
 
 **callback_index**: Column index - data source for callback-function (by default - 0).
 
@@ -74,56 +76,57 @@
 
 **previous_index**: Content of the button to go to the previous page (by default - '<---').
 
 ```py
 TEXT_INDEX = 0 # in this example, full airport name
 CALLBACK_INDEX = 1 # in this example, IATA/ICAO airport code
 BUTTON_TEXT_MODE = 2 # in this example, "full airport name (IATA/ICAO airport code)"
+ROW_WIDTH = 1
 ROWS_PER_PAGE = 3
 NEXT_PAGE = '>'
 PREVIOUS_PAGE = '<'
 ```
 
 ### Step 3. Creating the pageable keyboard instance
 
 The standard pageable keyboard instance looks like this:
 
 ```py
-Keyboard(chat_id=message.chat.id, data=data, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)
+Keyboard(chat_id=message.chat.id, data=data, row_width=ROW_WIDTH, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)
 ```
 
 In this example, the instance is written to the variable **keyboards** to ensure multithreading:
 
 ```py
 keyboards = []
 
 ...
 
-    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, rows_per_page=rows_per_page, button_text_mode=button_text_mode, text_index=text_index, callback_index=callback_index)}
+    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, row_width=ROW_WIDTH, rows_per_page=rows_per_page, button_text_mode=button_text_mode, text_index=text_index, callback_index=callback_index)}
     keyboards.append(json)
 ```   
 
 ### Step 4. Creating the message handler for pageable keyboard
 
 The standard message handler for pageable keyboard looks like this:
 
 ```py
-bot.send_message(message.from_user.id, text_message, reply_markup=Keyboard.send_keyboard()
+bot.send_message(message.from_user.id, text_message, reply_markup=Keyboard.send_keyboard())
 ```
 
 In this example, the keyboard calls using the **/start** command. Also, 
 first, when using the **/start** command, all previously created instances are deleted. Second, a new instance is added to the message handler.
 
 ```py
 @bot.message_handler(commands=['start'])
 def demo_pagination(message):
     for i, j in enumerate(keyboards):
         if j["id"] == message.chat.id:
             del keyboards[i]    
-    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)}
+    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, row_width=ROW_WIDTH, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)}
     keyboards.append(json)
     for i in keyboards:
         if i["id"] == message.chat.id:
             bot.send_message(message.from_user.id, text_message, reply_markup=i["object"].send_keyboard())
 ```
 
 ### Step 5. Creating the callback query handler for pageable keyboard
@@ -158,15 +161,15 @@
 
 ```py
 from telebot import TeleBot
 
 bot = TeleBot('TOKEN', parse_mode=None) # Use your Telegram token
 
 from telebot.types import CallbackQuery
-from telebot_inline_pagination.keyboard import Keyboard
+from telebot_inline_pagination import Keyboard
 
 data = [
             ('Hartsfield-Jackson Atlanta International Airport', 'ATL/KATL', 'Atlanta, Georgia, United States'),
             ("O'Hare International Airport", 'ORD/KORD', 'Chicago, Illinois, United States'),
             ('Dallas/Fort Worth International Airport', 'DFW/KDFW', 'Coppell, Euless, Grapevine, and Irving, Texas, United States'),
             ('Denver International Airport', 'DEN/KDEN', 'Denver, Colorado, United States'),
             ('Charlotte Douglas International Airport', 'CLT/KCLT', 'Charlotte, North Carolina, United States'),
@@ -178,26 +181,27 @@
         ]
 
 text_message = 'Demo'
 
 BUTTON_TEXT_MODE = 2
 TEXT_INDEX = 0
 CALLBACK_INDEX = 1
+ROW_WIDTH = 1
 ROWS_PER_PAGE = 3
 NEXT_PAGE = '>'
 PREVIOUS_PAGE = '<'
 
 keyboards = []
 
 @bot.message_handler(commands=['start'])
 def demo_pagination(message):
     for i, j in enumerate(keyboards):
         if j["id"] == message.chat.id:
             del keyboards[i]
-    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)}
+    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, row_width=ROW_WIDTH, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)}
     keyboards.append(json)
     for i in keyboards:
         if i["id"] == message.chat.id:
             bot.send_message(message.from_user.id, text_message, reply_markup=i["object"].send_keyboard())
 
 @bot.callback_query_handler(func=lambda call: True)
 def demo_pagination_handler(call: CallbackQuery):
```

### Comparing `telebot_inline_pagination-1.1.0/README.md` & `telebot_inline_pagination-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             ('George Bush Intercontinental Airport', 'IAH/KIAH', 'Houston, Texas, United States')
         ]
 
 text_message = 'Demo'        
 ```
 
 ### Optional parameters
+**row_width**: The number of buttons per row (from 1 to 3, by default - 1).
 
 **rows_per_page**: The number of rows of buttons on one page, excluding the navigation bar (by default - 5).
 
 **text_index**: Column index - data source for button titles (by default - 0).
 
 **callback_index**: Column index - data source for callback-function (by default - 0).
 
@@ -63,56 +64,57 @@
 
 **previous_index**: Content of the button to go to the previous page (by default - '<---').
 
 ```py
 TEXT_INDEX = 0 # in this example, full airport name
 CALLBACK_INDEX = 1 # in this example, IATA/ICAO airport code
 BUTTON_TEXT_MODE = 2 # in this example, "full airport name (IATA/ICAO airport code)"
+ROW_WIDTH = 1
 ROWS_PER_PAGE = 3
 NEXT_PAGE = '>'
 PREVIOUS_PAGE = '<'
 ```
 
 ### Step 3. Creating the pageable keyboard instance
 
 The standard pageable keyboard instance looks like this:
 
 ```py
-Keyboard(chat_id=message.chat.id, data=data, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)
+Keyboard(chat_id=message.chat.id, data=data, row_width=ROW_WIDTH, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)
 ```
 
 In this example, the instance is written to the variable **keyboards** to ensure multithreading:
 
 ```py
 keyboards = []
 
 ...
 
-    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, rows_per_page=rows_per_page, button_text_mode=button_text_mode, text_index=text_index, callback_index=callback_index)}
+    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, row_width=ROW_WIDTH, rows_per_page=rows_per_page, button_text_mode=button_text_mode, text_index=text_index, callback_index=callback_index)}
     keyboards.append(json)
 ```   
 
 ### Step 4. Creating the message handler for pageable keyboard
 
 The standard message handler for pageable keyboard looks like this:
 
 ```py
-bot.send_message(message.from_user.id, text_message, reply_markup=Keyboard.send_keyboard()
+bot.send_message(message.from_user.id, text_message, reply_markup=Keyboard.send_keyboard())
 ```
 
 In this example, the keyboard calls using the **/start** command. Also, 
 first, when using the **/start** command, all previously created instances are deleted. Second, a new instance is added to the message handler.
 
 ```py
 @bot.message_handler(commands=['start'])
 def demo_pagination(message):
     for i, j in enumerate(keyboards):
         if j["id"] == message.chat.id:
             del keyboards[i]    
-    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)}
+    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, row_width=ROW_WIDTH, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)}
     keyboards.append(json)
     for i in keyboards:
         if i["id"] == message.chat.id:
             bot.send_message(message.from_user.id, text_message, reply_markup=i["object"].send_keyboard())
 ```
 
 ### Step 5. Creating the callback query handler for pageable keyboard
@@ -147,15 +149,15 @@
 
 ```py
 from telebot import TeleBot
 
 bot = TeleBot('TOKEN', parse_mode=None) # Use your Telegram token
 
 from telebot.types import CallbackQuery
-from telebot_inline_pagination.keyboard import Keyboard
+from telebot_inline_pagination import Keyboard
 
 data = [
             ('Hartsfield-Jackson Atlanta International Airport', 'ATL/KATL', 'Atlanta, Georgia, United States'),
             ("O'Hare International Airport", 'ORD/KORD', 'Chicago, Illinois, United States'),
             ('Dallas/Fort Worth International Airport', 'DFW/KDFW', 'Coppell, Euless, Grapevine, and Irving, Texas, United States'),
             ('Denver International Airport', 'DEN/KDEN', 'Denver, Colorado, United States'),
             ('Charlotte Douglas International Airport', 'CLT/KCLT', 'Charlotte, North Carolina, United States'),
@@ -167,26 +169,27 @@
         ]
 
 text_message = 'Demo'
 
 BUTTON_TEXT_MODE = 2
 TEXT_INDEX = 0
 CALLBACK_INDEX = 1
+ROW_WIDTH = 1
 ROWS_PER_PAGE = 3
 NEXT_PAGE = '>'
 PREVIOUS_PAGE = '<'
 
 keyboards = []
 
 @bot.message_handler(commands=['start'])
 def demo_pagination(message):
     for i, j in enumerate(keyboards):
         if j["id"] == message.chat.id:
             del keyboards[i]
-    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)}
+    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, row_width=ROW_WIDTH, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)}
     keyboards.append(json)
     for i in keyboards:
         if i["id"] == message.chat.id:
             bot.send_message(message.from_user.id, text_message, reply_markup=i["object"].send_keyboard())
 
 @bot.callback_query_handler(func=lambda call: True)
 def demo_pagination_handler(call: CallbackQuery):
@@ -205,8 +208,8 @@
 bot.infinity_polling()
 ```
 
 ## Result
 
 ![button_text_mode.jpg](https://github.com/kremastra/telebot-inline-pagination/raw/main/img/button_text_mode.jpg)
 
-## [MIT License](https://github.com/kremastra/telebot-inline-pagination/blob/main/LICENSE)
+## [MIT License](https://github.com/kremastra/telebot-inline-pagination/blob/main/LICENSE)
```

### Comparing `telebot_inline_pagination-1.1.0/setup.py` & `telebot_inline_pagination-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='telebot_inline_pagination',
-  version='1.1.0',
+  version='1.2.0',
   author='kremastra',
   author_email='fotisgrek@gmail.com',
   description='Pageable inline keyboard for pyTelegramBotAPI (telebot)',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/kremastra/telebot-inline-pagination',
   packages=find_packages(),
```

### Comparing `telebot_inline_pagination-1.1.0/telebot_inline_pagination.egg-info/PKG-INFO` & `telebot_inline_pagination-1.2.0/telebot_inline_pagination.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
-Name: telebot-inline-pagination
-Version: 1.1.0
+Name: telebot_inline_pagination
+Version: 1.2.0
 Summary: Pageable inline keyboard for pyTelegramBotAPI (telebot)
 Home-page: https://github.com/kremastra/telebot-inline-pagination
 Author: kremastra
 Author-email: fotisgrek@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: telebot
 
 # Pageable inline keyboard for [pyTelegramBotAPI](https://github.com/eternnoir/pyTelegramBotAPI/) (telebot)
 
 A library for pyTelegramBotAPI that allows you to display data in the format of a pageable inline keyboard.
 
 ## Installation
 You can use [pip](https://pip.pypa.io/en/stable/) to install this library.
@@ -53,14 +54,15 @@
             ('George Bush Intercontinental Airport', 'IAH/KIAH', 'Houston, Texas, United States')
         ]
 
 text_message = 'Demo'        
 ```
 
 ### Optional parameters
+**row_width**: The number of buttons per row (from 1 to 3, by default - 1).
 
 **rows_per_page**: The number of rows of buttons on one page, excluding the navigation bar (by default - 5).
 
 **text_index**: Column index - data source for button titles (by default - 0).
 
 **callback_index**: Column index - data source for callback-function (by default - 0).
 
@@ -74,56 +76,57 @@
 
 **previous_index**: Content of the button to go to the previous page (by default - '<---').
 
 ```py
 TEXT_INDEX = 0 # in this example, full airport name
 CALLBACK_INDEX = 1 # in this example, IATA/ICAO airport code
 BUTTON_TEXT_MODE = 2 # in this example, "full airport name (IATA/ICAO airport code)"
+ROW_WIDTH = 1
 ROWS_PER_PAGE = 3
 NEXT_PAGE = '>'
 PREVIOUS_PAGE = '<'
 ```
 
 ### Step 3. Creating the pageable keyboard instance
 
 The standard pageable keyboard instance looks like this:
 
 ```py
-Keyboard(chat_id=message.chat.id, data=data, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)
+Keyboard(chat_id=message.chat.id, data=data, row_width=ROW_WIDTH, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)
 ```
 
 In this example, the instance is written to the variable **keyboards** to ensure multithreading:
 
 ```py
 keyboards = []
 
 ...
 
-    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, rows_per_page=rows_per_page, button_text_mode=button_text_mode, text_index=text_index, callback_index=callback_index)}
+    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, row_width=ROW_WIDTH, rows_per_page=rows_per_page, button_text_mode=button_text_mode, text_index=text_index, callback_index=callback_index)}
     keyboards.append(json)
 ```   
 
 ### Step 4. Creating the message handler for pageable keyboard
 
 The standard message handler for pageable keyboard looks like this:
 
 ```py
-bot.send_message(message.from_user.id, text_message, reply_markup=Keyboard.send_keyboard()
+bot.send_message(message.from_user.id, text_message, reply_markup=Keyboard.send_keyboard())
 ```
 
 In this example, the keyboard calls using the **/start** command. Also, 
 first, when using the **/start** command, all previously created instances are deleted. Second, a new instance is added to the message handler.
 
 ```py
 @bot.message_handler(commands=['start'])
 def demo_pagination(message):
     for i, j in enumerate(keyboards):
         if j["id"] == message.chat.id:
             del keyboards[i]    
-    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)}
+    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, row_width=ROW_WIDTH, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)}
     keyboards.append(json)
     for i in keyboards:
         if i["id"] == message.chat.id:
             bot.send_message(message.from_user.id, text_message, reply_markup=i["object"].send_keyboard())
 ```
 
 ### Step 5. Creating the callback query handler for pageable keyboard
@@ -158,15 +161,15 @@
 
 ```py
 from telebot import TeleBot
 
 bot = TeleBot('TOKEN', parse_mode=None) # Use your Telegram token
 
 from telebot.types import CallbackQuery
-from telebot_inline_pagination.keyboard import Keyboard
+from telebot_inline_pagination import Keyboard
 
 data = [
             ('Hartsfield-Jackson Atlanta International Airport', 'ATL/KATL', 'Atlanta, Georgia, United States'),
             ("O'Hare International Airport", 'ORD/KORD', 'Chicago, Illinois, United States'),
             ('Dallas/Fort Worth International Airport', 'DFW/KDFW', 'Coppell, Euless, Grapevine, and Irving, Texas, United States'),
             ('Denver International Airport', 'DEN/KDEN', 'Denver, Colorado, United States'),
             ('Charlotte Douglas International Airport', 'CLT/KCLT', 'Charlotte, North Carolina, United States'),
@@ -178,26 +181,27 @@
         ]
 
 text_message = 'Demo'
 
 BUTTON_TEXT_MODE = 2
 TEXT_INDEX = 0
 CALLBACK_INDEX = 1
+ROW_WIDTH = 1
 ROWS_PER_PAGE = 3
 NEXT_PAGE = '>'
 PREVIOUS_PAGE = '<'
 
 keyboards = []
 
 @bot.message_handler(commands=['start'])
 def demo_pagination(message):
     for i, j in enumerate(keyboards):
         if j["id"] == message.chat.id:
             del keyboards[i]
-    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)}
+    json = {"id": message.chat.id, "object": Keyboard(chat_id=message.chat.id, data=data, row_width=ROW_WIDTH, rows_per_page=ROWS_PER_PAGE, button_text_mode=BUTTON_TEXT_MODE, text_index=TEXT_INDEX, callback_index=CALLBACK_INDEX, next_page=NEXT_PAGE, previous_page=PREVIOUS_PAGE)}
     keyboards.append(json)
     for i in keyboards:
         if i["id"] == message.chat.id:
             bot.send_message(message.from_user.id, text_message, reply_markup=i["object"].send_keyboard())
 
 @bot.callback_query_handler(func=lambda call: True)
 def demo_pagination_handler(call: CallbackQuery):
```

