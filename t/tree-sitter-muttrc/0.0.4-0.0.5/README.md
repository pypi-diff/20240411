# Comparing `tmp/tree-sitter-muttrc-0.0.4.tar.gz` & `tmp/tree-sitter-muttrc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-sitter-muttrc-0.0.4.tar", last modified: Wed Mar 27 02:58:35 2024, max compression
+gzip compressed data, was "tree-sitter-muttrc-0.0.5.tar", last modified: Thu Apr 11 10:37:01 2024, max compression
```

## Comparing `tree-sitter-muttrc-0.0.4.tar` & `tree-sitter-muttrc-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:58:34.995309 tree-sitter-muttrc-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-03-27 02:58:34.995309 tree-sitter-muttrc-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-03-27 02:58:30.000000 tree-sitter-muttrc-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:58:34.991309 tree-sitter-muttrc-0.0.4/bindings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:58:34.991309 tree-sitter-muttrc-0.0.4/bindings/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:58:34.991309 tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-27 02:58:30.000000 tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-27 02:58:30.000000 tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-27 02:58:30.000000 tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc/binding.c
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 02:58:30.000000 tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:58:34.995309 tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-03-27 02:58:34.000000 tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-27 02:58:34.000000 tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 02:58:34.000000 tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 02:58:34.000000 tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-27 02:58:34.000000 tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-27 02:58:34.000000 tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-27 02:58:30.000000 tree-sitter-muttrc-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 02:58:34.995309 tree-sitter-muttrc-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-27 02:58:30.000000 tree-sitter-muttrc-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:58:34.995309 tree-sitter-muttrc-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)   634176 2024-03-27 02:58:30.000000 tree-sitter-muttrc-0.0.4/src/parser.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:37:01.986286 tree-sitter-muttrc-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-04-11 10:37:01.986286 tree-sitter-muttrc-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-11 10:36:56.000000 tree-sitter-muttrc-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:37:01.982286 tree-sitter-muttrc-0.0.5/bindings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:37:01.982286 tree-sitter-muttrc-0.0.5/bindings/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:37:01.982286 tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-11 10:36:56.000000 tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 10:36:56.000000 tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-11 10:36:56.000000 tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc/binding.c
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:36:56.000000 tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:37:01.986286 tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-04-11 10:37:01.000000 tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-11 10:37:01.000000 tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:37:01.000000 tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:37:01.000000 tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 10:37:01.000000 tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 10:37:01.000000 tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-11 10:36:56.000000 tree-sitter-muttrc-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 10:37:01.986286 tree-sitter-muttrc-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-11 10:36:56.000000 tree-sitter-muttrc-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:37:01.986286 tree-sitter-muttrc-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)   629317 2024-04-11 10:36:56.000000 tree-sitter-muttrc-0.0.5/src/parser.c
```

### Comparing `tree-sitter-muttrc-0.0.4/PKG-INFO` & `tree-sitter-muttrc-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-muttrc
-Version: 0.0.4
+Version: 0.0.5
 Summary: Muttrc grammar for tree-sitter
 License: MIT
 Project-URL: Homepage, https://github.com/tree-sitter/tree-sitter-muttrc
 Keywords: incremental,parsing,tree-sitter,muttrc
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
```

### Comparing `tree-sitter-muttrc-0.0.4/README.md` & `tree-sitter-muttrc-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc/binding.c` & `tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc/binding.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc.egg-info/PKG-INFO` & `tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-muttrc
-Version: 0.0.4
+Version: 0.0.5
 Summary: Muttrc grammar for tree-sitter
 License: MIT
 Project-URL: Homepage, https://github.com/tree-sitter/tree-sitter-muttrc
 Keywords: incremental,parsing,tree-sitter,muttrc
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
```

### Comparing `tree-sitter-muttrc-0.0.4/bindings/python/tree_sitter_muttrc.egg-info/SOURCES.txt` & `tree-sitter-muttrc-0.0.5/bindings/python/tree_sitter_muttrc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tree-sitter-muttrc-0.0.4/pyproject.toml` & `tree-sitter-muttrc-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tree-sitter-muttrc"
 description = "Muttrc grammar for tree-sitter"
-version = "0.0.4"
+version = "0.0.5"
 keywords = ["incremental", "parsing", "tree-sitter", "muttrc"]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Topic :: Software Development :: Compilers",
   "Topic :: Text Processing :: Linguistic",
   "Typing :: Typed"
@@ -26,8 +26,7 @@
 
 [tool.cibuildwheel]
 build = "cp38-*"
 build-frontend = "build"
 
 [tool.codespell]
 ignore-words-list = "crate"
-
```

### Comparing `tree-sitter-muttrc-0.0.4/setup.py` & `tree-sitter-muttrc-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `tree-sitter-muttrc-0.0.4/src/parser.c` & `tree-sitter-muttrc-0.0.5/src/parser.c`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 #elif defined(__GNUC__)
 #pragma GCC optimize ("O0")
 #endif
 
 #define LANGUAGE_VERSION 14
 #define STATE_COUNT 566
 #define LARGE_STATE_COUNT 26
-#define SYMBOL_COUNT 345
+#define SYMBOL_COUNT 344
 #define ALIAS_COUNT 3
-#define TOKEN_COUNT 192
+#define TOKEN_COUNT 191
 #define EXTERNAL_TOKEN_COUNT 0
 #define FIELD_COUNT 1
 #define MAX_ALIAS_SEQUENCE_LENGTH 6
 #define PRODUCTION_ID_COUNT 20
 
 enum ts_symbol_identifiers {
   anon_sym_account_DASHhook = 1,
@@ -205,176 +205,175 @@
   sym_int = 179,
   anon_sym_SQUOTE = 180,
   aux_sym__string_token1 = 181,
   anon_sym_DQUOTE = 182,
   aux_sym__string_token2 = 183,
   anon_sym_BQUOTE = 184,
   aux_sym__string_token3 = 185,
-  anon_sym_LF = 186,
-  sym__word = 187,
-  anon_sym_source = 188,
-  sym_comment = 189,
-  sym__eol = 190,
-  aux_sym__space_token1 = 191,
-  sym_file = 192,
-  sym__command = 193,
-  sym_account_hook_directive = 194,
-  sym_group_name = 195,
-  sym__group = 196,
-  sym__addresses = 197,
-  sym_alias_directive = 198,
-  sym_address = 199,
-  sym_unalias_directive = 200,
-  sym_key = 201,
-  sym__regexes = 202,
-  sym_alternates_directive = 203,
-  sym_unalternates_directive = 204,
-  sym_alternative_order_directive = 205,
-  sym_unalternative_order_directive = 206,
-  sym_mime = 207,
-  sym__mime_types = 208,
-  sym__mimes = 209,
-  sym_disposition = 210,
-  sym_attachments_directive = 211,
-  sym_unattachments_directive = 212,
-  sym_auto_view_directive = 213,
-  sym_unauto_view_directive = 214,
-  sym_map = 215,
-  sym__maps = 216,
-  sym__functions = 217,
-  sym_bind_directive = 218,
-  sym_unbind_directive = 219,
-  sym_alias = 220,
-  sym_charset = 221,
-  sym_charset_hook_directive = 222,
-  sym_iconv_hook_directive = 223,
-  sym_pattern = 224,
-  sym_object = 225,
-  sym_composeobject = 226,
-  sym_color = 227,
-  sym_attribute = 228,
-  sym__attributes = 229,
-  sym_foreground = 230,
-  sym_background = 231,
-  sym_color_directive = 232,
-  sym_uncolor_directive = 233,
-  sym_keyid = 234,
-  sym_crypt_hook_directive = 235,
-  sym_name = 236,
-  sym_index_format_hook_directive = 237,
-  sym_exec_directive = 238,
-  sym_fcc_save_hook_directive = 239,
-  sym_fcc_hook_directive = 240,
-  sym_save_hook_directive = 241,
-  sym_folder_hook_directive = 242,
-  sym__rx_addr = 243,
-  sym_group_directive = 244,
-  sym_ungroup_directive = 245,
-  sym_header = 246,
-  sym__headers = 247,
-  sym_hdr_order_directive = 248,
-  sym_unhdr_order_directive = 249,
-  sym_symbol = 250,
-  sym_ifdef_directive = 251,
-  sym_ifndef_directive = 252,
-  sym_finish_directive = 253,
-  sym__strings = 254,
-  sym_ignore_directive = 255,
-  sym_unignore_directive = 256,
-  sym_lists_directive = 257,
-  sym_unlists_directive = 258,
-  sym_subscribe_directive = 259,
-  sym_unsubscribe_directive = 260,
-  sym_sequence = 261,
-  sym_macro_directive = 262,
-  sym_unmacro_directive = 263,
-  sym_mailbox = 264,
-  sym__mailboxes = 265,
-  sym_description = 266,
-  sym_mailboxes_directive = 267,
-  sym_named_mailboxes_directive = 268,
-  sym_unmailboxes_directive = 269,
-  sym_header_field = 270,
-  sym__header_fields = 271,
-  sym_mailto_allow_directive = 272,
-  sym_unmailto_allow_directive = 273,
-  sym_message = 274,
-  sym_echo_directive = 275,
-  sym_directory = 276,
-  sym_cd_directive = 277,
-  sym_mbox_hook_directive = 278,
-  sym_message_hook_directive = 279,
-  sym_mime_lookup_directive = 280,
-  sym_unmime_lookup_directive = 281,
-  sym_mono_directive = 282,
-  sym_unmono_directive = 283,
-  sym_my_hdr_directive = 284,
-  sym_unmy_hdr_directive = 285,
-  sym_shell_command = 286,
-  sym_open_hook_directive = 287,
-  sym_close_hook_directive = 288,
-  sym_append_hook_directive = 289,
-  sym_push_directive = 290,
-  sym_reply_hook_directive = 291,
-  sym_send_hook_directive = 292,
-  sym_send2_hook_directive = 293,
-  sym_format = 294,
-  sym_spam_directive = 295,
-  sym_nospam_directive = 296,
-  sym_replacement = 297,
-  sym_subjectrx_directive = 298,
-  sym_unsubjectrx_directive = 299,
-  sym_uri = 300,
-  sym_subscribe_to_directive = 301,
-  sym_unsubscribe_from_directive = 302,
-  sym_timeout_hook_directive = 303,
-  sym_startup_hook_directive = 304,
-  sym_shutdown_hook_directive = 305,
-  sym_hook_type = 306,
-  sym_unhook_directive = 307,
-  sym_set_directive = 308,
-  sym__options3 = 309,
-  sym__options2 = 310,
-  sym__options = 311,
-  sym_unset_directive = 312,
-  sym_reset_directive = 313,
-  sym_toggle_directive = 314,
-  sym_setenv_directive = 315,
-  sym_unsetenv_directive = 316,
-  sym_sidebar_pin_directive = 317,
-  sym_sidebar_unpin_directive = 318,
-  sym_score_directive = 319,
-  sym_unscore_directive = 320,
-  sym_quadoption = 321,
-  sym__string = 322,
-  sym__regex = 323,
-  sym_source_directive = 324,
-  sym__space = 325,
-  sym__end = 326,
-  aux_sym_file_repeat1 = 327,
-  aux_sym__addresses_repeat1 = 328,
-  aux_sym_key_repeat1 = 329,
-  aux_sym__regexes_repeat1 = 330,
-  aux_sym__mime_types_repeat1 = 331,
-  aux_sym__mimes_repeat1 = 332,
-  aux_sym__maps_repeat1 = 333,
-  aux_sym__functions_repeat1 = 334,
-  aux_sym__attributes_repeat1 = 335,
-  aux_sym__headers_repeat1 = 336,
-  aux_sym__strings_repeat1 = 337,
-  aux_sym__mailboxes_repeat1 = 338,
-  aux_sym_named_mailboxes_directive_repeat1 = 339,
-  aux_sym__header_fields_repeat1 = 340,
-  aux_sym__options3_repeat1 = 341,
-  aux_sym__options2_repeat1 = 342,
-  aux_sym__options_repeat1 = 343,
-  aux_sym__space_repeat1 = 344,
-  alias_sym_path = 345,
-  alias_sym_regex = 346,
-  alias_sym_sub_mime_type = 347,
+  sym__word = 186,
+  anon_sym_source = 187,
+  sym_comment = 188,
+  sym__eol = 189,
+  aux_sym__space_token1 = 190,
+  sym_file = 191,
+  sym__command = 192,
+  sym_account_hook_directive = 193,
+  sym_group_name = 194,
+  sym__group = 195,
+  sym__addresses = 196,
+  sym_alias_directive = 197,
+  sym_address = 198,
+  sym_unalias_directive = 199,
+  sym_key = 200,
+  sym__regexes = 201,
+  sym_alternates_directive = 202,
+  sym_unalternates_directive = 203,
+  sym_alternative_order_directive = 204,
+  sym_unalternative_order_directive = 205,
+  sym_mime = 206,
+  sym__mime_types = 207,
+  sym__mimes = 208,
+  sym_disposition = 209,
+  sym_attachments_directive = 210,
+  sym_unattachments_directive = 211,
+  sym_auto_view_directive = 212,
+  sym_unauto_view_directive = 213,
+  sym_map = 214,
+  sym__maps = 215,
+  sym__functions = 216,
+  sym_bind_directive = 217,
+  sym_unbind_directive = 218,
+  sym_alias = 219,
+  sym_charset = 220,
+  sym_charset_hook_directive = 221,
+  sym_iconv_hook_directive = 222,
+  sym_pattern = 223,
+  sym_object = 224,
+  sym_composeobject = 225,
+  sym_color = 226,
+  sym_attribute = 227,
+  sym__attributes = 228,
+  sym_foreground = 229,
+  sym_background = 230,
+  sym_color_directive = 231,
+  sym_uncolor_directive = 232,
+  sym_keyid = 233,
+  sym_crypt_hook_directive = 234,
+  sym_name = 235,
+  sym_index_format_hook_directive = 236,
+  sym_exec_directive = 237,
+  sym_fcc_save_hook_directive = 238,
+  sym_fcc_hook_directive = 239,
+  sym_save_hook_directive = 240,
+  sym_folder_hook_directive = 241,
+  sym__rx_addr = 242,
+  sym_group_directive = 243,
+  sym_ungroup_directive = 244,
+  sym_header = 245,
+  sym__headers = 246,
+  sym_hdr_order_directive = 247,
+  sym_unhdr_order_directive = 248,
+  sym_symbol = 249,
+  sym_ifdef_directive = 250,
+  sym_ifndef_directive = 251,
+  sym_finish_directive = 252,
+  sym__strings = 253,
+  sym_ignore_directive = 254,
+  sym_unignore_directive = 255,
+  sym_lists_directive = 256,
+  sym_unlists_directive = 257,
+  sym_subscribe_directive = 258,
+  sym_unsubscribe_directive = 259,
+  sym_sequence = 260,
+  sym_macro_directive = 261,
+  sym_unmacro_directive = 262,
+  sym_mailbox = 263,
+  sym__mailboxes = 264,
+  sym_description = 265,
+  sym_mailboxes_directive = 266,
+  sym_named_mailboxes_directive = 267,
+  sym_unmailboxes_directive = 268,
+  sym_header_field = 269,
+  sym__header_fields = 270,
+  sym_mailto_allow_directive = 271,
+  sym_unmailto_allow_directive = 272,
+  sym_message = 273,
+  sym_echo_directive = 274,
+  sym_directory = 275,
+  sym_cd_directive = 276,
+  sym_mbox_hook_directive = 277,
+  sym_message_hook_directive = 278,
+  sym_mime_lookup_directive = 279,
+  sym_unmime_lookup_directive = 280,
+  sym_mono_directive = 281,
+  sym_unmono_directive = 282,
+  sym_my_hdr_directive = 283,
+  sym_unmy_hdr_directive = 284,
+  sym_shell_command = 285,
+  sym_open_hook_directive = 286,
+  sym_close_hook_directive = 287,
+  sym_append_hook_directive = 288,
+  sym_push_directive = 289,
+  sym_reply_hook_directive = 290,
+  sym_send_hook_directive = 291,
+  sym_send2_hook_directive = 292,
+  sym_format = 293,
+  sym_spam_directive = 294,
+  sym_nospam_directive = 295,
+  sym_replacement = 296,
+  sym_subjectrx_directive = 297,
+  sym_unsubjectrx_directive = 298,
+  sym_uri = 299,
+  sym_subscribe_to_directive = 300,
+  sym_unsubscribe_from_directive = 301,
+  sym_timeout_hook_directive = 302,
+  sym_startup_hook_directive = 303,
+  sym_shutdown_hook_directive = 304,
+  sym_hook_type = 305,
+  sym_unhook_directive = 306,
+  sym_set_directive = 307,
+  sym__options3 = 308,
+  sym__options2 = 309,
+  sym__options = 310,
+  sym_unset_directive = 311,
+  sym_reset_directive = 312,
+  sym_toggle_directive = 313,
+  sym_setenv_directive = 314,
+  sym_unsetenv_directive = 315,
+  sym_sidebar_pin_directive = 316,
+  sym_sidebar_unpin_directive = 317,
+  sym_score_directive = 318,
+  sym_unscore_directive = 319,
+  sym_quadoption = 320,
+  sym__string = 321,
+  sym__regex = 322,
+  sym_source_directive = 323,
+  sym__space = 324,
+  sym__end = 325,
+  aux_sym_file_repeat1 = 326,
+  aux_sym__addresses_repeat1 = 327,
+  aux_sym_key_repeat1 = 328,
+  aux_sym__regexes_repeat1 = 329,
+  aux_sym__mime_types_repeat1 = 330,
+  aux_sym__mimes_repeat1 = 331,
+  aux_sym__maps_repeat1 = 332,
+  aux_sym__functions_repeat1 = 333,
+  aux_sym__attributes_repeat1 = 334,
+  aux_sym__headers_repeat1 = 335,
+  aux_sym__strings_repeat1 = 336,
+  aux_sym__mailboxes_repeat1 = 337,
+  aux_sym_named_mailboxes_directive_repeat1 = 338,
+  aux_sym__header_fields_repeat1 = 339,
+  aux_sym__options3_repeat1 = 340,
+  aux_sym__options2_repeat1 = 341,
+  aux_sym__options_repeat1 = 342,
+  aux_sym__space_repeat1 = 343,
+  alias_sym_path = 344,
+  alias_sym_regex = 345,
+  alias_sym_sub_mime_type = 346,
 };
 
 static const char * const ts_symbol_names[] = {
   [ts_builtin_sym_end] = "end",
   [anon_sym_account_DASHhook] = "account-hook",
   [anon_sym_DASHgroup] = "command_line_option",
   [anon_sym_COMMA] = ",",
@@ -556,15 +555,14 @@
   [sym_int] = "int",
   [anon_sym_SQUOTE] = "'",
   [aux_sym__string_token1] = "string",
   [anon_sym_DQUOTE] = "\"",
   [aux_sym__string_token2] = "shell",
   [anon_sym_BQUOTE] = "`",
   [aux_sym__string_token3] = "shell",
-  [anon_sym_LF] = "\n",
   [sym__word] = "shell",
   [anon_sym_source] = "command",
   [sym_comment] = "comment",
   [sym__eol] = "_eol",
   [aux_sym__space_token1] = "_space_token1",
   [sym_file] = "file",
   [sym__command] = "_command",
@@ -907,15 +905,14 @@
   [sym_int] = sym_int,
   [anon_sym_SQUOTE] = anon_sym_SQUOTE,
   [aux_sym__string_token1] = aux_sym__string_token1,
   [anon_sym_DQUOTE] = anon_sym_DQUOTE,
   [aux_sym__string_token2] = aux_sym__string_token2,
   [anon_sym_BQUOTE] = anon_sym_BQUOTE,
   [aux_sym__string_token3] = aux_sym__string_token2,
-  [anon_sym_LF] = anon_sym_LF,
   [sym__word] = aux_sym__string_token2,
   [anon_sym_source] = anon_sym_unalias,
   [sym_comment] = sym_comment,
   [sym__eol] = sym__eol,
   [aux_sym__space_token1] = aux_sym__space_token1,
   [sym_file] = sym_file,
   [sym__command] = sym__command,
@@ -1816,18 +1813,14 @@
     .visible = true,
     .named = false,
   },
   [aux_sym__string_token3] = {
     .visible = true,
     .named = true,
   },
-  [anon_sym_LF] = {
-    .visible = true,
-    .named = false,
-  },
   [sym__word] = {
     .visible = true,
     .named = true,
   },
   [anon_sym_source] = {
     .visible = true,
     .named = true,
@@ -2638,55 +2631,55 @@
   [71] = 71,
   [72] = 72,
   [73] = 73,
   [74] = 74,
   [75] = 75,
   [76] = 76,
   [77] = 77,
-  [78] = 78,
+  [78] = 57,
   [79] = 79,
   [80] = 80,
   [81] = 81,
   [82] = 82,
   [83] = 83,
   [84] = 84,
   [85] = 85,
   [86] = 86,
   [87] = 87,
   [88] = 88,
   [89] = 89,
-  [90] = 90,
+  [90] = 69,
   [91] = 91,
-  [92] = 92,
+  [92] = 62,
   [93] = 93,
   [94] = 94,
-  [95] = 93,
-  [96] = 93,
-  [97] = 68,
-  [98] = 63,
-  [99] = 93,
+  [95] = 95,
+  [96] = 96,
+  [97] = 97,
+  [98] = 98,
+  [99] = 99,
   [100] = 100,
-  [101] = 93,
-  [102] = 102,
-  [103] = 103,
+  [101] = 101,
+  [102] = 95,
+  [103] = 93,
   [104] = 104,
   [105] = 105,
   [106] = 106,
   [107] = 107,
   [108] = 108,
   [109] = 109,
   [110] = 110,
   [111] = 111,
   [112] = 112,
   [113] = 113,
   [114] = 114,
   [115] = 115,
   [116] = 116,
   [117] = 117,
-  [118] = 118,
+  [118] = 95,
   [119] = 119,
   [120] = 120,
   [121] = 121,
   [122] = 122,
   [123] = 123,
   [124] = 124,
   [125] = 125,
@@ -2704,76 +2697,76 @@
   [137] = 137,
   [138] = 138,
   [139] = 139,
   [140] = 140,
   [141] = 141,
   [142] = 142,
   [143] = 143,
-  [144] = 144,
-  [145] = 145,
+  [144] = 95,
+  [145] = 95,
   [146] = 146,
   [147] = 147,
   [148] = 148,
   [149] = 149,
   [150] = 150,
   [151] = 151,
   [152] = 152,
   [153] = 153,
-  [154] = 18,
+  [154] = 154,
   [155] = 155,
-  [156] = 16,
+  [156] = 156,
   [157] = 157,
   [158] = 158,
   [159] = 159,
   [160] = 160,
   [161] = 161,
   [162] = 162,
   [163] = 163,
-  [164] = 17,
+  [164] = 164,
   [165] = 165,
-  [166] = 17,
+  [166] = 166,
   [167] = 167,
   [168] = 168,
   [169] = 169,
   [170] = 170,
   [171] = 171,
   [172] = 172,
   [173] = 173,
-  [174] = 16,
+  [174] = 174,
   [175] = 175,
   [176] = 176,
   [177] = 177,
   [178] = 178,
   [179] = 179,
-  [180] = 75,
-  [181] = 181,
-  [182] = 182,
-  [183] = 183,
+  [180] = 180,
+  [181] = 17,
+  [182] = 16,
+  [183] = 17,
   [184] = 184,
   [185] = 185,
   [186] = 186,
-  [187] = 187,
-  [188] = 16,
-  [189] = 63,
+  [187] = 16,
+  [188] = 188,
+  [189] = 189,
   [190] = 190,
   [191] = 191,
   [192] = 192,
-  [193] = 152,
-  [194] = 165,
+  [193] = 69,
+  [194] = 194,
   [195] = 195,
   [196] = 196,
-  [197] = 68,
+  [197] = 197,
   [198] = 198,
-  [199] = 17,
-  [200] = 25,
-  [201] = 24,
-  [202] = 58,
-  [203] = 56,
-  [204] = 18,
-  [205] = 23,
+  [199] = 62,
+  [200] = 18,
+  [201] = 201,
+  [202] = 202,
+  [203] = 203,
+  [204] = 204,
+  [205] = 205,
   [206] = 206,
   [207] = 207,
   [208] = 208,
   [209] = 209,
   [210] = 210,
   [211] = 211,
   [212] = 212,
@@ -2823,57 +2816,57 @@
   [256] = 256,
   [257] = 257,
   [258] = 258,
   [259] = 259,
   [260] = 260,
   [261] = 261,
   [262] = 262,
-  [263] = 75,
+  [263] = 263,
   [264] = 264,
   [265] = 265,
   [266] = 266,
-  [267] = 16,
-  [268] = 17,
-  [269] = 16,
-  [270] = 17,
-  [271] = 16,
-  [272] = 17,
+  [267] = 267,
+  [268] = 268,
+  [269] = 269,
+  [270] = 270,
+  [271] = 22,
+  [272] = 18,
   [273] = 273,
   [274] = 274,
   [275] = 275,
-  [276] = 152,
-  [277] = 165,
-  [278] = 278,
-  [279] = 279,
-  [280] = 280,
+  [276] = 185,
+  [277] = 277,
+  [278] = 184,
+  [279] = 49,
+  [280] = 24,
   [281] = 281,
-  [282] = 282,
-  [283] = 283,
+  [282] = 25,
+  [283] = 16,
   [284] = 284,
   [285] = 285,
   [286] = 286,
   [287] = 287,
   [288] = 288,
-  [289] = 289,
-  [290] = 290,
+  [289] = 185,
+  [290] = 184,
   [291] = 291,
-  [292] = 292,
+  [292] = 17,
   [293] = 293,
-  [294] = 294,
+  [294] = 93,
   [295] = 295,
-  [296] = 296,
+  [296] = 22,
   [297] = 297,
-  [298] = 298,
-  [299] = 299,
-  [300] = 23,
-  [301] = 301,
+  [298] = 16,
+  [299] = 17,
+  [300] = 300,
+  [301] = 16,
   [302] = 302,
-  [303] = 303,
-  [304] = 304,
-  [305] = 305,
+  [303] = 17,
+  [304] = 16,
+  [305] = 17,
   [306] = 24,
   [307] = 25,
   [308] = 308,
   [309] = 309,
   [310] = 310,
   [311] = 311,
   [312] = 312,
@@ -2902,95 +2895,95 @@
   [335] = 335,
   [336] = 336,
   [337] = 337,
   [338] = 338,
   [339] = 339,
   [340] = 340,
   [341] = 341,
-  [342] = 342,
+  [342] = 17,
   [343] = 343,
-  [344] = 344,
+  [344] = 16,
   [345] = 345,
   [346] = 346,
-  [347] = 16,
-  [348] = 17,
+  [347] = 347,
+  [348] = 348,
   [349] = 349,
-  [350] = 152,
+  [350] = 350,
   [351] = 351,
   [352] = 352,
   [353] = 353,
   [354] = 354,
   [355] = 355,
   [356] = 356,
   [357] = 357,
-  [358] = 165,
+  [358] = 358,
   [359] = 359,
-  [360] = 152,
+  [360] = 360,
   [361] = 361,
-  [362] = 165,
+  [362] = 362,
   [363] = 363,
   [364] = 364,
-  [365] = 365,
-  [366] = 366,
-  [367] = 25,
+  [365] = 184,
+  [366] = 185,
+  [367] = 367,
   [368] = 368,
   [369] = 369,
   [370] = 370,
   [371] = 371,
   [372] = 372,
   [373] = 373,
-  [374] = 24,
+  [374] = 374,
   [375] = 375,
   [376] = 376,
   [377] = 377,
   [378] = 378,
-  [379] = 379,
-  [380] = 380,
+  [379] = 25,
+  [380] = 24,
   [381] = 381,
-  [382] = 18,
-  [383] = 23,
+  [382] = 382,
+  [383] = 383,
   [384] = 384,
   [385] = 385,
   [386] = 386,
   [387] = 387,
   [388] = 388,
   [389] = 389,
   [390] = 390,
-  [391] = 391,
+  [391] = 18,
   [392] = 392,
-  [393] = 393,
+  [393] = 22,
   [394] = 394,
   [395] = 395,
   [396] = 396,
   [397] = 397,
   [398] = 398,
-  [399] = 58,
+  [399] = 399,
   [400] = 400,
   [401] = 401,
   [402] = 402,
   [403] = 403,
-  [404] = 404,
+  [404] = 57,
   [405] = 405,
   [406] = 406,
   [407] = 407,
   [408] = 408,
   [409] = 409,
   [410] = 410,
   [411] = 411,
   [412] = 412,
-  [413] = 413,
-  [414] = 414,
+  [413] = 184,
+  [414] = 185,
   [415] = 415,
-  [416] = 234,
+  [416] = 416,
   [417] = 417,
   [418] = 418,
   [419] = 419,
   [420] = 420,
   [421] = 421,
-  [422] = 422,
+  [422] = 85,
   [423] = 423,
   [424] = 424,
   [425] = 425,
   [426] = 426,
   [427] = 427,
   [428] = 428,
   [429] = 429,
@@ -3004,18 +2997,18 @@
   [437] = 437,
   [438] = 438,
   [439] = 439,
   [440] = 440,
   [441] = 441,
   [442] = 442,
   [443] = 443,
-  [444] = 275,
-  [445] = 273,
+  [444] = 297,
+  [445] = 302,
   [446] = 446,
-  [447] = 261,
+  [447] = 284,
   [448] = 448,
   [449] = 449,
   [450] = 450,
   [451] = 451,
   [452] = 452,
   [453] = 453,
   [454] = 454,
@@ -3034,1942 +3027,1930 @@
   [467] = 467,
   [468] = 468,
   [469] = 469,
   [470] = 470,
   [471] = 471,
   [472] = 472,
   [473] = 473,
-  [474] = 474,
-  [475] = 475,
+  [474] = 464,
+  [475] = 465,
   [476] = 476,
   [477] = 477,
   [478] = 478,
-  [479] = 479,
+  [479] = 16,
   [480] = 480,
-  [481] = 481,
+  [481] = 17,
   [482] = 482,
   [483] = 483,
   [484] = 484,
-  [485] = 16,
+  [485] = 485,
   [486] = 486,
   [487] = 487,
   [488] = 488,
   [489] = 489,
   [490] = 490,
   [491] = 491,
-  [492] = 465,
-  [493] = 464,
-  [494] = 481,
-  [495] = 495,
-  [496] = 483,
-  [497] = 489,
-  [498] = 498,
+  [492] = 492,
+  [493] = 493,
+  [494] = 468,
+  [495] = 469,
+  [496] = 470,
+  [497] = 472,
+  [498] = 473,
   [499] = 464,
   [500] = 465,
-  [501] = 495,
-  [502] = 481,
-  [503] = 495,
-  [504] = 483,
-  [505] = 489,
-  [506] = 498,
-  [507] = 17,
+  [501] = 501,
+  [502] = 468,
+  [503] = 469,
+  [504] = 470,
+  [505] = 472,
+  [506] = 473,
+  [507] = 507,
   [508] = 465,
-  [509] = 498,
-  [510] = 481,
-  [511] = 495,
-  [512] = 483,
-  [513] = 498,
+  [509] = 509,
+  [510] = 468,
+  [511] = 469,
+  [512] = 470,
+  [513] = 473,
   [514] = 464,
   [515] = 515,
-  [516] = 481,
-  [517] = 495,
-  [518] = 483,
-  [519] = 481,
-  [520] = 495,
-  [521] = 483,
-  [522] = 481,
-  [523] = 495,
-  [524] = 483,
-  [525] = 481,
-  [526] = 495,
-  [527] = 483,
-  [528] = 481,
-  [529] = 495,
-  [530] = 483,
-  [531] = 467,
-  [532] = 468,
-  [533] = 469,
-  [534] = 470,
-  [535] = 474,
-  [536] = 471,
-  [537] = 478,
-  [538] = 467,
-  [539] = 468,
-  [540] = 469,
-  [541] = 470,
-  [542] = 474,
-  [543] = 471,
-  [544] = 478,
-  [545] = 467,
-  [546] = 468,
-  [547] = 469,
-  [548] = 474,
-  [549] = 471,
-  [550] = 478,
-  [551] = 467,
-  [552] = 468,
-  [553] = 469,
-  [554] = 467,
-  [555] = 468,
-  [556] = 469,
-  [557] = 467,
-  [558] = 468,
-  [559] = 469,
-  [560] = 467,
-  [561] = 468,
-  [562] = 469,
-  [563] = 467,
-  [564] = 468,
-  [565] = 469,
+  [516] = 468,
+  [517] = 469,
+  [518] = 470,
+  [519] = 468,
+  [520] = 469,
+  [521] = 470,
+  [522] = 468,
+  [523] = 469,
+  [524] = 470,
+  [525] = 468,
+  [526] = 469,
+  [527] = 470,
+  [528] = 468,
+  [529] = 469,
+  [530] = 470,
+  [531] = 487,
+  [532] = 489,
+  [533] = 490,
+  [534] = 491,
+  [535] = 493,
+  [536] = 501,
+  [537] = 509,
+  [538] = 487,
+  [539] = 489,
+  [540] = 490,
+  [541] = 491,
+  [542] = 493,
+  [543] = 501,
+  [544] = 509,
+  [545] = 487,
+  [546] = 489,
+  [547] = 490,
+  [548] = 493,
+  [549] = 501,
+  [550] = 509,
+  [551] = 487,
+  [552] = 489,
+  [553] = 490,
+  [554] = 487,
+  [555] = 489,
+  [556] = 490,
+  [557] = 487,
+  [558] = 489,
+  [559] = 490,
+  [560] = 487,
+  [561] = 489,
+  [562] = 490,
+  [563] = 487,
+  [564] = 489,
+  [565] = 490,
 };
 
 static bool ts_lex(TSLexer *lexer, TSStateId state) {
   START_LEXER();
   eof = lexer->eof(lexer);
   switch (state) {
     case 0:
-      if (eof) ADVANCE(966);
-      if (lookahead == '!') ADVANCE(1134);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '#') ADVANCE(960);
-      if (lookahead == '&') ADVANCE(1195);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '*') ADVANCE(973);
-      if (lookahead == '+') ADVANCE(1006);
-      if (lookahead == ',') ADVANCE(970);
-      if (lookahead == '-') ADVANCE(1008);
-      if (lookahead == '/') ADVANCE(1004);
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '=') ADVANCE(1194);
-      if (lookahead == '>') ADVANCE(978);
-      if (lookahead == '?') ADVANCE(1010);
-      if (lookahead == '\\') SKIP(962)
-      if (lookahead == '`') ADVANCE(1231);
-      if (lookahead == 'a') ADVANCE(199);
-      if (lookahead == 'b') ADVANCE(447);
-      if (lookahead == 'c') ADVANCE(230);
-      if (lookahead == 'd') ADVANCE(278);
-      if (lookahead == 'e') ADVANCE(203);
-      if (lookahead == 'f') ADVANCE(205);
-      if (lookahead == 'g') ADVANCE(315);
-      if (lookahead == 'h') ADVANCE(246);
-      if (lookahead == 'i') ADVANCE(208);
-      if (lookahead == 'l') ADVANCE(444);
-      if (lookahead == 'm') ADVANCE(120);
-      if (lookahead == 'n') ADVANCE(121);
-      if (lookahead == 'o') ADVANCE(728);
-      if (lookahead == 'p') ADVANCE(125);
-      if (lookahead == 'q') ADVANCE(894);
-      if (lookahead == 'r') ADVANCE(279);
-      if (lookahead == 's') ADVANCE(126);
-      if (lookahead == 't') ADVANCE(449);
-      if (lookahead == 'u') ADVANCE(567);
-      if (lookahead == 'w') ADVANCE(420);
-      if (lookahead == 'y') ADVANCE(280);
+      if (eof) ADVANCE(965);
+      if (lookahead == '!') ADVANCE(1133);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '#') ADVANCE(959);
+      if (lookahead == '&') ADVANCE(1194);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '*') ADVANCE(972);
+      if (lookahead == '+') ADVANCE(1005);
+      if (lookahead == ',') ADVANCE(969);
+      if (lookahead == '-') ADVANCE(1007);
+      if (lookahead == '/') ADVANCE(1003);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '=') ADVANCE(1193);
+      if (lookahead == '>') ADVANCE(977);
+      if (lookahead == '?') ADVANCE(1009);
+      if (lookahead == '\\') SKIP(961)
+      if (lookahead == '`') ADVANCE(1230);
+      if (lookahead == 'a') ADVANCE(198);
+      if (lookahead == 'b') ADVANCE(446);
+      if (lookahead == 'c') ADVANCE(229);
+      if (lookahead == 'd') ADVANCE(277);
+      if (lookahead == 'e') ADVANCE(202);
+      if (lookahead == 'f') ADVANCE(204);
+      if (lookahead == 'g') ADVANCE(314);
+      if (lookahead == 'h') ADVANCE(245);
+      if (lookahead == 'i') ADVANCE(207);
+      if (lookahead == 'l') ADVANCE(443);
+      if (lookahead == 'm') ADVANCE(119);
+      if (lookahead == 'n') ADVANCE(120);
+      if (lookahead == 'o') ADVANCE(727);
+      if (lookahead == 'p') ADVANCE(124);
+      if (lookahead == 'q') ADVANCE(893);
+      if (lookahead == 'r') ADVANCE(278);
+      if (lookahead == 's') ADVANCE(125);
+      if (lookahead == 't') ADVANCE(448);
+      if (lookahead == 'u') ADVANCE(566);
+      if (lookahead == 'w') ADVANCE(419);
+      if (lookahead == 'y') ADVANCE(279);
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(0)
       END_STATE();
     case 1:
-      if (lookahead == '\t') ADVANCE(1535);
-      if (lookahead == '\n') ADVANCE(1531);
+      if (lookahead == '\t') ADVANCE(1529);
+      if (lookahead == '\n') ADVANCE(1524);
       if (lookahead == '\r') ADVANCE(1);
-      if (lookahead == ' ') ADVANCE(996);
-      if (lookahead == '#') ADVANCE(1530);
-      if (lookahead == '+') ADVANCE(92);
-      if (lookahead == '-') ADVANCE(93);
-      if (lookahead == '/') ADVANCE(1004);
-      if (lookahead == '=') ADVANCE(1194);
-      if (lookahead == '\\') SKIP(29)
+      if (lookahead == ' ') ADVANCE(995);
+      if (lookahead == '#') ADVANCE(1523);
+      if (lookahead == '+') ADVANCE(94);
+      if (lookahead == '-') ADVANCE(95);
+      if (lookahead == '/') ADVANCE(1003);
+      if (lookahead == '=') ADVANCE(1193);
+      if (lookahead == '\\') SKIP(24)
       if (lookahead == 11 ||
           lookahead == '\f') SKIP(1)
       END_STATE();
     case 2:
-      if (lookahead == '\t') ADVANCE(980);
-      if (lookahead == '\n') ADVANCE(1532);
-      if (lookahead == '\r') ADVANCE(980);
-      if (lookahead == ' ') ADVANCE(1536);
-      if (lookahead == '#') ADVANCE(991);
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(31);
+      if (lookahead == '\t') ADVANCE(979);
+      if (lookahead == '\n') ADVANCE(1525);
+      if (lookahead == '\r') ADVANCE(979);
+      if (lookahead == ' ') ADVANCE(1530);
+      if (lookahead == '#') ADVANCE(990);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(30);
       if (lookahead == 11 ||
-          lookahead == '\f') ADVANCE(980);
-      if (lookahead != 0) ADVANCE(979);
+          lookahead == '\f') ADVANCE(979);
+      if (lookahead != 0) ADVANCE(978);
       END_STATE();
     case 3:
-      if (lookahead == '\n') ADVANCE(1533);
+      if (lookahead == '\n') ADVANCE(1526);
       if (lookahead == '\r') ADVANCE(3);
-      if (lookahead == '#') ADVANCE(1530);
-      if (lookahead == ',') ADVANCE(970);
+      if (lookahead == '#') ADVANCE(1523);
+      if (lookahead == ',') ADVANCE(969);
       if (lookahead == '\\') SKIP(5)
-      if (lookahead == 'a') ADVANCE(200);
-      if (lookahead == 'b') ADVANCE(446);
-      if (lookahead == 'c') ADVANCE(231);
-      if (lookahead == 'e') ADVANCE(204);
-      if (lookahead == 'f') ADVANCE(205);
-      if (lookahead == 'g') ADVANCE(799);
-      if (lookahead == 'h') ADVANCE(277);
-      if (lookahead == 'i') ADVANCE(209);
-      if (lookahead == 'l') ADVANCE(444);
-      if (lookahead == 'm') ADVANCE(175);
-      if (lookahead == 'n') ADVANCE(123);
-      if (lookahead == 'o') ADVANCE(728);
-      if (lookahead == 'p') ADVANCE(895);
-      if (lookahead == 'r') ADVANCE(305);
-      if (lookahead == 's') ADVANCE(128);
-      if (lookahead == 't') ADVANCE(475);
-      if (lookahead == 'u') ADVANCE(573);
+      if (lookahead == 'a') ADVANCE(199);
+      if (lookahead == 'b') ADVANCE(445);
+      if (lookahead == 'c') ADVANCE(230);
+      if (lookahead == 'e') ADVANCE(203);
+      if (lookahead == 'f') ADVANCE(204);
+      if (lookahead == 'g') ADVANCE(798);
+      if (lookahead == 'h') ADVANCE(276);
+      if (lookahead == 'i') ADVANCE(208);
+      if (lookahead == 'l') ADVANCE(443);
+      if (lookahead == 'm') ADVANCE(174);
+      if (lookahead == 'n') ADVANCE(122);
+      if (lookahead == 'o') ADVANCE(727);
+      if (lookahead == 'p') ADVANCE(894);
+      if (lookahead == 'r') ADVANCE(304);
+      if (lookahead == 's') ADVANCE(127);
+      if (lookahead == 't') ADVANCE(474);
+      if (lookahead == 'u') ADVANCE(572);
       if (lookahead == '\t' ||
-          lookahead == ' ') ADVANCE(1537);
+          lookahead == ' ') ADVANCE(1531);
       if (lookahead == 11 ||
           lookahead == '\f') SKIP(3)
       END_STATE();
     case 4:
       if (lookahead == '\n') SKIP(3)
       END_STATE();
     case 5:
       if (lookahead == '\n') SKIP(3)
       if (lookahead == '\r') SKIP(4)
       END_STATE();
     case 6:
-      if (lookahead == '\n') SKIP(60)
+      if (lookahead == '\n') SKIP(62)
       END_STATE();
     case 7:
-      if (lookahead == '\n') SKIP(60)
+      if (lookahead == '\n') SKIP(62)
       if (lookahead == '\r') SKIP(6)
       END_STATE();
     case 8:
-      if (lookahead == '\n') ADVANCE(1238);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '\\') ADVANCE(1251);
-      if (lookahead == '`') ADVANCE(1231);
-      if (lookahead == 'a') ADVANCE(1502);
-      if (lookahead == 'b') ADVANCE(1440);
-      if (lookahead == 'e') ADVANCE(1472);
-      if (lookahead == 'h') ADVANCE(1342);
-      if (lookahead == 'i') ADVANCE(1430);
-      if (lookahead == 'm') ADVANCE(1311);
-      if (lookahead == 'n') ADVANCE(1445);
-      if (lookahead == 'p') ADVANCE(1471);
-      if (lookahead == 'q') ADVANCE(1513);
-      if (lookahead == 's') ADVANCE(1363);
-      if (lookahead == 't') ADVANCE(1402);
-      if (lookahead == 'u') ADVANCE(1431);
-      if (('\t' <= lookahead && lookahead <= '\r') ||
-          lookahead == ' ') SKIP(8)
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == '\n') ADVANCE(1287);
       END_STATE();
     case 9:
-      if (lookahead == '\n') ADVANCE(1250);
+      if (lookahead == '\n') SKIP(60)
       END_STATE();
     case 10:
-      if (lookahead == '\n') SKIP(58)
+      if (lookahead == '\n') SKIP(60)
+      if (lookahead == '\r') SKIP(9)
       END_STATE();
     case 11:
-      if (lookahead == '\n') SKIP(58)
-      if (lookahead == '\r') SKIP(10)
+      if (lookahead == '\n') SKIP(65)
       END_STATE();
     case 12:
-      if (lookahead == '\n') SKIP(63)
+      if (lookahead == '\n') SKIP(65)
+      if (lookahead == '\r') SKIP(11)
       END_STATE();
     case 13:
-      if (lookahead == '\n') SKIP(63)
-      if (lookahead == '\r') SKIP(12)
+      if (lookahead == '\n') SKIP(47)
       END_STATE();
     case 14:
-      if (lookahead == '\n') ADVANCE(1239);
-      if (lookahead == ' ') ADVANCE(997);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '-') ADVANCE(1526);
-      if (lookahead == '\\') ADVANCE(1255);
-      if (lookahead == '`') ADVANCE(1231);
-      if (lookahead == 'a') ADVANCE(1493);
-      if (lookahead == 'n') ADVANCE(1442);
-      if (lookahead == 'y') ADVANCE(1373);
-      if (('\t' <= lookahead && lookahead <= '\r')) SKIP(14)
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1215);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == '\n') SKIP(47)
+      if (lookahead == '\r') SKIP(13)
       END_STATE();
     case 15:
-      if (lookahead == '\n') ADVANCE(1254);
+      if (lookahead == '\n') ADVANCE(1277);
       END_STATE();
     case 16:
-      if (lookahead == '\n') SKIP(57)
+      if (lookahead == '\n') ADVANCE(1283);
       END_STATE();
     case 17:
-      if (lookahead == '\n') SKIP(57)
-      if (lookahead == '\r') SKIP(16)
+      if (lookahead == '\n') ADVANCE(1280);
       END_STATE();
     case 18:
-      if (lookahead == '\n') ADVANCE(1288);
+      if (lookahead == '\n') ADVANCE(1279);
       END_STATE();
     case 19:
-      if (lookahead == '\n') ADVANCE(1289);
+      if (lookahead == '\n') ADVANCE(1282);
       END_STATE();
     case 20:
-      if (lookahead == '\n') ADVANCE(1290);
+      if (lookahead == '\n') ADVANCE(1281);
       END_STATE();
     case 21:
-      if (lookahead == '\n') ADVANCE(1291);
+      if (lookahead == '\n') SKIP(63)
+      if (lookahead == '\r') ADVANCE(991);
+      if (lookahead != 0) ADVANCE(991);
       END_STATE();
     case 22:
-      if (lookahead == '\n') ADVANCE(1292);
+      if (lookahead == '\n') ADVANCE(1285);
       END_STATE();
     case 23:
-      if (lookahead == '\n') ADVANCE(1240);
-      if (lookahead == ' ') SKIP(23)
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '<') ADVANCE(976);
-      if (lookahead == '\\') ADVANCE(1274);
-      if (lookahead == '`') ADVANCE(1231);
-      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(981);
-      if (lookahead != 0) ADVANCE(988);
+      if (lookahead == '\n') SKIP(1)
       END_STATE();
     case 24:
-      if (lookahead == '\n') ADVANCE(1293);
+      if (lookahead == '\n') SKIP(1)
+      if (lookahead == '\r') SKIP(23)
       END_STATE();
     case 25:
-      if (lookahead == '\n') ADVANCE(1294);
+      if (lookahead == '\n') ADVANCE(1527);
+      if (lookahead == '\r') ADVANCE(25);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '#') ADVANCE(1521);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '\\') ADVANCE(1265);
+      if (lookahead == '`') ADVANCE(1230);
+      if (lookahead == '\t' ||
+          lookahead == ' ') ADVANCE(1532);
+      if (lookahead == 11 ||
+          lookahead == '\f') SKIP(25)
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 26:
-      if (lookahead == '\n') ADVANCE(1295);
+      if (lookahead == '\n') ADVANCE(1264);
       END_STATE();
     case 27:
-      if (lookahead == '\n') SKIP(61)
-      if (lookahead == '\r') ADVANCE(992);
-      if (lookahead != 0) ADVANCE(992);
+      if (lookahead == '\n') ADVANCE(1278);
       END_STATE();
     case 28:
-      if (lookahead == '\n') SKIP(1)
+      if (lookahead == '\n') SKIP(70)
+      if (lookahead == '\r') ADVANCE(991);
+      if (lookahead != 0) ADVANCE(991);
       END_STATE();
     case 29:
-      if (lookahead == '\n') SKIP(1)
-      if (lookahead == '\r') SKIP(28)
+      if (lookahead == '\n') ADVANCE(1288);
       END_STATE();
     case 30:
-      if (lookahead == '\n') SKIP(68)
-      if (lookahead == '\r') ADVANCE(992);
-      if (lookahead != 0) ADVANCE(992);
+      if (lookahead == '\n') SKIP(2)
+      if (lookahead == '\r') ADVANCE(991);
+      if (lookahead != 0) ADVANCE(991);
       END_STATE();
     case 31:
-      if (lookahead == '\n') SKIP(2)
-      if (lookahead == '\r') ADVANCE(992);
-      if (lookahead != 0) ADVANCE(992);
+      if (lookahead == '\n') SKIP(61)
       END_STATE();
     case 32:
-      if (lookahead == '\n') SKIP(59)
+      if (lookahead == '\n') SKIP(61)
+      if (lookahead == '\r') SKIP(31)
       END_STATE();
     case 33:
-      if (lookahead == '\n') SKIP(59)
-      if (lookahead == '\r') SKIP(32)
+      if (lookahead == '\n') SKIP(64)
+      if (lookahead == '\r') ADVANCE(991);
+      if (lookahead != 0) ADVANCE(991);
       END_STATE();
     case 34:
-      if (lookahead == '\n') SKIP(62)
-      if (lookahead == '\r') ADVANCE(992);
-      if (lookahead != 0) ADVANCE(992);
+      if (lookahead == '\n') SKIP(92)
+      if (lookahead == '\r') ADVANCE(991);
+      if (lookahead != 0) ADVANCE(991);
       END_STATE();
     case 35:
-      if (lookahead == '\n') SKIP(90)
-      if (lookahead == '\r') ADVANCE(992);
-      if (lookahead != 0) ADVANCE(992);
+      if (lookahead == '\n') SKIP(93)
+      if (lookahead == '\r') ADVANCE(991);
+      if (lookahead != 0) ADVANCE(991);
       END_STATE();
     case 36:
-      if (lookahead == '\n') SKIP(91)
-      if (lookahead == '\r') ADVANCE(992);
-      if (lookahead != 0) ADVANCE(992);
+      if (lookahead == '\n') SKIP(67)
+      if (lookahead == '\r') ADVANCE(991);
+      if (lookahead != 0) ADVANCE(991);
       END_STATE();
     case 37:
-      if (lookahead == '\n') SKIP(65)
-      if (lookahead == '\r') ADVANCE(992);
-      if (lookahead != 0) ADVANCE(992);
+      if (lookahead == '\n') SKIP(66)
       END_STATE();
     case 38:
-      if (lookahead == '\n') SKIP(64)
+      if (lookahead == '\n') SKIP(66)
+      if (lookahead == '\r') SKIP(37)
       END_STATE();
     case 39:
-      if (lookahead == '\n') SKIP(64)
-      if (lookahead == '\r') SKIP(38)
+      if (lookahead == '\n') SKIP(98)
       END_STATE();
     case 40:
-      if (lookahead == '\n') SKIP(99)
+      if (lookahead == '\n') SKIP(98)
+      if (lookahead == '\r') SKIP(39)
       END_STATE();
     case 41:
-      if (lookahead == '\n') SKIP(99)
-      if (lookahead == '\r') SKIP(40)
+      if (lookahead == '\n') SKIP(43)
       END_STATE();
     case 42:
-      if (lookahead == '\n') SKIP(44)
+      if (lookahead == '\n') SKIP(43)
+      if (lookahead == '\r') SKIP(41)
       END_STATE();
     case 43:
-      if (lookahead == '\n') SKIP(44)
-      if (lookahead == '\r') SKIP(42)
+      if (lookahead == '\n') ADVANCE(1528);
+      if (lookahead == '\r') ADVANCE(43);
+      if (lookahead == '#') ADVANCE(1523);
+      if (lookahead == '\\') SKIP(42)
+      if (('\t' <= lookahead && lookahead <= '\f') ||
+          lookahead == ' ') SKIP(43)
       END_STATE();
     case 44:
-      if (lookahead == '\n') ADVANCE(1534);
-      if (lookahead == '\r') ADVANCE(44);
-      if (lookahead == '#') ADVANCE(1530);
-      if (lookahead == '\\') SKIP(43)
-      if (('\t' <= lookahead && lookahead <= '\f') ||
-          lookahead == ' ') SKIP(44)
+      if (lookahead == '\n') SKIP(99)
       END_STATE();
     case 45:
-      if (lookahead == '\n') SKIP(100)
+      if (lookahead == '\n') SKIP(99)
+      if (lookahead == '\r') SKIP(44)
       END_STATE();
     case 46:
-      if (lookahead == '\n') SKIP(100)
-      if (lookahead == '\r') SKIP(45)
+      if (lookahead == '\n') ADVANCE(1284);
       END_STATE();
     case 47:
-      if (lookahead == '\n') ADVANCE(1296);
+      if (lookahead == ' ') ADVANCE(996);
+      if (lookahead == '#') ADVANCE(959);
+      if (lookahead == '+') ADVANCE(94);
+      if (lookahead == '-') ADVANCE(95);
+      if (lookahead == '=') ADVANCE(1193);
+      if (lookahead == '\\') SKIP(14)
+      if (lookahead == 'b') ADVANCE(509);
+      if (lookahead == 'c') ADVANCE(713);
+      if (lookahead == 'd') ADVANCE(277);
+      if (lookahead == 'g') ADVANCE(794);
+      if (lookahead == 'm') ADVANCE(173);
+      if (lookahead == 'r') ADVANCE(348);
+      if (lookahead == 'w') ADVANCE(419);
+      if (lookahead == 'y') ADVANCE(370);
+      if (('\t' <= lookahead && lookahead <= '\r')) SKIP(47)
       END_STATE();
     case 48:
-      if (lookahead == '\n') ADVANCE(1241);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '-') ADVANCE(1526);
-      if (lookahead == '\\') ADVANCE(1258);
-      if (lookahead == '`') ADVANCE(1231);
-      if (lookahead == 'a') ADVANCE(1493);
-      if (lookahead == 'n') ADVANCE(1442);
-      if (lookahead == 'y') ADVANCE(1373);
-      if (('\t' <= lookahead && lookahead <= '\r') ||
-          lookahead == ' ') SKIP(48)
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1215);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == ' ') ADVANCE(997);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '-') ADVANCE(1518);
+      if (lookahead == '\\') ADVANCE(1241);
+      if (lookahead == '`') ADVANCE(1230);
+      if (lookahead == 'a') ADVANCE(1485);
+      if (lookahead == 'n') ADVANCE(1434);
+      if (lookahead == 'y') ADVANCE(1365);
+      if (('\t' <= lookahead && lookahead <= '\r')) SKIP(48)
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1214);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 49:
-      if (lookahead == '\n') ADVANCE(1242);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '*') ADVANCE(974);
-      if (lookahead == '-') ADVANCE(1395);
-      if (lookahead == '\\') ADVANCE(1261);
-      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == '!') ADVANCE(1134);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '\\') ADVANCE(1268);
+      if (lookahead == '`') ADVANCE(1230);
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(49)
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 50:
-      if (lookahead == '\n') ADVANCE(1243);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '+') ADVANCE(1007);
-      if (lookahead == '-') ADVANCE(1009);
-      if (lookahead == '?') ADVANCE(1011);
-      if (lookahead == '\\') ADVANCE(1264);
-      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '*') ADVANCE(973);
+      if (lookahead == '+') ADVANCE(1006);
+      if (lookahead == '-') ADVANCE(1008);
+      if (lookahead == '\\') ADVANCE(1250);
+      if (lookahead == '`') ADVANCE(1230);
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(50)
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 51:
-      if (lookahead == '\n') ADVANCE(1244);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '*') ADVANCE(974);
-      if (lookahead == '+') ADVANCE(1007);
-      if (lookahead == '-') ADVANCE(1009);
-      if (lookahead == '\\') ADVANCE(1267);
-      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '*') ADVANCE(973);
+      if (lookahead == '-') ADVANCE(1387);
+      if (lookahead == '\\') ADVANCE(1247);
+      if (lookahead == '`') ADVANCE(1230);
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(51)
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 52:
-      if (lookahead == '\n') ADVANCE(1245);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '*') ADVANCE(974);
-      if (lookahead == '\\') ADVANCE(1270);
-      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '*') ADVANCE(973);
+      if (lookahead == '\\') ADVANCE(1258);
+      if (lookahead == '`') ADVANCE(1230);
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(52)
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 53:
-      if (lookahead == '\n') ADVANCE(1246);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '-') ADVANCE(1395);
-      if (lookahead == '\\') ADVANCE(1276);
-      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '+') ADVANCE(1006);
+      if (lookahead == '-') ADVANCE(1008);
+      if (lookahead == '?') ADVANCE(1010);
+      if (lookahead == '\\') ADVANCE(1253);
+      if (lookahead == '`') ADVANCE(1230);
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(53)
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 54:
-      if (lookahead == '\n') ADVANCE(1247);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '\\') ADVANCE(1279);
-      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '-') ADVANCE(1518);
+      if (lookahead == '\\') ADVANCE(1244);
+      if (lookahead == '`') ADVANCE(1230);
+      if (lookahead == 'a') ADVANCE(1485);
+      if (lookahead == 'n') ADVANCE(1434);
+      if (lookahead == 'y') ADVANCE(1365);
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(54)
-      if (lookahead != 0) ADVANCE(1527);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1214);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 55:
-      if (lookahead == '\n') ADVANCE(1248);
-      if (lookahead == '!') ADVANCE(1135);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '\\') ADVANCE(1282);
-      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '-') ADVANCE(1431);
+      if (lookahead == '\\') ADVANCE(1274);
+      if (lookahead == '`') ADVANCE(1230);
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(55)
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 56:
-      if (lookahead == '\n') ADVANCE(1249);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '-') ADVANCE(1439);
-      if (lookahead == '\\') ADVANCE(1285);
-      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '-') ADVANCE(1387);
+      if (lookahead == '\\') ADVANCE(1261);
+      if (lookahead == '`') ADVANCE(1230);
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(56)
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 57:
-      if (lookahead == ' ') ADVANCE(998);
-      if (lookahead == '#') ADVANCE(960);
-      if (lookahead == '+') ADVANCE(92);
-      if (lookahead == '-') ADVANCE(93);
-      if (lookahead == '=') ADVANCE(1194);
-      if (lookahead == '\\') SKIP(17)
-      if (lookahead == 'b') ADVANCE(510);
-      if (lookahead == 'c') ADVANCE(714);
-      if (lookahead == 'd') ADVANCE(278);
-      if (lookahead == 'g') ADVANCE(795);
-      if (lookahead == 'm') ADVANCE(174);
-      if (lookahead == 'r') ADVANCE(349);
-      if (lookahead == 'w') ADVANCE(420);
-      if (lookahead == 'y') ADVANCE(371);
-      if (('\t' <= lookahead && lookahead <= '\r')) SKIP(57)
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '<') ADVANCE(975);
+      if (lookahead == '\\') ADVANCE(1256);
+      if (lookahead == '`') ADVANCE(1230);
+      if (lookahead == '\n' ||
+          lookahead == ' ') SKIP(57)
+      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(980);
+      if (lookahead != 0) ADVANCE(987);
       END_STATE();
     case 58:
-      if (lookahead == '#') ADVANCE(960);
-      if (lookahead == '\\') SKIP(11)
-      if (lookahead == 'a') ADVANCE(884);
-      if (lookahead == 'b') ADVANCE(511);
-      if (lookahead == 'c') ADVANCE(699);
-      if (lookahead == 'd') ADVANCE(278);
-      if (lookahead == 'e') ADVANCE(742);
-      if (lookahead == 'g') ADVANCE(795);
-      if (lookahead == 'h') ADVANCE(254);
-      if (lookahead == 'i') ADVANCE(566);
-      if (lookahead == 'm') ADVANCE(135);
-      if (lookahead == 'n') ADVANCE(625);
-      if (lookahead == 'p') ADVANCE(769);
-      if (lookahead == 'q') ADVANCE(910);
-      if (lookahead == 'r') ADVANCE(307);
-      if (lookahead == 's') ADVANCE(365);
-      if (lookahead == 't') ADVANCE(476);
-      if (lookahead == 'u') ADVANCE(609);
-      if (lookahead == 'w') ADVANCE(420);
-      if (lookahead == 'y') ADVANCE(371);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '\\') ADVANCE(1238);
+      if (lookahead == '`') ADVANCE(1230);
+      if (lookahead == 'a') ADVANCE(1494);
+      if (lookahead == 'b') ADVANCE(1432);
+      if (lookahead == 'e') ADVANCE(1464);
+      if (lookahead == 'h') ADVANCE(1334);
+      if (lookahead == 'i') ADVANCE(1422);
+      if (lookahead == 'm') ADVANCE(1303);
+      if (lookahead == 'n') ADVANCE(1437);
+      if (lookahead == 'p') ADVANCE(1463);
+      if (lookahead == 'q') ADVANCE(1505);
+      if (lookahead == 's') ADVANCE(1355);
+      if (lookahead == 't') ADVANCE(1394);
+      if (lookahead == 'u') ADVANCE(1423);
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(58)
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 59:
-      if (lookahead == '&') ADVANCE(1195);
-      if (lookahead == '+') ADVANCE(92);
-      if (lookahead == '-') ADVANCE(93);
-      if (lookahead == '=') ADVANCE(1194);
-      if (lookahead == '?') ADVANCE(1010);
-      if (lookahead == '\\') SKIP(33)
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
+      if (lookahead == '\\') ADVANCE(1271);
+      if (lookahead == '`') ADVANCE(1230);
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(59)
-      if (('0' <= lookahead && lookahead <= '9') ||
-          lookahead == '_' ||
-          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1206);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 60:
-      if (lookahead == '*') ADVANCE(973);
-      if (lookahead == '+') ADVANCE(92);
-      if (lookahead == '-') ADVANCE(94);
-      if (lookahead == '=') ADVANCE(1194);
-      if (lookahead == '\\') SKIP(7)
-      if (lookahead == 'a') ADVANCE(200);
-      if (lookahead == 'b') ADVANCE(448);
-      if (lookahead == 'c') ADVANCE(231);
-      if (lookahead == 'e') ADVANCE(204);
-      if (lookahead == 'f') ADVANCE(205);
-      if (lookahead == 'g') ADVANCE(799);
-      if (lookahead == 'h') ADVANCE(277);
-      if (lookahead == 'i') ADVANCE(209);
-      if (lookahead == 'l') ADVANCE(444);
-      if (lookahead == 'm') ADVANCE(175);
-      if (lookahead == 'n') ADVANCE(122);
-      if (lookahead == 'o') ADVANCE(728);
-      if (lookahead == 'p') ADVANCE(895);
+      if (lookahead == '#') ADVANCE(959);
+      if (lookahead == '\\') SKIP(10)
+      if (lookahead == 'a') ADVANCE(883);
+      if (lookahead == 'b') ADVANCE(510);
+      if (lookahead == 'c') ADVANCE(698);
+      if (lookahead == 'd') ADVANCE(277);
+      if (lookahead == 'e') ADVANCE(741);
+      if (lookahead == 'g') ADVANCE(794);
+      if (lookahead == 'h') ADVANCE(253);
+      if (lookahead == 'i') ADVANCE(565);
+      if (lookahead == 'm') ADVANCE(134);
+      if (lookahead == 'n') ADVANCE(624);
+      if (lookahead == 'p') ADVANCE(768);
+      if (lookahead == 'q') ADVANCE(909);
       if (lookahead == 'r') ADVANCE(306);
-      if (lookahead == 's') ADVANCE(127);
+      if (lookahead == 's') ADVANCE(364);
       if (lookahead == 't') ADVANCE(475);
-      if (lookahead == 'u') ADVANCE(567);
+      if (lookahead == 'u') ADVANCE(608);
+      if (lookahead == 'w') ADVANCE(419);
+      if (lookahead == 'y') ADVANCE(370);
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(60)
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1216);
       END_STATE();
     case 61:
-      if (lookahead == '*') ADVANCE(973);
-      if (lookahead == '-') ADVANCE(989);
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(27);
-      if (lookahead == '\n' ||
+      if (lookahead == '&') ADVANCE(1194);
+      if (lookahead == '+') ADVANCE(94);
+      if (lookahead == '-') ADVANCE(95);
+      if (lookahead == '=') ADVANCE(1193);
+      if (lookahead == '?') ADVANCE(1009);
+      if (lookahead == '\\') SKIP(32)
+      if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(61)
-      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(982);
-      if (lookahead != 0) ADVANCE(979);
+      if (('0' <= lookahead && lookahead <= '9') ||
+          lookahead == '_' ||
+          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1205);
       END_STATE();
     case 62:
-      if (lookahead == '*') ADVANCE(973);
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(34);
-      if (lookahead == '\n' ||
+      if (lookahead == '*') ADVANCE(972);
+      if (lookahead == '+') ADVANCE(94);
+      if (lookahead == '-') ADVANCE(96);
+      if (lookahead == '=') ADVANCE(1193);
+      if (lookahead == '\\') SKIP(7)
+      if (lookahead == 'a') ADVANCE(199);
+      if (lookahead == 'b') ADVANCE(447);
+      if (lookahead == 'c') ADVANCE(230);
+      if (lookahead == 'e') ADVANCE(203);
+      if (lookahead == 'f') ADVANCE(204);
+      if (lookahead == 'g') ADVANCE(798);
+      if (lookahead == 'h') ADVANCE(276);
+      if (lookahead == 'i') ADVANCE(208);
+      if (lookahead == 'l') ADVANCE(443);
+      if (lookahead == 'm') ADVANCE(174);
+      if (lookahead == 'n') ADVANCE(121);
+      if (lookahead == 'o') ADVANCE(727);
+      if (lookahead == 'p') ADVANCE(894);
+      if (lookahead == 'r') ADVANCE(305);
+      if (lookahead == 's') ADVANCE(126);
+      if (lookahead == 't') ADVANCE(474);
+      if (lookahead == 'u') ADVANCE(566);
+      if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(62)
-      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(983);
-      if (lookahead != 0) ADVANCE(979);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1215);
       END_STATE();
     case 63:
-      if (lookahead == '*') ADVANCE(973);
-      if (lookahead == '\\') SKIP(13)
-      if (lookahead == 'a') ADVANCE(525);
-      if (lookahead == 'b') ADVANCE(741);
-      if (lookahead == 'c') ADVANCE(644);
-      if (lookahead == 'e') ADVANCE(244);
-      if (lookahead == 'g') ADVANCE(314);
-      if (lookahead == 'i') ADVANCE(607);
-      if (lookahead == 'm') ADVANCE(454);
-      if (lookahead == 'p') ADVANCE(124);
-      if (lookahead == 'q') ADVANCE(911);
-      if (lookahead == 's') ADVANCE(552);
-      if (('\t' <= lookahead && lookahead <= '\r') ||
+      if (lookahead == '*') ADVANCE(972);
+      if (lookahead == '-') ADVANCE(988);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(21);
+      if (lookahead == '\n' ||
           lookahead == ' ') SKIP(63)
+      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(981);
+      if (lookahead != 0) ADVANCE(978);
       END_STATE();
     case 64:
-      if (lookahead == '*') ADVANCE(973);
-      if (lookahead == '\\') SKIP(39)
-      if (('\t' <= lookahead && lookahead <= '\r') ||
+      if (lookahead == '*') ADVANCE(972);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(33);
+      if (lookahead == '\n' ||
           lookahead == ' ') SKIP(64)
-      if (lookahead == '-' ||
-          lookahead == '.' ||
-          ('0' <= lookahead && lookahead <= '9') ||
-          ('A' <= lookahead && lookahead <= 'Z') ||
-          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1003);
+      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(982);
+      if (lookahead != 0) ADVANCE(978);
       END_STATE();
     case 65:
-      if (lookahead == ',') ADVANCE(970);
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(37);
-      if (lookahead == '\n' ||
+      if (lookahead == '*') ADVANCE(972);
+      if (lookahead == '\\') SKIP(12)
+      if (lookahead == 'a') ADVANCE(524);
+      if (lookahead == 'b') ADVANCE(740);
+      if (lookahead == 'c') ADVANCE(643);
+      if (lookahead == 'e') ADVANCE(243);
+      if (lookahead == 'g') ADVANCE(313);
+      if (lookahead == 'i') ADVANCE(606);
+      if (lookahead == 'm') ADVANCE(453);
+      if (lookahead == 'p') ADVANCE(123);
+      if (lookahead == 'q') ADVANCE(910);
+      if (lookahead == 's') ADVANCE(551);
+      if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(65)
-      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(984);
-      if (lookahead != 0) ADVANCE(979);
       END_STATE();
     case 66:
-      if (lookahead == '-') ADVANCE(592);
+      if (lookahead == '*') ADVANCE(972);
+      if (lookahead == '\\') SKIP(38)
+      if (('\t' <= lookahead && lookahead <= '\r') ||
+          lookahead == ' ') SKIP(66)
+      if (lookahead == '-' ||
+          lookahead == '.' ||
+          ('0' <= lookahead && lookahead <= '9') ||
+          ('A' <= lookahead && lookahead <= 'Z') ||
+          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1002);
       END_STATE();
     case 67:
-      if (lookahead == '-') ADVANCE(417);
+      if (lookahead == ',') ADVANCE(969);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(36);
+      if (lookahead == '\n' ||
+          lookahead == ' ') SKIP(67)
+      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(983);
+      if (lookahead != 0) ADVANCE(978);
       END_STATE();
     case 68:
-      if (lookahead == '-') ADVANCE(989);
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(30);
-      if (lookahead == '\n' ||
-          lookahead == ' ') SKIP(68)
-      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(985);
-      if (lookahead != 0) ADVANCE(979);
+      if (lookahead == '-') ADVANCE(591);
       END_STATE();
     case 69:
-      if (lookahead == '-') ADVANCE(388);
+      if (lookahead == '-') ADVANCE(416);
       END_STATE();
     case 70:
-      if (lookahead == '-') ADVANCE(422);
+      if (lookahead == '-') ADVANCE(988);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(28);
+      if (lookahead == '\n' ||
+          lookahead == ' ') SKIP(70)
+      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(984);
+      if (lookahead != 0) ADVANCE(978);
       END_STATE();
     case 71:
-      if (lookahead == '-') ADVANCE(560);
+      if (lookahead == '-') ADVANCE(387);
       END_STATE();
     case 72:
-      if (lookahead == '-') ADVANCE(424);
+      if (lookahead == '-') ADVANCE(421);
       END_STATE();
     case 73:
-      if (lookahead == '-') ADVANCE(426);
+      if (lookahead == '-') ADVANCE(559);
       END_STATE();
     case 74:
-      if (lookahead == '-') ADVANCE(427);
-      if (lookahead == '2') ADVANCE(79);
+      if (lookahead == '-') ADVANCE(423);
       END_STATE();
     case 75:
-      if (lookahead == '-') ADVANCE(428);
+      if (lookahead == '-') ADVANCE(425);
       END_STATE();
     case 76:
-      if (lookahead == '-') ADVANCE(429);
+      if (lookahead == '-') ADVANCE(426);
+      if (lookahead == '2') ADVANCE(81);
       END_STATE();
     case 77:
-      if (lookahead == '-') ADVANCE(430);
+      if (lookahead == '-') ADVANCE(427);
       END_STATE();
     case 78:
-      if (lookahead == '-') ADVANCE(431);
+      if (lookahead == '-') ADVANCE(428);
       END_STATE();
     case 79:
-      if (lookahead == '-') ADVANCE(432);
+      if (lookahead == '-') ADVANCE(429);
       END_STATE();
     case 80:
-      if (lookahead == '-') ADVANCE(433);
+      if (lookahead == '-') ADVANCE(430);
       END_STATE();
     case 81:
-      if (lookahead == '-') ADVANCE(434);
+      if (lookahead == '-') ADVANCE(431);
       END_STATE();
     case 82:
-      if (lookahead == '-') ADVANCE(435);
+      if (lookahead == '-') ADVANCE(432);
       END_STATE();
     case 83:
-      if (lookahead == '-') ADVANCE(436);
+      if (lookahead == '-') ADVANCE(433);
       END_STATE();
     case 84:
-      if (lookahead == '-') ADVANCE(437);
+      if (lookahead == '-') ADVANCE(434);
       END_STATE();
     case 85:
-      if (lookahead == '-') ADVANCE(438);
+      if (lookahead == '-') ADVANCE(435);
       END_STATE();
     case 86:
-      if (lookahead == '-') ADVANCE(439);
+      if (lookahead == '-') ADVANCE(436);
       END_STATE();
     case 87:
-      if (lookahead == '-') ADVANCE(440);
+      if (lookahead == '-') ADVANCE(437);
       END_STATE();
     case 88:
-      if (lookahead == '-') ADVANCE(441);
+      if (lookahead == '-') ADVANCE(438);
       END_STATE();
     case 89:
-      if (lookahead == '-') ADVANCE(442);
+      if (lookahead == '-') ADVANCE(439);
       END_STATE();
     case 90:
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(35);
-      if (lookahead == '\n' ||
-          lookahead == ' ') SKIP(90)
-      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(986);
-      if (lookahead != 0) ADVANCE(979);
+      if (lookahead == '-') ADVANCE(440);
       END_STATE();
     case 91:
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(36);
-      if (lookahead == '\n' ||
-          lookahead == ' ') SKIP(91)
-      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(987);
-      if (lookahead == '-' ||
-          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(990);
-      if (lookahead != 0) ADVANCE(979);
+      if (lookahead == '-') ADVANCE(441);
       END_STATE();
     case 92:
-      if (lookahead == '=') ADVANCE(1192);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(34);
+      if (lookahead == '\n' ||
+          lookahead == ' ') SKIP(92)
+      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(985);
+      if (lookahead != 0) ADVANCE(978);
       END_STATE();
     case 93:
-      if (lookahead == '=') ADVANCE(1193);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(35);
+      if (lookahead == '\n' ||
+          lookahead == ' ') SKIP(93)
+      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(986);
+      if (lookahead == '-' ||
+          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(989);
+      if (lookahead != 0) ADVANCE(978);
       END_STATE();
     case 94:
-      if (lookahead == '=') ADVANCE(1193);
-      if (lookahead == 'a') ADVANCE(264);
-      if (lookahead == 'g') ADVANCE(806);
-      if (lookahead == 'r') ADVANCE(939);
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1216);
+      if (lookahead == '=') ADVANCE(1191);
       END_STATE();
     case 95:
-      if (lookahead == '\\') ADVANCE(1219);
-      if (('\t' <= lookahead && lookahead <= '\r') ||
-          lookahead == ' ') ADVANCE(1221);
-      if (lookahead != 0 &&
-          lookahead != '\'') ADVANCE(1222);
+      if (lookahead == '=') ADVANCE(1192);
       END_STATE();
     case 96:
-      if (lookahead == '\\') ADVANCE(1226);
-      if (('\t' <= lookahead && lookahead <= '\r') ||
-          lookahead == ' ') ADVANCE(1228);
-      if (lookahead != 0 &&
-          lookahead != '"') ADVANCE(1229);
+      if (lookahead == '=') ADVANCE(1192);
+      if (lookahead == 'a') ADVANCE(263);
+      if (lookahead == 'g') ADVANCE(805);
+      if (lookahead == 'r') ADVANCE(938);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1215);
       END_STATE();
     case 97:
-      if (lookahead == '\\') ADVANCE(1233);
+      if (lookahead == '\\') ADVANCE(1199);
       if (('\t' <= lookahead && lookahead <= '\r') ||
-          lookahead == ' ') ADVANCE(1235);
-      if (lookahead != 0 &&
-          lookahead != '`') ADVANCE(1236);
+          lookahead == ' ') SKIP(97)
+      if (lookahead != 0) ADVANCE(1199);
       END_STATE();
     case 98:
-      if (lookahead == '\\') ADVANCE(1200);
+      if (lookahead == '\\') SKIP(40)
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(98)
-      if (lookahead != 0) ADVANCE(1200);
+      if (lookahead == '-' ||
+          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1028);
       END_STATE();
     case 99:
-      if (lookahead == '\\') SKIP(41)
+      if (lookahead == '\\') SKIP(45)
       if (('\t' <= lookahead && lookahead <= '\r') ||
           lookahead == ' ') SKIP(99)
       if (lookahead == '-' ||
-          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1029);
+          ('A' <= lookahead && lookahead <= 'Z') ||
+          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(976);
       END_STATE();
     case 100:
-      if (lookahead == '\\') SKIP(46)
-      if (('\t' <= lookahead && lookahead <= '\r') ||
-          lookahead == ' ') SKIP(100)
-      if (lookahead == '-' ||
-          ('A' <= lookahead && lookahead <= 'Z') ||
-          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(977);
+      if (lookahead == '_') ADVANCE(185);
       END_STATE();
     case 101:
-      if (lookahead == '_') ADVANCE(186);
+      if (lookahead == '_') ADVANCE(189);
       END_STATE();
     case 102:
-      if (lookahead == '_') ADVANCE(190);
+      if (lookahead == '_') ADVANCE(732);
       END_STATE();
     case 103:
-      if (lookahead == '_') ADVANCE(733);
+      if (lookahead == '_') ADVANCE(186);
       END_STATE();
     case 104:
-      if (lookahead == '_') ADVANCE(187);
+      if (lookahead == '_') ADVANCE(413);
       END_STATE();
     case 105:
-      if (lookahead == '_') ADVANCE(414);
+      if (lookahead == '_') ADVANCE(918);
       END_STATE();
     case 106:
-      if (lookahead == '_') ADVANCE(919);
+      if (lookahead == '_') ADVANCE(385);
       END_STATE();
     case 107:
-      if (lookahead == '_') ADVANCE(386);
+      if (lookahead == '_') ADVANCE(418);
+      if (lookahead == 'm') ADVANCE(349);
       END_STATE();
     case 108:
-      if (lookahead == '_') ADVANCE(419);
-      if (lookahead == 'm') ADVANCE(350);
+      if (lookahead == '_') ADVANCE(154);
       END_STATE();
     case 109:
-      if (lookahead == '_') ADVANCE(155);
+      if (lookahead == '_') ADVANCE(537);
       END_STATE();
     case 110:
-      if (lookahead == '_') ADVANCE(538);
+      if (lookahead == '_') ADVANCE(659);
       END_STATE();
     case 111:
-      if (lookahead == '_') ADVANCE(660);
+      if (lookahead == '_') ADVANCE(659);
+      if (lookahead == 'd') ADVANCE(373);
       END_STATE();
     case 112:
-      if (lookahead == '_') ADVANCE(660);
-      if (lookahead == 'd') ADVANCE(374);
+      if (lookahead == '_') ADVANCE(420);
       END_STATE();
     case 113:
-      if (lookahead == '_') ADVANCE(421);
+      if (lookahead == '_') ADVANCE(922);
       END_STATE();
     case 114:
-      if (lookahead == '_') ADVANCE(923);
+      if (lookahead == '_') ADVANCE(178);
       END_STATE();
     case 115:
-      if (lookahead == '_') ADVANCE(179);
+      if (lookahead == '_') ADVANCE(546);
       END_STATE();
     case 116:
-      if (lookahead == '_') ADVANCE(547);
+      if (lookahead == '_') ADVANCE(715);
       END_STATE();
     case 117:
       if (lookahead == '_') ADVANCE(716);
       END_STATE();
     case 118:
       if (lookahead == '_') ADVANCE(717);
       END_STATE();
     case 119:
-      if (lookahead == '_') ADVANCE(718);
+      if (lookahead == 'a') ADVANCE(221);
+      if (lookahead == 'b') ADVANCE(613);
+      if (lookahead == 'e') ADVANCE(833);
+      if (lookahead == 'i') ADVANCE(554);
+      if (lookahead == 'o') ADVANCE(585);
+      if (lookahead == 'y') ADVANCE(104);
       END_STATE();
     case 120:
-      if (lookahead == 'a') ADVANCE(222);
-      if (lookahead == 'b') ADVANCE(614);
-      if (lookahead == 'e') ADVANCE(834);
-      if (lookahead == 'i') ADVANCE(555);
-      if (lookahead == 'o') ADVANCE(586);
-      if (lookahead == 'y') ADVANCE(105);
+      if (lookahead == 'a') ADVANCE(556);
+      if (lookahead == 'o') ADVANCE(1209);
       END_STATE();
     case 121:
-      if (lookahead == 'a') ADVANCE(557);
-      if (lookahead == 'o') ADVANCE(1210);
+      if (lookahead == 'a') ADVANCE(556);
+      if (lookahead == 'o') ADVANCE(583);
       END_STATE();
     case 122:
-      if (lookahead == 'a') ADVANCE(557);
-      if (lookahead == 'o') ADVANCE(584);
+      if (lookahead == 'a') ADVANCE(556);
+      if (lookahead == 'o') ADVANCE(832);
       END_STATE();
     case 123:
-      if (lookahead == 'a') ADVANCE(557);
-      if (lookahead == 'o') ADVANCE(833);
+      if (lookahead == 'a') ADVANCE(403);
+      if (lookahead == 'g') ADVANCE(719);
+      if (lookahead == 'o') ADVANCE(831);
       END_STATE();
     case 124:
-      if (lookahead == 'a') ADVANCE(404);
-      if (lookahead == 'g') ADVANCE(720);
-      if (lookahead == 'o') ADVANCE(832);
+      if (lookahead == 'a') ADVANCE(403);
+      if (lookahead == 'g') ADVANCE(719);
+      if (lookahead == 'o') ADVANCE(831);
+      if (lookahead == 'r') ADVANCE(614);
+      if (lookahead == 'u') ADVANCE(830);
       END_STATE();
     case 125:
-      if (lookahead == 'a') ADVANCE(404);
-      if (lookahead == 'g') ADVANCE(720);
-      if (lookahead == 'o') ADVANCE(832);
-      if (lookahead == 'r') ADVANCE(615);
-      if (lookahead == 'u') ADVANCE(831);
+      if (lookahead == 'a') ADVANCE(920);
+      if (lookahead == 'c') ADVANCE(633);
+      if (lookahead == 'e') ADVANCE(145);
+      if (lookahead == 'h') ADVANCE(897);
+      if (lookahead == 'i') ADVANCE(248);
+      if (lookahead == 'm') ADVANCE(462);
+      if (lookahead == 'o') ADVANCE(911);
+      if (lookahead == 'p') ADVANCE(138);
+      if (lookahead == 't') ADVANCE(128);
+      if (lookahead == 'u') ADVANCE(182);
       END_STATE();
     case 126:
-      if (lookahead == 'a') ADVANCE(921);
-      if (lookahead == 'c') ADVANCE(634);
-      if (lookahead == 'e') ADVANCE(146);
-      if (lookahead == 'h') ADVANCE(898);
-      if (lookahead == 'i') ADVANCE(249);
-      if (lookahead == 'm') ADVANCE(463);
-      if (lookahead == 'o') ADVANCE(912);
-      if (lookahead == 'p') ADVANCE(139);
-      if (lookahead == 't') ADVANCE(129);
-      if (lookahead == 'u') ADVANCE(183);
+      if (lookahead == 'a') ADVANCE(920);
+      if (lookahead == 'c') ADVANCE(633);
+      if (lookahead == 'e') ADVANCE(577);
+      if (lookahead == 'h') ADVANCE(897);
+      if (lookahead == 'i') ADVANCE(271);
+      if (lookahead == 'o') ADVANCE(911);
+      if (lookahead == 'p') ADVANCE(138);
+      if (lookahead == 't') ADVANCE(133);
+      if (lookahead == 'u') ADVANCE(182);
       END_STATE();
     case 127:
-      if (lookahead == 'a') ADVANCE(921);
-      if (lookahead == 'c') ADVANCE(634);
-      if (lookahead == 'e') ADVANCE(578);
-      if (lookahead == 'h') ADVANCE(898);
-      if (lookahead == 'i') ADVANCE(272);
-      if (lookahead == 'o') ADVANCE(912);
-      if (lookahead == 'p') ADVANCE(139);
-      if (lookahead == 't') ADVANCE(134);
-      if (lookahead == 'u') ADVANCE(183);
+      if (lookahead == 'a') ADVANCE(920);
+      if (lookahead == 'c') ADVANCE(633);
+      if (lookahead == 'e') ADVANCE(577);
+      if (lookahead == 'h') ADVANCE(897);
+      if (lookahead == 'i') ADVANCE(271);
+      if (lookahead == 'o') ADVANCE(911);
+      if (lookahead == 'p') ADVANCE(138);
+      if (lookahead == 't') ADVANCE(160);
+      if (lookahead == 'u') ADVANCE(182);
       END_STATE();
     case 128:
-      if (lookahead == 'a') ADVANCE(921);
-      if (lookahead == 'c') ADVANCE(634);
-      if (lookahead == 'e') ADVANCE(578);
-      if (lookahead == 'h') ADVANCE(898);
-      if (lookahead == 'i') ADVANCE(272);
-      if (lookahead == 'o') ADVANCE(912);
-      if (lookahead == 'p') ADVANCE(139);
-      if (lookahead == 't') ADVANCE(161);
-      if (lookahead == 'u') ADVANCE(183);
+      if (lookahead == 'a') ADVANCE(579);
       END_STATE();
     case 129:
-      if (lookahead == 'a') ADVANCE(580);
+      if (lookahead == 'a') ADVANCE(543);
+      if (lookahead == 'b') ADVANCE(471);
+      if (lookahead == 'c') ADVANCE(636);
+      if (lookahead == 'd') ADVANCE(333);
+      if (lookahead == 'g') ADVANCE(783);
+      if (lookahead == 'h') ADVANCE(247);
+      if (lookahead == 'i') ADVANCE(405);
+      if (lookahead == 'l') ADVANCE(476);
+      if (lookahead == 'm') ADVANCE(131);
+      if (lookahead == 's') ADVANCE(225);
       END_STATE();
     case 130:
-      if (lookahead == 'a') ADVANCE(544);
-      if (lookahead == 'b') ADVANCE(472);
-      if (lookahead == 'c') ADVANCE(637);
-      if (lookahead == 'd') ADVANCE(334);
-      if (lookahead == 'g') ADVANCE(784);
-      if (lookahead == 'h') ADVANCE(248);
-      if (lookahead == 'i') ADVANCE(406);
-      if (lookahead == 'l') ADVANCE(477);
-      if (lookahead == 'm') ADVANCE(132);
-      if (lookahead == 's') ADVANCE(226);
+      if (lookahead == 'a') ADVANCE(543);
+      if (lookahead == 'b') ADVANCE(471);
+      if (lookahead == 'c') ADVANCE(636);
+      if (lookahead == 'g') ADVANCE(783);
+      if (lookahead == 'h') ADVANCE(247);
+      if (lookahead == 'i') ADVANCE(405);
+      if (lookahead == 'l') ADVANCE(476);
+      if (lookahead == 'm') ADVANCE(131);
+      if (lookahead == 's') ADVANCE(225);
       END_STATE();
     case 131:
-      if (lookahead == 'a') ADVANCE(544);
-      if (lookahead == 'b') ADVANCE(472);
-      if (lookahead == 'c') ADVANCE(637);
-      if (lookahead == 'g') ADVANCE(784);
-      if (lookahead == 'h') ADVANCE(248);
-      if (lookahead == 'i') ADVANCE(406);
-      if (lookahead == 'l') ADVANCE(477);
-      if (lookahead == 'm') ADVANCE(132);
-      if (lookahead == 's') ADVANCE(226);
+      if (lookahead == 'a') ADVANCE(226);
+      if (lookahead == 'i') ADVANCE(564);
+      if (lookahead == 'o') ADVANCE(592);
+      if (lookahead == 'y') ADVANCE(112);
       END_STATE();
     case 132:
-      if (lookahead == 'a') ADVANCE(227);
-      if (lookahead == 'i') ADVANCE(565);
-      if (lookahead == 'o') ADVANCE(593);
-      if (lookahead == 'y') ADVANCE(113);
+      if (lookahead == 'a') ADVANCE(1120);
       END_STATE();
     case 133:
-      if (lookahead == 'a') ADVANCE(1121);
+      if (lookahead == 'a') ADVANCE(578);
       END_STATE();
     case 134:
-      if (lookahead == 'a') ADVANCE(579);
+      if (lookahead == 'a') ADVANCE(401);
+      if (lookahead == 'e') ADVANCE(846);
       END_STATE();
     case 135:
-      if (lookahead == 'a') ADVANCE(402);
-      if (lookahead == 'e') ADVANCE(847);
+      if (lookahead == 'a') ADVANCE(580);
       END_STATE();
     case 136:
-      if (lookahead == 'a') ADVANCE(581);
+      if (lookahead == 'a') ADVANCE(206);
+      if (lookahead == 'u') ADVANCE(280);
       END_STATE();
     case 137:
-      if (lookahead == 'a') ADVANCE(207);
-      if (lookahead == 'u') ADVANCE(281);
+      if (lookahead == 'a') ADVANCE(801);
       END_STATE();
     case 138:
-      if (lookahead == 'a') ADVANCE(802);
+      if (lookahead == 'a') ADVANCE(548);
       END_STATE();
     case 139:
       if (lookahead == 'a') ADVANCE(549);
       END_STATE();
     case 140:
-      if (lookahead == 'a') ADVANCE(550);
+      if (lookahead == 'a') ADVANCE(209);
       END_STATE();
     case 141:
-      if (lookahead == 'a') ADVANCE(210);
+      if (lookahead == 'a') ADVANCE(389);
       END_STATE();
     case 142:
-      if (lookahead == 'a') ADVANCE(390);
+      if (lookahead == 'a') ADVANCE(898);
       END_STATE();
     case 143:
-      if (lookahead == 'a') ADVANCE(899);
+      if (lookahead == 'a') ADVANCE(567);
       END_STATE();
     case 144:
-      if (lookahead == 'a') ADVANCE(568);
+      if (lookahead == 'a') ADVANCE(773);
       END_STATE();
     case 145:
-      if (lookahead == 'a') ADVANCE(774);
+      if (lookahead == 'a') ADVANCE(773);
+      if (lookahead == 'c') ADVANCE(903);
+      if (lookahead == 'n') ADVANCE(237);
+      if (lookahead == 't') ADVANCE(1190);
       END_STATE();
     case 146:
-      if (lookahead == 'a') ADVANCE(774);
-      if (lookahead == 'c') ADVANCE(904);
-      if (lookahead == 'n') ADVANCE(238);
-      if (lookahead == 't') ADVANCE(1191);
+      if (lookahead == 'a') ADVANCE(812);
       END_STATE();
     case 147:
-      if (lookahead == 'a') ADVANCE(813);
+      if (lookahead == 'a') ADVANCE(394);
       END_STATE();
     case 148:
-      if (lookahead == 'a') ADVANCE(395);
+      if (lookahead == 'a') ADVANCE(512);
       END_STATE();
     case 149:
-      if (lookahead == 'a') ADVANCE(513);
+      if (lookahead == 'a') ADVANCE(399);
       END_STATE();
     case 150:
-      if (lookahead == 'a') ADVANCE(400);
+      if (lookahead == 'a') ADVANCE(455);
       END_STATE();
     case 151:
-      if (lookahead == 'a') ADVANCE(456);
+      if (lookahead == 'a') ADVANCE(817);
       END_STATE();
     case 152:
-      if (lookahead == 'a') ADVANCE(818);
+      if (lookahead == 'a') ADVANCE(212);
       END_STATE();
     case 153:
-      if (lookahead == 'a') ADVANCE(213);
+      if (lookahead == 'a') ADVANCE(882);
       END_STATE();
     case 154:
-      if (lookahead == 'a') ADVANCE(883);
+      if (lookahead == 'a') ADVANCE(545);
       END_STATE();
     case 155:
-      if (lookahead == 'a') ADVANCE(546);
+      if (lookahead == 'a') ADVANCE(736);
       END_STATE();
     case 156:
-      if (lookahead == 'a') ADVANCE(737);
+      if (lookahead == 'a') ADVANCE(213);
       END_STATE();
     case 157:
-      if (lookahead == 'a') ADVANCE(214);
+      if (lookahead == 'a') ADVANCE(858);
       END_STATE();
     case 158:
-      if (lookahead == 'a') ADVANCE(859);
+      if (lookahead == 'a') ADVANCE(771);
       END_STATE();
     case 159:
-      if (lookahead == 'a') ADVANCE(772);
+      if (lookahead == 'a') ADVANCE(770);
       END_STATE();
     case 160:
-      if (lookahead == 'a') ADVANCE(771);
+      if (lookahead == 'a') ADVANCE(775);
       END_STATE();
     case 161:
-      if (lookahead == 'a') ADVANCE(776);
+      if (lookahead == 'a') ADVANCE(777);
       END_STATE();
     case 162:
-      if (lookahead == 'a') ADVANCE(778);
+      if (lookahead == 'a') ADVANCE(779);
       END_STATE();
     case 163:
-      if (lookahead == 'a') ADVANCE(780);
+      if (lookahead == 'a') ADVANCE(396);
       END_STATE();
     case 164:
-      if (lookahead == 'a') ADVANCE(397);
+      if (lookahead == 'a') ADVANCE(217);
       END_STATE();
     case 165:
-      if (lookahead == 'a') ADVANCE(218);
+      if (lookahead == 'a') ADVANCE(188);
       END_STATE();
     case 166:
-      if (lookahead == 'a') ADVANCE(189);
+      if (lookahead == 'a') ADVANCE(879);
       END_STATE();
     case 167:
-      if (lookahead == 'a') ADVANCE(880);
+      if (lookahead == 'a') ADVANCE(884);
       END_STATE();
     case 168:
-      if (lookahead == 'a') ADVANCE(885);
+      if (lookahead == 'a') ADVANCE(877);
       END_STATE();
     case 169:
-      if (lookahead == 'a') ADVANCE(878);
+      if (lookahead == 'a') ADVANCE(406);
       END_STATE();
     case 170:
-      if (lookahead == 'a') ADVANCE(407);
+      if (lookahead == 'a') ADVANCE(908);
+      if (lookahead == 'c') ADVANCE(650);
+      if (lookahead == 'd') ADVANCE(168);
+      if (lookahead == 'f') ADVANCE(526);
+      if (lookahead == 'l') ADVANCE(165);
+      if (lookahead == 'n') ADVANCE(895);
+      if (lookahead == 's') ADVANCE(444);
+      if (lookahead == 't') ADVANCE(141);
       END_STATE();
     case 171:
-      if (lookahead == 'a') ADVANCE(909);
-      if (lookahead == 'c') ADVANCE(651);
-      if (lookahead == 'd') ADVANCE(169);
-      if (lookahead == 'f') ADVANCE(527);
-      if (lookahead == 'l') ADVANCE(166);
-      if (lookahead == 'n') ADVANCE(896);
-      if (lookahead == 's') ADVANCE(445);
-      if (lookahead == 't') ADVANCE(142);
+      if (lookahead == 'a') ADVANCE(398);
       END_STATE();
     case 172:
-      if (lookahead == 'a') ADVANCE(399);
+      if (lookahead == 'a') ADVANCE(261);
       END_STATE();
     case 173:
-      if (lookahead == 'a') ADVANCE(262);
+      if (lookahead == 'a') ADVANCE(400);
       END_STATE();
     case 174:
-      if (lookahead == 'a') ADVANCE(401);
+      if (lookahead == 'a') ADVANCE(222);
+      if (lookahead == 'b') ADVANCE(613);
+      if (lookahead == 'e') ADVANCE(845);
+      if (lookahead == 'i') ADVANCE(553);
+      if (lookahead == 'o') ADVANCE(585);
+      if (lookahead == 'y') ADVANCE(104);
       END_STATE();
     case 175:
-      if (lookahead == 'a') ADVANCE(223);
-      if (lookahead == 'b') ADVANCE(614);
-      if (lookahead == 'e') ADVANCE(846);
-      if (lookahead == 'i') ADVANCE(554);
-      if (lookahead == 'o') ADVANCE(586);
-      if (lookahead == 'y') ADVANCE(105);
+      if (lookahead == 'a') ADVANCE(265);
       END_STATE();
     case 176:
-      if (lookahead == 'a') ADVANCE(266);
+      if (lookahead == 'a') ADVANCE(912);
       END_STATE();
     case 177:
-      if (lookahead == 'a') ADVANCE(913);
+      if (lookahead == 'a') ADVANCE(885);
       END_STATE();
     case 178:
-      if (lookahead == 'a') ADVANCE(886);
+      if (lookahead == 'a') ADVANCE(547);
       END_STATE();
     case 179:
-      if (lookahead == 'a') ADVANCE(548);
+      if (lookahead == 'a') ADVANCE(228);
       END_STATE();
     case 180:
-      if (lookahead == 'a') ADVANCE(229);
+      if (lookahead == 'a') ADVANCE(891);
       END_STATE();
     case 181:
-      if (lookahead == 'a') ADVANCE(892);
+      if (lookahead == 'a') ADVANCE(924);
       END_STATE();
     case 182:
-      if (lookahead == 'a') ADVANCE(925);
+      if (lookahead == 'b') ADVANCE(479);
       END_STATE();
     case 183:
       if (lookahead == 'b') ADVANCE(480);
       END_STATE();
     case 184:
-      if (lookahead == 'b') ADVANCE(481);
+      if (lookahead == 'b') ADVANCE(626);
+      if (lookahead == 't') ADVANCE(634);
       END_STATE();
     case 185:
-      if (lookahead == 'b') ADVANCE(627);
-      if (lookahead == 't') ADVANCE(635);
+      if (lookahead == 'b') ADVANCE(164);
+      if (lookahead == 'd') ADVANCE(465);
+      if (lookahead == 'f') ADVANCE(528);
+      if (lookahead == 'h') ADVANCE(452);
+      if (lookahead == 'i') ADVANCE(588);
+      if (lookahead == 'n') ADVANCE(319);
+      if (lookahead == 'o') ADVANCE(782);
+      if (lookahead == 'p') ADVANCE(457);
+      if (lookahead == 's') ADVANCE(737);
+      if (lookahead == 'u') ADVANCE(584);
       END_STATE();
     case 186:
-      if (lookahead == 'b') ADVANCE(165);
-      if (lookahead == 'd') ADVANCE(466);
-      if (lookahead == 'f') ADVANCE(529);
-      if (lookahead == 'h') ADVANCE(453);
-      if (lookahead == 'i') ADVANCE(589);
-      if (lookahead == 'n') ADVANCE(320);
-      if (lookahead == 'o') ADVANCE(783);
-      if (lookahead == 'p') ADVANCE(458);
-      if (lookahead == 's') ADVANCE(738);
-      if (lookahead == 'u') ADVANCE(585);
+      if (lookahead == 'b') ADVANCE(164);
+      if (lookahead == 'd') ADVANCE(465);
+      if (lookahead == 'f') ADVANCE(528);
+      if (lookahead == 'h') ADVANCE(452);
+      if (lookahead == 'i') ADVANCE(588);
+      if (lookahead == 'n') ADVANCE(319);
+      if (lookahead == 'o') ADVANCE(782);
+      if (lookahead == 's') ADVANCE(737);
       END_STATE();
     case 187:
-      if (lookahead == 'b') ADVANCE(165);
-      if (lookahead == 'd') ADVANCE(466);
-      if (lookahead == 'f') ADVANCE(529);
-      if (lookahead == 'h') ADVANCE(453);
-      if (lookahead == 'i') ADVANCE(589);
-      if (lookahead == 'n') ADVANCE(320);
-      if (lookahead == 'o') ADVANCE(783);
-      if (lookahead == 's') ADVANCE(738);
+      if (lookahead == 'b') ADVANCE(297);
       END_STATE();
     case 188:
-      if (lookahead == 'b') ADVANCE(298);
+      if (lookahead == 'b') ADVANCE(334);
       END_STATE();
     case 189:
-      if (lookahead == 'b') ADVANCE(335);
+      if (lookahead == 'b') ADVANCE(663);
+      if (lookahead == 'e') ADVANCE(600);
+      if (lookahead == 'n') ADVANCE(706);
+      if (lookahead == 's') ADVANCE(466);
       END_STATE();
     case 190:
-      if (lookahead == 'b') ADVANCE(664);
-      if (lookahead == 'e') ADVANCE(601);
-      if (lookahead == 'n') ADVANCE(707);
-      if (lookahead == 's') ADVANCE(467);
+      if (lookahead == 'b') ADVANCE(301);
       END_STATE();
     case 191:
-      if (lookahead == 'b') ADVANCE(302);
+      if (lookahead == 'b') ADVANCE(158);
       END_STATE();
     case 192:
-      if (lookahead == 'b') ADVANCE(159);
+      if (lookahead == 'b') ADVANCE(700);
+      if (lookahead == 't') ADVANCE(718);
       END_STATE();
     case 193:
-      if (lookahead == 'b') ADVANCE(701);
-      if (lookahead == 't') ADVANCE(719);
+      if (lookahead == 'b') ADVANCE(704);
       END_STATE();
     case 194:
-      if (lookahead == 'b') ADVANCE(705);
+      if (lookahead == 'b') ADVANCE(161);
       END_STATE();
     case 195:
       if (lookahead == 'b') ADVANCE(162);
       END_STATE();
     case 196:
-      if (lookahead == 'b') ADVANCE(163);
+      if (lookahead == 'b') ADVANCE(352);
       END_STATE();
     case 197:
-      if (lookahead == 'b') ADVANCE(353);
+      if (lookahead == 'b') ADVANCE(481);
       END_STATE();
     case 198:
-      if (lookahead == 'b') ADVANCE(482);
+      if (lookahead == 'c') ADVANCE(211);
+      if (lookahead == 'l') ADVANCE(451);
+      if (lookahead == 'p') ADVANCE(729);
+      if (lookahead == 's') ADVANCE(482);
+      if (lookahead == 't') ADVANCE(861);
+      if (lookahead == 'u') ADVANCE(863);
       END_STATE();
     case 199:
-      if (lookahead == 'c') ADVANCE(212);
-      if (lookahead == 'l') ADVANCE(452);
-      if (lookahead == 'p') ADVANCE(730);
-      if (lookahead == 's') ADVANCE(483);
-      if (lookahead == 't') ADVANCE(862);
-      if (lookahead == 'u') ADVANCE(864);
+      if (lookahead == 'c') ADVANCE(211);
+      if (lookahead == 'l') ADVANCE(451);
+      if (lookahead == 'p') ADVANCE(729);
+      if (lookahead == 't') ADVANCE(892);
+      if (lookahead == 'u') ADVANCE(863);
       END_STATE();
     case 200:
-      if (lookahead == 'c') ADVANCE(212);
-      if (lookahead == 'l') ADVANCE(452);
-      if (lookahead == 'p') ADVANCE(730);
-      if (lookahead == 't') ADVANCE(893);
-      if (lookahead == 'u') ADVANCE(864);
+      if (lookahead == 'c') ADVANCE(1135);
       END_STATE();
     case 201:
-      if (lookahead == 'c') ADVANCE(1136);
+      if (lookahead == 'c') ADVANCE(1018);
       END_STATE();
     case 202:
-      if (lookahead == 'c') ADVANCE(1019);
+      if (lookahead == 'c') ADVANCE(414);
+      if (lookahead == 'd') ADVANCE(463);
+      if (lookahead == 'r') ADVANCE(780);
+      if (lookahead == 'x') ADVANCE(315);
       END_STATE();
     case 203:
-      if (lookahead == 'c') ADVANCE(415);
-      if (lookahead == 'd') ADVANCE(464);
-      if (lookahead == 'r') ADVANCE(781);
-      if (lookahead == 'x') ADVANCE(316);
+      if (lookahead == 'c') ADVANCE(414);
+      if (lookahead == 'x') ADVANCE(315);
       END_STATE();
     case 204:
-      if (lookahead == 'c') ADVANCE(415);
-      if (lookahead == 'x') ADVANCE(316);
+      if (lookahead == 'c') ADVANCE(205);
+      if (lookahead == 'i') ADVANCE(597);
+      if (lookahead == 'o') ADVANCE(518);
       END_STATE();
     case 205:
-      if (lookahead == 'c') ADVANCE(206);
-      if (lookahead == 'i') ADVANCE(598);
-      if (lookahead == 'o') ADVANCE(519);
+      if (lookahead == 'c') ADVANCE(69);
       END_STATE();
     case 206:
-      if (lookahead == 'c') ADVANCE(67);
+      if (lookahead == 'c') ADVANCE(483);
       END_STATE();
     case 207:
-      if (lookahead == 'c') ADVANCE(484);
+      if (lookahead == 'c') ADVANCE(638);
+      if (lookahead == 'f') ADVANCE(256);
+      if (lookahead == 'g') ADVANCE(598);
+      if (lookahead == 'n') ADVANCE(231);
       END_STATE();
     case 208:
-      if (lookahead == 'c') ADVANCE(639);
-      if (lookahead == 'f') ADVANCE(257);
-      if (lookahead == 'g') ADVANCE(599);
-      if (lookahead == 'n') ADVANCE(232);
+      if (lookahead == 'c') ADVANCE(638);
+      if (lookahead == 'f') ADVANCE(256);
+      if (lookahead == 'g') ADVANCE(598);
+      if (lookahead == 'n') ADVANCE(254);
       END_STATE();
     case 209:
-      if (lookahead == 'c') ADVANCE(639);
-      if (lookahead == 'f') ADVANCE(257);
-      if (lookahead == 'g') ADVANCE(599);
-      if (lookahead == 'n') ADVANCE(255);
+      if (lookahead == 'c') ADVANCE(408);
       END_STATE();
     case 210:
-      if (lookahead == 'c') ADVANCE(409);
+      if (lookahead == 'c') ADVANCE(410);
       END_STATE();
     case 211:
-      if (lookahead == 'c') ADVANCE(411);
+      if (lookahead == 'c') ADVANCE(630);
       END_STATE();
     case 212:
-      if (lookahead == 'c') ADVANCE(631);
+      if (lookahead == 'c') ADVANCE(422);
       END_STATE();
     case 213:
-      if (lookahead == 'c') ADVANCE(423);
+      if (lookahead == 'c') ADVANCE(412);
       END_STATE();
     case 214:
-      if (lookahead == 'c') ADVANCE(413);
+      if (lookahead == 'c') ADVANCE(167);
       END_STATE();
     case 215:
-      if (lookahead == 'c') ADVANCE(168);
+      if (lookahead == 'c') ADVANCE(874);
       END_STATE();
     case 216:
-      if (lookahead == 'c') ADVANCE(875);
+      if (lookahead == 'c') ADVANCE(772);
       END_STATE();
     case 217:
-      if (lookahead == 'c') ADVANCE(773);
+      if (lookahead == 'c') ADVANCE(505);
       END_STATE();
     case 218:
-      if (lookahead == 'c') ADVANCE(506);
+      if (lookahead == 'c') ADVANCE(854);
       END_STATE();
     case 219:
-      if (lookahead == 'c') ADVANCE(855);
+      if (lookahead == 'c') ADVANCE(288);
       END_STATE();
     case 220:
-      if (lookahead == 'c') ADVANCE(289);
+      if (lookahead == 'c') ADVANCE(804);
       END_STATE();
     case 221:
-      if (lookahead == 'c') ADVANCE(805);
+      if (lookahead == 'c') ADVANCE(781);
+      if (lookahead == 'g') ADVANCE(330);
+      if (lookahead == 'i') ADVANCE(511);
+      if (lookahead == 'r') ADVANCE(506);
       END_STATE();
     case 222:
-      if (lookahead == 'c') ADVANCE(782);
-      if (lookahead == 'g') ADVANCE(331);
-      if (lookahead == 'i') ADVANCE(512);
-      if (lookahead == 'r') ADVANCE(507);
+      if (lookahead == 'c') ADVANCE(781);
+      if (lookahead == 'i') ADVANCE(511);
       END_STATE();
     case 223:
-      if (lookahead == 'c') ADVANCE(782);
-      if (lookahead == 'i') ADVANCE(512);
+      if (lookahead == 'c') ADVANCE(875);
       END_STATE();
     case 224:
-      if (lookahead == 'c') ADVANCE(876);
+      if (lookahead == 'c') ADVANCE(796);
       END_STATE();
     case 225:
-      if (lookahead == 'c') ADVANCE(797);
+      if (lookahead == 'c') ADVANCE(708);
+      if (lookahead == 'e') ADVANCE(849);
+      if (lookahead == 'u') ADVANCE(197);
       END_STATE();
     case 226:
-      if (lookahead == 'c') ADVANCE(709);
-      if (lookahead == 'e') ADVANCE(850);
-      if (lookahead == 'u') ADVANCE(198);
+      if (lookahead == 'c') ADVANCE(786);
+      if (lookahead == 'i') ADVANCE(544);
       END_STATE();
     case 227:
-      if (lookahead == 'c') ADVANCE(787);
-      if (lookahead == 'i') ADVANCE(545);
+      if (lookahead == 'c') ADVANCE(177);
       END_STATE();
     case 228:
-      if (lookahead == 'c') ADVANCE(178);
+      if (lookahead == 'c') ADVANCE(442);
       END_STATE();
     case 229:
-      if (lookahead == 'c') ADVANCE(443);
+      if (lookahead == 'd') ADVANCE(1164);
+      if (lookahead == 'h') ADVANCE(137);
+      if (lookahead == 'l') ADVANCE(629);
+      if (lookahead == 'o') ADVANCE(522);
+      if (lookahead == 'r') ADVANCE(948);
+      if (lookahead == 'y') ADVANCE(143);
       END_STATE();
     case 230:
-      if (lookahead == 'd') ADVANCE(1165);
-      if (lookahead == 'h') ADVANCE(138);
-      if (lookahead == 'l') ADVANCE(630);
-      if (lookahead == 'o') ADVANCE(523);
-      if (lookahead == 'r') ADVANCE(949);
-      if (lookahead == 'y') ADVANCE(144);
+      if (lookahead == 'd') ADVANCE(1164);
+      if (lookahead == 'h') ADVANCE(137);
+      if (lookahead == 'l') ADVANCE(629);
+      if (lookahead == 'o') ADVANCE(540);
+      if (lookahead == 'r') ADVANCE(948);
       END_STATE();
     case 231:
-      if (lookahead == 'd') ADVANCE(1165);
-      if (lookahead == 'h') ADVANCE(138);
-      if (lookahead == 'l') ADVANCE(630);
-      if (lookahead == 'o') ADVANCE(541);
-      if (lookahead == 'r') ADVANCE(949);
+      if (lookahead == 'd') ADVANCE(310);
       END_STATE();
     case 232:
-      if (lookahead == 'd') ADVANCE(311);
+      if (lookahead == 'd') ADVANCE(1116);
       END_STATE();
     case 233:
-      if (lookahead == 'd') ADVANCE(1117);
+      if (lookahead == 'd') ADVANCE(1116);
+      if (lookahead == 'p') ADVANCE(515);
+      if (lookahead == 's') ADVANCE(323);
+      if (lookahead == 'v') ADVANCE(367);
       END_STATE();
     case 234:
-      if (lookahead == 'd') ADVANCE(1117);
-      if (lookahead == 'p') ADVANCE(516);
-      if (lookahead == 's') ADVANCE(324);
-      if (lookahead == 'v') ADVANCE(368);
+      if (lookahead == 'd') ADVANCE(1116);
+      if (lookahead == 'v') ADVANCE(367);
       END_STATE();
     case 235:
-      if (lookahead == 'd') ADVANCE(1117);
-      if (lookahead == 'v') ADVANCE(368);
+      if (lookahead == 'd') ADVANCE(1029);
       END_STATE();
     case 236:
-      if (lookahead == 'd') ADVANCE(1030);
+      if (lookahead == 'd') ADVANCE(1039);
       END_STATE();
     case 237:
-      if (lookahead == 'd') ADVANCE(1040);
+      if (lookahead == 'd') ADVANCE(76);
       END_STATE();
     case 238:
-      if (lookahead == 'd') ADVANCE(74);
+      if (lookahead == 'd') ADVANCE(1081);
       END_STATE();
     case 239:
-      if (lookahead == 'd') ADVANCE(1082);
+      if (lookahead == 'd') ADVANCE(1030);
       END_STATE();
     case 240:
-      if (lookahead == 'd') ADVANCE(1031);
+      if (lookahead == 'd') ADVANCE(1049);
       END_STATE();
     case 241:
-      if (lookahead == 'd') ADVANCE(1050);
+      if (lookahead == 'd') ADVANCE(1098);
       END_STATE();
     case 242:
-      if (lookahead == 'd') ADVANCE(1099);
+      if (lookahead == 'd') ADVANCE(1094);
       END_STATE();
     case 243:
-      if (lookahead == 'd') ADVANCE(1095);
+      if (lookahead == 'd') ADVANCE(463);
       END_STATE();
     case 244:
-      if (lookahead == 'd') ADVANCE(464);
+      if (lookahead == 'd') ADVANCE(945);
+      if (lookahead == 'l') ADVANCE(236);
       END_STATE();
     case 245:
-      if (lookahead == 'd') ADVANCE(946);
-      if (lookahead == 'l') ADVANCE(237);
+      if (lookahead == 'd') ADVANCE(742);
+      if (lookahead == 'e') ADVANCE(175);
       END_STATE();
     case 246:
-      if (lookahead == 'd') ADVANCE(743);
-      if (lookahead == 'e') ADVANCE(176);
+      if (lookahead == 'd') ADVANCE(73);
       END_STATE();
     case 247:
-      if (lookahead == 'd') ADVANCE(71);
+      if (lookahead == 'd') ADVANCE(765);
+      if (lookahead == 'o') ADVANCE(628);
       END_STATE();
     case 248:
-      if (lookahead == 'd') ADVANCE(766);
-      if (lookahead == 'o') ADVANCE(629);
+      if (lookahead == 'd') ADVANCE(309);
+      if (lookahead == 'g') ADVANCE(586);
       END_STATE();
     case 249:
-      if (lookahead == 'd') ADVANCE(310);
-      if (lookahead == 'g') ADVANCE(587);
+      if (lookahead == 'd') ADVANCE(748);
       END_STATE();
     case 250:
-      if (lookahead == 'd') ADVANCE(749);
+      if (lookahead == 'd') ADVANCE(285);
       END_STATE();
     case 251:
-      if (lookahead == 'd') ADVANCE(286);
+      if (lookahead == 'd') ADVANCE(751);
       END_STATE();
     case 252:
-      if (lookahead == 'd') ADVANCE(752);
+      if (lookahead == 'd') ADVANCE(762);
       END_STATE();
     case 253:
-      if (lookahead == 'd') ADVANCE(763);
+      if (lookahead == 'd') ADVANCE(795);
+      if (lookahead == 'e') ADVANCE(175);
       END_STATE();
     case 254:
-      if (lookahead == 'd') ADVANCE(796);
-      if (lookahead == 'e') ADVANCE(176);
+      if (lookahead == 'd') ADVANCE(356);
       END_STATE();
     case 255:
-      if (lookahead == 'd') ADVANCE(357);
+      if (lookahead == 'd') ADVANCE(325);
       END_STATE();
     case 256:
-      if (lookahead == 'd') ADVANCE(326);
+      if (lookahead == 'd') ADVANCE(308);
+      if (lookahead == 'n') ADVANCE(259);
       END_STATE();
     case 257:
-      if (lookahead == 'd') ADVANCE(309);
-      if (lookahead == 'n') ADVANCE(260);
+      if (lookahead == 'd') ADVANCE(478);
       END_STATE();
     case 258:
-      if (lookahead == 'd') ADVANCE(479);
+      if (lookahead == 'd') ADVANCE(458);
       END_STATE();
     case 259:
-      if (lookahead == 'd') ADVANCE(459);
+      if (lookahead == 'd') ADVANCE(311);
       END_STATE();
     case 260:
-      if (lookahead == 'd') ADVANCE(312);
+      if (lookahead == 'd') ADVANCE(625);
       END_STATE();
     case 261:
-      if (lookahead == 'd') ADVANCE(626);
+      if (lookahead == 'd') ADVANCE(363);
       END_STATE();
     case 262:
-      if (lookahead == 'd') ADVANCE(364);
+      if (lookahead == 'd') ADVANCE(333);
       END_STATE();
     case 263:
-      if (lookahead == 'd') ADVANCE(334);
+      if (lookahead == 'd') ADVANCE(252);
       END_STATE();
     case 264:
-      if (lookahead == 'd') ADVANCE(253);
+      if (lookahead == 'd') ADVANCE(338);
       END_STATE();
     case 265:
-      if (lookahead == 'd') ADVANCE(339);
+      if (lookahead == 'd') ADVANCE(344);
       END_STATE();
     case 266:
-      if (lookahead == 'd') ADVANCE(345);
+      if (lookahead == 'd') ADVANCE(350);
       END_STATE();
     case 267:
       if (lookahead == 'd') ADVANCE(351);
       END_STATE();
     case 268:
-      if (lookahead == 'd') ADVANCE(352);
+      if (lookahead == 'd') ADVANCE(353);
       END_STATE();
     case 269:
       if (lookahead == 'd') ADVANCE(354);
       END_STATE();
     case 270:
       if (lookahead == 'd') ADVANCE(355);
       END_STATE();
     case 271:
-      if (lookahead == 'd') ADVANCE(356);
+      if (lookahead == 'd') ADVANCE(365);
       END_STATE();
     case 272:
-      if (lookahead == 'd') ADVANCE(366);
+      if (lookahead == 'd') ADVANCE(703);
       END_STATE();
     case 273:
-      if (lookahead == 'd') ADVANCE(704);
+      if (lookahead == 'd') ADVANCE(372);
+      if (lookahead == 'g') ADVANCE(586);
       END_STATE();
     case 274:
-      if (lookahead == 'd') ADVANCE(373);
-      if (lookahead == 'g') ADVANCE(587);
+      if (lookahead == 'd') ADVANCE(82);
       END_STATE();
     case 275:
-      if (lookahead == 'd') ADVANCE(80);
+      if (lookahead == 'd') ADVANCE(373);
       END_STATE();
     case 276:
-      if (lookahead == 'd') ADVANCE(374);
+      if (lookahead == 'd') ADVANCE(811);
       END_STATE();
     case 277:
-      if (lookahead == 'd') ADVANCE(812);
+      if (lookahead == 'e') ADVANCE(384);
       END_STATE();
     case 278:
-      if (lookahead == 'e') ADVANCE(385);
+      if (lookahead == 'e') ADVANCE(233);
       END_STATE();
     case 279:
-      if (lookahead == 'e') ADVANCE(234);
+      if (lookahead == 'e') ADVANCE(517);
       END_STATE();
     case 280:
-      if (lookahead == 'e') ADVANCE(518);
+      if (lookahead == 'e') ADVANCE(1119);
       END_STATE();
     case 281:
-      if (lookahead == 'e') ADVANCE(1120);
+      if (lookahead == 'e') ADVANCE(1125);
       END_STATE();
     case 282:
-      if (lookahead == 'e') ADVANCE(1126);
+      if (lookahead == 'e') ADVANCE(1090);
       END_STATE();
     case 283:
-      if (lookahead == 'e') ADVANCE(1091);
+      if (lookahead == 'e') ADVANCE(1203);
       END_STATE();
     case 284:
-      if (lookahead == 'e') ADVANCE(1204);
+      if (lookahead == 'e') ADVANCE(1027);
       END_STATE();
     case 285:
-      if (lookahead == 'e') ADVANCE(1028);
+      if (lookahead == 'e') ADVANCE(1088);
       END_STATE();
     case 286:
-      if (lookahead == 'e') ADVANCE(1089);
+      if (lookahead == 'e') ADVANCE(1122);
       END_STATE();
     case 287:
-      if (lookahead == 'e') ADVANCE(1123);
+      if (lookahead == 'e') ADVANCE(1150);
       END_STATE();
     case 288:
-      if (lookahead == 'e') ADVANCE(1151);
+      if (lookahead == 'e') ADVANCE(1522);
       END_STATE();
     case 289:
-      if (lookahead == 'e') ADVANCE(1529);
+      if (lookahead == 'e') ADVANCE(1197);
       END_STATE();
     case 290:
-      if (lookahead == 'e') ADVANCE(1198);
+      if (lookahead == 'e') ADVANCE(1016);
       END_STATE();
     case 291:
-      if (lookahead == 'e') ADVANCE(1017);
+      if (lookahead == 'e') ADVANCE(1072);
       END_STATE();
     case 292:
-      if (lookahead == 'e') ADVANCE(1073);
+      if (lookahead == 'e') ADVANCE(1126);
       END_STATE();
     case 293:
-      if (lookahead == 'e') ADVANCE(1127);
+      if (lookahead == 'e') ADVANCE(1204);
       END_STATE();
     case 294:
-      if (lookahead == 'e') ADVANCE(1205);
+      if (lookahead == 'e') ADVANCE(1025);
       END_STATE();
     case 295:
-      if (lookahead == 'e') ADVANCE(1026);
+      if (lookahead == 'e') ADVANCE(1151);
       END_STATE();
     case 296:
-      if (lookahead == 'e') ADVANCE(1152);
+      if (lookahead == 'e') ADVANCE(1084);
       END_STATE();
     case 297:
-      if (lookahead == 'e') ADVANCE(1085);
+      if (lookahead == 'e') ADVANCE(1154);
       END_STATE();
     case 298:
-      if (lookahead == 'e') ADVANCE(1155);
+      if (lookahead == 'e') ADVANCE(1092);
       END_STATE();
     case 299:
-      if (lookahead == 'e') ADVANCE(1093);
+      if (lookahead == 'e') ADVANCE(1051);
       END_STATE();
     case 300:
-      if (lookahead == 'e') ADVANCE(1052);
+      if (lookahead == 'e') ADVANCE(1059);
       END_STATE();
     case 301:
-      if (lookahead == 'e') ADVANCE(1060);
+      if (lookahead == 'e') ADVANCE(1155);
       END_STATE();
     case 302:
-      if (lookahead == 'e') ADVANCE(1156);
+      if (lookahead == 'e') ADVANCE(1113);
       END_STATE();
     case 303:
-      if (lookahead == 'e') ADVANCE(1114);
+      if (lookahead == 'e') ADVANCE(1108);
       END_STATE();
     case 304:
-      if (lookahead == 'e') ADVANCE(1109);
+      if (lookahead == 'e') ADVANCE(725);
       END_STATE();
     case 305:
       if (lookahead == 'e') ADVANCE(726);
       END_STATE();
     case 306:
-      if (lookahead == 'e') ADVANCE(727);
+      if (lookahead == 'e') ADVANCE(234);
       END_STATE();
     case 307:
-      if (lookahead == 'e') ADVANCE(235);
+      if (lookahead == 'e') ADVANCE(1071);
       END_STATE();
     case 308:
-      if (lookahead == 'e') ADVANCE(1072);
+      if (lookahead == 'e') ADVANCE(382);
       END_STATE();
     case 309:
-      if (lookahead == 'e') ADVANCE(383);
+      if (lookahead == 'e') ADVANCE(191);
       END_STATE();
     case 310:
-      if (lookahead == 'e') ADVANCE(192);
+      if (lookahead == 'e') ADVANCE(935);
+      if (lookahead == 'i') ADVANCE(214);
       END_STATE();
     case 311:
-      if (lookahead == 'e') ADVANCE(936);
-      if (lookahead == 'i') ADVANCE(215);
+      if (lookahead == 'e') ADVANCE(383);
       END_STATE();
     case 312:
-      if (lookahead == 'e') ADVANCE(384);
+      if (lookahead == 'e') ADVANCE(109);
       END_STATE();
     case 313:
-      if (lookahead == 'e') ADVANCE(110);
+      if (lookahead == 'e') ADVANCE(599);
       END_STATE();
     case 314:
-      if (lookahead == 'e') ADVANCE(600);
+      if (lookahead == 'e') ADVANCE(599);
+      if (lookahead == 'r') ADVANCE(361);
       END_STATE();
     case 315:
-      if (lookahead == 'e') ADVANCE(600);
-      if (lookahead == 'r') ADVANCE(362);
+      if (lookahead == 'e') ADVANCE(200);
       END_STATE();
     case 316:
-      if (lookahead == 'e') ADVANCE(201);
+      if (lookahead == 'e') ADVANCE(764);
       END_STATE();
     case 317:
-      if (lookahead == 'e') ADVANCE(765);
+      if (lookahead == 'e') ADVANCE(764);
+      if (lookahead == 'o') ADVANCE(870);
       END_STATE();
     case 318:
-      if (lookahead == 'e') ADVANCE(765);
-      if (lookahead == 'o') ADVANCE(871);
+      if (lookahead == 'e') ADVANCE(927);
       END_STATE();
     case 319:
       if (lookahead == 'e') ADVANCE(928);
       END_STATE();
     case 320:
       if (lookahead == 'e') ADVANCE(929);
       END_STATE();
     case 321:
-      if (lookahead == 'e') ADVANCE(930);
+      if (lookahead == 'e') ADVANCE(797);
       END_STATE();
     case 322:
-      if (lookahead == 'e') ADVANCE(798);
+      if (lookahead == 'e') ADVANCE(609);
       END_STATE();
     case 323:
-      if (lookahead == 'e') ADVANCE(610);
+      if (lookahead == 'e') ADVANCE(848);
       END_STATE();
     case 324:
-      if (lookahead == 'e') ADVANCE(849);
+      if (lookahead == 'e') ADVANCE(246);
       END_STATE();
     case 325:
-      if (lookahead == 'e') ADVANCE(247);
+      if (lookahead == 'e') ADVANCE(939);
       END_STATE();
     case 326:
-      if (lookahead == 'e') ADVANCE(940);
+      if (lookahead == 'e') ADVANCE(815);
       END_STATE();
     case 327:
-      if (lookahead == 'e') ADVANCE(816);
+      if (lookahead == 'e') ADVANCE(568);
       END_STATE();
     case 328:
-      if (lookahead == 'e') ADVANCE(569);
+      if (lookahead == 'e') ADVANCE(215);
       END_STATE();
     case 329:
-      if (lookahead == 'e') ADVANCE(216);
+      if (lookahead == 'e') ADVANCE(767);
       END_STATE();
     case 330:
-      if (lookahead == 'e') ADVANCE(768);
+      if (lookahead == 'e') ADVANCE(602);
       END_STATE();
     case 331:
-      if (lookahead == 'e') ADVANCE(603);
+      if (lookahead == 'e') ADVANCE(745);
       END_STATE();
     case 332:
-      if (lookahead == 'e') ADVANCE(746);
+      if (lookahead == 'e') ADVANCE(238);
       END_STATE();
     case 333:
-      if (lookahead == 'e') ADVANCE(239);
+      if (lookahead == 'e') ADVANCE(776);
       END_STATE();
     case 334:
-      if (lookahead == 'e') ADVANCE(777);
+      if (lookahead == 'e') ADVANCE(513);
       END_STATE();
     case 335:
-      if (lookahead == 'e') ADVANCE(514);
+      if (lookahead == 'e') ADVANCE(820);
       END_STATE();
     case 336:
       if (lookahead == 'e') ADVANCE(821);
+      if (lookahead == 'i') ADVANCE(921);
       END_STATE();
     case 337:
-      if (lookahead == 'e') ADVANCE(822);
-      if (lookahead == 'i') ADVANCE(922);
+      if (lookahead == 'e') ADVANCE(699);
       END_STATE();
     case 338:
-      if (lookahead == 'e') ADVANCE(700);
+      if (lookahead == 'e') ADVANCE(810);
       END_STATE();
     case 339:
-      if (lookahead == 'e') ADVANCE(811);
+      if (lookahead == 'e') ADVANCE(240);
       END_STATE();
     case 340:
       if (lookahead == 'e') ADVANCE(241);
       END_STATE();
     case 341:
-      if (lookahead == 'e') ADVANCE(242);
+      if (lookahead == 'e') ADVANCE(823);
       END_STATE();
     case 342:
-      if (lookahead == 'e') ADVANCE(824);
+      if (lookahead == 'e') ADVANCE(282);
       END_STATE();
     case 343:
-      if (lookahead == 'e') ADVANCE(283);
+      if (lookahead == 'e') ADVANCE(604);
       END_STATE();
     case 344:
-      if (lookahead == 'e') ADVANCE(605);
+      if (lookahead == 'e') ADVANCE(747);
       END_STATE();
     case 345:
-      if (lookahead == 'e') ADVANCE(748);
+      if (lookahead == 'e') ADVANCE(824);
+      if (lookahead == 'i') ADVANCE(925);
       END_STATE();
     case 346:
-      if (lookahead == 'e') ADVANCE(825);
-      if (lookahead == 'i') ADVANCE(926);
+      if (lookahead == 'e') ADVANCE(826);
       END_STATE();
     case 347:
-      if (lookahead == 'e') ADVANCE(827);
+      if (lookahead == 'e') ADVANCE(749);
       END_STATE();
     case 348:
-      if (lookahead == 'e') ADVANCE(750);
+      if (lookahead == 'e') ADVANCE(232);
       END_STATE();
     case 349:
-      if (lookahead == 'e') ADVANCE(233);
+      if (lookahead == 'e') ADVANCE(593);
       END_STATE();
     case 350:
-      if (lookahead == 'e') ADVANCE(594);
+      if (lookahead == 'e') ADVANCE(752);
       END_STATE();
     case 351:
-      if (lookahead == 'e') ADVANCE(753);
+      if (lookahead == 'e') ADVANCE(754);
       END_STATE();
     case 352:
-      if (lookahead == 'e') ADVANCE(755);
+      if (lookahead == 'e') ADVANCE(756);
       END_STATE();
     case 353:
       if (lookahead == 'e') ADVANCE(757);
       END_STATE();
     case 354:
       if (lookahead == 'e') ADVANCE(758);
       END_STATE();
     case 355:
-      if (lookahead == 'e') ADVANCE(759);
+      if (lookahead == 'e') ADVANCE(760);
       END_STATE();
     case 356:
-      if (lookahead == 'e') ADVANCE(761);
+      if (lookahead == 'e') ADVANCE(941);
       END_STATE();
     case 357:
-      if (lookahead == 'e') ADVANCE(942);
+      if (lookahead == 'e') ADVANCE(581);
       END_STATE();
     case 358:
-      if (lookahead == 'e') ADVANCE(582);
+      if (lookahead == 'e') ADVANCE(836);
       END_STATE();
     case 359:
-      if (lookahead == 'e') ADVANCE(837);
+      if (lookahead == 'e') ADVANCE(778);
       END_STATE();
     case 360:
-      if (lookahead == 'e') ADVANCE(779);
+      if (lookahead == 'e') ADVANCE(327);
       END_STATE();
     case 361:
-      if (lookahead == 'e') ADVANCE(328);
+      if (lookahead == 'e') ADVANCE(327);
+      if (lookahead == 'o') ADVANCE(896);
       END_STATE();
     case 362:
-      if (lookahead == 'e') ADVANCE(328);
-      if (lookahead == 'o') ADVANCE(897);
+      if (lookahead == 'e') ADVANCE(218);
       END_STATE();
     case 363:
-      if (lookahead == 'e') ADVANCE(219);
+      if (lookahead == 'e') ADVANCE(785);
       END_STATE();
     case 364:
-      if (lookahead == 'e') ADVANCE(786);
+      if (lookahead == 'e') ADVANCE(144);
+      if (lookahead == 'i') ADVANCE(273);
+      if (lookahead == 't') ADVANCE(135);
       END_STATE();
     case 365:
-      if (lookahead == 'e') ADVANCE(145);
-      if (lookahead == 'i') ADVANCE(274);
-      if (lookahead == 't') ADVANCE(136);
+      if (lookahead == 'e') ADVANCE(194);
       END_STATE();
     case 366:
-      if (lookahead == 'e') ADVANCE(195);
+      if (lookahead == 'e') ADVANCE(172);
       END_STATE();
     case 367:
-      if (lookahead == 'e') ADVANCE(173);
+      if (lookahead == 'e') ADVANCE(803);
       END_STATE();
     case 368:
-      if (lookahead == 'e') ADVANCE(804);
+      if (lookahead == 'e') ADVANCE(802);
       END_STATE();
     case 369:
-      if (lookahead == 'e') ADVANCE(803);
+      if (lookahead == 'e') ADVANCE(223);
       END_STATE();
     case 370:
-      if (lookahead == 'e') ADVANCE(224);
+      if (lookahead == 'e') ADVANCE(516);
       END_STATE();
     case 371:
-      if (lookahead == 'e') ADVANCE(517);
+      if (lookahead == 'e') ADVANCE(605);
       END_STATE();
     case 372:
-      if (lookahead == 'e') ADVANCE(606);
+      if (lookahead == 'e') ADVANCE(195);
       END_STATE();
     case 373:
-      if (lookahead == 'e') ADVANCE(196);
+      if (lookahead == 'e') ADVANCE(388);
       END_STATE();
     case 374:
-      if (lookahead == 'e') ADVANCE(389);
+      if (lookahead == 'e') ADVANCE(75);
       END_STATE();
     case 375:
-      if (lookahead == 'e') ADVANCE(73);
+      if (lookahead == 'e') ADVANCE(77);
       END_STATE();
     case 376:
-      if (lookahead == 'e') ADVANCE(75);
+      if (lookahead == 'e') ADVANCE(89);
       END_STATE();
     case 377:
-      if (lookahead == 'e') ADVANCE(87);
+      if (lookahead == 'e') ADVANCE(86);
       END_STATE();
     case 378:
-      if (lookahead == 'e') ADVANCE(84);
+      if (lookahead == 'e') ADVANCE(115);
       END_STATE();
     case 379:
-      if (lookahead == 'e') ADVANCE(116);
+      if (lookahead == 'e') ADVANCE(117);
       END_STATE();
     case 380:
       if (lookahead == 'e') ADVANCE(118);
       END_STATE();
     case 381:
-      if (lookahead == 'e') ADVANCE(119);
+      if (lookahead == 'e') ADVANCE(889);
       END_STATE();
     case 382:
-      if (lookahead == 'e') ADVANCE(890);
+      if (lookahead == 'f') ADVANCE(1147);
       END_STATE();
     case 383:
       if (lookahead == 'f') ADVANCE(1148);
       END_STATE();
     case 384:
-      if (lookahead == 'f') ADVANCE(1149);
+      if (lookahead == 'f') ADVANCE(142);
       END_STATE();
     case 385:
-      if (lookahead == 'f') ADVANCE(143);
+      if (lookahead == 'f') ADVANCE(468);
       END_STATE();
     case 386:
-      if (lookahead == 'f') ADVANCE(469);
+      if (lookahead == 'f') ADVANCE(793);
       END_STATE();
     case 387:
-      if (lookahead == 'f') ADVANCE(794);
+      if (lookahead == 'f') ADVANCE(690);
       END_STATE();
     case 388:
-      if (lookahead == 'f') ADVANCE(691);
+      if (lookahead == 'f') ADVANCE(176);
       END_STATE();
     case 389:
-      if (lookahead == 'f') ADVANCE(177);
+      if (lookahead == 'g') ADVANCE(1064);
       END_STATE();
     case 390:
-      if (lookahead == 'g') ADVANCE(1065);
+      if (lookahead == 'g') ADVANCE(391);
       END_STATE();
     case 391:
-      if (lookahead == 'g') ADVANCE(392);
+      if (lookahead == 'g') ADVANCE(529);
       END_STATE();
     case 392:
-      if (lookahead == 'g') ADVANCE(530);
+      if (lookahead == 'g') ADVANCE(415);
       END_STATE();
     case 393:
-      if (lookahead == 'g') ADVANCE(416);
+      if (lookahead == 'g') ADVANCE(417);
       END_STATE();
     case 394:
-      if (lookahead == 'g') ADVANCE(418);
+      if (lookahead == 'g') ADVANCE(822);
       END_STATE();
     case 395:
-      if (lookahead == 'g') ADVANCE(823);
+      if (lookahead == 'g') ADVANCE(570);
       END_STATE();
     case 396:
-      if (lookahead == 'g') ADVANCE(571);
+      if (lookahead == 'g') ADVANCE(291);
       END_STATE();
     case 397:
-      if (lookahead == 'g') ADVANCE(292);
+      if (lookahead == 'g') ADVANCE(340);
       END_STATE();
     case 398:
-      if (lookahead == 'g') ADVANCE(341);
+      if (lookahead == 'g') ADVANCE(307);
       END_STATE();
     case 399:
-      if (lookahead == 'g') ADVANCE(308);
+      if (lookahead == 'g') ADVANCE(397);
       END_STATE();
     case 400:
-      if (lookahead == 'g') ADVANCE(398);
+      if (lookahead == 'g') ADVANCE(330);
       END_STATE();
     case 401:
-      if (lookahead == 'g') ADVANCE(331);
+      if (lookahead == 'g') ADVANCE(330);
+      if (lookahead == 'r') ADVANCE(506);
       END_STATE();
     case 402:
-      if (lookahead == 'g') ADVANCE(331);
-      if (lookahead == 'r') ADVANCE(507);
+      if (lookahead == 'g') ADVANCE(788);
+      if (lookahead == 'm') ADVANCE(730);
       END_STATE();
     case 403:
-      if (lookahead == 'g') ADVANCE(789);
-      if (lookahead == 'm') ADVANCE(731);
+      if (lookahead == 'g') ADVANCE(331);
       END_STATE();
     case 404:
-      if (lookahead == 'g') ADVANCE(332);
+      if (lookahead == 'g') ADVANCE(792);
       END_STATE();
     case 405:
-      if (lookahead == 'g') ADVANCE(793);
+      if (lookahead == 'g') ADVANCE(607);
       END_STATE();
     case 406:
-      if (lookahead == 'g') ADVANCE(608);
+      if (lookahead == 'g') ADVANCE(377);
       END_STATE();
     case 407:
-      if (lookahead == 'g') ADVANCE(378);
+      if (lookahead == 'h') ADVANCE(1176);
       END_STATE();
     case 408:
-      if (lookahead == 'h') ADVANCE(1177);
+      if (lookahead == 'h') ADVANCE(1014);
       END_STATE();
     case 409:
-      if (lookahead == 'h') ADVANCE(1015);
+      if (lookahead == 'h') ADVANCE(1149);
       END_STATE();
     case 410:
-      if (lookahead == 'h') ADVANCE(1150);
+      if (lookahead == 'h') ADVANCE(1082);
       END_STATE();
     case 411:
-      if (lookahead == 'h') ADVANCE(1083);
+      if (lookahead == 'h') ADVANCE(1112);
       END_STATE();
     case 412:
-      if (lookahead == 'h') ADVANCE(1113);
+      if (lookahead == 'h') ADVANCE(107);
       END_STATE();
     case 413:
-      if (lookahead == 'h') ADVANCE(108);
+      if (lookahead == 'h') ADVANCE(249);
       END_STATE();
     case 414:
-      if (lookahead == 'h') ADVANCE(250);
+      if (lookahead == 'h') ADVANCE(615);
       END_STATE();
     case 415:
-      if (lookahead == 'h') ADVANCE(616);
+      if (lookahead == 'h') ADVANCE(535);
       END_STATE();
     case 416:
-      if (lookahead == 'h') ADVANCE(536);
+      if (lookahead == 'h') ADVANCE(668);
+      if (lookahead == 's') ADVANCE(181);
       END_STATE();
     case 417:
-      if (lookahead == 'h') ADVANCE(669);
-      if (lookahead == 's') ADVANCE(182);
+      if (lookahead == 'h') ADVANCE(856);
       END_STATE();
     case 418:
-      if (lookahead == 'h') ADVANCE(857);
+      if (lookahead == 'h') ADVANCE(366);
       END_STATE();
     case 419:
-      if (lookahead == 'h') ADVANCE(367);
+      if (lookahead == 'h') ADVANCE(467);
       END_STATE();
     case 420:
-      if (lookahead == 'h') ADVANCE(468);
+      if (lookahead == 'h') ADVANCE(251);
       END_STATE();
     case 421:
-      if (lookahead == 'h') ADVANCE(252);
+      if (lookahead == 'h') ADVANCE(671);
       END_STATE();
     case 422:
-      if (lookahead == 'h') ADVANCE(672);
+      if (lookahead == 'h') ADVANCE(562);
       END_STATE();
     case 423:
-      if (lookahead == 'h') ADVANCE(563);
+      if (lookahead == 'h') ADVANCE(674);
       END_STATE();
     case 424:
-      if (lookahead == 'h') ADVANCE(675);
+      if (lookahead == 'h') ADVANCE(677);
       END_STATE();
     case 425:
-      if (lookahead == 'h') ADVANCE(678);
+      if (lookahead == 'h') ADVANCE(675);
       END_STATE();
     case 426:
       if (lookahead == 'h') ADVANCE(676);
       END_STATE();
     case 427:
-      if (lookahead == 'h') ADVANCE(677);
+      if (lookahead == 'h') ADVANCE(678);
       END_STATE();
     case 428:
       if (lookahead == 'h') ADVANCE(679);
       END_STATE();
     case 429:
       if (lookahead == 'h') ADVANCE(680);
       END_STATE();
@@ -4979,5870 +4960,5865 @@
     case 431:
       if (lookahead == 'h') ADVANCE(682);
       END_STATE();
     case 432:
       if (lookahead == 'h') ADVANCE(683);
       END_STATE();
     case 433:
-      if (lookahead == 'h') ADVANCE(684);
+      if (lookahead == 'h') ADVANCE(685);
       END_STATE();
     case 434:
       if (lookahead == 'h') ADVANCE(686);
       END_STATE();
     case 435:
       if (lookahead == 'h') ADVANCE(687);
       END_STATE();
     case 436:
-      if (lookahead == 'h') ADVANCE(688);
+      if (lookahead == 'h') ADVANCE(689);
       END_STATE();
     case 437:
-      if (lookahead == 'h') ADVANCE(690);
+      if (lookahead == 'h') ADVANCE(691);
       END_STATE();
     case 438:
       if (lookahead == 'h') ADVANCE(692);
       END_STATE();
     case 439:
       if (lookahead == 'h') ADVANCE(693);
       END_STATE();
     case 440:
       if (lookahead == 'h') ADVANCE(694);
       END_STATE();
     case 441:
-      if (lookahead == 'h') ADVANCE(695);
+      if (lookahead == 'h') ADVANCE(697);
       END_STATE();
     case 442:
-      if (lookahead == 'h') ADVANCE(698);
+      if (lookahead == 'h') ADVANCE(563);
       END_STATE();
     case 443:
-      if (lookahead == 'h') ADVANCE(564);
+      if (lookahead == 'i') ADVANCE(829);
       END_STATE();
     case 444:
-      if (lookahead == 'i') ADVANCE(830);
+      if (lookahead == 'i') ADVANCE(952);
+      if (lookahead == 'u') ADVANCE(183);
       END_STATE();
     case 445:
-      if (lookahead == 'i') ADVANCE(953);
-      if (lookahead == 'u') ADVANCE(184);
+      if (lookahead == 'i') ADVANCE(573);
       END_STATE();
     case 446:
-      if (lookahead == 'i') ADVANCE(574);
+      if (lookahead == 'i') ADVANCE(573);
+      if (lookahead == 'l') ADVANCE(136);
+      if (lookahead == 'o') ADVANCE(244);
+      if (lookahead == 'r') ADVANCE(612);
       END_STATE();
     case 447:
-      if (lookahead == 'i') ADVANCE(574);
-      if (lookahead == 'l') ADVANCE(137);
-      if (lookahead == 'o') ADVANCE(245);
-      if (lookahead == 'r') ADVANCE(613);
+      if (lookahead == 'i') ADVANCE(573);
+      if (lookahead == 'o') ADVANCE(514);
       END_STATE();
     case 448:
-      if (lookahead == 'i') ADVANCE(574);
-      if (lookahead == 'o') ADVANCE(515);
+      if (lookahead == 'i') ADVANCE(533);
+      if (lookahead == 'o') ADVANCE(390);
+      if (lookahead == 'r') ADVANCE(342);
       END_STATE();
     case 449:
-      if (lookahead == 'i') ADVANCE(534);
-      if (lookahead == 'o') ADVANCE(391);
-      if (lookahead == 'r') ADVANCE(343);
+      if (lookahead == 'i') ADVANCE(187);
       END_STATE();
     case 450:
-      if (lookahead == 'i') ADVANCE(188);
+      if (lookahead == 'i') ADVANCE(146);
       END_STATE();
     case 451:
-      if (lookahead == 'i') ADVANCE(147);
+      if (lookahead == 'i') ADVANCE(146);
+      if (lookahead == 't') ADVANCE(321);
       END_STATE();
     case 452:
-      if (lookahead == 'i') ADVANCE(147);
-      if (lookahead == 't') ADVANCE(322);
+      if (lookahead == 'i') ADVANCE(392);
       END_STATE();
     case 453:
-      if (lookahead == 'i') ADVANCE(393);
+      if (lookahead == 'i') ADVANCE(934);
       END_STATE();
     case 454:
-      if (lookahead == 'i') ADVANCE(935);
+      if (lookahead == 'i') ADVANCE(201);
       END_STATE();
     case 455:
-      if (lookahead == 'i') ADVANCE(202);
+      if (lookahead == 'i') ADVANCE(519);
       END_STATE();
     case 456:
-      if (lookahead == 'i') ADVANCE(520);
+      if (lookahead == 'i') ADVANCE(859);
       END_STATE();
     case 457:
-      if (lookahead == 'i') ADVANCE(860);
+      if (lookahead == 'i') ADVANCE(569);
       END_STATE();
     case 458:
-      if (lookahead == 'i') ADVANCE(570);
+      if (lookahead == 'i') ADVANCE(603);
       END_STATE();
     case 459:
-      if (lookahead == 'i') ADVANCE(604);
+      if (lookahead == 'i') ADVANCE(571);
       END_STATE();
     case 460:
-      if (lookahead == 'i') ADVANCE(572);
+      if (lookahead == 'i') ADVANCE(318);
       END_STATE();
     case 461:
-      if (lookahead == 'i') ADVANCE(319);
+      if (lookahead == 'i') ADVANCE(320);
       END_STATE();
     case 462:
-      if (lookahead == 'i') ADVANCE(321);
+      if (lookahead == 'i') ADVANCE(558);
       END_STATE();
     case 463:
-      if (lookahead == 'i') ADVANCE(559);
+      if (lookahead == 'i') ADVANCE(867);
       END_STATE();
     case 464:
-      if (lookahead == 'i') ADVANCE(868);
+      if (lookahead == 'i') ADVANCE(834);
       END_STATE();
     case 465:
-      if (lookahead == 'i') ADVANCE(835);
+      if (lookahead == 'i') ADVANCE(919);
       END_STATE();
     case 466:
-      if (lookahead == 'i') ADVANCE(920);
+      if (lookahead == 'i') ADVANCE(395);
       END_STATE();
     case 467:
-      if (lookahead == 'i') ADVANCE(396);
+      if (lookahead == 'i') ADVANCE(873);
       END_STATE();
     case 468:
-      if (lookahead == 'i') ADVANCE(874);
+      if (lookahead == 'i') ADVANCE(530);
       END_STATE();
     case 469:
-      if (lookahead == 'i') ADVANCE(531);
+      if (lookahead == 'i') ADVANCE(151);
+      if (lookahead == 't') ADVANCE(368);
       END_STATE();
     case 470:
-      if (lookahead == 'i') ADVANCE(152);
-      if (lookahead == 't') ADVANCE(369);
+      if (lookahead == 'i') ADVANCE(393);
       END_STATE();
     case 471:
-      if (lookahead == 'i') ADVANCE(394);
+      if (lookahead == 'i') ADVANCE(587);
       END_STATE();
     case 472:
-      if (lookahead == 'i') ADVANCE(588);
+      if (lookahead == 'i') ADVANCE(595);
       END_STATE();
     case 473:
-      if (lookahead == 'i') ADVANCE(596);
+      if (lookahead == 'i') ADVANCE(190);
       END_STATE();
     case 474:
-      if (lookahead == 'i') ADVANCE(191);
+      if (lookahead == 'i') ADVANCE(557);
+      if (lookahead == 'o') ADVANCE(390);
       END_STATE();
     case 475:
-      if (lookahead == 'i') ADVANCE(558);
-      if (lookahead == 'o') ADVANCE(391);
+      if (lookahead == 'i') ADVANCE(532);
+      if (lookahead == 'r') ADVANCE(342);
       END_STATE();
     case 476:
-      if (lookahead == 'i') ADVANCE(533);
-      if (lookahead == 'r') ADVANCE(343);
+      if (lookahead == 'i') ADVANCE(841);
       END_STATE();
     case 477:
-      if (lookahead == 'i') ADVANCE(842);
+      if (lookahead == 'i') ADVANCE(268);
       END_STATE();
     case 478:
-      if (lookahead == 'i') ADVANCE(269);
+      if (lookahead == 'i') ADVANCE(227);
       END_STATE();
     case 479:
-      if (lookahead == 'i') ADVANCE(228);
+      if (lookahead == 'j') ADVANCE(328);
+      if (lookahead == 's') ADVANCE(216);
       END_STATE();
     case 480:
-      if (lookahead == 'j') ADVANCE(329);
-      if (lookahead == 's') ADVANCE(217);
+      if (lookahead == 'j') ADVANCE(362);
       END_STATE();
     case 481:
-      if (lookahead == 'j') ADVANCE(363);
+      if (lookahead == 'j') ADVANCE(369);
+      if (lookahead == 's') ADVANCE(224);
       END_STATE();
     case 482:
-      if (lookahead == 'j') ADVANCE(370);
-      if (lookahead == 's') ADVANCE(225);
+      if (lookahead == 'k') ADVANCE(68);
       END_STATE();
     case 483:
-      if (lookahead == 'k') ADVANCE(66);
+      if (lookahead == 'k') ADVANCE(1115);
       END_STATE();
     case 484:
-      if (lookahead == 'k') ADVANCE(1116);
+      if (lookahead == 'k') ADVANCE(1189);
       END_STATE();
     case 485:
-      if (lookahead == 'k') ADVANCE(1190);
+      if (lookahead == 'k') ADVANCE(1137);
       END_STATE();
     case 486:
-      if (lookahead == 'k') ADVANCE(1138);
+      if (lookahead == 'k') ADVANCE(1165);
       END_STATE();
     case 487:
-      if (lookahead == 'k') ADVANCE(1166);
+      if (lookahead == 'k') ADVANCE(1173);
       END_STATE();
     case 488:
-      if (lookahead == 'k') ADVANCE(1174);
+      if (lookahead == 'k') ADVANCE(1138);
       END_STATE();
     case 489:
-      if (lookahead == 'k') ADVANCE(1139);
+      if (lookahead == 'k') ADVANCE(1178);
       END_STATE();
     case 490:
-      if (lookahead == 'k') ADVANCE(1179);
+      if (lookahead == 'k') ADVANCE(1174);
       END_STATE();
     case 491:
-      if (lookahead == 'k') ADVANCE(1175);
+      if (lookahead == 'k') ADVANCE(1131);
       END_STATE();
     case 492:
-      if (lookahead == 'k') ADVANCE(1132);
+      if (lookahead == 'k') ADVANCE(1032);
       END_STATE();
     case 493:
-      if (lookahead == 'k') ADVANCE(1033);
+      if (lookahead == 'k') ADVANCE(1177);
       END_STATE();
     case 494:
-      if (lookahead == 'k') ADVANCE(1178);
+      if (lookahead == 'k') ADVANCE(1179);
       END_STATE();
     case 495:
-      if (lookahead == 'k') ADVANCE(1180);
+      if (lookahead == 'k') ADVANCE(1175);
       END_STATE();
     case 496:
-      if (lookahead == 'k') ADVANCE(1176);
+      if (lookahead == 'k') ADVANCE(1139);
       END_STATE();
     case 497:
-      if (lookahead == 'k') ADVANCE(1140);
+      if (lookahead == 'k') ADVANCE(966);
       END_STATE();
     case 498:
-      if (lookahead == 'k') ADVANCE(967);
+      if (lookahead == 'k') ADVANCE(1031);
       END_STATE();
     case 499:
-      if (lookahead == 'k') ADVANCE(1032);
+      if (lookahead == 'k') ADVANCE(1166);
       END_STATE();
     case 500:
-      if (lookahead == 'k') ADVANCE(1167);
+      if (lookahead == 'k') ADVANCE(1187);
       END_STATE();
     case 501:
-      if (lookahead == 'k') ADVANCE(1188);
+      if (lookahead == 'k') ADVANCE(1186);
       END_STATE();
     case 502:
-      if (lookahead == 'k') ADVANCE(1187);
+      if (lookahead == 'k') ADVANCE(1136);
       END_STATE();
     case 503:
-      if (lookahead == 'k') ADVANCE(1137);
+      if (lookahead == 'k') ADVANCE(1188);
       END_STATE();
     case 504:
-      if (lookahead == 'k') ADVANCE(1189);
+      if (lookahead == 'k') ADVANCE(1132);
       END_STATE();
     case 505:
-      if (lookahead == 'k') ADVANCE(1133);
+      if (lookahead == 'k') ADVANCE(404);
       END_STATE();
     case 506:
-      if (lookahead == 'k') ADVANCE(405);
+      if (lookahead == 'k') ADVANCE(359);
       END_STATE();
     case 507:
-      if (lookahead == 'k') ADVANCE(360);
+      if (lookahead == 'k') ADVANCE(902);
       END_STATE();
     case 508:
-      if (lookahead == 'k') ADVANCE(903);
+      if (lookahead == 'k') ADVANCE(905);
       END_STATE();
     case 509:
-      if (lookahead == 'k') ADVANCE(906);
+      if (lookahead == 'l') ADVANCE(136);
       END_STATE();
     case 510:
-      if (lookahead == 'l') ADVANCE(137);
+      if (lookahead == 'l') ADVANCE(136);
+      if (lookahead == 'o') ADVANCE(244);
       END_STATE();
     case 511:
-      if (lookahead == 'l') ADVANCE(137);
-      if (lookahead == 'o') ADVANCE(245);
+      if (lookahead == 'l') ADVANCE(184);
       END_STATE();
     case 512:
-      if (lookahead == 'l') ADVANCE(185);
+      if (lookahead == 'l') ADVANCE(1074);
       END_STATE();
     case 513:
-      if (lookahead == 'l') ADVANCE(1075);
+      if (lookahead == 'l') ADVANCE(1055);
       END_STATE();
     case 514:
-      if (lookahead == 'l') ADVANCE(1056);
+      if (lookahead == 'l') ADVANCE(236);
       END_STATE();
     case 515:
-      if (lookahead == 'l') ADVANCE(237);
+      if (lookahead == 'l') ADVANCE(951);
       END_STATE();
     case 516:
-      if (lookahead == 'l') ADVANCE(952);
+      if (lookahead == 'l') ADVANCE(531);
       END_STATE();
     case 517:
-      if (lookahead == 'l') ADVANCE(532);
+      if (lookahead == 'l') ADVANCE(531);
+      if (lookahead == 's') ADVANCE(1206);
       END_STATE();
     case 518:
-      if (lookahead == 'l') ADVANCE(532);
-      if (lookahead == 's') ADVANCE(1207);
+      if (lookahead == 'l') ADVANCE(264);
       END_STATE();
     case 519:
-      if (lookahead == 'l') ADVANCE(265);
+      if (lookahead == 'l') ADVANCE(193);
       END_STATE();
     case 520:
-      if (lookahead == 'l') ADVANCE(194);
+      if (lookahead == 'l') ADVANCE(472);
       END_STATE();
     case 521:
-      if (lookahead == 'l') ADVANCE(473);
+      if (lookahead == 'l') ADVANCE(106);
       END_STATE();
     case 522:
-      if (lookahead == 'l') ADVANCE(107);
+      if (lookahead == 'l') ADVANCE(642);
+      if (lookahead == 'm') ADVANCE(738);
       END_STATE();
     case 523:
-      if (lookahead == 'l') ADVANCE(643);
-      if (lookahead == 'm') ADVANCE(739);
+      if (lookahead == 'l') ADVANCE(851);
       END_STATE();
     case 524:
-      if (lookahead == 'l') ADVANCE(852);
+      if (lookahead == 'l') ADVANCE(450);
+      if (lookahead == 't') ADVANCE(861);
       END_STATE();
     case 525:
-      if (lookahead == 'l') ADVANCE(451);
-      if (lookahead == 't') ADVANCE(862);
+      if (lookahead == 'l') ADVANCE(853);
       END_STATE();
     case 526:
-      if (lookahead == 'l') ADVANCE(854);
+      if (lookahead == 'l') ADVANCE(147);
       END_STATE();
     case 527:
-      if (lookahead == 'l') ADVANCE(148);
+      if (lookahead == 'l') ADVANCE(155);
       END_STATE();
     case 528:
-      if (lookahead == 'l') ADVANCE(156);
+      if (lookahead == 'l') ADVANCE(149);
       END_STATE();
     case 529:
-      if (lookahead == 'l') ADVANCE(150);
+      if (lookahead == 'l') ADVANCE(289);
       END_STATE();
     case 530:
-      if (lookahead == 'l') ADVANCE(290);
+      if (lookahead == 'l') ADVANCE(303);
       END_STATE();
     case 531:
-      if (lookahead == 'l') ADVANCE(304);
+      if (lookahead == 'l') ADVANCE(623);
       END_STATE();
     case 532:
-      if (lookahead == 'l') ADVANCE(624);
+      if (lookahead == 'l') ADVANCE(250);
       END_STATE();
     case 533:
-      if (lookahead == 'l') ADVANCE(251);
+      if (lookahead == 'l') ADVANCE(250);
+      if (lookahead == 'm') ADVANCE(337);
       END_STATE();
     case 534:
-      if (lookahead == 'l') ADVANCE(251);
-      if (lookahead == 'm') ADVANCE(338);
+      if (lookahead == 'l') ADVANCE(527);
       END_STATE();
     case 535:
-      if (lookahead == 'l') ADVANCE(528);
+      if (lookahead == 'l') ADVANCE(470);
       END_STATE();
     case 536:
-      if (lookahead == 'l') ADVANCE(471);
+      if (lookahead == 'l') ADVANCE(666);
       END_STATE();
     case 537:
-      if (lookahead == 'l') ADVANCE(667);
+      if (lookahead == 'l') ADVANCE(673);
       END_STATE();
     case 538:
-      if (lookahead == 'l') ADVANCE(674);
+      if (lookahead == 'l') ADVANCE(640);
       END_STATE();
     case 539:
-      if (lookahead == 'l') ADVANCE(641);
+      if (lookahead == 'l') ADVANCE(644);
       END_STATE();
     case 540:
-      if (lookahead == 'l') ADVANCE(645);
+      if (lookahead == 'l') ADVANCE(688);
       END_STATE();
     case 541:
-      if (lookahead == 'l') ADVANCE(689);
+      if (lookahead == 'l') ADVANCE(695);
       END_STATE();
     case 542:
-      if (lookahead == 'l') ADVANCE(696);
+      if (lookahead == 'l') ADVANCE(695);
+      if (lookahead == 'm') ADVANCE(738);
       END_STATE();
     case 543:
-      if (lookahead == 'l') ADVANCE(696);
-      if (lookahead == 'm') ADVANCE(739);
+      if (lookahead == 'l') ADVANCE(469);
+      if (lookahead == 't') ADVANCE(868);
+      if (lookahead == 'u') ADVANCE(886);
       END_STATE();
     case 544:
-      if (lookahead == 'l') ADVANCE(470);
-      if (lookahead == 't') ADVANCE(869);
-      if (lookahead == 'u') ADVANCE(887);
+      if (lookahead == 'l') ADVANCE(192);
       END_STATE();
     case 545:
-      if (lookahead == 'l') ADVANCE(193);
+      if (lookahead == 'l') ADVANCE(538);
       END_STATE();
     case 546:
-      if (lookahead == 'l') ADVANCE(539);
+      if (lookahead == 'l') ADVANCE(712);
       END_STATE();
     case 547:
-      if (lookahead == 'l') ADVANCE(713);
+      if (lookahead == 'l') ADVANCE(539);
       END_STATE();
     case 548:
-      if (lookahead == 'l') ADVANCE(540);
+      if (lookahead == 'm') ADVANCE(1180);
       END_STATE();
     case 549:
       if (lookahead == 'm') ADVANCE(1181);
       END_STATE();
     case 550:
-      if (lookahead == 'm') ADVANCE(1182);
+      if (lookahead == 'm') ADVANCE(1185);
       END_STATE();
     case 551:
-      if (lookahead == 'm') ADVANCE(1186);
+      if (lookahead == 'm') ADVANCE(462);
       END_STATE();
     case 552:
-      if (lookahead == 'm') ADVANCE(463);
+      if (lookahead == 'm') ADVANCE(738);
       END_STATE();
     case 553:
-      if (lookahead == 'm') ADVANCE(739);
+      if (lookahead == 'm') ADVANCE(312);
       END_STATE();
     case 554:
-      if (lookahead == 'm') ADVANCE(313);
+      if (lookahead == 'm') ADVANCE(312);
+      if (lookahead == 'x') ADVANCE(1022);
       END_STATE();
     case 555:
-      if (lookahead == 'm') ADVANCE(313);
-      if (lookahead == 'x') ADVANCE(1023);
+      if (lookahead == 'm') ADVANCE(148);
       END_STATE();
     case 556:
-      if (lookahead == 'm') ADVANCE(149);
+      if (lookahead == 'm') ADVANCE(324);
       END_STATE();
     case 557:
-      if (lookahead == 'm') ADVANCE(325);
+      if (lookahead == 'm') ADVANCE(337);
       END_STATE();
     case 558:
-      if (lookahead == 'm') ADVANCE(338);
+      if (lookahead == 'm') ADVANCE(284);
       END_STATE();
     case 559:
-      if (lookahead == 'm') ADVANCE(285);
+      if (lookahead == 'm') ADVANCE(150);
       END_STATE();
     case 560:
-      if (lookahead == 'm') ADVANCE(151);
+      if (lookahead == 'm') ADVANCE(180);
       END_STATE();
     case 561:
-      if (lookahead == 'm') ADVANCE(181);
+      if (lookahead == 'm') ADVANCE(196);
       END_STATE();
     case 562:
-      if (lookahead == 'm') ADVANCE(197);
+      if (lookahead == 'm') ADVANCE(343);
       END_STATE();
     case 563:
-      if (lookahead == 'm') ADVANCE(344);
+      if (lookahead == 'm') ADVANCE(371);
       END_STATE();
     case 564:
-      if (lookahead == 'm') ADVANCE(372);
+      if (lookahead == 'm') ADVANCE(378);
       END_STATE();
     case 565:
-      if (lookahead == 'm') ADVANCE(379);
+      if (lookahead == 'n') ADVANCE(231);
       END_STATE();
     case 566:
-      if (lookahead == 'n') ADVANCE(232);
+      if (lookahead == 'n') ADVANCE(129);
       END_STATE();
     case 567:
-      if (lookahead == 'n') ADVANCE(130);
+      if (lookahead == 'n') ADVANCE(1121);
       END_STATE();
     case 568:
-      if (lookahead == 'n') ADVANCE(1122);
+      if (lookahead == 'n') ADVANCE(1117);
       END_STATE();
     case 569:
-      if (lookahead == 'n') ADVANCE(1118);
+      if (lookahead == 'n') ADVANCE(1201);
       END_STATE();
     case 570:
-      if (lookahead == 'n') ADVANCE(1202);
+      if (lookahead == 'n') ADVANCE(1111);
       END_STATE();
     case 571:
-      if (lookahead == 'n') ADVANCE(1112);
+      if (lookahead == 'n') ADVANCE(1202);
       END_STATE();
     case 572:
-      if (lookahead == 'n') ADVANCE(1203);
+      if (lookahead == 'n') ADVANCE(130);
       END_STATE();
     case 573:
-      if (lookahead == 'n') ADVANCE(131);
+      if (lookahead == 'n') ADVANCE(235);
       END_STATE();
     case 574:
-      if (lookahead == 'n') ADVANCE(236);
+      if (lookahead == 'n') ADVANCE(923);
       END_STATE();
     case 575:
-      if (lookahead == 'n') ADVANCE(924);
+      if (lookahead == 'n') ADVANCE(916);
       END_STATE();
     case 576:
       if (lookahead == 'n') ADVANCE(917);
       END_STATE();
     case 577:
-      if (lookahead == 'n') ADVANCE(918);
+      if (lookahead == 'n') ADVANCE(237);
+      if (lookahead == 't') ADVANCE(1190);
       END_STATE();
     case 578:
-      if (lookahead == 'n') ADVANCE(238);
-      if (lookahead == 't') ADVANCE(1191);
+      if (lookahead == 'n') ADVANCE(272);
+      if (lookahead == 'r') ADVANCE(880);
       END_STATE();
     case 579:
-      if (lookahead == 'n') ADVANCE(273);
-      if (lookahead == 'r') ADVANCE(881);
+      if (lookahead == 'n') ADVANCE(272);
+      if (lookahead == 'r') ADVANCE(880);
+      if (lookahead == 't') ADVANCE(900);
       END_STATE();
     case 580:
-      if (lookahead == 'n') ADVANCE(273);
-      if (lookahead == 'r') ADVANCE(881);
-      if (lookahead == 't') ADVANCE(901);
+      if (lookahead == 'n') ADVANCE(272);
+      if (lookahead == 't') ADVANCE(900);
       END_STATE();
     case 581:
-      if (lookahead == 'n') ADVANCE(273);
-      if (lookahead == 't') ADVANCE(901);
+      if (lookahead == 'n') ADVANCE(274);
       END_STATE();
     case 582:
-      if (lookahead == 'n') ADVANCE(275);
+      if (lookahead == 'n') ADVANCE(281);
+      if (lookahead == 'r') ADVANCE(555);
       END_STATE();
     case 583:
-      if (lookahead == 'n') ADVANCE(282);
-      if (lookahead == 'r') ADVANCE(556);
+      if (lookahead == 'n') ADVANCE(281);
+      if (lookahead == 's') ADVANCE(731);
       END_STATE();
     case 584:
-      if (lookahead == 'n') ADVANCE(282);
-      if (lookahead == 's') ADVANCE(732);
+      if (lookahead == 'n') ADVANCE(735);
       END_STATE();
     case 585:
-      if (lookahead == 'n') ADVANCE(736);
+      if (lookahead == 'n') ADVANCE(616);
       END_STATE();
     case 586:
-      if (lookahead == 'n') ADVANCE(617);
+      if (lookahead == 'n') ADVANCE(153);
       END_STATE();
     case 587:
-      if (lookahead == 'n') ADVANCE(154);
+      if (lookahead == 'n') ADVANCE(239);
       END_STATE();
     case 588:
-      if (lookahead == 'n') ADVANCE(240);
+      if (lookahead == 'n') ADVANCE(257);
       END_STATE();
     case 589:
-      if (lookahead == 'n') ADVANCE(258);
+      if (lookahead == 'n') ADVANCE(157);
       END_STATE();
     case 590:
-      if (lookahead == 'n') ADVANCE(158);
+      if (lookahead == 'n') ADVANCE(242);
       END_STATE();
     case 591:
-      if (lookahead == 'n') ADVANCE(243);
+      if (lookahead == 'n') ADVANCE(618);
+      if (lookahead == 'y') ADVANCE(326);
       END_STATE();
     case 592:
       if (lookahead == 'n') ADVANCE(619);
-      if (lookahead == 'y') ADVANCE(327);
       END_STATE();
     case 593:
-      if (lookahead == 'n') ADVANCE(620);
+      if (lookahead == 'n') ADVANCE(857);
       END_STATE();
     case 594:
-      if (lookahead == 'n') ADVANCE(858);
+      if (lookahead == 'n') ADVANCE(294);
       END_STATE();
     case 595:
-      if (lookahead == 'n') ADVANCE(295);
+      if (lookahead == 'n') ADVANCE(298);
       END_STATE();
     case 596:
-      if (lookahead == 'n') ADVANCE(299);
+      if (lookahead == 'n') ADVANCE(302);
       END_STATE();
     case 597:
-      if (lookahead == 'n') ADVANCE(303);
+      if (lookahead == 'n') ADVANCE(464);
       END_STATE();
     case 598:
-      if (lookahead == 'n') ADVANCE(465);
+      if (lookahead == 'n') ADVANCE(702);
       END_STATE();
     case 599:
-      if (lookahead == 'n') ADVANCE(703);
+      if (lookahead == 'n') ADVANCE(329);
       END_STATE();
     case 600:
-      if (lookahead == 'n') ADVANCE(330);
+      if (lookahead == 'n') ADVANCE(220);
       END_STATE();
     case 601:
-      if (lookahead == 'n') ADVANCE(221);
+      if (lookahead == 'n') ADVANCE(166);
       END_STATE();
     case 602:
-      if (lookahead == 'n') ADVANCE(167);
+      if (lookahead == 'n') ADVANCE(869);
       END_STATE();
     case 603:
-      if (lookahead == 'n') ADVANCE(870);
+      if (lookahead == 'n') ADVANCE(159);
       END_STATE();
     case 604:
-      if (lookahead == 'n') ADVANCE(160);
+      if (lookahead == 'n') ADVANCE(871);
       END_STATE();
     case 605:
       if (lookahead == 'n') ADVANCE(872);
       END_STATE();
     case 606:
-      if (lookahead == 'n') ADVANCE(873);
+      if (lookahead == 'n') ADVANCE(255);
       END_STATE();
     case 607:
-      if (lookahead == 'n') ADVANCE(256);
+      if (lookahead == 'n') ADVANCE(709);
       END_STATE();
     case 608:
-      if (lookahead == 'n') ADVANCE(710);
+      if (lookahead == 'n') ADVANCE(262);
       END_STATE();
     case 609:
-      if (lookahead == 'n') ADVANCE(263);
+      if (lookahead == 'n') ADVANCE(74);
       END_STATE();
     case 610:
-      if (lookahead == 'n') ADVANCE(72);
+      if (lookahead == 'n') ADVANCE(90);
       END_STATE();
     case 611:
-      if (lookahead == 'n') ADVANCE(88);
+      if (lookahead == 'n') ADVANCE(888);
       END_STATE();
     case 612:
-      if (lookahead == 'n') ADVANCE(889);
+      if (lookahead == 'o') ADVANCE(932);
       END_STATE();
     case 613:
-      if (lookahead == 'o') ADVANCE(933);
+      if (lookahead == 'o') ADVANCE(940);
       END_STATE();
     case 614:
-      if (lookahead == 'o') ADVANCE(941);
+      if (lookahead == 'o') ADVANCE(402);
       END_STATE();
     case 615:
-      if (lookahead == 'o') ADVANCE(403);
+      if (lookahead == 'o') ADVANCE(1163);
       END_STATE();
     case 616:
-      if (lookahead == 'o') ADVANCE(1164);
+      if (lookahead == 'o') ADVANCE(1169);
       END_STATE();
     case 617:
-      if (lookahead == 'o') ADVANCE(1170);
+      if (lookahead == 'o') ADVANCE(1156);
       END_STATE();
     case 618:
-      if (lookahead == 'o') ADVANCE(1157);
+      if (lookahead == 'o') ADVANCE(1212);
       END_STATE();
     case 619:
-      if (lookahead == 'o') ADVANCE(1213);
+      if (lookahead == 'o') ADVANCE(1170);
       END_STATE();
     case 620:
-      if (lookahead == 'o') ADVANCE(1171);
+      if (lookahead == 'o') ADVANCE(1157);
       END_STATE();
     case 621:
-      if (lookahead == 'o') ADVANCE(1158);
+      if (lookahead == 'o') ADVANCE(1184);
       END_STATE();
     case 622:
-      if (lookahead == 'o') ADVANCE(1185);
+      if (lookahead == 'o') ADVANCE(105);
       END_STATE();
     case 623:
-      if (lookahead == 'o') ADVANCE(106);
+      if (lookahead == 'o') ADVANCE(926);
       END_STATE();
     case 624:
-      if (lookahead == 'o') ADVANCE(927);
+      if (lookahead == 'o') ADVANCE(582);
       END_STATE();
     case 625:
-      if (lookahead == 'o') ADVANCE(583);
+      if (lookahead == 'o') ADVANCE(933);
       END_STATE();
     case 626:
-      if (lookahead == 'o') ADVANCE(934);
+      if (lookahead == 'o') ADVANCE(942);
       END_STATE();
     case 627:
-      if (lookahead == 'o') ADVANCE(943);
+      if (lookahead == 'o') ADVANCE(896);
       END_STATE();
     case 628:
-      if (lookahead == 'o') ADVANCE(897);
+      if (lookahead == 'o') ADVANCE(484);
       END_STATE();
     case 629:
-      if (lookahead == 'o') ADVANCE(485);
+      if (lookahead == 'o') ADVANCE(847);
       END_STATE();
     case 630:
-      if (lookahead == 'o') ADVANCE(848);
+      if (lookahead == 'o') ADVANCE(904);
       END_STATE();
     case 631:
-      if (lookahead == 'o') ADVANCE(905);
+      if (lookahead == 'o') ADVANCE(485);
       END_STATE();
     case 632:
-      if (lookahead == 'o') ADVANCE(486);
+      if (lookahead == 'o') ADVANCE(870);
       END_STATE();
     case 633:
-      if (lookahead == 'o') ADVANCE(871);
+      if (lookahead == 'o') ADVANCE(784);
       END_STATE();
     case 634:
-      if (lookahead == 'o') ADVANCE(785);
+      if (lookahead == 'o') ADVANCE(108);
       END_STATE();
     case 635:
-      if (lookahead == 'o') ADVANCE(109);
+      if (lookahead == 'o') ADVANCE(486);
       END_STATE();
     case 636:
-      if (lookahead == 'o') ADVANCE(487);
+      if (lookahead == 'o') ADVANCE(536);
       END_STATE();
     case 637:
-      if (lookahead == 'o') ADVANCE(537);
+      if (lookahead == 'o') ADVANCE(550);
       END_STATE();
     case 638:
-      if (lookahead == 'o') ADVANCE(551);
+      if (lookahead == 'o') ADVANCE(574);
       END_STATE();
     case 639:
-      if (lookahead == 'o') ADVANCE(575);
+      if (lookahead == 'o') ADVANCE(507);
       END_STATE();
     case 640:
-      if (lookahead == 'o') ADVANCE(508);
+      if (lookahead == 'o') ADVANCE(930);
       END_STATE();
     case 641:
-      if (lookahead == 'o') ADVANCE(931);
+      if (lookahead == 'o') ADVANCE(487);
       END_STATE();
     case 642:
-      if (lookahead == 'o') ADVANCE(488);
+      if (lookahead == 'o') ADVANCE(743);
       END_STATE();
     case 643:
-      if (lookahead == 'o') ADVANCE(744);
+      if (lookahead == 'o') ADVANCE(552);
       END_STATE();
     case 644:
-      if (lookahead == 'o') ADVANCE(553);
+      if (lookahead == 'o') ADVANCE(931);
       END_STATE();
     case 645:
-      if (lookahead == 'o') ADVANCE(932);
+      if (lookahead == 'o') ADVANCE(913);
       END_STATE();
     case 646:
-      if (lookahead == 'o') ADVANCE(914);
+      if (lookahead == 'o') ADVANCE(488);
       END_STATE();
     case 647:
-      if (lookahead == 'o') ADVANCE(489);
+      if (lookahead == 'o') ADVANCE(744);
       END_STATE();
     case 648:
-      if (lookahead == 'o') ADVANCE(745);
+      if (lookahead == 'o') ADVANCE(489);
       END_STATE();
     case 649:
       if (lookahead == 'o') ADVANCE(490);
       END_STATE();
     case 650:
-      if (lookahead == 'o') ADVANCE(491);
+      if (lookahead == 'o') ADVANCE(534);
       END_STATE();
     case 651:
-      if (lookahead == 'o') ADVANCE(535);
+      if (lookahead == 'o') ADVANCE(491);
       END_STATE();
     case 652:
       if (lookahead == 'o') ADVANCE(492);
       END_STATE();
     case 653:
       if (lookahead == 'o') ADVANCE(493);
       END_STATE();
     case 654:
       if (lookahead == 'o') ADVANCE(494);
       END_STATE();
     case 655:
-      if (lookahead == 'o') ADVANCE(495);
+      if (lookahead == 'o') ADVANCE(746);
       END_STATE();
     case 656:
-      if (lookahead == 'o') ADVANCE(747);
+      if (lookahead == 'o') ADVANCE(495);
       END_STATE();
     case 657:
-      if (lookahead == 'o') ADVANCE(496);
+      if (lookahead == 'o') ADVANCE(521);
       END_STATE();
     case 658:
-      if (lookahead == 'o') ADVANCE(522);
+      if (lookahead == 'o') ADVANCE(496);
       END_STATE();
     case 659:
-      if (lookahead == 'o') ADVANCE(497);
+      if (lookahead == 'o') ADVANCE(806);
       END_STATE();
     case 660:
-      if (lookahead == 'o') ADVANCE(807);
+      if (lookahead == 'o') ADVANCE(497);
       END_STATE();
     case 661:
       if (lookahead == 'o') ADVANCE(498);
       END_STATE();
     case 662:
       if (lookahead == 'o') ADVANCE(499);
       END_STATE();
     case 663:
-      if (lookahead == 'o') ADVANCE(500);
+      if (lookahead == 'o') ADVANCE(865);
       END_STATE();
     case 664:
-      if (lookahead == 'o') ADVANCE(866);
+      if (lookahead == 'o') ADVANCE(500);
       END_STATE();
     case 665:
       if (lookahead == 'o') ADVANCE(501);
       END_STATE();
     case 666:
-      if (lookahead == 'o') ADVANCE(502);
+      if (lookahead == 'o') ADVANCE(750);
       END_STATE();
     case 667:
-      if (lookahead == 'o') ADVANCE(751);
+      if (lookahead == 'o') ADVANCE(502);
       END_STATE();
     case 668:
-      if (lookahead == 'o') ADVANCE(503);
+      if (lookahead == 'o') ADVANCE(631);
       END_STATE();
     case 669:
-      if (lookahead == 'o') ADVANCE(632);
+      if (lookahead == 'o') ADVANCE(503);
       END_STATE();
     case 670:
       if (lookahead == 'o') ADVANCE(504);
       END_STATE();
     case 671:
-      if (lookahead == 'o') ADVANCE(505);
+      if (lookahead == 'o') ADVANCE(635);
       END_STATE();
     case 672:
-      if (lookahead == 'o') ADVANCE(636);
+      if (lookahead == 'o') ADVANCE(753);
       END_STATE();
     case 673:
-      if (lookahead == 'o') ADVANCE(754);
+      if (lookahead == 'o') ADVANCE(639);
       END_STATE();
     case 674:
-      if (lookahead == 'o') ADVANCE(640);
+      if (lookahead == 'o') ADVANCE(641);
       END_STATE();
     case 675:
-      if (lookahead == 'o') ADVANCE(642);
+      if (lookahead == 'o') ADVANCE(646);
       END_STATE();
     case 676:
-      if (lookahead == 'o') ADVANCE(647);
+      if (lookahead == 'o') ADVANCE(648);
       END_STATE();
     case 677:
-      if (lookahead == 'o') ADVANCE(649);
+      if (lookahead == 'o') ADVANCE(755);
       END_STATE();
     case 678:
-      if (lookahead == 'o') ADVANCE(756);
+      if (lookahead == 'o') ADVANCE(649);
       END_STATE();
     case 679:
-      if (lookahead == 'o') ADVANCE(650);
+      if (lookahead == 'o') ADVANCE(651);
       END_STATE();
     case 680:
       if (lookahead == 'o') ADVANCE(652);
       END_STATE();
     case 681:
       if (lookahead == 'o') ADVANCE(653);
       END_STATE();
     case 682:
       if (lookahead == 'o') ADVANCE(654);
       END_STATE();
     case 683:
-      if (lookahead == 'o') ADVANCE(655);
+      if (lookahead == 'o') ADVANCE(656);
       END_STATE();
     case 684:
-      if (lookahead == 'o') ADVANCE(657);
+      if (lookahead == 'o') ADVANCE(759);
       END_STATE();
     case 685:
-      if (lookahead == 'o') ADVANCE(760);
+      if (lookahead == 'o') ADVANCE(658);
       END_STATE();
     case 686:
-      if (lookahead == 'o') ADVANCE(659);
+      if (lookahead == 'o') ADVANCE(660);
       END_STATE();
     case 687:
       if (lookahead == 'o') ADVANCE(661);
       END_STATE();
     case 688:
-      if (lookahead == 'o') ADVANCE(662);
+      if (lookahead == 'o') ADVANCE(761);
       END_STATE();
     case 689:
-      if (lookahead == 'o') ADVANCE(762);
+      if (lookahead == 'o') ADVANCE(662);
       END_STATE();
     case 690:
-      if (lookahead == 'o') ADVANCE(663);
+      if (lookahead == 'o') ADVANCE(800);
       END_STATE();
     case 691:
-      if (lookahead == 'o') ADVANCE(801);
+      if (lookahead == 'o') ADVANCE(664);
       END_STATE();
     case 692:
       if (lookahead == 'o') ADVANCE(665);
       END_STATE();
     case 693:
-      if (lookahead == 'o') ADVANCE(666);
+      if (lookahead == 'o') ADVANCE(667);
       END_STATE();
     case 694:
-      if (lookahead == 'o') ADVANCE(668);
+      if (lookahead == 'o') ADVANCE(669);
       END_STATE();
     case 695:
-      if (lookahead == 'o') ADVANCE(670);
+      if (lookahead == 'o') ADVANCE(763);
       END_STATE();
     case 696:
-      if (lookahead == 'o') ADVANCE(764);
+      if (lookahead == 'o') ADVANCE(657);
       END_STATE();
     case 697:
-      if (lookahead == 'o') ADVANCE(658);
+      if (lookahead == 'o') ADVANCE(670);
       END_STATE();
     case 698:
-      if (lookahead == 'o') ADVANCE(671);
+      if (lookahead == 'o') ADVANCE(542);
+      if (lookahead == 'y') ADVANCE(143);
       END_STATE();
     case 699:
-      if (lookahead == 'o') ADVANCE(543);
-      if (lookahead == 'y') ADVANCE(144);
+      if (lookahead == 'o') ADVANCE(915);
       END_STATE();
     case 700:
-      if (lookahead == 'o') ADVANCE(916);
+      if (lookahead == 'o') ADVANCE(943);
       END_STATE();
     case 701:
-      if (lookahead == 'o') ADVANCE(944);
+      if (lookahead == 'o') ADVANCE(594);
       END_STATE();
     case 702:
-      if (lookahead == 'o') ADVANCE(595);
+      if (lookahead == 'o') ADVANCE(787);
       END_STATE();
     case 703:
-      if (lookahead == 'o') ADVANCE(788);
+      if (lookahead == 'o') ADVANCE(907);
       END_STATE();
     case 704:
-      if (lookahead == 'o') ADVANCE(908);
+      if (lookahead == 'o') ADVANCE(944);
       END_STATE();
     case 705:
-      if (lookahead == 'o') ADVANCE(945);
+      if (lookahead == 'o') ADVANCE(901);
       END_STATE();
     case 706:
-      if (lookahead == 'o') ADVANCE(902);
+      if (lookahead == 'o') ADVANCE(596);
       END_STATE();
     case 707:
-      if (lookahead == 'o') ADVANCE(597);
+      if (lookahead == 'o') ADVANCE(838);
       END_STATE();
     case 708:
-      if (lookahead == 'o') ADVANCE(839);
+      if (lookahead == 'o') ADVANCE(789);
       END_STATE();
     case 709:
       if (lookahead == 'o') ADVANCE(790);
       END_STATE();
     case 710:
-      if (lookahead == 'o') ADVANCE(791);
+      if (lookahead == 'o') ADVANCE(906);
       END_STATE();
     case 711:
-      if (lookahead == 'o') ADVANCE(907);
+      if (lookahead == 'o') ADVANCE(508);
       END_STATE();
     case 712:
-      if (lookahead == 'o') ADVANCE(509);
+      if (lookahead == 'o') ADVANCE(711);
       END_STATE();
     case 713:
-      if (lookahead == 'o') ADVANCE(712);
+      if (lookahead == 'o') ADVANCE(541);
+      if (lookahead == 'y') ADVANCE(143);
       END_STATE();
     case 714:
-      if (lookahead == 'o') ADVANCE(542);
-      if (lookahead == 'y') ADVANCE(144);
+      if (lookahead == 'o') ADVANCE(113);
       END_STATE();
     case 715:
-      if (lookahead == 'o') ADVANCE(114);
+      if (lookahead == 'o') ADVANCE(807);
       END_STATE();
     case 716:
       if (lookahead == 'o') ADVANCE(808);
       END_STATE();
     case 717:
       if (lookahead == 'o') ADVANCE(809);
       END_STATE();
     case 718:
-      if (lookahead == 'o') ADVANCE(810);
+      if (lookahead == 'o') ADVANCE(114);
       END_STATE();
     case 719:
-      if (lookahead == 'o') ADVANCE(115);
+      if (lookahead == 'p') ADVANCE(1024);
       END_STATE();
     case 720:
-      if (lookahead == 'p') ADVANCE(1025);
+      if (lookahead == 'p') ADVANCE(1143);
       END_STATE();
     case 721:
       if (lookahead == 'p') ADVANCE(1144);
       END_STATE();
     case 722:
-      if (lookahead == 'p') ADVANCE(1145);
+      if (lookahead == 'p') ADVANCE(1167);
       END_STATE();
     case 723:
       if (lookahead == 'p') ADVANCE(1168);
       END_STATE();
     case 724:
-      if (lookahead == 'p') ADVANCE(1169);
+      if (lookahead == 'p') ADVANCE(967);
       END_STATE();
     case 725:
-      if (lookahead == 'p') ADVANCE(968);
+      if (lookahead == 'p') ADVANCE(515);
+      if (lookahead == 's') ADVANCE(323);
       END_STATE();
     case 726:
-      if (lookahead == 'p') ADVANCE(516);
-      if (lookahead == 's') ADVANCE(324);
+      if (lookahead == 'p') ADVANCE(515);
+      if (lookahead == 's') ADVANCE(323);
+      if (lookahead == 'v') ADVANCE(367);
       END_STATE();
     case 727:
-      if (lookahead == 'p') ADVANCE(516);
-      if (lookahead == 's') ADVANCE(324);
-      if (lookahead == 'v') ADVANCE(368);
+      if (lookahead == 'p') ADVANCE(322);
       END_STATE();
     case 728:
-      if (lookahead == 'p') ADVANCE(323);
+      if (lookahead == 'p') ADVANCE(887);
       END_STATE();
     case 729:
-      if (lookahead == 'p') ADVANCE(888);
+      if (lookahead == 'p') ADVANCE(357);
       END_STATE();
     case 730:
-      if (lookahead == 'p') ADVANCE(358);
+      if (lookahead == 'p') ADVANCE(850);
       END_STATE();
     case 731:
-      if (lookahead == 'p') ADVANCE(851);
+      if (lookahead == 'p') ADVANCE(139);
       END_STATE();
     case 732:
-      if (lookahead == 'p') ADVANCE(140);
+      if (lookahead == 'p') ADVANCE(457);
+      if (lookahead == 'u') ADVANCE(584);
       END_STATE();
     case 733:
-      if (lookahead == 'p') ADVANCE(458);
-      if (lookahead == 'u') ADVANCE(585);
+      if (lookahead == 'p') ADVANCE(855);
       END_STATE();
     case 734:
-      if (lookahead == 'p') ADVANCE(856);
+      if (lookahead == 'p') ADVANCE(701);
       END_STATE();
     case 735:
-      if (lookahead == 'p') ADVANCE(702);
+      if (lookahead == 'p') ADVANCE(459);
       END_STATE();
     case 736:
-      if (lookahead == 'p') ADVANCE(460);
+      if (lookahead == 'p') ADVANCE(840);
       END_STATE();
     case 737:
-      if (lookahead == 'p') ADVANCE(841);
+      if (lookahead == 'p') ADVANCE(696);
       END_STATE();
     case 738:
-      if (lookahead == 'p') ADVANCE(697);
+      if (lookahead == 'p') ADVANCE(707);
       END_STATE();
     case 739:
-      if (lookahead == 'p') ADVANCE(708);
+      if (lookahead == 'p') ADVANCE(87);
       END_STATE();
     case 740:
-      if (lookahead == 'p') ADVANCE(85);
+      if (lookahead == 'r') ADVANCE(612);
       END_STATE();
     case 741:
-      if (lookahead == 'r') ADVANCE(613);
+      if (lookahead == 'r') ADVANCE(780);
       END_STATE();
     case 742:
-      if (lookahead == 'r') ADVANCE(781);
+      if (lookahead == 'r') ADVANCE(111);
       END_STATE();
     case 743:
-      if (lookahead == 'r') ADVANCE(112);
+      if (lookahead == 'r') ADVANCE(1129);
       END_STATE();
     case 744:
-      if (lookahead == 'r') ADVANCE(1130);
+      if (lookahead == 'r') ADVANCE(1041);
       END_STATE();
     case 745:
-      if (lookahead == 'r') ADVANCE(1042);
+      if (lookahead == 'r') ADVANCE(1023);
       END_STATE();
     case 746:
-      if (lookahead == 'r') ADVANCE(1024);
+      if (lookahead == 'r') ADVANCE(1017);
       END_STATE();
     case 747:
-      if (lookahead == 'r') ADVANCE(1018);
+      if (lookahead == 'r') ADVANCE(1045);
       END_STATE();
     case 748:
-      if (lookahead == 'r') ADVANCE(1046);
+      if (lookahead == 'r') ADVANCE(1171);
       END_STATE();
     case 749:
-      if (lookahead == 'r') ADVANCE(1172);
+      if (lookahead == 'r') ADVANCE(1015);
       END_STATE();
     case 750:
-      if (lookahead == 'r') ADVANCE(1016);
+      if (lookahead == 'r') ADVANCE(1130);
       END_STATE();
     case 751:
-      if (lookahead == 'r') ADVANCE(1131);
+      if (lookahead == 'r') ADVANCE(1172);
       END_STATE();
     case 752:
-      if (lookahead == 'r') ADVANCE(1173);
+      if (lookahead == 'r') ADVANCE(1145);
       END_STATE();
     case 753:
-      if (lookahead == 'r') ADVANCE(1146);
+      if (lookahead == 'r') ADVANCE(1067);
       END_STATE();
     case 754:
-      if (lookahead == 'r') ADVANCE(1068);
+      if (lookahead == 'r') ADVANCE(1146);
       END_STATE();
     case 755:
-      if (lookahead == 'r') ADVANCE(1147);
+      if (lookahead == 'r') ADVANCE(1047);
       END_STATE();
     case 756:
-      if (lookahead == 'r') ADVANCE(1048);
+      if (lookahead == 'r') ADVANCE(1057);
       END_STATE();
     case 757:
-      if (lookahead == 'r') ADVANCE(1058);
+      if (lookahead == 'r') ADVANCE(1096);
       END_STATE();
     case 758:
-      if (lookahead == 'r') ADVANCE(1097);
+      if (lookahead == 'r') ADVANCE(1000);
       END_STATE();
     case 759:
-      if (lookahead == 'r') ADVANCE(1001);
+      if (lookahead == 'r') ADVANCE(1102);
       END_STATE();
     case 760:
-      if (lookahead == 'r') ADVANCE(1103);
+      if (lookahead == 'r') ADVANCE(1001);
       END_STATE();
     case 761:
-      if (lookahead == 'r') ADVANCE(1002);
+      if (lookahead == 'r') ADVANCE(1128);
       END_STATE();
     case 762:
-      if (lookahead == 'r') ADVANCE(1129);
+      if (lookahead == 'r') ADVANCE(1142);
       END_STATE();
     case 763:
-      if (lookahead == 'r') ADVANCE(1143);
+      if (lookahead == 'r') ADVANCE(953);
       END_STATE();
     case 764:
-      if (lookahead == 'r') ADVANCE(954);
+      if (lookahead == 'r') ADVANCE(946);
       END_STATE();
     case 765:
-      if (lookahead == 'r') ADVANCE(947);
+      if (lookahead == 'r') ADVANCE(116);
       END_STATE();
     case 766:
-      if (lookahead == 'r') ADVANCE(117);
+      if (lookahead == 'r') ADVANCE(936);
       END_STATE();
     case 767:
-      if (lookahead == 'r') ADVANCE(937);
+      if (lookahead == 'r') ADVANCE(454);
       END_STATE();
     case 768:
-      if (lookahead == 'r') ADVANCE(455);
+      if (lookahead == 'r') ADVANCE(614);
       END_STATE();
     case 769:
-      if (lookahead == 'r') ADVANCE(615);
+      if (lookahead == 'r') ADVANCE(937);
       END_STATE();
     case 770:
-      if (lookahead == 'r') ADVANCE(938);
+      if (lookahead == 'r') ADVANCE(947);
       END_STATE();
     case 771:
-      if (lookahead == 'r') ADVANCE(948);
+      if (lookahead == 'r') ADVANCE(100);
       END_STATE();
     case 772:
-      if (lookahead == 'r') ADVANCE(101);
+      if (lookahead == 'r') ADVANCE(449);
       END_STATE();
     case 773:
-      if (lookahead == 'r') ADVANCE(450);
+      if (lookahead == 'r') ADVANCE(210);
       END_STATE();
     case 774:
-      if (lookahead == 'r') ADVANCE(211);
+      if (lookahead == 'r') ADVANCE(219);
       END_STATE();
     case 775:
-      if (lookahead == 'r') ADVANCE(220);
+      if (lookahead == 'r') ADVANCE(880);
       END_STATE();
     case 776:
-      if (lookahead == 'r') ADVANCE(881);
+      if (lookahead == 'r') ADVANCE(520);
       END_STATE();
     case 777:
-      if (lookahead == 'r') ADVANCE(521);
+      if (lookahead == 'r') ADVANCE(102);
       END_STATE();
     case 778:
-      if (lookahead == 'r') ADVANCE(103);
+      if (lookahead == 'r') ADVANCE(816);
       END_STATE();
     case 779:
-      if (lookahead == 'r') ADVANCE(817);
+      if (lookahead == 'r') ADVANCE(103);
       END_STATE();
     case 780:
-      if (lookahead == 'r') ADVANCE(104);
+      if (lookahead == 'r') ADVANCE(647);
       END_STATE();
     case 781:
-      if (lookahead == 'r') ADVANCE(648);
+      if (lookahead == 'r') ADVANCE(617);
       END_STATE();
     case 782:
-      if (lookahead == 'r') ADVANCE(618);
+      if (lookahead == 'r') ADVANCE(258);
       END_STATE();
     case 783:
-      if (lookahead == 'r') ADVANCE(259);
+      if (lookahead == 'r') ADVANCE(705);
       END_STATE();
     case 784:
-      if (lookahead == 'r') ADVANCE(706);
+      if (lookahead == 'r') ADVANCE(283);
       END_STATE();
     case 785:
-      if (lookahead == 'r') ADVANCE(284);
+      if (lookahead == 'r') ADVANCE(828);
       END_STATE();
     case 786:
-      if (lookahead == 'r') ADVANCE(829);
+      if (lookahead == 'r') ADVANCE(620);
       END_STATE();
     case 787:
-      if (lookahead == 'r') ADVANCE(621);
+      if (lookahead == 'r') ADVANCE(287);
       END_STATE();
     case 788:
-      if (lookahead == 'r') ADVANCE(288);
+      if (lookahead == 'r') ADVANCE(358);
       END_STATE();
     case 789:
-      if (lookahead == 'r') ADVANCE(359);
+      if (lookahead == 'r') ADVANCE(293);
       END_STATE();
     case 790:
-      if (lookahead == 'r') ADVANCE(294);
+      if (lookahead == 'r') ADVANCE(295);
       END_STATE();
     case 791:
       if (lookahead == 'r') ADVANCE(296);
       END_STATE();
     case 792:
-      if (lookahead == 'r') ADVANCE(297);
+      if (lookahead == 'r') ADVANCE(645);
       END_STATE();
     case 793:
-      if (lookahead == 'r') ADVANCE(646);
+      if (lookahead == 'r') ADVANCE(637);
       END_STATE();
     case 794:
-      if (lookahead == 'r') ADVANCE(638);
+      if (lookahead == 'r') ADVANCE(360);
       END_STATE();
     case 795:
-      if (lookahead == 'r') ADVANCE(361);
+      if (lookahead == 'r') ADVANCE(275);
       END_STATE();
     case 796:
-      if (lookahead == 'r') ADVANCE(276);
+      if (lookahead == 'r') ADVANCE(473);
       END_STATE();
     case 797:
-      if (lookahead == 'r') ADVANCE(474);
+      if (lookahead == 'r') ADVANCE(589);
       END_STATE();
     case 798:
-      if (lookahead == 'r') ADVANCE(590);
+      if (lookahead == 'r') ADVANCE(627);
       END_STATE();
     case 799:
-      if (lookahead == 'r') ADVANCE(628);
+      if (lookahead == 'r') ADVANCE(456);
       END_STATE();
     case 800:
-      if (lookahead == 'r') ADVANCE(457);
+      if (lookahead == 'r') ADVANCE(560);
       END_STATE();
     case 801:
-      if (lookahead == 'r') ADVANCE(561);
+      if (lookahead == 'r') ADVANCE(837);
       END_STATE();
     case 802:
-      if (lookahead == 'r') ADVANCE(838);
+      if (lookahead == 'r') ADVANCE(601);
       END_STATE();
     case 803:
-      if (lookahead == 'r') ADVANCE(602);
+      if (lookahead == 'r') ADVANCE(839);
       END_STATE();
     case 804:
-      if (lookahead == 'r') ADVANCE(840);
+      if (lookahead == 'r') ADVANCE(950);
       END_STATE();
     case 805:
-      if (lookahead == 'r') ADVANCE(951);
+      if (lookahead == 'r') ADVANCE(710);
       END_STATE();
     case 806:
-      if (lookahead == 'r') ADVANCE(711);
+      if (lookahead == 'r') ADVANCE(266);
       END_STATE();
     case 807:
       if (lookahead == 'r') ADVANCE(267);
       END_STATE();
     case 808:
-      if (lookahead == 'r') ADVANCE(268);
+      if (lookahead == 'r') ADVANCE(269);
       END_STATE();
     case 809:
       if (lookahead == 'r') ADVANCE(270);
       END_STATE();
     case 810:
-      if (lookahead == 'r') ADVANCE(271);
+      if (lookahead == 'r') ADVANCE(83);
       END_STATE();
     case 811:
-      if (lookahead == 'r') ADVANCE(81);
+      if (lookahead == 'r') ADVANCE(110);
       END_STATE();
     case 812:
-      if (lookahead == 'r') ADVANCE(111);
+      if (lookahead == 's') ADVANCE(970);
       END_STATE();
     case 813:
-      if (lookahead == 's') ADVANCE(971);
+      if (lookahead == 's') ADVANCE(1152);
       END_STATE();
     case 814:
-      if (lookahead == 's') ADVANCE(1153);
+      if (lookahead == 's') ADVANCE(1086);
       END_STATE();
     case 815:
-      if (lookahead == 's') ADVANCE(1087);
+      if (lookahead == 's') ADVANCE(1210);
       END_STATE();
     case 816:
-      if (lookahead == 's') ADVANCE(1211);
+      if (lookahead == 's') ADVANCE(1069);
       END_STATE();
     case 817:
-      if (lookahead == 's') ADVANCE(1070);
+      if (lookahead == 's') ADVANCE(971);
       END_STATE();
     case 818:
-      if (lookahead == 's') ADVANCE(972);
+      if (lookahead == 's') ADVANCE(1153);
       END_STATE();
     case 819:
-      if (lookahead == 's') ADVANCE(1154);
+      if (lookahead == 's') ADVANCE(1076);
       END_STATE();
     case 820:
-      if (lookahead == 's') ADVANCE(1077);
+      if (lookahead == 's') ADVANCE(1158);
       END_STATE();
     case 821:
-      if (lookahead == 's') ADVANCE(1159);
+      if (lookahead == 's') ADVANCE(998);
       END_STATE();
     case 822:
-      if (lookahead == 's') ADVANCE(999);
+      if (lookahead == 's') ADVANCE(1053);
       END_STATE();
     case 823:
-      if (lookahead == 's') ADVANCE(1054);
+      if (lookahead == 's') ADVANCE(1160);
       END_STATE();
     case 824:
-      if (lookahead == 's') ADVANCE(1161);
+      if (lookahead == 's') ADVANCE(999);
       END_STATE();
     case 825:
-      if (lookahead == 's') ADVANCE(1000);
+      if (lookahead == 's') ADVANCE(1011);
       END_STATE();
     case 826:
-      if (lookahead == 's') ADVANCE(1012);
+      if (lookahead == 's') ADVANCE(1159);
       END_STATE();
     case 827:
-      if (lookahead == 's') ADVANCE(1160);
+      if (lookahead == 's') ADVANCE(1004);
       END_STATE();
     case 828:
-      if (lookahead == 's') ADVANCE(1005);
+      if (lookahead == 's') ADVANCE(1033);
       END_STATE();
     case 829:
-      if (lookahead == 's') ADVANCE(1034);
+      if (lookahead == 's') ADVANCE(862);
       END_STATE();
     case 830:
-      if (lookahead == 's') ADVANCE(863);
+      if (lookahead == 's') ADVANCE(407);
       END_STATE();
     case 831:
-      if (lookahead == 's') ADVANCE(408);
+      if (lookahead == 's') ADVANCE(860);
       END_STATE();
     case 832:
-      if (lookahead == 's') ADVANCE(861);
+      if (lookahead == 's') ADVANCE(731);
       END_STATE();
     case 833:
-      if (lookahead == 's') ADVANCE(732);
+      if (lookahead == 's') ADVANCE(835);
       END_STATE();
     case 834:
-      if (lookahead == 's') ADVANCE(836);
+      if (lookahead == 's') ADVANCE(409);
       END_STATE();
     case 835:
-      if (lookahead == 's') ADVANCE(410);
+      if (lookahead == 's') ADVANCE(163);
       END_STATE();
     case 836:
-      if (lookahead == 's') ADVANCE(164);
+      if (lookahead == 's') ADVANCE(819);
       END_STATE();
     case 837:
-      if (lookahead == 's') ADVANCE(820);
+      if (lookahead == 's') ADVANCE(381);
       END_STATE();
     case 838:
-      if (lookahead == 's') ADVANCE(382);
+      if (lookahead == 's') ADVANCE(290);
       END_STATE();
     case 839:
-      if (lookahead == 's') ADVANCE(291);
+      if (lookahead == 's') ADVANCE(292);
       END_STATE();
     case 840:
-      if (lookahead == 's') ADVANCE(293);
+      if (lookahead == 's') ADVANCE(339);
       END_STATE();
     case 841:
-      if (lookahead == 's') ADVANCE(340);
+      if (lookahead == 's') ADVANCE(866);
       END_STATE();
     case 842:
-      if (lookahead == 's') ADVANCE(867);
+      if (lookahead == 's') ADVANCE(347);
       END_STATE();
     case 843:
-      if (lookahead == 's') ADVANCE(348);
+      if (lookahead == 's') ADVANCE(169);
       END_STATE();
     case 844:
-      if (lookahead == 's') ADVANCE(170);
+      if (lookahead == 's') ADVANCE(171);
       END_STATE();
     case 845:
-      if (lookahead == 's') ADVANCE(172);
+      if (lookahead == 's') ADVANCE(843);
       END_STATE();
     case 846:
       if (lookahead == 's') ADVANCE(844);
       END_STATE();
     case 847:
-      if (lookahead == 's') ADVANCE(845);
+      if (lookahead == 's') ADVANCE(375);
       END_STATE();
     case 848:
-      if (lookahead == 's') ADVANCE(376);
+      if (lookahead == 't') ADVANCE(1196);
       END_STATE();
     case 849:
-      if (lookahead == 't') ADVANCE(1197);
+      if (lookahead == 't') ADVANCE(1195);
       END_STATE();
     case 850:
-      if (lookahead == 't') ADVANCE(1196);
+      if (lookahead == 't') ADVANCE(1078);
       END_STATE();
     case 851:
-      if (lookahead == 't') ADVANCE(1079);
+      if (lookahead == 't') ADVANCE(1114);
       END_STATE();
     case 852:
-      if (lookahead == 't') ADVANCE(1115);
+      if (lookahead == 't') ADVANCE(1127);
       END_STATE();
     case 853:
-      if (lookahead == 't') ADVANCE(1128);
+      if (lookahead == 't') ADVANCE(1043);
       END_STATE();
     case 854:
-      if (lookahead == 't') ADVANCE(1044);
+      if (lookahead == 't') ADVANCE(1061);
       END_STATE();
     case 855:
-      if (lookahead == 't') ADVANCE(1062);
+      if (lookahead == 't') ADVANCE(1110);
       END_STATE();
     case 856:
-      if (lookahead == 't') ADVANCE(1111);
+      if (lookahead == 't') ADVANCE(1100);
       END_STATE();
     case 857:
-      if (lookahead == 't') ADVANCE(1101);
+      if (lookahead == 't') ADVANCE(1035);
       END_STATE();
     case 858:
-      if (lookahead == 't') ADVANCE(1036);
+      if (lookahead == 't') ADVANCE(336);
       END_STATE();
     case 859:
-      if (lookahead == 't') ADVANCE(337);
+      if (lookahead == 't') ADVANCE(949);
       END_STATE();
     case 860:
-      if (lookahead == 't') ADVANCE(950);
+      if (lookahead == 't') ADVANCE(734);
       END_STATE();
     case 861:
-      if (lookahead == 't') ADVANCE(735);
+      if (lookahead == 't') ADVANCE(140);
       END_STATE();
     case 862:
-      if (lookahead == 't') ADVANCE(141);
+      if (lookahead == 't') ADVANCE(813);
       END_STATE();
     case 863:
-      if (lookahead == 't') ADVANCE(814);
+      if (lookahead == 't') ADVANCE(622);
       END_STATE();
     case 864:
-      if (lookahead == 't') ADVANCE(623);
+      if (lookahead == 't') ADVANCE(260);
       END_STATE();
     case 865:
-      if (lookahead == 't') ADVANCE(261);
+      if (lookahead == 't') ADVANCE(411);
       END_STATE();
     case 866:
-      if (lookahead == 't') ADVANCE(412);
+      if (lookahead == 't') ADVANCE(818);
       END_STATE();
     case 867:
-      if (lookahead == 't') ADVANCE(819);
+      if (lookahead == 't') ADVANCE(655);
       END_STATE();
     case 868:
-      if (lookahead == 't') ADVANCE(656);
+      if (lookahead == 't') ADVANCE(152);
       END_STATE();
     case 869:
-      if (lookahead == 't') ADVANCE(153);
+      if (lookahead == 't') ADVANCE(132);
       END_STATE();
     case 870:
-      if (lookahead == 't') ADVANCE(133);
+      if (lookahead == 't') ADVANCE(332);
       END_STATE();
     case 871:
-      if (lookahead == 't') ADVANCE(333);
+      if (lookahead == 't') ADVANCE(825);
       END_STATE();
     case 872:
-      if (lookahead == 't') ADVANCE(826);
+      if (lookahead == 't') ADVANCE(827);
       END_STATE();
     case 873:
-      if (lookahead == 't') ADVANCE(828);
+      if (lookahead == 't') ADVANCE(286);
       END_STATE();
     case 874:
-      if (lookahead == 't') ADVANCE(287);
+      if (lookahead == 't') ADVANCE(766);
       END_STATE();
     case 875:
-      if (lookahead == 't') ADVANCE(767);
+      if (lookahead == 't') ADVANCE(769);
       END_STATE();
     case 876:
-      if (lookahead == 't') ADVANCE(770);
+      if (lookahead == 't') ADVANCE(156);
       END_STATE();
     case 877:
-      if (lookahead == 't') ADVANCE(157);
+      if (lookahead == 't') ADVANCE(299);
       END_STATE();
     case 878:
-      if (lookahead == 't') ADVANCE(300);
+      if (lookahead == 't') ADVANCE(621);
       END_STATE();
     case 879:
-      if (lookahead == 't') ADVANCE(622);
+      if (lookahead == 't') ADVANCE(345);
       END_STATE();
     case 880:
-      if (lookahead == 't') ADVANCE(346);
+      if (lookahead == 't') ADVANCE(899);
       END_STATE();
     case 881:
-      if (lookahead == 't') ADVANCE(900);
+      if (lookahead == 't') ADVANCE(424);
       END_STATE();
     case 882:
-      if (lookahead == 't') ADVANCE(425);
+      if (lookahead == 't') ADVANCE(914);
       END_STATE();
     case 883:
-      if (lookahead == 't') ADVANCE(915);
+      if (lookahead == 't') ADVANCE(876);
       END_STATE();
     case 884:
-      if (lookahead == 't') ADVANCE(877);
+      if (lookahead == 't') ADVANCE(672);
       END_STATE();
     case 885:
-      if (lookahead == 't') ADVANCE(673);
+      if (lookahead == 't') ADVANCE(684);
       END_STATE();
     case 886:
-      if (lookahead == 't') ADVANCE(685);
+      if (lookahead == 't') ADVANCE(714);
       END_STATE();
     case 887:
-      if (lookahead == 't') ADVANCE(715);
+      if (lookahead == 't') ADVANCE(78);
       END_STATE();
     case 888:
-      if (lookahead == 't') ADVANCE(76);
+      if (lookahead == 't') ADVANCE(84);
       END_STATE();
     case 889:
-      if (lookahead == 't') ADVANCE(82);
+      if (lookahead == 't') ADVANCE(85);
       END_STATE();
     case 890:
-      if (lookahead == 't') ADVANCE(83);
+      if (lookahead == 't') ADVANCE(88);
       END_STATE();
     case 891:
-      if (lookahead == 't') ADVANCE(86);
+      if (lookahead == 't') ADVANCE(91);
       END_STATE();
     case 892:
-      if (lookahead == 't') ADVANCE(89);
+      if (lookahead == 't') ADVANCE(179);
       END_STATE();
     case 893:
-      if (lookahead == 't') ADVANCE(180);
+      if (lookahead == 'u') ADVANCE(317);
       END_STATE();
     case 894:
-      if (lookahead == 'u') ADVANCE(318);
+      if (lookahead == 'u') ADVANCE(830);
       END_STATE();
     case 895:
-      if (lookahead == 'u') ADVANCE(831);
+      if (lookahead == 'u') ADVANCE(561);
       END_STATE();
     case 896:
-      if (lookahead == 'u') ADVANCE(562);
+      if (lookahead == 'u') ADVANCE(720);
       END_STATE();
     case 897:
-      if (lookahead == 'u') ADVANCE(721);
+      if (lookahead == 'u') ADVANCE(864);
       END_STATE();
     case 898:
-      if (lookahead == 'u') ADVANCE(865);
+      if (lookahead == 'u') ADVANCE(523);
       END_STATE();
     case 899:
-      if (lookahead == 'u') ADVANCE(524);
+      if (lookahead == 'u') ADVANCE(739);
       END_STATE();
     case 900:
-      if (lookahead == 'u') ADVANCE(740);
+      if (lookahead == 'u') ADVANCE(814);
       END_STATE();
     case 901:
-      if (lookahead == 'u') ADVANCE(815);
+      if (lookahead == 'u') ADVANCE(721);
       END_STATE();
     case 902:
       if (lookahead == 'u') ADVANCE(722);
       END_STATE();
     case 903:
-      if (lookahead == 'u') ADVANCE(723);
+      if (lookahead == 'u') ADVANCE(799);
       END_STATE();
     case 904:
-      if (lookahead == 'u') ADVANCE(800);
+      if (lookahead == 'u') ADVANCE(611);
       END_STATE();
     case 905:
-      if (lookahead == 'u') ADVANCE(612);
+      if (lookahead == 'u') ADVANCE(723);
       END_STATE();
     case 906:
       if (lookahead == 'u') ADVANCE(724);
       END_STATE();
     case 907:
-      if (lookahead == 'u') ADVANCE(725);
+      if (lookahead == 'u') ADVANCE(852);
       END_STATE();
     case 908:
-      if (lookahead == 'u') ADVANCE(853);
+      if (lookahead == 'u') ADVANCE(881);
       END_STATE();
     case 909:
-      if (lookahead == 'u') ADVANCE(882);
+      if (lookahead == 'u') ADVANCE(632);
       END_STATE();
     case 910:
-      if (lookahead == 'u') ADVANCE(633);
+      if (lookahead == 'u') ADVANCE(316);
       END_STATE();
     case 911:
-      if (lookahead == 'u') ADVANCE(317);
+      if (lookahead == 'u') ADVANCE(774);
       END_STATE();
     case 912:
-      if (lookahead == 'u') ADVANCE(775);
+      if (lookahead == 'u') ADVANCE(525);
       END_STATE();
     case 913:
-      if (lookahead == 'u') ADVANCE(526);
+      if (lookahead == 'u') ADVANCE(590);
       END_STATE();
     case 914:
-      if (lookahead == 'u') ADVANCE(591);
+      if (lookahead == 'u') ADVANCE(791);
       END_STATE();
     case 915:
-      if (lookahead == 'u') ADVANCE(792);
+      if (lookahead == 'u') ADVANCE(890);
       END_STATE();
     case 916:
-      if (lookahead == 'u') ADVANCE(891);
+      if (lookahead == 'v') ADVANCE(1198);
       END_STATE();
     case 917:
-      if (lookahead == 'v') ADVANCE(1199);
+      if (lookahead == 'v') ADVANCE(1200);
       END_STATE();
     case 918:
-      if (lookahead == 'v') ADVANCE(1201);
+      if (lookahead == 'v') ADVANCE(460);
       END_STATE();
     case 919:
-      if (lookahead == 'v') ADVANCE(461);
+      if (lookahead == 'v') ADVANCE(477);
       END_STATE();
     case 920:
-      if (lookahead == 'v') ADVANCE(478);
+      if (lookahead == 'v') ADVANCE(374);
       END_STATE();
     case 921:
-      if (lookahead == 'v') ADVANCE(375);
+      if (lookahead == 'v') ADVANCE(379);
       END_STATE();
     case 922:
-      if (lookahead == 'v') ADVANCE(380);
+      if (lookahead == 'v') ADVANCE(461);
       END_STATE();
     case 923:
-      if (lookahead == 'v') ADVANCE(462);
+      if (lookahead == 'v') ADVANCE(79);
       END_STATE();
     case 924:
-      if (lookahead == 'v') ADVANCE(77);
+      if (lookahead == 'v') ADVANCE(376);
       END_STATE();
     case 925:
-      if (lookahead == 'v') ADVANCE(377);
+      if (lookahead == 'v') ADVANCE(380);
       END_STATE();
     case 926:
-      if (lookahead == 'v') ADVANCE(381);
+      if (lookahead == 'w') ADVANCE(1118);
       END_STATE();
     case 927:
-      if (lookahead == 'w') ADVANCE(1119);
+      if (lookahead == 'w') ADVANCE(1012);
       END_STATE();
     case 928:
-      if (lookahead == 'w') ADVANCE(1013);
+      if (lookahead == 'w') ADVANCE(1104);
       END_STATE();
     case 929:
-      if (lookahead == 'w') ADVANCE(1105);
+      if (lookahead == 'w') ADVANCE(1013);
       END_STATE();
     case 930:
-      if (lookahead == 'w') ADVANCE(1014);
+      if (lookahead == 'w') ADVANCE(1161);
       END_STATE();
     case 931:
       if (lookahead == 'w') ADVANCE(1162);
       END_STATE();
     case 932:
-      if (lookahead == 'w') ADVANCE(1163);
+      if (lookahead == 'w') ADVANCE(842);
       END_STATE();
     case 933:
-      if (lookahead == 'w') ADVANCE(843);
+      if (lookahead == 'w') ADVANCE(610);
       END_STATE();
     case 934:
-      if (lookahead == 'w') ADVANCE(611);
+      if (lookahead == 'x') ADVANCE(1022);
       END_STATE();
     case 935:
-      if (lookahead == 'x') ADVANCE(1023);
+      if (lookahead == 'x') ADVANCE(1021);
       END_STATE();
     case 936:
-      if (lookahead == 'x') ADVANCE(1022);
+      if (lookahead == 'x') ADVANCE(1182);
       END_STATE();
     case 937:
       if (lookahead == 'x') ADVANCE(1183);
       END_STATE();
     case 938:
-      if (lookahead == 'x') ADVANCE(1184);
+      if (lookahead == 'x') ADVANCE(1141);
       END_STATE();
     case 939:
-      if (lookahead == 'x') ADVANCE(1142);
+      if (lookahead == 'x') ADVANCE(1019);
       END_STATE();
     case 940:
-      if (lookahead == 'x') ADVANCE(1020);
+      if (lookahead == 'x') ADVANCE(72);
       END_STATE();
     case 941:
-      if (lookahead == 'x') ADVANCE(70);
+      if (lookahead == 'x') ADVANCE(71);
       END_STATE();
     case 942:
-      if (lookahead == 'x') ADVANCE(69);
+      if (lookahead == 'x') ADVANCE(335);
       END_STATE();
     case 943:
-      if (lookahead == 'x') ADVANCE(336);
+      if (lookahead == 'x') ADVANCE(341);
       END_STATE();
     case 944:
-      if (lookahead == 'x') ADVANCE(342);
+      if (lookahead == 'x') ADVANCE(346);
       END_STATE();
     case 945:
-      if (lookahead == 'x') ADVANCE(347);
+      if (lookahead == 'y') ADVANCE(1037);
       END_STATE();
     case 946:
-      if (lookahead == 'y') ADVANCE(1038);
+      if (lookahead == 'y') ADVANCE(1026);
       END_STATE();
     case 947:
-      if (lookahead == 'y') ADVANCE(1027);
+      if (lookahead == 'y') ADVANCE(1106);
       END_STATE();
     case 948:
-      if (lookahead == 'y') ADVANCE(1107);
+      if (lookahead == 'y') ADVANCE(728);
       END_STATE();
     case 949:
-      if (lookahead == 'y') ADVANCE(729);
+      if (lookahead == 'y') ADVANCE(101);
       END_STATE();
     case 950:
-      if (lookahead == 'y') ADVANCE(102);
+      if (lookahead == 'y') ADVANCE(733);
       END_STATE();
     case 951:
-      if (lookahead == 'y') ADVANCE(734);
+      if (lookahead == 'y') ADVANCE(80);
       END_STATE();
     case 952:
-      if (lookahead == 'y') ADVANCE(78);
+      if (lookahead == 'z') ADVANCE(300);
       END_STATE();
     case 953:
-      if (lookahead == 'z') ADVANCE(301);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1124);
       END_STATE();
     case 954:
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1125);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1123);
       END_STATE();
     case 955:
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1124);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(954);
       END_STATE();
     case 956:
       if (('0' <= lookahead && lookahead <= '9')) ADVANCE(955);
       END_STATE();
     case 957:
       if (('0' <= lookahead && lookahead <= '9')) ADVANCE(956);
       END_STATE();
     case 958:
       if (('0' <= lookahead && lookahead <= '9')) ADVANCE(957);
       END_STATE();
     case 959:
       if (('0' <= lookahead && lookahead <= '9')) ADVANCE(958);
       END_STATE();
     case 960:
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(959);
+      if (eof) ADVANCE(965);
+      if (lookahead == '\n') SKIP(0)
       END_STATE();
     case 961:
-      if (eof) ADVANCE(966);
+      if (eof) ADVANCE(965);
       if (lookahead == '\n') SKIP(0)
+      if (lookahead == '\r') SKIP(960)
       END_STATE();
     case 962:
-      if (eof) ADVANCE(966);
-      if (lookahead == '\n') SKIP(0)
-      if (lookahead == '\r') SKIP(961)
+      if (eof) ADVANCE(965);
+      if (lookahead == '\n') SKIP(964)
       END_STATE();
     case 963:
-      if (eof) ADVANCE(966);
-      if (lookahead == '\n') SKIP(965)
+      if (eof) ADVANCE(965);
+      if (lookahead == '\n') SKIP(964)
+      if (lookahead == '\r') SKIP(962)
       END_STATE();
     case 964:
-      if (eof) ADVANCE(966);
-      if (lookahead == '\n') SKIP(965)
-      if (lookahead == '\r') SKIP(963)
-      END_STATE();
-    case 965:
-      if (eof) ADVANCE(966);
-      if (lookahead == '\n') ADVANCE(1533);
+      if (eof) ADVANCE(965);
+      if (lookahead == '\n') ADVANCE(1526);
       if (lookahead == '\r') ADVANCE(3);
-      if (lookahead == '#') ADVANCE(1530);
-      if (lookahead == ',') ADVANCE(970);
-      if (lookahead == '\\') SKIP(964)
-      if (lookahead == 'a') ADVANCE(200);
-      if (lookahead == 'b') ADVANCE(446);
-      if (lookahead == 'c') ADVANCE(231);
-      if (lookahead == 'e') ADVANCE(204);
-      if (lookahead == 'f') ADVANCE(205);
-      if (lookahead == 'g') ADVANCE(799);
-      if (lookahead == 'h') ADVANCE(277);
-      if (lookahead == 'i') ADVANCE(209);
-      if (lookahead == 'l') ADVANCE(444);
-      if (lookahead == 'm') ADVANCE(175);
-      if (lookahead == 'n') ADVANCE(123);
-      if (lookahead == 'o') ADVANCE(728);
-      if (lookahead == 'p') ADVANCE(895);
-      if (lookahead == 'r') ADVANCE(305);
-      if (lookahead == 's') ADVANCE(128);
-      if (lookahead == 't') ADVANCE(475);
-      if (lookahead == 'u') ADVANCE(573);
+      if (lookahead == '#') ADVANCE(1523);
+      if (lookahead == ',') ADVANCE(969);
+      if (lookahead == '\\') SKIP(963)
+      if (lookahead == 'a') ADVANCE(199);
+      if (lookahead == 'b') ADVANCE(445);
+      if (lookahead == 'c') ADVANCE(230);
+      if (lookahead == 'e') ADVANCE(203);
+      if (lookahead == 'f') ADVANCE(204);
+      if (lookahead == 'g') ADVANCE(798);
+      if (lookahead == 'h') ADVANCE(276);
+      if (lookahead == 'i') ADVANCE(208);
+      if (lookahead == 'l') ADVANCE(443);
+      if (lookahead == 'm') ADVANCE(174);
+      if (lookahead == 'n') ADVANCE(122);
+      if (lookahead == 'o') ADVANCE(727);
+      if (lookahead == 'p') ADVANCE(894);
+      if (lookahead == 'r') ADVANCE(304);
+      if (lookahead == 's') ADVANCE(127);
+      if (lookahead == 't') ADVANCE(474);
+      if (lookahead == 'u') ADVANCE(572);
       if (lookahead == '\t' ||
-          lookahead == ' ') ADVANCE(1537);
+          lookahead == ' ') ADVANCE(1531);
       if (lookahead == 11 ||
-          lookahead == '\f') SKIP(965)
+          lookahead == '\f') SKIP(964)
       END_STATE();
-    case 966:
+    case 965:
       ACCEPT_TOKEN(ts_builtin_sym_end);
       END_STATE();
-    case 967:
+    case 966:
       ACCEPT_TOKEN(anon_sym_account_DASHhook);
       END_STATE();
-    case 968:
+    case 967:
       ACCEPT_TOKEN(anon_sym_DASHgroup);
       END_STATE();
-    case 969:
+    case 968:
       ACCEPT_TOKEN(anon_sym_DASHgroup);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 970:
+    case 969:
       ACCEPT_TOKEN(anon_sym_COMMA);
       END_STATE();
-    case 971:
+    case 970:
       ACCEPT_TOKEN(anon_sym_alias);
       END_STATE();
-    case 972:
+    case 971:
       ACCEPT_TOKEN(anon_sym_unalias);
       END_STATE();
-    case 973:
+    case 972:
       ACCEPT_TOKEN(anon_sym_STAR);
       END_STATE();
-    case 974:
+    case 973:
       ACCEPT_TOKEN(anon_sym_STAR);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 975:
+    case 974:
       ACCEPT_TOKEN(anon_sym_LT);
       END_STATE();
-    case 976:
+    case 975:
       ACCEPT_TOKEN(anon_sym_LT);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 977:
+    case 976:
       ACCEPT_TOKEN(aux_sym_key_token1);
       if (lookahead == '-' ||
           ('A' <= lookahead && lookahead <= 'Z') ||
-          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(977);
+          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(976);
       END_STATE();
-    case 978:
+    case 977:
       ACCEPT_TOKEN(anon_sym_GT);
       END_STATE();
+    case 978:
+      ACCEPT_TOKEN(aux_sym_key_token2);
+      END_STATE();
     case 979:
       ACCEPT_TOKEN(aux_sym_key_token2);
+      if (lookahead == '\t') ADVANCE(979);
+      if (lookahead == '\n') ADVANCE(1525);
+      if (lookahead == '\r') ADVANCE(979);
+      if (lookahead == ' ') ADVANCE(1530);
+      if (lookahead == '#') ADVANCE(990);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(30);
+      if (lookahead == 11 ||
+          lookahead == '\f') ADVANCE(979);
+      if (lookahead != 0) ADVANCE(978);
       END_STATE();
     case 980:
       ACCEPT_TOKEN(aux_sym_key_token2);
-      if (lookahead == '\t') ADVANCE(980);
-      if (lookahead == '\n') ADVANCE(1532);
-      if (lookahead == '\r') ADVANCE(980);
-      if (lookahead == ' ') ADVANCE(1536);
-      if (lookahead == '#') ADVANCE(991);
+      if (lookahead == '"') ADVANCE(1223);
+      if (lookahead == '\'') ADVANCE(1216);
       if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(31);
-      if (lookahead == 11 ||
-          lookahead == '\f') ADVANCE(980);
-      if (lookahead != 0) ADVANCE(979);
+      if (lookahead == '\\') ADVANCE(1256);
+      if (lookahead == '`') ADVANCE(1230);
+      if (lookahead == '\t' ||
+          (11 <= lookahead && lookahead <= '\r')) ADVANCE(980);
+      if (lookahead != 0 &&
+          lookahead != '\n' &&
+          lookahead != ' ') ADVANCE(987);
       END_STATE();
     case 981:
       ACCEPT_TOKEN(aux_sym_key_token2);
-      if (lookahead == '\n') ADVANCE(1240);
-      if (lookahead == '"') ADVANCE(1224);
-      if (lookahead == '\'') ADVANCE(1217);
-      if (lookahead == '<') ADVANCE(976);
-      if (lookahead == '\\') ADVANCE(1274);
-      if (lookahead == '`') ADVANCE(1231);
-      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(981);
+      if (lookahead == '*') ADVANCE(972);
+      if (lookahead == '-') ADVANCE(988);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(21);
+      if (lookahead == '\t' ||
+          (11 <= lookahead && lookahead <= '\r')) ADVANCE(981);
       if (lookahead != 0 &&
-          lookahead != ' ') ADVANCE(988);
+          lookahead != '\n' &&
+          lookahead != ' ') ADVANCE(978);
       END_STATE();
     case 982:
       ACCEPT_TOKEN(aux_sym_key_token2);
-      if (lookahead == '*') ADVANCE(973);
-      if (lookahead == '-') ADVANCE(989);
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(27);
+      if (lookahead == '*') ADVANCE(972);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(33);
       if (lookahead == '\t' ||
           (11 <= lookahead && lookahead <= '\r')) ADVANCE(982);
       if (lookahead != 0 &&
           lookahead != '\n' &&
-          lookahead != ' ') ADVANCE(979);
+          lookahead != ' ') ADVANCE(978);
       END_STATE();
     case 983:
       ACCEPT_TOKEN(aux_sym_key_token2);
-      if (lookahead == '*') ADVANCE(973);
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(34);
+      if (lookahead == ',') ADVANCE(969);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(36);
       if (lookahead == '\t' ||
           (11 <= lookahead && lookahead <= '\r')) ADVANCE(983);
       if (lookahead != 0 &&
           lookahead != '\n' &&
-          lookahead != ' ') ADVANCE(979);
+          lookahead != ' ') ADVANCE(978);
       END_STATE();
     case 984:
       ACCEPT_TOKEN(aux_sym_key_token2);
-      if (lookahead == ',') ADVANCE(970);
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(37);
+      if (lookahead == '-') ADVANCE(988);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(28);
       if (lookahead == '\t' ||
           (11 <= lookahead && lookahead <= '\r')) ADVANCE(984);
       if (lookahead != 0 &&
           lookahead != '\n' &&
-          lookahead != ' ') ADVANCE(979);
+          lookahead != ' ') ADVANCE(978);
       END_STATE();
     case 985:
       ACCEPT_TOKEN(aux_sym_key_token2);
-      if (lookahead == '-') ADVANCE(989);
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(30);
+      if (lookahead == '<') ADVANCE(974);
+      if (lookahead == '\\') ADVANCE(34);
       if (lookahead == '\t' ||
           (11 <= lookahead && lookahead <= '\r')) ADVANCE(985);
       if (lookahead != 0 &&
           lookahead != '\n' &&
-          lookahead != ' ') ADVANCE(979);
+          lookahead != ' ') ADVANCE(978);
       END_STATE();
     case 986:
       ACCEPT_TOKEN(aux_sym_key_token2);
-      if (lookahead == '<') ADVANCE(975);
+      if (lookahead == '<') ADVANCE(974);
       if (lookahead == '\\') ADVANCE(35);
       if (lookahead == '\t' ||
           (11 <= lookahead && lookahead <= '\r')) ADVANCE(986);
+      if (lookahead == '-' ||
+          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(989);
       if (lookahead != 0 &&
           lookahead != '\n' &&
-          lookahead != ' ') ADVANCE(979);
+          lookahead != ' ') ADVANCE(978);
       END_STATE();
     case 987:
       ACCEPT_TOKEN(aux_sym_key_token2);
-      if (lookahead == '<') ADVANCE(975);
-      if (lookahead == '\\') ADVANCE(36);
-      if (lookahead == '\t' ||
-          (11 <= lookahead && lookahead <= '\r')) ADVANCE(987);
-      if (lookahead == '-' ||
-          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(990);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
-          lookahead != '\n' &&
-          lookahead != ' ') ADVANCE(979);
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 988:
       ACCEPT_TOKEN(aux_sym_key_token2);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+      if (lookahead == 'g') ADVANCE(805);
       END_STATE();
     case 989:
       ACCEPT_TOKEN(aux_sym_key_token2);
-      if (lookahead == 'g') ADVANCE(806);
+      if (lookahead == '-' ||
+          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1028);
       END_STATE();
     case 990:
       ACCEPT_TOKEN(aux_sym_key_token2);
-      if (lookahead == '-' ||
-          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1029);
+      if (lookahead != 0 &&
+          lookahead != '\n') ADVANCE(1523);
       END_STATE();
     case 991:
-      ACCEPT_TOKEN(aux_sym_key_token2);
-      if (lookahead != 0 &&
-          lookahead != '\n') ADVANCE(1530);
+      ACCEPT_TOKEN(aux_sym_key_token3);
       END_STATE();
     case 992:
       ACCEPT_TOKEN(aux_sym_key_token3);
+      if (lookahead == '\n') ADVANCE(1286);
       END_STATE();
     case 993:
       ACCEPT_TOKEN(aux_sym_key_token3);
-      if (lookahead == '\n') ADVANCE(1273);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 994:
       ACCEPT_TOKEN(aux_sym_key_token3);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 995:
-      ACCEPT_TOKEN(aux_sym_key_token3);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
+      ACCEPT_TOKEN(anon_sym_SPACE);
+      if (lookahead == '\t') ADVANCE(1529);
+      if (lookahead == '\n') ADVANCE(1524);
+      if (lookahead == '\r') ADVANCE(1);
+      if (lookahead == ' ') ADVANCE(995);
       END_STATE();
     case 996:
       ACCEPT_TOKEN(anon_sym_SPACE);
-      if (lookahead == '\t') ADVANCE(1535);
-      if (lookahead == '\n') ADVANCE(1531);
-      if (lookahead == '\r') ADVANCE(1);
       if (lookahead == ' ') ADVANCE(996);
       END_STATE();
     case 997:
       ACCEPT_TOKEN(anon_sym_SPACE);
-      if (lookahead == '\n') ADVANCE(1239);
       if (lookahead == ' ') ADVANCE(997);
-      if (lookahead == '\\') ADVANCE(1255);
+      if (lookahead == '\\') ADVANCE(1241);
       END_STATE();
     case 998:
-      ACCEPT_TOKEN(anon_sym_SPACE);
-      if (lookahead == ' ') ADVANCE(998);
-      END_STATE();
-    case 999:
       ACCEPT_TOKEN(anon_sym_alternates);
       END_STATE();
-    case 1000:
+    case 999:
       ACCEPT_TOKEN(anon_sym_unalternates);
       END_STATE();
-    case 1001:
+    case 1000:
       ACCEPT_TOKEN(anon_sym_alternative_order);
       END_STATE();
-    case 1002:
+    case 1001:
       ACCEPT_TOKEN(anon_sym_unalternative_order);
       END_STATE();
-    case 1003:
+    case 1002:
       ACCEPT_TOKEN(sym_mime_type);
       if (lookahead == '-' ||
           lookahead == '.' ||
           ('0' <= lookahead && lookahead <= '9') ||
           ('A' <= lookahead && lookahead <= 'Z') ||
-          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1003);
+          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1002);
       END_STATE();
-    case 1004:
+    case 1003:
       ACCEPT_TOKEN(anon_sym_SLASH);
       END_STATE();
-    case 1005:
+    case 1004:
       ACCEPT_TOKEN(anon_sym_attachments);
       END_STATE();
-    case 1006:
+    case 1005:
       ACCEPT_TOKEN(anon_sym_PLUS);
       END_STATE();
-    case 1007:
+    case 1006:
       ACCEPT_TOKEN(anon_sym_PLUS);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1008:
+    case 1007:
       ACCEPT_TOKEN(anon_sym_DASH);
       END_STATE();
-    case 1009:
+    case 1008:
       ACCEPT_TOKEN(anon_sym_DASH);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1010:
+    case 1009:
       ACCEPT_TOKEN(anon_sym_QMARK);
       END_STATE();
-    case 1011:
+    case 1010:
       ACCEPT_TOKEN(anon_sym_QMARK);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1012:
+    case 1011:
       ACCEPT_TOKEN(anon_sym_unattachments);
       END_STATE();
-    case 1013:
+    case 1012:
       ACCEPT_TOKEN(anon_sym_auto_view);
       END_STATE();
-    case 1014:
+    case 1013:
       ACCEPT_TOKEN(anon_sym_unauto_view);
       END_STATE();
-    case 1015:
+    case 1014:
       ACCEPT_TOKEN(anon_sym_attach);
       END_STATE();
-    case 1016:
+    case 1015:
       ACCEPT_TOKEN(anon_sym_browser);
       END_STATE();
-    case 1017:
+    case 1016:
       ACCEPT_TOKEN(anon_sym_compose);
       END_STATE();
-    case 1018:
+    case 1017:
       ACCEPT_TOKEN(anon_sym_editor);
       END_STATE();
-    case 1019:
+    case 1018:
       ACCEPT_TOKEN(anon_sym_generic);
       END_STATE();
-    case 1020:
+    case 1019:
       ACCEPT_TOKEN(anon_sym_index);
       END_STATE();
-    case 1021:
+    case 1020:
       ACCEPT_TOKEN(anon_sym_index);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == '_') ADVANCE(1312);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == '_') ADVANCE(1304);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1022:
+    case 1021:
       ACCEPT_TOKEN(anon_sym_index);
-      if (lookahead == '_') ADVANCE(171);
+      if (lookahead == '_') ADVANCE(170);
       END_STATE();
-    case 1023:
+    case 1022:
       ACCEPT_TOKEN(anon_sym_mix);
       END_STATE();
-    case 1024:
+    case 1023:
       ACCEPT_TOKEN(anon_sym_pager);
       END_STATE();
-    case 1025:
+    case 1024:
       ACCEPT_TOKEN(anon_sym_pgp);
       END_STATE();
-    case 1026:
+    case 1025:
       ACCEPT_TOKEN(anon_sym_postpone);
       END_STATE();
-    case 1027:
+    case 1026:
       ACCEPT_TOKEN(anon_sym_query);
       END_STATE();
-    case 1028:
+    case 1027:
       ACCEPT_TOKEN(anon_sym_smime);
       END_STATE();
-    case 1029:
+    case 1028:
       ACCEPT_TOKEN(sym_function);
       if (lookahead == '-' ||
-          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1029);
+          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1028);
       END_STATE();
-    case 1030:
+    case 1029:
       ACCEPT_TOKEN(anon_sym_bind);
       END_STATE();
-    case 1031:
+    case 1030:
       ACCEPT_TOKEN(anon_sym_unbind);
       END_STATE();
-    case 1032:
+    case 1031:
       ACCEPT_TOKEN(anon_sym_charset_DASHhook);
       END_STATE();
-    case 1033:
+    case 1032:
       ACCEPT_TOKEN(anon_sym_iconv_DASHhook);
       END_STATE();
-    case 1034:
+    case 1033:
       ACCEPT_TOKEN(anon_sym_attach_headers);
       END_STATE();
-    case 1035:
+    case 1034:
       ACCEPT_TOKEN(anon_sym_attach_headers);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1036:
+    case 1035:
       ACCEPT_TOKEN(anon_sym_attachment);
       END_STATE();
-    case 1037:
+    case 1036:
       ACCEPT_TOKEN(anon_sym_attachment);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1038:
+    case 1037:
       ACCEPT_TOKEN(anon_sym_body);
       END_STATE();
-    case 1039:
+    case 1038:
       ACCEPT_TOKEN(anon_sym_body);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1040:
+    case 1039:
       ACCEPT_TOKEN(anon_sym_bold);
       END_STATE();
-    case 1041:
+    case 1040:
       ACCEPT_TOKEN(anon_sym_bold);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1042:
+    case 1041:
       ACCEPT_TOKEN(anon_sym_error);
       END_STATE();
-    case 1043:
+    case 1042:
       ACCEPT_TOKEN(anon_sym_error);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1044:
+    case 1043:
       ACCEPT_TOKEN(anon_sym_hdrdefault);
       END_STATE();
-    case 1045:
+    case 1044:
       ACCEPT_TOKEN(anon_sym_hdrdefault);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1046:
+    case 1045:
       ACCEPT_TOKEN(anon_sym_header);
       END_STATE();
-    case 1047:
+    case 1046:
       ACCEPT_TOKEN(anon_sym_header);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1048:
+    case 1047:
       ACCEPT_TOKEN(anon_sym_index_author);
       END_STATE();
-    case 1049:
+    case 1048:
       ACCEPT_TOKEN(anon_sym_index_author);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1050:
+    case 1049:
       ACCEPT_TOKEN(anon_sym_index_collapsed);
       END_STATE();
-    case 1051:
+    case 1050:
       ACCEPT_TOKEN(anon_sym_index_collapsed);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1052:
+    case 1051:
       ACCEPT_TOKEN(anon_sym_index_date);
       END_STATE();
-    case 1053:
+    case 1052:
       ACCEPT_TOKEN(anon_sym_index_date);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1054:
+    case 1053:
       ACCEPT_TOKEN(anon_sym_index_flags);
       END_STATE();
-    case 1055:
+    case 1054:
       ACCEPT_TOKEN(anon_sym_index_flags);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1056:
+    case 1055:
       ACCEPT_TOKEN(anon_sym_index_label);
       END_STATE();
-    case 1057:
+    case 1056:
       ACCEPT_TOKEN(anon_sym_index_label);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1058:
+    case 1057:
       ACCEPT_TOKEN(anon_sym_index_number);
       END_STATE();
-    case 1059:
+    case 1058:
       ACCEPT_TOKEN(anon_sym_index_number);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1060:
+    case 1059:
       ACCEPT_TOKEN(anon_sym_index_size);
       END_STATE();
-    case 1061:
+    case 1060:
       ACCEPT_TOKEN(anon_sym_index_size);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1062:
+    case 1061:
       ACCEPT_TOKEN(anon_sym_index_subject);
       END_STATE();
-    case 1063:
+    case 1062:
       ACCEPT_TOKEN(anon_sym_index_subject);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1064:
+    case 1063:
       ACCEPT_TOKEN(anon_sym_index_tag);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1067);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1066);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1065:
+    case 1064:
       ACCEPT_TOKEN(anon_sym_index_tag);
-      if (lookahead == 's') ADVANCE(1066);
+      if (lookahead == 's') ADVANCE(1065);
       END_STATE();
-    case 1066:
+    case 1065:
       ACCEPT_TOKEN(anon_sym_index_tags);
       END_STATE();
-    case 1067:
+    case 1066:
       ACCEPT_TOKEN(anon_sym_index_tags);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1068:
+    case 1067:
       ACCEPT_TOKEN(anon_sym_indicator);
       END_STATE();
-    case 1069:
+    case 1068:
       ACCEPT_TOKEN(anon_sym_indicator);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1070:
+    case 1069:
       ACCEPT_TOKEN(anon_sym_markers);
       END_STATE();
-    case 1071:
+    case 1070:
       ACCEPT_TOKEN(anon_sym_markers);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1072:
+    case 1071:
       ACCEPT_TOKEN(anon_sym_message);
       END_STATE();
-    case 1073:
+    case 1072:
       ACCEPT_TOKEN(anon_sym_message);
-      if (lookahead == '-') ADVANCE(437);
+      if (lookahead == '-') ADVANCE(436);
       END_STATE();
-    case 1074:
+    case 1073:
       ACCEPT_TOKEN(anon_sym_message);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1075:
+    case 1074:
       ACCEPT_TOKEN(anon_sym_normal);
       END_STATE();
-    case 1076:
+    case 1075:
       ACCEPT_TOKEN(anon_sym_normal);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1077:
+    case 1076:
       ACCEPT_TOKEN(anon_sym_progress);
       END_STATE();
-    case 1078:
+    case 1077:
       ACCEPT_TOKEN(anon_sym_progress);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1079:
+    case 1078:
       ACCEPT_TOKEN(anon_sym_prompt);
       END_STATE();
-    case 1080:
+    case 1079:
       ACCEPT_TOKEN(anon_sym_prompt);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1081:
+    case 1080:
       ACCEPT_TOKEN(aux_sym_object_token1);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1081);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1080);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1082:
+    case 1081:
       ACCEPT_TOKEN(aux_sym_object_token1);
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1082);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1081);
       END_STATE();
-    case 1083:
+    case 1082:
       ACCEPT_TOKEN(anon_sym_search);
       END_STATE();
-    case 1084:
+    case 1083:
       ACCEPT_TOKEN(anon_sym_search);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1085:
+    case 1084:
       ACCEPT_TOKEN(anon_sym_signature);
       END_STATE();
-    case 1086:
+    case 1085:
       ACCEPT_TOKEN(anon_sym_signature);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1087:
+    case 1086:
       ACCEPT_TOKEN(anon_sym_status);
       END_STATE();
-    case 1088:
+    case 1087:
       ACCEPT_TOKEN(anon_sym_status);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1089:
+    case 1088:
       ACCEPT_TOKEN(anon_sym_tilde);
       END_STATE();
-    case 1090:
+    case 1089:
       ACCEPT_TOKEN(anon_sym_tilde);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1091:
+    case 1090:
       ACCEPT_TOKEN(anon_sym_tree);
       END_STATE();
-    case 1092:
+    case 1091:
       ACCEPT_TOKEN(anon_sym_tree);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1093:
+    case 1092:
       ACCEPT_TOKEN(anon_sym_underline);
       END_STATE();
-    case 1094:
+    case 1093:
       ACCEPT_TOKEN(anon_sym_underline);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1095:
+    case 1094:
       ACCEPT_TOKEN(anon_sym_sidebar_background);
       END_STATE();
-    case 1096:
+    case 1095:
       ACCEPT_TOKEN(anon_sym_sidebar_background);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1097:
+    case 1096:
       ACCEPT_TOKEN(anon_sym_sidebar_divider);
       END_STATE();
-    case 1098:
+    case 1097:
       ACCEPT_TOKEN(anon_sym_sidebar_divider);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1099:
+    case 1098:
       ACCEPT_TOKEN(anon_sym_sidebar_flagged);
       END_STATE();
-    case 1100:
+    case 1099:
       ACCEPT_TOKEN(anon_sym_sidebar_flagged);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1101:
+    case 1100:
       ACCEPT_TOKEN(anon_sym_sidebar_highlight);
       END_STATE();
-    case 1102:
+    case 1101:
       ACCEPT_TOKEN(anon_sym_sidebar_highlight);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1103:
+    case 1102:
       ACCEPT_TOKEN(anon_sym_sidebar_indicator);
       END_STATE();
-    case 1104:
+    case 1103:
       ACCEPT_TOKEN(anon_sym_sidebar_indicator);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1105:
+    case 1104:
       ACCEPT_TOKEN(anon_sym_sidebar_new);
       END_STATE();
-    case 1106:
+    case 1105:
       ACCEPT_TOKEN(anon_sym_sidebar_new);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1107:
+    case 1106:
       ACCEPT_TOKEN(anon_sym_sidebar_ordinary);
       END_STATE();
-    case 1108:
+    case 1107:
       ACCEPT_TOKEN(anon_sym_sidebar_ordinary);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1109:
+    case 1108:
       ACCEPT_TOKEN(anon_sym_sidebar_spool_file);
       END_STATE();
-    case 1110:
+    case 1109:
       ACCEPT_TOKEN(anon_sym_sidebar_spool_file);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1111:
+    case 1110:
       ACCEPT_TOKEN(anon_sym_security_encrypt);
       END_STATE();
-    case 1112:
+    case 1111:
       ACCEPT_TOKEN(anon_sym_security_sign);
       END_STATE();
-    case 1113:
+    case 1112:
       ACCEPT_TOKEN(anon_sym_security_both);
       END_STATE();
-    case 1114:
+    case 1113:
       ACCEPT_TOKEN(anon_sym_security_none);
       END_STATE();
-    case 1115:
+    case 1114:
       ACCEPT_TOKEN(anon_sym_default);
       END_STATE();
-    case 1116:
+    case 1115:
       ACCEPT_TOKEN(anon_sym_black);
       END_STATE();
-    case 1117:
+    case 1116:
       ACCEPT_TOKEN(anon_sym_red);
       END_STATE();
-    case 1118:
+    case 1117:
       ACCEPT_TOKEN(anon_sym_green);
       END_STATE();
-    case 1119:
+    case 1118:
       ACCEPT_TOKEN(anon_sym_yellow);
       END_STATE();
-    case 1120:
+    case 1119:
       ACCEPT_TOKEN(anon_sym_blue);
       END_STATE();
-    case 1121:
+    case 1120:
       ACCEPT_TOKEN(anon_sym_magenta);
       END_STATE();
-    case 1122:
+    case 1121:
       ACCEPT_TOKEN(anon_sym_cyan);
       END_STATE();
-    case 1123:
+    case 1122:
       ACCEPT_TOKEN(anon_sym_white);
       END_STATE();
-    case 1124:
+    case 1123:
       ACCEPT_TOKEN(aux_sym_color_token1);
       END_STATE();
-    case 1125:
+    case 1124:
       ACCEPT_TOKEN(aux_sym_color_token2);
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1125);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1124);
       END_STATE();
-    case 1126:
+    case 1125:
       ACCEPT_TOKEN(anon_sym_none);
       END_STATE();
-    case 1127:
+    case 1126:
       ACCEPT_TOKEN(anon_sym_reverse);
       END_STATE();
-    case 1128:
+    case 1127:
       ACCEPT_TOKEN(anon_sym_standout);
       END_STATE();
-    case 1129:
+    case 1128:
       ACCEPT_TOKEN(anon_sym_color);
       END_STATE();
-    case 1130:
+    case 1129:
       ACCEPT_TOKEN(anon_sym_color);
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1125);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1124);
       END_STATE();
-    case 1131:
+    case 1130:
       ACCEPT_TOKEN(anon_sym_uncolor);
       END_STATE();
-    case 1132:
+    case 1131:
       ACCEPT_TOKEN(anon_sym_crypt_DASHhook);
       END_STATE();
-    case 1133:
+    case 1132:
       ACCEPT_TOKEN(anon_sym_index_DASHformat_DASHhook);
       END_STATE();
-    case 1134:
+    case 1133:
       ACCEPT_TOKEN(anon_sym_BANG);
       END_STATE();
-    case 1135:
+    case 1134:
       ACCEPT_TOKEN(anon_sym_BANG);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1136:
+    case 1135:
       ACCEPT_TOKEN(anon_sym_exec);
       END_STATE();
-    case 1137:
+    case 1136:
       ACCEPT_TOKEN(anon_sym_fcc_DASHsave_DASHhook);
       END_STATE();
-    case 1138:
+    case 1137:
       ACCEPT_TOKEN(anon_sym_fcc_DASHhook);
       END_STATE();
-    case 1139:
+    case 1138:
       ACCEPT_TOKEN(anon_sym_save_DASHhook);
       END_STATE();
-    case 1140:
+    case 1139:
       ACCEPT_TOKEN(anon_sym_folder_DASHhook);
       END_STATE();
-    case 1141:
+    case 1140:
       ACCEPT_TOKEN(anon_sym_DASHnoregex);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1142:
+    case 1141:
       ACCEPT_TOKEN(anon_sym_DASHrx);
       END_STATE();
-    case 1143:
+    case 1142:
       ACCEPT_TOKEN(anon_sym_DASHaddr);
       END_STATE();
-    case 1144:
+    case 1143:
       ACCEPT_TOKEN(anon_sym_group);
       END_STATE();
-    case 1145:
+    case 1144:
       ACCEPT_TOKEN(anon_sym_ungroup);
       END_STATE();
-    case 1146:
+    case 1145:
       ACCEPT_TOKEN(anon_sym_hdr_order);
       END_STATE();
-    case 1147:
+    case 1146:
       ACCEPT_TOKEN(anon_sym_unhdr_order);
       END_STATE();
-    case 1148:
+    case 1147:
       ACCEPT_TOKEN(anon_sym_ifdef);
       END_STATE();
-    case 1149:
+    case 1148:
       ACCEPT_TOKEN(anon_sym_ifndef);
       END_STATE();
-    case 1150:
+    case 1149:
       ACCEPT_TOKEN(anon_sym_finish);
       END_STATE();
-    case 1151:
+    case 1150:
       ACCEPT_TOKEN(anon_sym_ignore);
       END_STATE();
-    case 1152:
+    case 1151:
       ACCEPT_TOKEN(anon_sym_unignore);
       END_STATE();
-    case 1153:
+    case 1152:
       ACCEPT_TOKEN(anon_sym_lists);
       END_STATE();
-    case 1154:
+    case 1153:
       ACCEPT_TOKEN(anon_sym_unlists);
       END_STATE();
-    case 1155:
+    case 1154:
       ACCEPT_TOKEN(anon_sym_subscribe);
-      if (lookahead == '-') ADVANCE(879);
+      if (lookahead == '-') ADVANCE(878);
       END_STATE();
-    case 1156:
+    case 1155:
       ACCEPT_TOKEN(anon_sym_unsubscribe);
-      if (lookahead == '-') ADVANCE(387);
+      if (lookahead == '-') ADVANCE(386);
       END_STATE();
-    case 1157:
+    case 1156:
       ACCEPT_TOKEN(anon_sym_macro);
       END_STATE();
-    case 1158:
+    case 1157:
       ACCEPT_TOKEN(anon_sym_unmacro);
       END_STATE();
-    case 1159:
+    case 1158:
       ACCEPT_TOKEN(anon_sym_mailboxes);
       END_STATE();
-    case 1160:
+    case 1159:
       ACCEPT_TOKEN(anon_sym_named_DASHmailboxes);
       END_STATE();
-    case 1161:
+    case 1160:
       ACCEPT_TOKEN(anon_sym_unmailboxes);
       END_STATE();
-    case 1162:
+    case 1161:
       ACCEPT_TOKEN(anon_sym_mailto_allow);
       END_STATE();
-    case 1163:
+    case 1162:
       ACCEPT_TOKEN(anon_sym_unmailto_allow);
       END_STATE();
-    case 1164:
+    case 1163:
       ACCEPT_TOKEN(anon_sym_echo);
       END_STATE();
-    case 1165:
+    case 1164:
       ACCEPT_TOKEN(anon_sym_cd);
       END_STATE();
-    case 1166:
+    case 1165:
       ACCEPT_TOKEN(anon_sym_mbox_DASHhook);
       END_STATE();
-    case 1167:
+    case 1166:
       ACCEPT_TOKEN(anon_sym_message_DASHhook);
       END_STATE();
-    case 1168:
+    case 1167:
       ACCEPT_TOKEN(anon_sym_mime_lookup);
       END_STATE();
-    case 1169:
+    case 1168:
       ACCEPT_TOKEN(anon_sym_unmime_lookup);
       END_STATE();
-    case 1170:
+    case 1169:
       ACCEPT_TOKEN(anon_sym_mono);
       END_STATE();
-    case 1171:
+    case 1170:
       ACCEPT_TOKEN(anon_sym_unmono);
       END_STATE();
-    case 1172:
+    case 1171:
       ACCEPT_TOKEN(anon_sym_my_hdr);
       END_STATE();
-    case 1173:
+    case 1172:
       ACCEPT_TOKEN(anon_sym_unmy_hdr);
       END_STATE();
-    case 1174:
+    case 1173:
       ACCEPT_TOKEN(anon_sym_open_DASHhook);
       END_STATE();
-    case 1175:
+    case 1174:
       ACCEPT_TOKEN(anon_sym_close_DASHhook);
       END_STATE();
-    case 1176:
+    case 1175:
       ACCEPT_TOKEN(anon_sym_append_DASHhook);
       END_STATE();
-    case 1177:
+    case 1176:
       ACCEPT_TOKEN(anon_sym_push);
       END_STATE();
-    case 1178:
+    case 1177:
       ACCEPT_TOKEN(anon_sym_reply_DASHhook);
       END_STATE();
-    case 1179:
+    case 1178:
       ACCEPT_TOKEN(anon_sym_send_DASHhook);
       END_STATE();
-    case 1180:
+    case 1179:
       ACCEPT_TOKEN(anon_sym_send2_DASHhook);
       END_STATE();
-    case 1181:
+    case 1180:
       ACCEPT_TOKEN(anon_sym_spam);
       END_STATE();
-    case 1182:
+    case 1181:
       ACCEPT_TOKEN(anon_sym_nospam);
       END_STATE();
-    case 1183:
+    case 1182:
       ACCEPT_TOKEN(anon_sym_subjectrx);
       END_STATE();
-    case 1184:
+    case 1183:
       ACCEPT_TOKEN(anon_sym_unsubjectrx);
       END_STATE();
-    case 1185:
+    case 1184:
       ACCEPT_TOKEN(anon_sym_subscribe_DASHto);
       END_STATE();
-    case 1186:
+    case 1185:
       ACCEPT_TOKEN(anon_sym_unsubscribe_DASHfrom);
       END_STATE();
-    case 1187:
+    case 1186:
       ACCEPT_TOKEN(anon_sym_timeout_DASHhook);
       END_STATE();
-    case 1188:
+    case 1187:
       ACCEPT_TOKEN(anon_sym_startup_DASHhook);
       END_STATE();
-    case 1189:
+    case 1188:
       ACCEPT_TOKEN(anon_sym_shutdown_DASHhook);
       END_STATE();
-    case 1190:
+    case 1189:
       ACCEPT_TOKEN(anon_sym_unhook);
       END_STATE();
-    case 1191:
+    case 1190:
       ACCEPT_TOKEN(anon_sym_set);
-      if (lookahead == 'e') ADVANCE(576);
+      if (lookahead == 'e') ADVANCE(575);
       END_STATE();
-    case 1192:
+    case 1191:
       ACCEPT_TOKEN(anon_sym_PLUS_EQ);
       END_STATE();
-    case 1193:
+    case 1192:
       ACCEPT_TOKEN(anon_sym_DASH_EQ);
       END_STATE();
-    case 1194:
+    case 1193:
       ACCEPT_TOKEN(anon_sym_EQ);
       END_STATE();
-    case 1195:
+    case 1194:
       ACCEPT_TOKEN(anon_sym_AMP);
       END_STATE();
-    case 1196:
+    case 1195:
       ACCEPT_TOKEN(anon_sym_unset);
-      if (lookahead == 'e') ADVANCE(577);
+      if (lookahead == 'e') ADVANCE(576);
       END_STATE();
-    case 1197:
+    case 1196:
       ACCEPT_TOKEN(anon_sym_reset);
       END_STATE();
-    case 1198:
+    case 1197:
       ACCEPT_TOKEN(anon_sym_toggle);
       END_STATE();
-    case 1199:
+    case 1198:
       ACCEPT_TOKEN(anon_sym_setenv);
       END_STATE();
-    case 1200:
+    case 1199:
       ACCEPT_TOKEN(aux_sym_setenv_directive_token1);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1200);
+          lookahead != ' ') ADVANCE(1199);
       END_STATE();
-    case 1201:
+    case 1200:
       ACCEPT_TOKEN(anon_sym_unsetenv);
       END_STATE();
-    case 1202:
+    case 1201:
       ACCEPT_TOKEN(anon_sym_sidebar_pin);
       END_STATE();
-    case 1203:
+    case 1202:
       ACCEPT_TOKEN(anon_sym_sidebar_unpin);
       END_STATE();
-    case 1204:
+    case 1203:
       ACCEPT_TOKEN(anon_sym_score);
       END_STATE();
-    case 1205:
+    case 1204:
       ACCEPT_TOKEN(anon_sym_unscore);
       END_STATE();
-    case 1206:
+    case 1205:
       ACCEPT_TOKEN(sym_option);
       if (('0' <= lookahead && lookahead <= '9') ||
           lookahead == '_' ||
-          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1206);
+          ('a' <= lookahead && lookahead <= 'z')) ADVANCE(1205);
       END_STATE();
-    case 1207:
+    case 1206:
       ACCEPT_TOKEN(anon_sym_yes);
       END_STATE();
-    case 1208:
+    case 1207:
       ACCEPT_TOKEN(anon_sym_yes);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1209:
+    case 1208:
       ACCEPT_TOKEN(anon_sym_no);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1210:
+    case 1209:
       ACCEPT_TOKEN(anon_sym_no);
-      if (lookahead == 'n') ADVANCE(282);
-      if (lookahead == 'r') ADVANCE(556);
-      if (lookahead == 's') ADVANCE(732);
+      if (lookahead == 'n') ADVANCE(281);
+      if (lookahead == 'r') ADVANCE(555);
+      if (lookahead == 's') ADVANCE(731);
       END_STATE();
-    case 1211:
+    case 1210:
       ACCEPT_TOKEN(anon_sym_ask_DASHyes);
       END_STATE();
-    case 1212:
+    case 1211:
       ACCEPT_TOKEN(anon_sym_ask_DASHyes);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
+      END_STATE();
+    case 1212:
+      ACCEPT_TOKEN(anon_sym_ask_DASHno);
       END_STATE();
     case 1213:
       ACCEPT_TOKEN(anon_sym_ask_DASHno);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1214:
-      ACCEPT_TOKEN(anon_sym_ask_DASHno);
-      if (lookahead == '\\') ADVANCE(1528);
+      ACCEPT_TOKEN(sym_int);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1214);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1215:
       ACCEPT_TOKEN(sym_int);
-      if (lookahead == '\\') ADVANCE(1528);
       if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1215);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
       END_STATE();
     case 1216:
-      ACCEPT_TOKEN(sym_int);
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1216);
+      ACCEPT_TOKEN(anon_sym_SQUOTE);
       END_STATE();
     case 1217:
       ACCEPT_TOKEN(anon_sym_SQUOTE);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1218:
-      ACCEPT_TOKEN(anon_sym_SQUOTE);
-      if (lookahead == '\\') ADVANCE(1528);
+      ACCEPT_TOKEN(aux_sym__string_token1);
+      if (lookahead == '\n') ADVANCE(1220);
+      if (lookahead == '\r') ADVANCE(1219);
       if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != '\\') ADVANCE(1221);
+      if (lookahead == '\\') ADVANCE(1222);
       END_STATE();
     case 1219:
       ACCEPT_TOKEN(aux_sym__string_token1);
-      if (lookahead == '\n') ADVANCE(1221);
-      if (lookahead == '\r') ADVANCE(1220);
+      if (lookahead == '\n') ADVANCE(1220);
+      if (lookahead == '\\') ADVANCE(1222);
       if (lookahead != 0 &&
-          lookahead != '\\') ADVANCE(1222);
-      if (lookahead == '\\') ADVANCE(1223);
+          lookahead != '\'') ADVANCE(1221);
       END_STATE();
     case 1220:
       ACCEPT_TOKEN(aux_sym__string_token1);
-      if (lookahead == '\n') ADVANCE(1221);
-      if (lookahead == '\\') ADVANCE(1223);
+      if (lookahead == '\\') ADVANCE(1218);
+      if (('\t' <= lookahead && lookahead <= '\r') ||
+          lookahead == ' ') ADVANCE(1220);
       if (lookahead != 0 &&
-          lookahead != '\'') ADVANCE(1222);
+          lookahead != '\'') ADVANCE(1221);
       END_STATE();
     case 1221:
       ACCEPT_TOKEN(aux_sym__string_token1);
-      if (lookahead == '\\') ADVANCE(1219);
-      if (('\t' <= lookahead && lookahead <= '\r') ||
-          lookahead == ' ') ADVANCE(1221);
+      if (lookahead == '\\') ADVANCE(1222);
       if (lookahead != 0 &&
-          lookahead != '\'') ADVANCE(1222);
+          lookahead != '\'') ADVANCE(1221);
       END_STATE();
     case 1222:
       ACCEPT_TOKEN(aux_sym__string_token1);
-      if (lookahead == '\\') ADVANCE(1223);
       if (lookahead != 0 &&
-          lookahead != '\'') ADVANCE(1222);
+          lookahead != '\\') ADVANCE(1221);
+      if (lookahead == '\\') ADVANCE(1222);
       END_STATE();
     case 1223:
-      ACCEPT_TOKEN(aux_sym__string_token1);
-      if (lookahead != 0 &&
-          lookahead != '\\') ADVANCE(1222);
-      if (lookahead == '\\') ADVANCE(1223);
+      ACCEPT_TOKEN(anon_sym_DQUOTE);
       END_STATE();
     case 1224:
       ACCEPT_TOKEN(anon_sym_DQUOTE);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1225:
-      ACCEPT_TOKEN(anon_sym_DQUOTE);
-      if (lookahead == '\\') ADVANCE(1528);
+      ACCEPT_TOKEN(aux_sym__string_token2);
+      if (lookahead == '\n') ADVANCE(1227);
+      if (lookahead == '\r') ADVANCE(1226);
       if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != '\\') ADVANCE(1228);
+      if (lookahead == '\\') ADVANCE(1229);
       END_STATE();
     case 1226:
       ACCEPT_TOKEN(aux_sym__string_token2);
-      if (lookahead == '\n') ADVANCE(1228);
-      if (lookahead == '\r') ADVANCE(1227);
+      if (lookahead == '\n') ADVANCE(1227);
+      if (lookahead == '\\') ADVANCE(1229);
       if (lookahead != 0 &&
-          lookahead != '\\') ADVANCE(1229);
-      if (lookahead == '\\') ADVANCE(1230);
+          lookahead != '"') ADVANCE(1228);
       END_STATE();
     case 1227:
       ACCEPT_TOKEN(aux_sym__string_token2);
-      if (lookahead == '\n') ADVANCE(1228);
-      if (lookahead == '\\') ADVANCE(1230);
+      if (lookahead == '\\') ADVANCE(1225);
+      if (('\t' <= lookahead && lookahead <= '\r') ||
+          lookahead == ' ') ADVANCE(1227);
       if (lookahead != 0 &&
-          lookahead != '"') ADVANCE(1229);
+          lookahead != '"') ADVANCE(1228);
       END_STATE();
     case 1228:
       ACCEPT_TOKEN(aux_sym__string_token2);
-      if (lookahead == '\\') ADVANCE(1226);
-      if (('\t' <= lookahead && lookahead <= '\r') ||
-          lookahead == ' ') ADVANCE(1228);
+      if (lookahead == '\\') ADVANCE(1229);
       if (lookahead != 0 &&
-          lookahead != '"') ADVANCE(1229);
+          lookahead != '"') ADVANCE(1228);
       END_STATE();
     case 1229:
       ACCEPT_TOKEN(aux_sym__string_token2);
-      if (lookahead == '\\') ADVANCE(1230);
       if (lookahead != 0 &&
-          lookahead != '"') ADVANCE(1229);
+          lookahead != '\\') ADVANCE(1228);
+      if (lookahead == '\\') ADVANCE(1229);
       END_STATE();
     case 1230:
-      ACCEPT_TOKEN(aux_sym__string_token2);
-      if (lookahead != 0 &&
-          lookahead != '\\') ADVANCE(1229);
-      if (lookahead == '\\') ADVANCE(1230);
-      END_STATE();
-    case 1231:
       ACCEPT_TOKEN(anon_sym_BQUOTE);
       END_STATE();
-    case 1232:
+    case 1231:
       ACCEPT_TOKEN(anon_sym_BQUOTE);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
+      END_STATE();
+    case 1232:
+      ACCEPT_TOKEN(aux_sym__string_token3);
+      if (lookahead == '\n') ADVANCE(1234);
+      if (lookahead == '\r') ADVANCE(1233);
+      if (lookahead == '\\') ADVANCE(1236);
+      if (lookahead != 0) ADVANCE(1235);
       END_STATE();
     case 1233:
       ACCEPT_TOKEN(aux_sym__string_token3);
-      if (lookahead == '\n') ADVANCE(1235);
-      if (lookahead == '\r') ADVANCE(1234);
-      if (lookahead == '\\') ADVANCE(1237);
-      if (lookahead != 0) ADVANCE(1236);
+      if (lookahead == '\n') ADVANCE(1234);
+      if (lookahead == '\\') ADVANCE(1236);
+      if (lookahead != 0 &&
+          lookahead != '`') ADVANCE(1235);
       END_STATE();
     case 1234:
       ACCEPT_TOKEN(aux_sym__string_token3);
-      if (lookahead == '\n') ADVANCE(1235);
-      if (lookahead == '\\') ADVANCE(1237);
+      if (lookahead == '\\') ADVANCE(1232);
+      if (('\t' <= lookahead && lookahead <= '\r') ||
+          lookahead == ' ') ADVANCE(1234);
       if (lookahead != 0 &&
-          lookahead != '`') ADVANCE(1236);
+          lookahead != '`') ADVANCE(1235);
       END_STATE();
     case 1235:
       ACCEPT_TOKEN(aux_sym__string_token3);
-      if (lookahead == '\\') ADVANCE(1233);
-      if (('\t' <= lookahead && lookahead <= '\r') ||
-          lookahead == ' ') ADVANCE(1235);
+      if (lookahead == '\\') ADVANCE(1236);
       if (lookahead != 0 &&
-          lookahead != '`') ADVANCE(1236);
+          lookahead != '`') ADVANCE(1235);
       END_STATE();
     case 1236:
       ACCEPT_TOKEN(aux_sym__string_token3);
-      if (lookahead == '\\') ADVANCE(1237);
-      if (lookahead != 0 &&
-          lookahead != '`') ADVANCE(1236);
+      if (lookahead == '\\') ADVANCE(1236);
+      if (lookahead != 0) ADVANCE(1235);
       END_STATE();
     case 1237:
-      ACCEPT_TOKEN(aux_sym__string_token3);
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1519);
       if (lookahead == '\\') ADVANCE(1237);
-      if (lookahead != 0) ADVANCE(1236);
+      if (lookahead != 0) ADVANCE(1521);
       END_STATE();
     case 1238:
-      ACCEPT_TOKEN(anon_sym_LF);
-      if (lookahead == '\n') ADVANCE(1238);
-      if (lookahead == '\\') ADVANCE(1251);
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1287);
+      if (lookahead == '\r') ADVANCE(8);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\f' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1239:
-      ACCEPT_TOKEN(anon_sym_LF);
-      if (lookahead == '\n') ADVANCE(1239);
-      if (lookahead == ' ') ADVANCE(997);
-      if (lookahead == '\\') ADVANCE(1255);
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1287);
+      if (lookahead == '\r') ADVANCE(1240);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1240:
-      ACCEPT_TOKEN(anon_sym_LF);
-      if (lookahead == '\n') ADVANCE(1240);
-      if (lookahead == '\\') ADVANCE(1274);
-      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(981);
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1287);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1241:
-      ACCEPT_TOKEN(anon_sym_LF);
-      if (lookahead == '\n') ADVANCE(1241);
-      if (lookahead == '\\') ADVANCE(1258);
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1277);
+      if (lookahead == '\r') ADVANCE(15);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\f' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1242:
-      ACCEPT_TOKEN(anon_sym_LF);
-      if (lookahead == '\n') ADVANCE(1242);
-      if (lookahead == '\\') ADVANCE(1261);
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1277);
+      if (lookahead == '\r') ADVANCE(1243);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1243:
-      ACCEPT_TOKEN(anon_sym_LF);
-      if (lookahead == '\n') ADVANCE(1243);
-      if (lookahead == '\\') ADVANCE(1264);
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1277);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1244:
-      ACCEPT_TOKEN(anon_sym_LF);
-      if (lookahead == '\n') ADVANCE(1244);
-      if (lookahead == '\\') ADVANCE(1267);
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1283);
+      if (lookahead == '\r') ADVANCE(16);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\f' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1245:
-      ACCEPT_TOKEN(anon_sym_LF);
-      if (lookahead == '\n') ADVANCE(1245);
-      if (lookahead == '\\') ADVANCE(1270);
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1283);
+      if (lookahead == '\r') ADVANCE(1246);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1246:
-      ACCEPT_TOKEN(anon_sym_LF);
-      if (lookahead == '\n') ADVANCE(1246);
-      if (lookahead == '\\') ADVANCE(1276);
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1283);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1247:
-      ACCEPT_TOKEN(anon_sym_LF);
-      if (lookahead == '\n') ADVANCE(1247);
-      if (lookahead == '\\') ADVANCE(1279);
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1280);
+      if (lookahead == '\r') ADVANCE(17);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\f' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1248:
-      ACCEPT_TOKEN(anon_sym_LF);
-      if (lookahead == '\n') ADVANCE(1248);
-      if (lookahead == '\\') ADVANCE(1282);
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1280);
+      if (lookahead == '\r') ADVANCE(1249);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1249:
-      ACCEPT_TOKEN(anon_sym_LF);
-      if (lookahead == '\n') ADVANCE(1249);
-      if (lookahead == '\\') ADVANCE(1285);
-      END_STATE();
-    case 1250:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1238);
-      if (lookahead == '"') ADVANCE(1225);
-      if (lookahead == '\'') ADVANCE(1218);
-      if (lookahead == '\\') ADVANCE(1252);
-      if (lookahead == '`') ADVANCE(1232);
-      if (lookahead == 'a') ADVANCE(1502);
-      if (lookahead == 'b') ADVANCE(1440);
-      if (lookahead == 'e') ADVANCE(1472);
-      if (lookahead == 'h') ADVANCE(1342);
-      if (lookahead == 'i') ADVANCE(1430);
-      if (lookahead == 'm') ADVANCE(1311);
-      if (lookahead == 'n') ADVANCE(1445);
-      if (lookahead == 'p') ADVANCE(1471);
-      if (lookahead == 'q') ADVANCE(1513);
-      if (lookahead == 's') ADVANCE(1363);
-      if (lookahead == 't') ADVANCE(1402);
-      if (lookahead == 'u') ADVANCE(1431);
+      if (lookahead == '\n') ADVANCE(1280);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
-    case 1251:
+    case 1250:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1250);
-      if (lookahead == '\r') ADVANCE(9);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\n') ADVANCE(1279);
+      if (lookahead == '\r') ADVANCE(18);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\f' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
+      END_STATE();
+    case 1251:
+      ACCEPT_TOKEN(sym__word);
+      if (lookahead == '\n') ADVANCE(1279);
+      if (lookahead == '\r') ADVANCE(1252);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1252:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1250);
-      if (lookahead == '\r') ADVANCE(1253);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == '\n') ADVANCE(1279);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1253:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1250);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\n') ADVANCE(1282);
+      if (lookahead == '\r') ADVANCE(19);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          (lookahead < '\t' || '\f' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1254:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1239);
-      if (lookahead == ' ') ADVANCE(997);
-      if (lookahead == '"') ADVANCE(1225);
-      if (lookahead == '\'') ADVANCE(1218);
-      if (lookahead == '-') ADVANCE(1526);
-      if (lookahead == '\\') ADVANCE(1256);
-      if (lookahead == '`') ADVANCE(1232);
-      if (lookahead == 'a') ADVANCE(1493);
-      if (lookahead == 'n') ADVANCE(1442);
-      if (lookahead == 'y') ADVANCE(1373);
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1215);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead)) ADVANCE(1527);
+      if (lookahead == '\n') ADVANCE(1282);
+      if (lookahead == '\r') ADVANCE(1255);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1255:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1254);
-      if (lookahead == '\r') ADVANCE(15);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\n') ADVANCE(1282);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
-          (lookahead < '\t' || '\f' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1256:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1254);
-      if (lookahead == '\r') ADVANCE(1257);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == '\n') ADVANCE(1286);
+      if (lookahead == '\r') ADVANCE(992);
+      if (lookahead == '\\') ADVANCE(994);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\f' < lookahead) &&
+          lookahead != ' ') ADVANCE(993);
       END_STATE();
     case 1257:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1254);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+      if (lookahead == '\n') ADVANCE(1286);
+      if (lookahead == '\r') ADVANCE(992);
+      if (lookahead == '\\') ADVANCE(994);
+      if (lookahead != 0) ADVANCE(993);
       END_STATE();
     case 1258:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1288);
-      if (lookahead == '\r') ADVANCE(18);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\n') ADVANCE(1281);
+      if (lookahead == '\r') ADVANCE(20);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\f' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1259:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1288);
+      if (lookahead == '\n') ADVANCE(1281);
       if (lookahead == '\r') ADVANCE(1260);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1260:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1288);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\n') ADVANCE(1281);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1261:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1289);
-      if (lookahead == '\r') ADVANCE(19);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\n') ADVANCE(1285);
+      if (lookahead == '\r') ADVANCE(22);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\f' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1262:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1289);
+      if (lookahead == '\n') ADVANCE(1285);
       if (lookahead == '\r') ADVANCE(1263);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1263:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1289);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\n') ADVANCE(1285);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1264:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1290);
-      if (lookahead == '\r') ADVANCE(20);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\n') ADVANCE(1527);
+      if (lookahead == '\r') ADVANCE(25);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '#') ADVANCE(1521);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '\\') ADVANCE(1266);
+      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == '\t' ||
+          lookahead == ' ') ADVANCE(1532);
       if (lookahead != 0 &&
-          (lookahead < '\t' || '\f' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != 11 &&
+          lookahead != '\f') ADVANCE(1519);
       END_STATE();
     case 1265:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1290);
-      if (lookahead == '\r') ADVANCE(1266);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == '\n') ADVANCE(1264);
+      if (lookahead == '\r') ADVANCE(26);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\f' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1266:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1290);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+      if (lookahead == '\n') ADVANCE(1264);
+      if (lookahead == '\r') ADVANCE(1267);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1267:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1291);
-      if (lookahead == '\r') ADVANCE(21);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\n') ADVANCE(1264);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
-          (lookahead < '\t' || '\f' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1268:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1291);
-      if (lookahead == '\r') ADVANCE(1269);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == '\n') ADVANCE(1278);
+      if (lookahead == '\r') ADVANCE(27);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\f' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1269:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1291);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+      if (lookahead == '\n') ADVANCE(1278);
+      if (lookahead == '\r') ADVANCE(1270);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1270:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1292);
-      if (lookahead == '\r') ADVANCE(22);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\n') ADVANCE(1278);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
-          (lookahead < '\t' || '\f' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1271:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1292);
-      if (lookahead == '\r') ADVANCE(1272);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == '\n') ADVANCE(1288);
+      if (lookahead == '\r') ADVANCE(29);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\f' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1272:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1292);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+      if (lookahead == '\n') ADVANCE(1288);
+      if (lookahead == '\r') ADVANCE(1273);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1273:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1240);
-      if (lookahead == '"') ADVANCE(1225);
-      if (lookahead == '\'') ADVANCE(1218);
-      if (lookahead == '<') ADVANCE(976);
-      if (lookahead == '\\') ADVANCE(1275);
-      if (lookahead == '`') ADVANCE(1232);
-      if (('\t' <= lookahead && lookahead <= '\r')) ADVANCE(981);
+      if (lookahead == '\n') ADVANCE(1288);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
-          lookahead != ' ') ADVANCE(988);
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1274:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1273);
-      if (lookahead == '\r') ADVANCE(993);
-      if (lookahead == '\\') ADVANCE(995);
+      if (lookahead == '\n') ADVANCE(1284);
+      if (lookahead == '\r') ADVANCE(46);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\f' < lookahead) &&
-          lookahead != ' ') ADVANCE(994);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1275:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1273);
-      if (lookahead == '\r') ADVANCE(993);
-      if (lookahead == '\\') ADVANCE(995);
-      if (lookahead != 0) ADVANCE(994);
+      if (lookahead == '\n') ADVANCE(1284);
+      if (lookahead == '\r') ADVANCE(1276);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1276:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1293);
-      if (lookahead == '\r') ADVANCE(24);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\n') ADVANCE(1284);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
-          (lookahead < '\t' || '\f' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1277:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1293);
-      if (lookahead == '\r') ADVANCE(1278);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == ' ') ADVANCE(997);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '-') ADVANCE(1518);
+      if (lookahead == '\\') ADVANCE(1242);
+      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == 'a') ADVANCE(1485);
+      if (lookahead == 'n') ADVANCE(1434);
+      if (lookahead == 'y') ADVANCE(1365);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1214);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\r' < lookahead)) ADVANCE(1519);
       END_STATE();
     case 1278:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1293);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '!') ADVANCE(1134);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '\\') ADVANCE(1269);
+      if (lookahead == '`') ADVANCE(1231);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1279:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1294);
-      if (lookahead == '\r') ADVANCE(25);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '*') ADVANCE(973);
+      if (lookahead == '+') ADVANCE(1006);
+      if (lookahead == '-') ADVANCE(1008);
+      if (lookahead == '\\') ADVANCE(1251);
+      if (lookahead == '`') ADVANCE(1231);
       if (lookahead != 0 &&
-          (lookahead < '\t' || '\f' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1280:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1294);
-      if (lookahead == '\r') ADVANCE(1281);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '*') ADVANCE(973);
+      if (lookahead == '-') ADVANCE(1387);
+      if (lookahead == '\\') ADVANCE(1248);
+      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1281:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1294);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '*') ADVANCE(973);
+      if (lookahead == '\\') ADVANCE(1259);
+      if (lookahead == '`') ADVANCE(1231);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1282:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1295);
-      if (lookahead == '\r') ADVANCE(26);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '+') ADVANCE(1006);
+      if (lookahead == '-') ADVANCE(1008);
+      if (lookahead == '?') ADVANCE(1010);
+      if (lookahead == '\\') ADVANCE(1254);
+      if (lookahead == '`') ADVANCE(1231);
       if (lookahead != 0 &&
-          (lookahead < '\t' || '\f' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1283:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1295);
-      if (lookahead == '\r') ADVANCE(1284);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '-') ADVANCE(1518);
+      if (lookahead == '\\') ADVANCE(1245);
+      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == 'a') ADVANCE(1485);
+      if (lookahead == 'n') ADVANCE(1434);
+      if (lookahead == 'y') ADVANCE(1365);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1214);
+      if (lookahead != 0 &&
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1284:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1295);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '-') ADVANCE(1431);
+      if (lookahead == '\\') ADVANCE(1275);
+      if (lookahead == '`') ADVANCE(1231);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1285:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1296);
-      if (lookahead == '\r') ADVANCE(47);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '-') ADVANCE(1387);
+      if (lookahead == '\\') ADVANCE(1262);
+      if (lookahead == '`') ADVANCE(1231);
       if (lookahead != 0 &&
-          (lookahead < '\t' || '\f' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          (lookahead < '\t' || '\r' < lookahead) &&
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1286:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1296);
-      if (lookahead == '\r') ADVANCE(1287);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '<') ADVANCE(975);
+      if (lookahead == '\\') ADVANCE(1257);
+      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == '\t' ||
+          (11 <= lookahead && lookahead <= '\r')) ADVANCE(980);
+      if (lookahead != 0 &&
+          lookahead != '\n' &&
+          lookahead != ' ') ADVANCE(987);
       END_STATE();
     case 1287:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1296);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '\\') ADVANCE(1239);
+      if (lookahead == '`') ADVANCE(1231);
+      if (lookahead == 'a') ADVANCE(1494);
+      if (lookahead == 'b') ADVANCE(1432);
+      if (lookahead == 'e') ADVANCE(1464);
+      if (lookahead == 'h') ADVANCE(1334);
+      if (lookahead == 'i') ADVANCE(1422);
+      if (lookahead == 'm') ADVANCE(1303);
+      if (lookahead == 'n') ADVANCE(1437);
+      if (lookahead == 'p') ADVANCE(1463);
+      if (lookahead == 'q') ADVANCE(1505);
+      if (lookahead == 's') ADVANCE(1355);
+      if (lookahead == 't') ADVANCE(1394);
+      if (lookahead == 'u') ADVANCE(1423);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1288:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1241);
-      if (lookahead == '"') ADVANCE(1225);
-      if (lookahead == '\'') ADVANCE(1218);
-      if (lookahead == '-') ADVANCE(1526);
-      if (lookahead == '\\') ADVANCE(1259);
-      if (lookahead == '`') ADVANCE(1232);
-      if (lookahead == 'a') ADVANCE(1493);
-      if (lookahead == 'n') ADVANCE(1442);
-      if (lookahead == 'y') ADVANCE(1373);
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1215);
+      if (lookahead == '"') ADVANCE(1224);
+      if (lookahead == '\'') ADVANCE(1217);
+      if (lookahead == '\\') ADVANCE(1272);
+      if (lookahead == '`') ADVANCE(1231);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1289:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1242);
-      if (lookahead == '"') ADVANCE(1225);
-      if (lookahead == '\'') ADVANCE(1218);
-      if (lookahead == '*') ADVANCE(974);
-      if (lookahead == '-') ADVANCE(1395);
-      if (lookahead == '\\') ADVANCE(1262);
-      if (lookahead == '`') ADVANCE(1232);
+      if (lookahead == '-') ADVANCE(1426);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1290:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1243);
-      if (lookahead == '"') ADVANCE(1225);
-      if (lookahead == '\'') ADVANCE(1218);
-      if (lookahead == '+') ADVANCE(1007);
-      if (lookahead == '-') ADVANCE(1009);
-      if (lookahead == '?') ADVANCE(1011);
-      if (lookahead == '\\') ADVANCE(1265);
-      if (lookahead == '`') ADVANCE(1232);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == '_') ADVANCE(1316);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1291:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1244);
-      if (lookahead == '"') ADVANCE(1225);
-      if (lookahead == '\'') ADVANCE(1218);
-      if (lookahead == '*') ADVANCE(974);
-      if (lookahead == '+') ADVANCE(1007);
-      if (lookahead == '-') ADVANCE(1009);
-      if (lookahead == '\\') ADVANCE(1268);
-      if (lookahead == '`') ADVANCE(1232);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == '_') ADVANCE(1375);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1292:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1245);
-      if (lookahead == '"') ADVANCE(1225);
-      if (lookahead == '\'') ADVANCE(1218);
-      if (lookahead == '*') ADVANCE(974);
-      if (lookahead == '\\') ADVANCE(1271);
-      if (lookahead == '`') ADVANCE(1232);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == '_') ADVANCE(1391);
+      if (lookahead == 'm') ADVANCE(1358);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1293:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1246);
-      if (lookahead == '"') ADVANCE(1225);
-      if (lookahead == '\'') ADVANCE(1218);
-      if (lookahead == '-') ADVANCE(1395);
-      if (lookahead == '\\') ADVANCE(1277);
-      if (lookahead == '`') ADVANCE(1232);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1320);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1294:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1247);
-      if (lookahead == '"') ADVANCE(1225);
-      if (lookahead == '\'') ADVANCE(1218);
-      if (lookahead == '\\') ADVANCE(1280);
-      if (lookahead == '`') ADVANCE(1232);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1382);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1295:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1248);
-      if (lookahead == '!') ADVANCE(1135);
-      if (lookahead == '"') ADVANCE(1225);
-      if (lookahead == '\'') ADVANCE(1218);
-      if (lookahead == '\\') ADVANCE(1283);
-      if (lookahead == '`') ADVANCE(1232);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1408);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1296:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\n') ADVANCE(1249);
-      if (lookahead == '"') ADVANCE(1225);
-      if (lookahead == '\'') ADVANCE(1218);
-      if (lookahead == '-') ADVANCE(1439);
-      if (lookahead == '\\') ADVANCE(1286);
-      if (lookahead == '`') ADVANCE(1232);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1317);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1297:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '-') ADVANCE(1434);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1377);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1298:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == '_') ADVANCE(1324);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1321);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1299:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == '_') ADVANCE(1383);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1451);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1300:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == '_') ADVANCE(1399);
-      if (lookahead == 'm') ADVANCE(1366);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1379);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1301:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1328);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1495);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1302:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1390);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1507);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1303:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1416);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1452);
+      if (lookahead == 'e') ADVANCE(1484);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1304:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1325);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1508);
+      if (lookahead == 'c') ADVANCE(1438);
+      if (lookahead == 'd') ADVANCE(1311);
+      if (lookahead == 'f') ADVANCE(1413);
+      if (lookahead == 'l') ADVANCE(1296);
+      if (lookahead == 'n') ADVANCE(1503);
+      if (lookahead == 's') ADVANCE(1395);
+      if (lookahead == 't') ADVANCE(1297);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1305:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead == 'a') ADVANCE(1385);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1306:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1329);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1496);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1307:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1459);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1501);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1308:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1387);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1473);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1309:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1503);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1456);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1310:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1515);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1462);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1311:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1460);
-      if (lookahead == 'e') ADVANCE(1492);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1500);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1312:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1516);
-      if (lookahead == 'c') ADVANCE(1446);
-      if (lookahead == 'd') ADVANCE(1319);
-      if (lookahead == 'f') ADVANCE(1421);
-      if (lookahead == 'l') ADVANCE(1304);
-      if (lookahead == 'n') ADVANCE(1511);
-      if (lookahead == 's') ADVANCE(1403);
-      if (lookahead == 't') ADVANCE(1305);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1340);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1313:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1393);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1502);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1314:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1504);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'a') ADVANCE(1341);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1315:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1509);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'b') ADVANCE(1404);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1316:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1481);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'b') ADVANCE(1298);
+      if (lookahead == 'd') ADVANCE(1396);
+      if (lookahead == 'f') ADVANCE(1415);
+      if (lookahead == 'h') ADVANCE(1398);
+      if (lookahead == 'i') ADVANCE(1424);
+      if (lookahead == 'n') ADVANCE(1353);
+      if (lookahead == 'o') ADVANCE(1467);
+      if (lookahead == 's') ADVANCE(1450);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1317:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1464);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'b') ADVANCE(1362);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1318:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1470);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'b') ADVANCE(1309);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1319:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1508);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'b') ADVANCE(1369);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1320:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1348);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'c') ADVANCE(1388);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1321:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1510);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'c') ADVANCE(1406);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1322:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'a') ADVANCE(1349);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'c') ADVANCE(1389);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1323:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'b') ADVANCE(1412);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'c') ADVANCE(1492);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1324:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'b') ADVANCE(1306);
-      if (lookahead == 'd') ADVANCE(1404);
-      if (lookahead == 'f') ADVANCE(1423);
-      if (lookahead == 'h') ADVANCE(1406);
-      if (lookahead == 'i') ADVANCE(1432);
-      if (lookahead == 'n') ADVANCE(1361);
-      if (lookahead == 'o') ADVANCE(1475);
-      if (lookahead == 's') ADVANCE(1458);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'c') ADVANCE(1307);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1325:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'b') ADVANCE(1370);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'c') ADVANCE(1313);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1326:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'b') ADVANCE(1317);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1515);
+      if (lookahead == 'l') ADVANCE(1328);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1327:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'b') ADVANCE(1377);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1343);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1328:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'c') ADVANCE(1396);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1040);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1329:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'c') ADVANCE(1414);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1080);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1330:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'c') ADVANCE(1397);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1050);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1331:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'c') ADVANCE(1500);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1099);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1332:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'c') ADVANCE(1315);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1095);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1333:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'c') ADVANCE(1321);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1344);
+      if (lookahead == 'g') ADVANCE(1429);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1334:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1523);
-      if (lookahead == 'l') ADVANCE(1336);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1475);
+      if (lookahead == 'e') ADVANCE(1312);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1335:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1351);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1364);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1336:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1041);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1346);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1337:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1081);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1403);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1338:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1051);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1347);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1339:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1100);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1400);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1340:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1096);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1366);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1341:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1352);
-      if (lookahead == 'g') ADVANCE(1437);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1370);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1342:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1483);
-      if (lookahead == 'e') ADVANCE(1320);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'd') ADVANCE(1371);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1343:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1372);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1513);
+      if (lookahead == 'i') ADVANCE(1324);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1344:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1354);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1318);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1345:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1411);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1091);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1346:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1355);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1376);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1347:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1408);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1089);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1348:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1374);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1073);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1349:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1378);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1085);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1350:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'd') ADVANCE(1379);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1093);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1351:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1521);
-      if (lookahead == 'i') ADVANCE(1332);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1052);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1352:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1326);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1060);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1353:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1092);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1512);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1354:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1384);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1109);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1355:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1090);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1308);
+      if (lookahead == 'i') ADVANCE(1333);
+      if (lookahead == 't') ADVANCE(1301);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1356:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1074);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1514);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1357:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1086);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1345);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1358:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1094);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1425);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1359:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1053);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1329);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1360:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1061);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1323);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1361:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1520);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1330);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1362:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1110);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1410);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1363:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1316);
-      if (lookahead == 'i') ADVANCE(1341);
-      if (lookahead == 't') ADVANCE(1309);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1331);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1364:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1522);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1465);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1365:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1353);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1482);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1366:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1433);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1455);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1367:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1337);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1483);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1368:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1331);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1466);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1369:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1338);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1459);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1370:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1418);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1469);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1371:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1339);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1460);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1372:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1473);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1487);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1373:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1490);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1384);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1374:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1463);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'e') ADVANCE(1314);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1375:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1491);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'f') ADVANCE(1399);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1376:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1474);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'f') ADVANCE(1302);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1377:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1467);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'g') ADVANCE(1063);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1378:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1477);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'g') ADVANCE(1390);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1379:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1468);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'g') ADVANCE(1480);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1380:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1495);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'g') ADVANCE(1392);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1381:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1392);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'g') ADVANCE(1470);
+      if (lookahead == 'm') ADVANCE(1449);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1382:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'e') ADVANCE(1322);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'g') ADVANCE(1348);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1383:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'f') ADVANCE(1407);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'g') ADVANCE(1363);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1384:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'f') ADVANCE(1310);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'g') ADVANCE(1356);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1385:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'g') ADVANCE(1064);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'g') ADVANCE(1383);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1386:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'g') ADVANCE(1398);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'g') ADVANCE(1468);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1387:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'g') ADVANCE(1488);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'g') ADVANCE(1476);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1388:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'g') ADVANCE(1400);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'h') ADVANCE(1292);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1389:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'g') ADVANCE(1478);
-      if (lookahead == 'm') ADVANCE(1457);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'h') ADVANCE(1083);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1390:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'g') ADVANCE(1356);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'h') ADVANCE(1419);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1391:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'g') ADVANCE(1371);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'h') ADVANCE(1374);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1392:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'g') ADVANCE(1364);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'h') ADVANCE(1493);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1393:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'g') ADVANCE(1391);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'h') ADVANCE(1444);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1394:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'g') ADVANCE(1476);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'i') ADVANCE(1418);
+      if (lookahead == 'r') ADVANCE(1357);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1395:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'g') ADVANCE(1484);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'i') ADVANCE(1517);
+      if (lookahead == 'u') ADVANCE(1315);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1396:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'h') ADVANCE(1300);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'i') ADVANCE(1511);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1397:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'h') ADVANCE(1084);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'i') ADVANCE(1428);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1398:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'h') ADVANCE(1427);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'i') ADVANCE(1378);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1399:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'h') ADVANCE(1382);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'i') ADVANCE(1416);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1400:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'h') ADVANCE(1501);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'i') ADVANCE(1430);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1401:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'h') ADVANCE(1452);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'i') ADVANCE(1380);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1402:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'i') ADVANCE(1426);
-      if (lookahead == 'r') ADVANCE(1365);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'i') ADVANCE(1342);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1403:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'i') ADVANCE(1525);
-      if (lookahead == 'u') ADVANCE(1323);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'i') ADVANCE(1325);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1404:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'i') ADVANCE(1519);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'j') ADVANCE(1360);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1405:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'i') ADVANCE(1436);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'k') ADVANCE(1289);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1406:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'i') ADVANCE(1386);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'k') ADVANCE(1386);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1407:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'i') ADVANCE(1424);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'k') ADVANCE(1368);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1408:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'i') ADVANCE(1438);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'l') ADVANCE(1075);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1409:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'i') ADVANCE(1388);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'l') ADVANCE(1397);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1410:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'i') ADVANCE(1350);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'l') ADVANCE(1056);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1411:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'i') ADVANCE(1333);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'l') ADVANCE(1291);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1412:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'j') ADVANCE(1368);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'l') ADVANCE(1491);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1413:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'k') ADVANCE(1297);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'l') ADVANCE(1300);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1414:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'k') ADVANCE(1394);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'l') ADVANCE(1299);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1415:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'k') ADVANCE(1376);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'l') ADVANCE(1305);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1416:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'l') ADVANCE(1076);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'l') ADVANCE(1354);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1417:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'l') ADVANCE(1405);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'l') ADVANCE(1414);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1418:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'l') ADVANCE(1057);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'l') ADVANCE(1338);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1419:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'l') ADVANCE(1299);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'l') ADVANCE(1401);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1420:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'l') ADVANCE(1499);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'm') ADVANCE(1295);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1421:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'l') ADVANCE(1308);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'm') ADVANCE(1319);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1422:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'l') ADVANCE(1307);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'n') ADVANCE(1327);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1423:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'l') ADVANCE(1313);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'n') ADVANCE(1335);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1424:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'l') ADVANCE(1362);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'n') ADVANCE(1337);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1425:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'l') ADVANCE(1422);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'n') ADVANCE(1490);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1426:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'l') ADVANCE(1346);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'n') ADVANCE(1435);
+      if (lookahead == 'y') ADVANCE(1367);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1427:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'l') ADVANCE(1409);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'n') ADVANCE(1332);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1428:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'm') ADVANCE(1303);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'n') ADVANCE(1350);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1429:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'm') ADVANCE(1327);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'n') ADVANCE(1306);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1430:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'n') ADVANCE(1335);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'n') ADVANCE(1310);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1431:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'n') ADVANCE(1343);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'n') ADVANCE(1446);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1432:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'n') ADVANCE(1345);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1326);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1433:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'n') ADVANCE(1498);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1381);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1434:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'n') ADVANCE(1443);
-      if (lookahead == 'y') ADVANCE(1375);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1208);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1435:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'n') ADVANCE(1340);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1213);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1436:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'n') ADVANCE(1358);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1499);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1437:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'n') ADVANCE(1314);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1453);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1438:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'n') ADVANCE(1318);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1417);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1439:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'n') ADVANCE(1454);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1510);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1440:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1334);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1454);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1441:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1389);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1506);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1442:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1209);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1411);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1443:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1214);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1457);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1444:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1507);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1458);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1445:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead == 'o') ADVANCE(1461);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1446:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1425);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1472);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1447:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1518);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'o') ADVANCE(1442);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1448:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1462);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'p') ADVANCE(968);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1449:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1514);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'p') ADVANCE(1489);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1450:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1419);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'p') ADVANCE(1447);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1451:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1465);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'p') ADVANCE(1488);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1452:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1466);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1407);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1453:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1469);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1420);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1454:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1480);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1042);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1455:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'o') ADVANCE(1450);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1046);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1456:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'p') ADVANCE(969);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1290);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1457:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'p') ADVANCE(1497);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1068);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1458:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'p') ADVANCE(1455);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1048);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1459:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'p') ADVANCE(1496);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1058);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1460:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1415);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1097);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1461:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1428);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1103);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1462:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1043);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1516);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1463:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1047);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1433);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1464:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1298);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1474);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1465:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1069);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1409);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1466:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1049);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1478);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1467:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1059);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1339);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1468:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1098);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1439);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1469:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1104);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1481);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1470:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1524);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1372);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1471:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1441);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1349);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1472:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1482);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1373);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1473:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1417);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1322);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1474:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1486);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1440);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1475:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1347);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1336);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1476:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1447);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'r') ADVANCE(1441);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1477:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1489);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1087);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1478:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1380);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1070);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1479:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1357);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1077);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1480:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1381);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1054);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1481:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1330);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1034);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1482:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1448);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1207);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1483:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1344);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1211);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1484:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'r') ADVANCE(1449);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1486);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1485:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1088);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1405);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1486:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1071);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1294);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1487:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1078);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1479);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1488:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1055);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 's') ADVANCE(1361);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1489:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1035);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1079);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1490:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1208);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1036);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1491:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1212);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1044);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1492:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1494);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1062);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1493:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1413);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1101);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1494:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1302);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1497);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1495:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1487);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1504);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1496:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 's') ADVANCE(1369);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1509);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1497:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1080);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1293);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1498:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1037);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1393);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1499:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1045);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1359);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1500:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1063);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1351);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1501:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1102);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1443);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1502:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1505);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 't') ADVANCE(1445);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1503:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1512);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'u') ADVANCE(1421);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1504:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1517);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'u') ADVANCE(1477);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1505:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1301);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'u') ADVANCE(1436);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1506:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1401);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'u') ADVANCE(1448);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1507:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1367);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'u') ADVANCE(1412);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1508:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1359);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'u') ADVANCE(1498);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1509:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1451);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'u') ADVANCE(1471);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1510:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 't') ADVANCE(1453);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'u') ADVANCE(1427);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1511:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'u') ADVANCE(1429);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'v') ADVANCE(1402);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1512:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'u') ADVANCE(1485);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'w') ADVANCE(1105);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1513:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'u') ADVANCE(1444);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'x') ADVANCE(1020);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1514:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'u') ADVANCE(1456);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'x') ADVANCE(1140);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1515:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'u') ADVANCE(1420);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'y') ADVANCE(1038);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1516:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'u') ADVANCE(1506);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'y') ADVANCE(1107);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1517:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'u') ADVANCE(1479);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead == 'z') ADVANCE(1352);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1518:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'u') ADVANCE(1435);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1214);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1519:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'v') ADVANCE(1410);
+      if (lookahead == '\\') ADVANCE(1520);
       if (lookahead != 0 &&
           (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != ' ') ADVANCE(1519);
       END_STATE();
     case 1520:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'w') ADVANCE(1106);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+      if (lookahead == '\\') ADVANCE(1520);
+      if (lookahead != 0) ADVANCE(1519);
       END_STATE();
     case 1521:
       ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'x') ADVANCE(1021);
+      if (lookahead == '\\') ADVANCE(1237);
+      if (lookahead == '\t' ||
+          (11 <= lookahead && lookahead <= '\r') ||
+          lookahead == ' ') ADVANCE(1523);
       if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
+          lookahead != '\n') ADVANCE(1521);
       END_STATE();
     case 1522:
-      ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'x') ADVANCE(1141);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
-      END_STATE();
-    case 1523:
-      ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'y') ADVANCE(1039);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
-      END_STATE();
-    case 1524:
-      ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'y') ADVANCE(1108);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
-      END_STATE();
-    case 1525:
-      ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead == 'z') ADVANCE(1360);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
-      END_STATE();
-    case 1526:
-      ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (('0' <= lookahead && lookahead <= '9')) ADVANCE(1215);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
-      END_STATE();
-    case 1527:
-      ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0 &&
-          (lookahead < '\t' || '\r' < lookahead) &&
-          lookahead != ' ') ADVANCE(1527);
-      END_STATE();
-    case 1528:
-      ACCEPT_TOKEN(sym__word);
-      if (lookahead == '\\') ADVANCE(1528);
-      if (lookahead != 0) ADVANCE(1527);
-      END_STATE();
-    case 1529:
       ACCEPT_TOKEN(anon_sym_source);
       END_STATE();
-    case 1530:
+    case 1523:
       ACCEPT_TOKEN(sym_comment);
       if (lookahead != 0 &&
-          lookahead != '\n') ADVANCE(1530);
+          lookahead != '\n') ADVANCE(1523);
       END_STATE();
-    case 1531:
+    case 1524:
       ACCEPT_TOKEN(sym__eol);
-      if (lookahead == '\t') ADVANCE(1535);
-      if (lookahead == '\n') ADVANCE(1531);
+      if (lookahead == '\t') ADVANCE(1529);
+      if (lookahead == '\n') ADVANCE(1524);
       if (lookahead == '\r') ADVANCE(1);
-      if (lookahead == ' ') ADVANCE(996);
+      if (lookahead == ' ') ADVANCE(995);
       END_STATE();
-    case 1532:
+    case 1525:
       ACCEPT_TOKEN(sym__eol);
-      if (lookahead == '\t') ADVANCE(980);
-      if (lookahead == '\n') ADVANCE(1532);
-      if (lookahead == '\r') ADVANCE(980);
-      if (lookahead == ' ') ADVANCE(1536);
-      if (lookahead == '\\') ADVANCE(31);
+      if (lookahead == '\t') ADVANCE(979);
+      if (lookahead == '\n') ADVANCE(1525);
+      if (lookahead == '\r') ADVANCE(979);
+      if (lookahead == ' ') ADVANCE(1530);
+      if (lookahead == '\\') ADVANCE(30);
       if (lookahead == 11 ||
-          lookahead == '\f') ADVANCE(980);
+          lookahead == '\f') ADVANCE(979);
       END_STATE();
-    case 1533:
+    case 1526:
       ACCEPT_TOKEN(sym__eol);
-      if (lookahead == '\n') ADVANCE(1533);
+      if (lookahead == '\n') ADVANCE(1526);
       if (lookahead == '\r') ADVANCE(3);
       if (lookahead == '\t' ||
-          lookahead == ' ') ADVANCE(1537);
+          lookahead == ' ') ADVANCE(1531);
+      END_STATE();
+    case 1527:
+      ACCEPT_TOKEN(sym__eol);
+      if (lookahead == '\n') ADVANCE(1527);
+      if (lookahead == '\r') ADVANCE(25);
+      if (lookahead == '\\') ADVANCE(1265);
+      if (lookahead == '\t' ||
+          lookahead == ' ') ADVANCE(1532);
       END_STATE();
-    case 1534:
+    case 1528:
       ACCEPT_TOKEN(sym__eol);
-      if (lookahead == '\n') ADVANCE(1534);
-      if (lookahead == '\r') ADVANCE(44);
+      if (lookahead == '\n') ADVANCE(1528);
+      if (lookahead == '\r') ADVANCE(43);
       END_STATE();
-    case 1535:
+    case 1529:
       ACCEPT_TOKEN(aux_sym__space_token1);
-      if (lookahead == '\t') ADVANCE(1535);
-      if (lookahead == '\n') ADVANCE(1531);
+      if (lookahead == '\t') ADVANCE(1529);
+      if (lookahead == '\n') ADVANCE(1524);
       if (lookahead == '\r') ADVANCE(1);
-      if (lookahead == ' ') ADVANCE(996);
+      if (lookahead == ' ') ADVANCE(995);
       END_STATE();
-    case 1536:
+    case 1530:
       ACCEPT_TOKEN(aux_sym__space_token1);
-      if (lookahead == '\t') ADVANCE(980);
-      if (lookahead == '\n') ADVANCE(1532);
-      if (lookahead == '\r') ADVANCE(980);
-      if (lookahead == ' ') ADVANCE(1536);
-      if (lookahead == '\\') ADVANCE(31);
+      if (lookahead == '\t') ADVANCE(979);
+      if (lookahead == '\n') ADVANCE(1525);
+      if (lookahead == '\r') ADVANCE(979);
+      if (lookahead == ' ') ADVANCE(1530);
+      if (lookahead == '\\') ADVANCE(30);
       if (lookahead == 11 ||
-          lookahead == '\f') ADVANCE(980);
+          lookahead == '\f') ADVANCE(979);
       END_STATE();
-    case 1537:
+    case 1531:
       ACCEPT_TOKEN(aux_sym__space_token1);
-      if (lookahead == '\n') ADVANCE(1533);
+      if (lookahead == '\n') ADVANCE(1526);
       if (lookahead == '\r') ADVANCE(3);
       if (lookahead == '\t' ||
-          lookahead == ' ') ADVANCE(1537);
+          lookahead == ' ') ADVANCE(1531);
+      END_STATE();
+    case 1532:
+      ACCEPT_TOKEN(aux_sym__space_token1);
+      if (lookahead == '\n') ADVANCE(1527);
+      if (lookahead == '\r') ADVANCE(25);
+      if (lookahead == '\\') ADVANCE(1265);
+      if (lookahead == '\t' ||
+          lookahead == ' ') ADVANCE(1532);
       END_STATE();
     default:
       return false;
   }
 }
 
 static const TSLexMode ts_lex_modes[STATE_COUNT] = {
   [0] = {.lex_state = 0},
-  [1] = {.lex_state = 965},
-  [2] = {.lex_state = 965},
-  [3] = {.lex_state = 965},
-  [4] = {.lex_state = 60},
-  [5] = {.lex_state = 60},
-  [6] = {.lex_state = 60},
-  [7] = {.lex_state = 60},
-  [8] = {.lex_state = 60},
-  [9] = {.lex_state = 60},
-  [10] = {.lex_state = 60},
-  [11] = {.lex_state = 60},
-  [12] = {.lex_state = 60},
-  [13] = {.lex_state = 60},
-  [14] = {.lex_state = 60},
-  [15] = {.lex_state = 60},
-  [16] = {.lex_state = 60},
-  [17] = {.lex_state = 60},
-  [18] = {.lex_state = 60},
-  [19] = {.lex_state = 965},
-  [20] = {.lex_state = 965},
-  [21] = {.lex_state = 965},
-  [22] = {.lex_state = 60},
-  [23] = {.lex_state = 60},
-  [24] = {.lex_state = 60},
-  [25] = {.lex_state = 60},
-  [26] = {.lex_state = 8},
-  [27] = {.lex_state = 58},
-  [28] = {.lex_state = 58},
-  [29] = {.lex_state = 58},
+  [1] = {.lex_state = 964},
+  [2] = {.lex_state = 964},
+  [3] = {.lex_state = 964},
+  [4] = {.lex_state = 62},
+  [5] = {.lex_state = 62},
+  [6] = {.lex_state = 62},
+  [7] = {.lex_state = 62},
+  [8] = {.lex_state = 62},
+  [9] = {.lex_state = 62},
+  [10] = {.lex_state = 62},
+  [11] = {.lex_state = 62},
+  [12] = {.lex_state = 62},
+  [13] = {.lex_state = 62},
+  [14] = {.lex_state = 62},
+  [15] = {.lex_state = 62},
+  [16] = {.lex_state = 62},
+  [17] = {.lex_state = 62},
+  [18] = {.lex_state = 62},
+  [19] = {.lex_state = 964},
+  [20] = {.lex_state = 964},
+  [21] = {.lex_state = 964},
+  [22] = {.lex_state = 62},
+  [23] = {.lex_state = 62},
+  [24] = {.lex_state = 62},
+  [25] = {.lex_state = 62},
+  [26] = {.lex_state = 58},
+  [27] = {.lex_state = 60},
+  [28] = {.lex_state = 60},
+  [29] = {.lex_state = 62},
   [30] = {.lex_state = 60},
-  [31] = {.lex_state = 63},
-  [32] = {.lex_state = 58},
-  [33] = {.lex_state = 58},
-  [34] = {.lex_state = 63},
-  [35] = {.lex_state = 63},
-  [36] = {.lex_state = 63},
-  [37] = {.lex_state = 63},
-  [38] = {.lex_state = 14},
-  [39] = {.lex_state = 14},
-  [40] = {.lex_state = 14},
-  [41] = {.lex_state = 58},
-  [42] = {.lex_state = 14},
-  [43] = {.lex_state = 57},
-  [44] = {.lex_state = 58},
-  [45] = {.lex_state = 58},
-  [46] = {.lex_state = 57},
-  [47] = {.lex_state = 58},
-  [48] = {.lex_state = 57},
-  [49] = {.lex_state = 58},
-  [50] = {.lex_state = 58},
+  [31] = {.lex_state = 60},
+  [32] = {.lex_state = 60},
+  [33] = {.lex_state = 65},
+  [34] = {.lex_state = 65},
+  [35] = {.lex_state = 65},
+  [36] = {.lex_state = 65},
+  [37] = {.lex_state = 65},
+  [38] = {.lex_state = 47},
+  [39] = {.lex_state = 60},
+  [40] = {.lex_state = 60},
+  [41] = {.lex_state = 47},
+  [42] = {.lex_state = 47},
+  [43] = {.lex_state = 60},
+  [44] = {.lex_state = 60},
+  [45] = {.lex_state = 60},
+  [46] = {.lex_state = 60},
+  [47] = {.lex_state = 48},
+  [48] = {.lex_state = 47},
+  [49] = {.lex_state = 47},
+  [50] = {.lex_state = 48},
   [51] = {.lex_state = 48},
   [52] = {.lex_state = 48},
-  [53] = {.lex_state = 48},
-  [54] = {.lex_state = 57},
-  [55] = {.lex_state = 48},
-  [56] = {.lex_state = 57},
-  [57] = {.lex_state = 58},
-  [58] = {.lex_state = 58},
-  [59] = {.lex_state = 49},
+  [53] = {.lex_state = 60},
+  [54] = {.lex_state = 54},
+  [55] = {.lex_state = 54},
+  [56] = {.lex_state = 54},
+  [57] = {.lex_state = 60},
+  [58] = {.lex_state = 54},
+  [59] = {.lex_state = 51},
   [60] = {.lex_state = 50},
-  [61] = {.lex_state = 51},
-  [62] = {.lex_state = 52},
-  [63] = {.lex_state = 23},
-  [64] = {.lex_state = 53},
-  [65] = {.lex_state = 52},
-  [66] = {.lex_state = 52},
+  [61] = {.lex_state = 53},
+  [62] = {.lex_state = 57},
+  [63] = {.lex_state = 52},
+  [64] = {.lex_state = 52},
+  [65] = {.lex_state = 63},
+  [66] = {.lex_state = 56},
   [67] = {.lex_state = 52},
-  [68] = {.lex_state = 23},
-  [69] = {.lex_state = 52},
+  [68] = {.lex_state = 1},
+  [69] = {.lex_state = 57},
   [70] = {.lex_state = 52},
-  [71] = {.lex_state = 54},
-  [72] = {.lex_state = 52},
-  [73] = {.lex_state = 54},
-  [74] = {.lex_state = 52},
-  [75] = {.lex_state = 23},
-  [76] = {.lex_state = 54},
-  [77] = {.lex_state = 55},
-  [78] = {.lex_state = 61},
-  [79] = {.lex_state = 54},
+  [71] = {.lex_state = 52},
+  [72] = {.lex_state = 25},
+  [73] = {.lex_state = 25},
+  [74] = {.lex_state = 49},
+  [75] = {.lex_state = 52},
+  [76] = {.lex_state = 70},
+  [77] = {.lex_state = 52},
+  [78] = {.lex_state = 25},
+  [79] = {.lex_state = 52},
   [80] = {.lex_state = 52},
-  [81] = {.lex_state = 1},
+  [81] = {.lex_state = 59},
   [82] = {.lex_state = 52},
   [83] = {.lex_state = 52},
-  [84] = {.lex_state = 52},
-  [85] = {.lex_state = 52},
-  [86] = {.lex_state = 54},
-  [87] = {.lex_state = 54},
-  [88] = {.lex_state = 54},
-  [89] = {.lex_state = 54},
-  [90] = {.lex_state = 54},
-  [91] = {.lex_state = 54},
-  [92] = {.lex_state = 68},
-  [93] = {.lex_state = 54},
-  [94] = {.lex_state = 54},
-  [95] = {.lex_state = 54},
-  [96] = {.lex_state = 54},
-  [97] = {.lex_state = 2},
-  [98] = {.lex_state = 2},
-  [99] = {.lex_state = 54},
-  [100] = {.lex_state = 54},
-  [101] = {.lex_state = 54},
-  [102] = {.lex_state = 54},
-  [103] = {.lex_state = 54},
-  [104] = {.lex_state = 54},
-  [105] = {.lex_state = 54},
-  [106] = {.lex_state = 54},
-  [107] = {.lex_state = 52},
-  [108] = {.lex_state = 54},
-  [109] = {.lex_state = 54},
-  [110] = {.lex_state = 52},
-  [111] = {.lex_state = 54},
-  [112] = {.lex_state = 54},
-  [113] = {.lex_state = 54},
-  [114] = {.lex_state = 54},
-  [115] = {.lex_state = 54},
-  [116] = {.lex_state = 54},
-  [117] = {.lex_state = 54},
-  [118] = {.lex_state = 54},
-  [119] = {.lex_state = 54},
-  [120] = {.lex_state = 54},
-  [121] = {.lex_state = 54},
-  [122] = {.lex_state = 54},
-  [123] = {.lex_state = 54},
-  [124] = {.lex_state = 54},
-  [125] = {.lex_state = 54},
-  [126] = {.lex_state = 54},
-  [127] = {.lex_state = 54},
-  [128] = {.lex_state = 54},
-  [129] = {.lex_state = 54},
-  [130] = {.lex_state = 54},
-  [131] = {.lex_state = 54},
-  [132] = {.lex_state = 54},
-  [133] = {.lex_state = 54},
-  [134] = {.lex_state = 54},
-  [135] = {.lex_state = 56},
-  [136] = {.lex_state = 54},
-  [137] = {.lex_state = 54},
-  [138] = {.lex_state = 54},
-  [139] = {.lex_state = 54},
-  [140] = {.lex_state = 54},
-  [141] = {.lex_state = 56},
-  [142] = {.lex_state = 54},
-  [143] = {.lex_state = 54},
-  [144] = {.lex_state = 54},
-  [145] = {.lex_state = 54},
-  [146] = {.lex_state = 54},
-  [147] = {.lex_state = 54},
-  [148] = {.lex_state = 54},
-  [149] = {.lex_state = 54},
-  [150] = {.lex_state = 54},
-  [151] = {.lex_state = 54},
-  [152] = {.lex_state = 52},
-  [153] = {.lex_state = 55},
-  [154] = {.lex_state = 52},
-  [155] = {.lex_state = 60},
-  [156] = {.lex_state = 52},
-  [157] = {.lex_state = 54},
-  [158] = {.lex_state = 54},
-  [159] = {.lex_state = 965},
-  [160] = {.lex_state = 54},
-  [161] = {.lex_state = 0},
-  [162] = {.lex_state = 54},
-  [163] = {.lex_state = 54},
-  [164] = {.lex_state = 55},
-  [165] = {.lex_state = 52},
-  [166] = {.lex_state = 52},
-  [167] = {.lex_state = 54},
-  [168] = {.lex_state = 59},
-  [169] = {.lex_state = 54},
-  [170] = {.lex_state = 54},
-  [171] = {.lex_state = 60},
-  [172] = {.lex_state = 54},
-  [173] = {.lex_state = 54},
-  [174] = {.lex_state = 55},
-  [175] = {.lex_state = 60},
-  [176] = {.lex_state = 54},
-  [177] = {.lex_state = 54},
-  [178] = {.lex_state = 54},
-  [179] = {.lex_state = 62},
-  [180] = {.lex_state = 2},
-  [181] = {.lex_state = 54},
-  [182] = {.lex_state = 54},
-  [183] = {.lex_state = 54},
-  [184] = {.lex_state = 1},
-  [185] = {.lex_state = 90},
-  [186] = {.lex_state = 60},
-  [187] = {.lex_state = 1},
-  [188] = {.lex_state = 54},
-  [189] = {.lex_state = 91},
-  [190] = {.lex_state = 90},
-  [191] = {.lex_state = 90},
+  [84] = {.lex_state = 59},
+  [85] = {.lex_state = 25},
+  [86] = {.lex_state = 59},
+  [87] = {.lex_state = 52},
+  [88] = {.lex_state = 52},
+  [89] = {.lex_state = 59},
+  [90] = {.lex_state = 2},
+  [91] = {.lex_state = 59},
+  [92] = {.lex_state = 2},
+  [93] = {.lex_state = 57},
+  [94] = {.lex_state = 59},
+  [95] = {.lex_state = 59},
+  [96] = {.lex_state = 59},
+  [97] = {.lex_state = 62},
+  [98] = {.lex_state = 964},
+  [99] = {.lex_state = 59},
+  [100] = {.lex_state = 59},
+  [101] = {.lex_state = 62},
+  [102] = {.lex_state = 59},
+  [103] = {.lex_state = 2},
+  [104] = {.lex_state = 59},
+  [105] = {.lex_state = 59},
+  [106] = {.lex_state = 61},
+  [107] = {.lex_state = 64},
+  [108] = {.lex_state = 59},
+  [109] = {.lex_state = 59},
+  [110] = {.lex_state = 59},
+  [111] = {.lex_state = 59},
+  [112] = {.lex_state = 59},
+  [113] = {.lex_state = 59},
+  [114] = {.lex_state = 55},
+  [115] = {.lex_state = 59},
+  [116] = {.lex_state = 59},
+  [117] = {.lex_state = 59},
+  [118] = {.lex_state = 59},
+  [119] = {.lex_state = 59},
+  [120] = {.lex_state = 59},
+  [121] = {.lex_state = 59},
+  [122] = {.lex_state = 59},
+  [123] = {.lex_state = 59},
+  [124] = {.lex_state = 59},
+  [125] = {.lex_state = 59},
+  [126] = {.lex_state = 59},
+  [127] = {.lex_state = 59},
+  [128] = {.lex_state = 59},
+  [129] = {.lex_state = 59},
+  [130] = {.lex_state = 59},
+  [131] = {.lex_state = 0},
+  [132] = {.lex_state = 59},
+  [133] = {.lex_state = 59},
+  [134] = {.lex_state = 59},
+  [135] = {.lex_state = 59},
+  [136] = {.lex_state = 59},
+  [137] = {.lex_state = 59},
+  [138] = {.lex_state = 59},
+  [139] = {.lex_state = 59},
+  [140] = {.lex_state = 59},
+  [141] = {.lex_state = 59},
+  [142] = {.lex_state = 59},
+  [143] = {.lex_state = 59},
+  [144] = {.lex_state = 59},
+  [145] = {.lex_state = 59},
+  [146] = {.lex_state = 59},
+  [147] = {.lex_state = 52},
+  [148] = {.lex_state = 59},
+  [149] = {.lex_state = 52},
+  [150] = {.lex_state = 59},
+  [151] = {.lex_state = 59},
+  [152] = {.lex_state = 59},
+  [153] = {.lex_state = 62},
+  [154] = {.lex_state = 59},
+  [155] = {.lex_state = 59},
+  [156] = {.lex_state = 59},
+  [157] = {.lex_state = 59},
+  [158] = {.lex_state = 55},
+  [159] = {.lex_state = 59},
+  [160] = {.lex_state = 59},
+  [161] = {.lex_state = 1},
+  [162] = {.lex_state = 1},
+  [163] = {.lex_state = 1},
+  [164] = {.lex_state = 1},
+  [165] = {.lex_state = 964},
+  [166] = {.lex_state = 59},
+  [167] = {.lex_state = 49},
+  [168] = {.lex_state = 1},
+  [169] = {.lex_state = 92},
+  [170] = {.lex_state = 92},
+  [171] = {.lex_state = 92},
+  [172] = {.lex_state = 1},
+  [173] = {.lex_state = 1},
+  [174] = {.lex_state = 1},
+  [175] = {.lex_state = 1},
+  [176] = {.lex_state = 59},
+  [177] = {.lex_state = 1},
+  [178] = {.lex_state = 1},
+  [179] = {.lex_state = 1},
+  [180] = {.lex_state = 1},
+  [181] = {.lex_state = 49},
+  [182] = {.lex_state = 49},
+  [183] = {.lex_state = 52},
+  [184] = {.lex_state = 52},
+  [185] = {.lex_state = 52},
+  [186] = {.lex_state = 59},
+  [187] = {.lex_state = 52},
+  [188] = {.lex_state = 1},
+  [189] = {.lex_state = 59},
+  [190] = {.lex_state = 59},
+  [191] = {.lex_state = 1},
   [192] = {.lex_state = 1},
-  [193] = {.lex_state = 54},
-  [194] = {.lex_state = 54},
-  [195] = {.lex_state = 54},
-  [196] = {.lex_state = 59},
-  [197] = {.lex_state = 91},
-  [198] = {.lex_state = 1},
-  [199] = {.lex_state = 54},
-  [200] = {.lex_state = 54},
-  [201] = {.lex_state = 54},
-  [202] = {.lex_state = 54},
-  [203] = {.lex_state = 54},
-  [204] = {.lex_state = 54},
-  [205] = {.lex_state = 54},
+  [193] = {.lex_state = 93},
+  [194] = {.lex_state = 1},
+  [195] = {.lex_state = 1},
+  [196] = {.lex_state = 1},
+  [197] = {.lex_state = 67},
+  [198] = {.lex_state = 62},
+  [199] = {.lex_state = 93},
+  [200] = {.lex_state = 52},
+  [201] = {.lex_state = 1},
+  [202] = {.lex_state = 59},
+  [203] = {.lex_state = 59},
+  [204] = {.lex_state = 59},
+  [205] = {.lex_state = 1},
   [206] = {.lex_state = 1},
   [207] = {.lex_state = 1},
   [208] = {.lex_state = 1},
   [209] = {.lex_state = 1},
   [210] = {.lex_state = 1},
   [211] = {.lex_state = 1},
   [212] = {.lex_state = 1},
-  [213] = {.lex_state = 1},
-  [214] = {.lex_state = 1},
+  [213] = {.lex_state = 67},
+  [214] = {.lex_state = 59},
   [215] = {.lex_state = 1},
   [216] = {.lex_state = 1},
-  [217] = {.lex_state = 1},
+  [217] = {.lex_state = 92},
   [218] = {.lex_state = 1},
-  [219] = {.lex_state = 90},
+  [219] = {.lex_state = 1},
   [220] = {.lex_state = 1},
-  [221] = {.lex_state = 965},
-  [222] = {.lex_state = 1},
+  [221] = {.lex_state = 59},
+  [222] = {.lex_state = 59},
   [223] = {.lex_state = 1},
   [224] = {.lex_state = 1},
   [225] = {.lex_state = 1},
   [226] = {.lex_state = 1},
   [227] = {.lex_state = 1},
   [228] = {.lex_state = 1},
   [229] = {.lex_state = 1},
-  [230] = {.lex_state = 1},
+  [230] = {.lex_state = 59},
   [231] = {.lex_state = 1},
-  [232] = {.lex_state = 1},
-  [233] = {.lex_state = 1},
-  [234] = {.lex_state = 54},
+  [232] = {.lex_state = 92},
+  [233] = {.lex_state = 67},
+  [234] = {.lex_state = 1},
   [235] = {.lex_state = 1},
-  [236] = {.lex_state = 1},
+  [236] = {.lex_state = 59},
   [237] = {.lex_state = 1},
-  [238] = {.lex_state = 65},
+  [238] = {.lex_state = 1},
   [239] = {.lex_state = 1},
   [240] = {.lex_state = 1},
   [241] = {.lex_state = 1},
-  [242] = {.lex_state = 965},
-  [243] = {.lex_state = 1},
+  [242] = {.lex_state = 59},
+  [243] = {.lex_state = 964},
   [244] = {.lex_state = 1},
-  [245] = {.lex_state = 1},
-  [246] = {.lex_state = 1},
-  [247] = {.lex_state = 965},
-  [248] = {.lex_state = 1},
-  [249] = {.lex_state = 1},
-  [250] = {.lex_state = 65},
-  [251] = {.lex_state = 65},
-  [252] = {.lex_state = 90},
-  [253] = {.lex_state = 54},
-  [254] = {.lex_state = 1},
-  [255] = {.lex_state = 1},
-  [256] = {.lex_state = 1},
+  [245] = {.lex_state = 59},
+  [246] = {.lex_state = 964},
+  [247] = {.lex_state = 1},
+  [248] = {.lex_state = 59},
+  [249] = {.lex_state = 59},
+  [250] = {.lex_state = 61},
+  [251] = {.lex_state = 964},
+  [252] = {.lex_state = 1},
+  [253] = {.lex_state = 1},
+  [254] = {.lex_state = 964},
+  [255] = {.lex_state = 67},
+  [256] = {.lex_state = 964},
   [257] = {.lex_state = 1},
   [258] = {.lex_state = 1},
-  [259] = {.lex_state = 1},
-  [260] = {.lex_state = 1},
-  [261] = {.lex_state = 54},
+  [259] = {.lex_state = 47},
+  [260] = {.lex_state = 66},
+  [261] = {.lex_state = 1},
   [262] = {.lex_state = 1},
-  [263] = {.lex_state = 91},
+  [263] = {.lex_state = 1},
   [264] = {.lex_state = 1},
-  [265] = {.lex_state = 64},
-  [266] = {.lex_state = 64},
-  [267] = {.lex_state = 62},
-  [268] = {.lex_state = 62},
-  [269] = {.lex_state = 965},
-  [270] = {.lex_state = 965},
-  [271] = {.lex_state = 1},
-  [272] = {.lex_state = 1},
+  [265] = {.lex_state = 1},
+  [266] = {.lex_state = 1},
+  [267] = {.lex_state = 1},
+  [268] = {.lex_state = 1},
+  [269] = {.lex_state = 1},
+  [270] = {.lex_state = 1},
+  [271] = {.lex_state = 59},
+  [272] = {.lex_state = 59},
   [273] = {.lex_state = 1},
-  [274] = {.lex_state = 64},
+  [274] = {.lex_state = 1},
   [275] = {.lex_state = 1},
-  [276] = {.lex_state = 62},
-  [277] = {.lex_state = 62},
-  [278] = {.lex_state = 1},
-  [279] = {.lex_state = 1},
-  [280] = {.lex_state = 1},
+  [276] = {.lex_state = 64},
+  [277] = {.lex_state = 1},
+  [278] = {.lex_state = 64},
+  [279] = {.lex_state = 59},
+  [280] = {.lex_state = 59},
   [281] = {.lex_state = 1},
-  [282] = {.lex_state = 1},
-  [283] = {.lex_state = 1},
-  [284] = {.lex_state = 1},
-  [285] = {.lex_state = 60},
-  [286] = {.lex_state = 1},
-  [287] = {.lex_state = 57},
-  [288] = {.lex_state = 965},
-  [289] = {.lex_state = 1},
-  [290] = {.lex_state = 965},
+  [282] = {.lex_state = 59},
+  [283] = {.lex_state = 59},
+  [284] = {.lex_state = 59},
+  [285] = {.lex_state = 964},
+  [286] = {.lex_state = 59},
+  [287] = {.lex_state = 1},
+  [288] = {.lex_state = 67},
+  [289] = {.lex_state = 59},
+  [290] = {.lex_state = 59},
   [291] = {.lex_state = 1},
-  [292] = {.lex_state = 1},
-  [293] = {.lex_state = 965},
-  [294] = {.lex_state = 1},
-  [295] = {.lex_state = 1},
+  [292] = {.lex_state = 59},
+  [293] = {.lex_state = 62},
+  [294] = {.lex_state = 93},
+  [295] = {.lex_state = 66},
   [296] = {.lex_state = 1},
   [297] = {.lex_state = 1},
-  [298] = {.lex_state = 965},
-  [299] = {.lex_state = 65},
-  [300] = {.lex_state = 1},
-  [301] = {.lex_state = 1},
+  [298] = {.lex_state = 1},
+  [299] = {.lex_state = 1},
+  [300] = {.lex_state = 59},
+  [301] = {.lex_state = 964},
   [302] = {.lex_state = 1},
-  [303] = {.lex_state = 1},
-  [304] = {.lex_state = 65},
-  [305] = {.lex_state = 1},
+  [303] = {.lex_state = 964},
+  [304] = {.lex_state = 64},
+  [305] = {.lex_state = 64},
   [306] = {.lex_state = 1},
   [307] = {.lex_state = 1},
   [308] = {.lex_state = 1},
-  [309] = {.lex_state = 1},
-  [310] = {.lex_state = 965},
-  [311] = {.lex_state = 965},
-  [312] = {.lex_state = 965},
-  [313] = {.lex_state = 965},
-  [314] = {.lex_state = 965},
-  [315] = {.lex_state = 965},
-  [316] = {.lex_state = 965},
-  [317] = {.lex_state = 965},
-  [318] = {.lex_state = 965},
-  [319] = {.lex_state = 965},
-  [320] = {.lex_state = 965},
-  [321] = {.lex_state = 965},
-  [322] = {.lex_state = 965},
-  [323] = {.lex_state = 965},
-  [324] = {.lex_state = 965},
-  [325] = {.lex_state = 965},
-  [326] = {.lex_state = 965},
-  [327] = {.lex_state = 965},
-  [328] = {.lex_state = 64},
-  [329] = {.lex_state = 965},
-  [330] = {.lex_state = 965},
-  [331] = {.lex_state = 965},
-  [332] = {.lex_state = 965},
-  [333] = {.lex_state = 965},
-  [334] = {.lex_state = 965},
-  [335] = {.lex_state = 965},
-  [336] = {.lex_state = 965},
-  [337] = {.lex_state = 965},
-  [338] = {.lex_state = 965},
-  [339] = {.lex_state = 965},
-  [340] = {.lex_state = 965},
-  [341] = {.lex_state = 965},
-  [342] = {.lex_state = 965},
-  [343] = {.lex_state = 965},
-  [344] = {.lex_state = 965},
-  [345] = {.lex_state = 965},
-  [346] = {.lex_state = 965},
-  [347] = {.lex_state = 90},
-  [348] = {.lex_state = 90},
-  [349] = {.lex_state = 965},
-  [350] = {.lex_state = 90},
-  [351] = {.lex_state = 965},
-  [352] = {.lex_state = 965},
-  [353] = {.lex_state = 965},
-  [354] = {.lex_state = 965},
-  [355] = {.lex_state = 965},
-  [356] = {.lex_state = 965},
-  [357] = {.lex_state = 965},
-  [358] = {.lex_state = 90},
-  [359] = {.lex_state = 965},
-  [360] = {.lex_state = 60},
-  [361] = {.lex_state = 965},
-  [362] = {.lex_state = 60},
-  [363] = {.lex_state = 965},
-  [364] = {.lex_state = 965},
-  [365] = {.lex_state = 965},
-  [366] = {.lex_state = 965},
-  [367] = {.lex_state = 965},
-  [368] = {.lex_state = 965},
-  [369] = {.lex_state = 965},
-  [370] = {.lex_state = 965},
-  [371] = {.lex_state = 965},
-  [372] = {.lex_state = 965},
-  [373] = {.lex_state = 965},
-  [374] = {.lex_state = 965},
-  [375] = {.lex_state = 965},
-  [376] = {.lex_state = 965},
-  [377] = {.lex_state = 965},
-  [378] = {.lex_state = 965},
-  [379] = {.lex_state = 965},
-  [380] = {.lex_state = 965},
-  [381] = {.lex_state = 965},
-  [382] = {.lex_state = 965},
-  [383] = {.lex_state = 965},
-  [384] = {.lex_state = 965},
-  [385] = {.lex_state = 965},
-  [386] = {.lex_state = 59},
-  [387] = {.lex_state = 965},
-  [388] = {.lex_state = 64},
-  [389] = {.lex_state = 64},
-  [390] = {.lex_state = 965},
-  [391] = {.lex_state = 965},
-  [392] = {.lex_state = 965},
-  [393] = {.lex_state = 965},
-  [394] = {.lex_state = 965},
-  [395] = {.lex_state = 965},
-  [396] = {.lex_state = 965},
-  [397] = {.lex_state = 965},
-  [398] = {.lex_state = 965},
-  [399] = {.lex_state = 965},
-  [400] = {.lex_state = 965},
-  [401] = {.lex_state = 965},
-  [402] = {.lex_state = 965},
-  [403] = {.lex_state = 965},
-  [404] = {.lex_state = 965},
-  [405] = {.lex_state = 965},
-  [406] = {.lex_state = 965},
-  [407] = {.lex_state = 965},
-  [408] = {.lex_state = 965},
-  [409] = {.lex_state = 965},
-  [410] = {.lex_state = 965},
-  [411] = {.lex_state = 965},
-  [412] = {.lex_state = 965},
-  [413] = {.lex_state = 965},
-  [414] = {.lex_state = 965},
-  [415] = {.lex_state = 965},
-  [416] = {.lex_state = 965},
-  [417] = {.lex_state = 965},
-  [418] = {.lex_state = 965},
-  [419] = {.lex_state = 965},
-  [420] = {.lex_state = 965},
-  [421] = {.lex_state = 965},
-  [422] = {.lex_state = 965},
-  [423] = {.lex_state = 965},
-  [424] = {.lex_state = 965},
-  [425] = {.lex_state = 965},
-  [426] = {.lex_state = 965},
-  [427] = {.lex_state = 60},
-  [428] = {.lex_state = 965},
-  [429] = {.lex_state = 965},
-  [430] = {.lex_state = 965},
-  [431] = {.lex_state = 60},
-  [432] = {.lex_state = 965},
-  [433] = {.lex_state = 965},
-  [434] = {.lex_state = 965},
-  [435] = {.lex_state = 965},
-  [436] = {.lex_state = 965},
-  [437] = {.lex_state = 965},
-  [438] = {.lex_state = 965},
-  [439] = {.lex_state = 965},
-  [440] = {.lex_state = 965},
-  [441] = {.lex_state = 965},
-  [442] = {.lex_state = 965},
-  [443] = {.lex_state = 965},
-  [444] = {.lex_state = 965},
-  [445] = {.lex_state = 965},
-  [446] = {.lex_state = 965},
-  [447] = {.lex_state = 965},
-  [448] = {.lex_state = 965},
-  [449] = {.lex_state = 60},
-  [450] = {.lex_state = 59},
-  [451] = {.lex_state = 59},
-  [452] = {.lex_state = 64},
-  [453] = {.lex_state = 59},
-  [454] = {.lex_state = 64},
-  [455] = {.lex_state = 64},
-  [456] = {.lex_state = 99},
-  [457] = {.lex_state = 59},
-  [458] = {.lex_state = 60},
-  [459] = {.lex_state = 44},
-  [460] = {.lex_state = 64},
-  [461] = {.lex_state = 60},
-  [462] = {.lex_state = 64},
-  [463] = {.lex_state = 60},
+  [309] = {.lex_state = 66},
+  [310] = {.lex_state = 964},
+  [311] = {.lex_state = 66},
+  [312] = {.lex_state = 964},
+  [313] = {.lex_state = 964},
+  [314] = {.lex_state = 66},
+  [315] = {.lex_state = 964},
+  [316] = {.lex_state = 964},
+  [317] = {.lex_state = 964},
+  [318] = {.lex_state = 964},
+  [319] = {.lex_state = 964},
+  [320] = {.lex_state = 964},
+  [321] = {.lex_state = 964},
+  [322] = {.lex_state = 964},
+  [323] = {.lex_state = 964},
+  [324] = {.lex_state = 964},
+  [325] = {.lex_state = 964},
+  [326] = {.lex_state = 964},
+  [327] = {.lex_state = 964},
+  [328] = {.lex_state = 964},
+  [329] = {.lex_state = 964},
+  [330] = {.lex_state = 964},
+  [331] = {.lex_state = 964},
+  [332] = {.lex_state = 964},
+  [333] = {.lex_state = 66},
+  [334] = {.lex_state = 964},
+  [335] = {.lex_state = 964},
+  [336] = {.lex_state = 964},
+  [337] = {.lex_state = 964},
+  [338] = {.lex_state = 964},
+  [339] = {.lex_state = 964},
+  [340] = {.lex_state = 964},
+  [341] = {.lex_state = 964},
+  [342] = {.lex_state = 92},
+  [343] = {.lex_state = 964},
+  [344] = {.lex_state = 92},
+  [345] = {.lex_state = 964},
+  [346] = {.lex_state = 964},
+  [347] = {.lex_state = 964},
+  [348] = {.lex_state = 964},
+  [349] = {.lex_state = 964},
+  [350] = {.lex_state = 964},
+  [351] = {.lex_state = 964},
+  [352] = {.lex_state = 964},
+  [353] = {.lex_state = 964},
+  [354] = {.lex_state = 62},
+  [355] = {.lex_state = 964},
+  [356] = {.lex_state = 964},
+  [357] = {.lex_state = 964},
+  [358] = {.lex_state = 964},
+  [359] = {.lex_state = 964},
+  [360] = {.lex_state = 964},
+  [361] = {.lex_state = 964},
+  [362] = {.lex_state = 964},
+  [363] = {.lex_state = 964},
+  [364] = {.lex_state = 964},
+  [365] = {.lex_state = 62},
+  [366] = {.lex_state = 62},
+  [367] = {.lex_state = 964},
+  [368] = {.lex_state = 964},
+  [369] = {.lex_state = 964},
+  [370] = {.lex_state = 964},
+  [371] = {.lex_state = 964},
+  [372] = {.lex_state = 964},
+  [373] = {.lex_state = 964},
+  [374] = {.lex_state = 964},
+  [375] = {.lex_state = 964},
+  [376] = {.lex_state = 964},
+  [377] = {.lex_state = 964},
+  [378] = {.lex_state = 964},
+  [379] = {.lex_state = 964},
+  [380] = {.lex_state = 964},
+  [381] = {.lex_state = 964},
+  [382] = {.lex_state = 964},
+  [383] = {.lex_state = 964},
+  [384] = {.lex_state = 964},
+  [385] = {.lex_state = 964},
+  [386] = {.lex_state = 61},
+  [387] = {.lex_state = 964},
+  [388] = {.lex_state = 964},
+  [389] = {.lex_state = 964},
+  [390] = {.lex_state = 964},
+  [391] = {.lex_state = 964},
+  [392] = {.lex_state = 964},
+  [393] = {.lex_state = 964},
+  [394] = {.lex_state = 964},
+  [395] = {.lex_state = 964},
+  [396] = {.lex_state = 964},
+  [397] = {.lex_state = 964},
+  [398] = {.lex_state = 964},
+  [399] = {.lex_state = 964},
+  [400] = {.lex_state = 964},
+  [401] = {.lex_state = 964},
+  [402] = {.lex_state = 964},
+  [403] = {.lex_state = 964},
+  [404] = {.lex_state = 964},
+  [405] = {.lex_state = 964},
+  [406] = {.lex_state = 964},
+  [407] = {.lex_state = 964},
+  [408] = {.lex_state = 964},
+  [409] = {.lex_state = 964},
+  [410] = {.lex_state = 964},
+  [411] = {.lex_state = 964},
+  [412] = {.lex_state = 964},
+  [413] = {.lex_state = 92},
+  [414] = {.lex_state = 92},
+  [415] = {.lex_state = 964},
+  [416] = {.lex_state = 964},
+  [417] = {.lex_state = 964},
+  [418] = {.lex_state = 964},
+  [419] = {.lex_state = 964},
+  [420] = {.lex_state = 964},
+  [421] = {.lex_state = 964},
+  [422] = {.lex_state = 964},
+  [423] = {.lex_state = 964},
+  [424] = {.lex_state = 964},
+  [425] = {.lex_state = 964},
+  [426] = {.lex_state = 964},
+  [427] = {.lex_state = 964},
+  [428] = {.lex_state = 964},
+  [429] = {.lex_state = 964},
+  [430] = {.lex_state = 964},
+  [431] = {.lex_state = 62},
+  [432] = {.lex_state = 964},
+  [433] = {.lex_state = 964},
+  [434] = {.lex_state = 964},
+  [435] = {.lex_state = 964},
+  [436] = {.lex_state = 964},
+  [437] = {.lex_state = 964},
+  [438] = {.lex_state = 964},
+  [439] = {.lex_state = 964},
+  [440] = {.lex_state = 964},
+  [441] = {.lex_state = 964},
+  [442] = {.lex_state = 964},
+  [443] = {.lex_state = 964},
+  [444] = {.lex_state = 964},
+  [445] = {.lex_state = 964},
+  [446] = {.lex_state = 964},
+  [447] = {.lex_state = 964},
+  [448] = {.lex_state = 964},
+  [449] = {.lex_state = 98},
+  [450] = {.lex_state = 62},
+  [451] = {.lex_state = 62},
+  [452] = {.lex_state = 43},
+  [453] = {.lex_state = 62},
+  [454] = {.lex_state = 66},
+  [455] = {.lex_state = 62},
+  [456] = {.lex_state = 61},
+  [457] = {.lex_state = 61},
+  [458] = {.lex_state = 66},
+  [459] = {.lex_state = 66},
+  [460] = {.lex_state = 66},
+  [461] = {.lex_state = 66},
+  [462] = {.lex_state = 61},
+  [463] = {.lex_state = 61},
   [464] = {.lex_state = 0},
   [465] = {.lex_state = 0},
-  [466] = {.lex_state = 59},
-  [467] = {.lex_state = 95},
-  [468] = {.lex_state = 96},
-  [469] = {.lex_state = 97},
-  [470] = {.lex_state = 100},
-  [471] = {.lex_state = 96},
-  [472] = {.lex_state = 59},
-  [473] = {.lex_state = 99},
-  [474] = {.lex_state = 95},
-  [475] = {.lex_state = 59},
-  [476] = {.lex_state = 59},
+  [466] = {.lex_state = 62},
+  [467] = {.lex_state = 43},
+  [468] = {.lex_state = 0},
+  [469] = {.lex_state = 0},
+  [470] = {.lex_state = 0},
+  [471] = {.lex_state = 61},
+  [472] = {.lex_state = 0},
+  [473] = {.lex_state = 0},
+  [474] = {.lex_state = 0},
+  [475] = {.lex_state = 0},
+  [476] = {.lex_state = 66},
   [477] = {.lex_state = 98},
-  [478] = {.lex_state = 97},
-  [479] = {.lex_state = 60},
-  [480] = {.lex_state = 44},
-  [481] = {.lex_state = 0},
-  [482] = {.lex_state = 64},
-  [483] = {.lex_state = 0},
-  [484] = {.lex_state = 99},
-  [485] = {.lex_state = 64},
-  [486] = {.lex_state = 64},
-  [487] = {.lex_state = 44},
-  [488] = {.lex_state = 59},
-  [489] = {.lex_state = 0},
-  [490] = {.lex_state = 64},
-  [491] = {.lex_state = 59},
-  [492] = {.lex_state = 0},
-  [493] = {.lex_state = 0},
+  [478] = {.lex_state = 61},
+  [479] = {.lex_state = 66},
+  [480] = {.lex_state = 66},
+  [481] = {.lex_state = 66},
+  [482] = {.lex_state = 61},
+  [483] = {.lex_state = 98},
+  [484] = {.lex_state = 43},
+  [485] = {.lex_state = 0},
+  [486] = {.lex_state = 61},
+  [487] = {.lex_state = 1220},
+  [488] = {.lex_state = 66},
+  [489] = {.lex_state = 1227},
+  [490] = {.lex_state = 1234},
+  [491] = {.lex_state = 99},
+  [492] = {.lex_state = 61},
+  [493] = {.lex_state = 1220},
   [494] = {.lex_state = 0},
   [495] = {.lex_state = 0},
   [496] = {.lex_state = 0},
   [497] = {.lex_state = 0},
   [498] = {.lex_state = 0},
   [499] = {.lex_state = 0},
   [500] = {.lex_state = 0},
-  [501] = {.lex_state = 0},
+  [501] = {.lex_state = 1227},
   [502] = {.lex_state = 0},
   [503] = {.lex_state = 0},
   [504] = {.lex_state = 0},
   [505] = {.lex_state = 0},
   [506] = {.lex_state = 0},
-  [507] = {.lex_state = 64},
+  [507] = {.lex_state = 61},
   [508] = {.lex_state = 0},
-  [509] = {.lex_state = 0},
+  [509] = {.lex_state = 1234},
   [510] = {.lex_state = 0},
   [511] = {.lex_state = 0},
   [512] = {.lex_state = 0},
   [513] = {.lex_state = 0},
   [514] = {.lex_state = 0},
-  [515] = {.lex_state = 0},
+  [515] = {.lex_state = 97},
   [516] = {.lex_state = 0},
   [517] = {.lex_state = 0},
   [518] = {.lex_state = 0},
   [519] = {.lex_state = 0},
   [520] = {.lex_state = 0},
   [521] = {.lex_state = 0},
   [522] = {.lex_state = 0},
@@ -10850,49 +10826,49 @@
   [524] = {.lex_state = 0},
   [525] = {.lex_state = 0},
   [526] = {.lex_state = 0},
   [527] = {.lex_state = 0},
   [528] = {.lex_state = 0},
   [529] = {.lex_state = 0},
   [530] = {.lex_state = 0},
-  [531] = {.lex_state = 95},
-  [532] = {.lex_state = 96},
-  [533] = {.lex_state = 97},
-  [534] = {.lex_state = 100},
-  [535] = {.lex_state = 95},
-  [536] = {.lex_state = 96},
-  [537] = {.lex_state = 97},
-  [538] = {.lex_state = 95},
-  [539] = {.lex_state = 96},
-  [540] = {.lex_state = 97},
-  [541] = {.lex_state = 100},
-  [542] = {.lex_state = 95},
-  [543] = {.lex_state = 96},
-  [544] = {.lex_state = 97},
-  [545] = {.lex_state = 95},
-  [546] = {.lex_state = 96},
-  [547] = {.lex_state = 97},
-  [548] = {.lex_state = 95},
-  [549] = {.lex_state = 96},
-  [550] = {.lex_state = 97},
-  [551] = {.lex_state = 95},
-  [552] = {.lex_state = 96},
-  [553] = {.lex_state = 97},
-  [554] = {.lex_state = 95},
-  [555] = {.lex_state = 96},
-  [556] = {.lex_state = 97},
-  [557] = {.lex_state = 95},
-  [558] = {.lex_state = 96},
-  [559] = {.lex_state = 97},
-  [560] = {.lex_state = 95},
-  [561] = {.lex_state = 96},
-  [562] = {.lex_state = 97},
-  [563] = {.lex_state = 95},
-  [564] = {.lex_state = 96},
-  [565] = {.lex_state = 97},
+  [531] = {.lex_state = 1220},
+  [532] = {.lex_state = 1227},
+  [533] = {.lex_state = 1234},
+  [534] = {.lex_state = 99},
+  [535] = {.lex_state = 1220},
+  [536] = {.lex_state = 1227},
+  [537] = {.lex_state = 1234},
+  [538] = {.lex_state = 1220},
+  [539] = {.lex_state = 1227},
+  [540] = {.lex_state = 1234},
+  [541] = {.lex_state = 99},
+  [542] = {.lex_state = 1220},
+  [543] = {.lex_state = 1227},
+  [544] = {.lex_state = 1234},
+  [545] = {.lex_state = 1220},
+  [546] = {.lex_state = 1227},
+  [547] = {.lex_state = 1234},
+  [548] = {.lex_state = 1220},
+  [549] = {.lex_state = 1227},
+  [550] = {.lex_state = 1234},
+  [551] = {.lex_state = 1220},
+  [552] = {.lex_state = 1227},
+  [553] = {.lex_state = 1234},
+  [554] = {.lex_state = 1220},
+  [555] = {.lex_state = 1227},
+  [556] = {.lex_state = 1234},
+  [557] = {.lex_state = 1220},
+  [558] = {.lex_state = 1227},
+  [559] = {.lex_state = 1234},
+  [560] = {.lex_state = 1220},
+  [561] = {.lex_state = 1227},
+  [562] = {.lex_state = 1234},
+  [563] = {.lex_state = 1220},
+  [564] = {.lex_state = 1227},
+  [565] = {.lex_state = 1234},
 };
 
 static const uint16_t ts_parse_table[LARGE_STATE_COUNT][SYMBOL_COUNT] = {
   [0] = {
     [ts_builtin_sym_end] = ACTIONS(1),
     [anon_sym_account_DASHhook] = ACTIONS(1),
     [anon_sym_COMMA] = ACTIONS(1),
@@ -11056,102 +11032,102 @@
     [anon_sym_ask_DASHno] = ACTIONS(1),
     [anon_sym_SQUOTE] = ACTIONS(1),
     [anon_sym_DQUOTE] = ACTIONS(1),
     [anon_sym_BQUOTE] = ACTIONS(1),
     [anon_sym_source] = ACTIONS(1),
   },
   [1] = {
-    [sym_file] = STATE(515),
-    [sym__command] = STATE(159),
-    [sym_account_hook_directive] = STATE(159),
-    [sym_alias_directive] = STATE(159),
-    [sym_unalias_directive] = STATE(159),
-    [sym_alternates_directive] = STATE(159),
-    [sym_unalternates_directive] = STATE(159),
-    [sym_alternative_order_directive] = STATE(159),
-    [sym_unalternative_order_directive] = STATE(159),
-    [sym_attachments_directive] = STATE(159),
-    [sym_unattachments_directive] = STATE(159),
-    [sym_auto_view_directive] = STATE(159),
-    [sym_unauto_view_directive] = STATE(159),
-    [sym_bind_directive] = STATE(159),
-    [sym_unbind_directive] = STATE(159),
-    [sym_charset_hook_directive] = STATE(159),
-    [sym_iconv_hook_directive] = STATE(159),
-    [sym_color_directive] = STATE(159),
-    [sym_uncolor_directive] = STATE(159),
-    [sym_crypt_hook_directive] = STATE(159),
-    [sym_index_format_hook_directive] = STATE(159),
-    [sym_exec_directive] = STATE(159),
-    [sym_fcc_save_hook_directive] = STATE(159),
-    [sym_fcc_hook_directive] = STATE(159),
-    [sym_save_hook_directive] = STATE(159),
-    [sym_folder_hook_directive] = STATE(159),
-    [sym_group_directive] = STATE(159),
-    [sym_ungroup_directive] = STATE(159),
-    [sym_hdr_order_directive] = STATE(159),
-    [sym_unhdr_order_directive] = STATE(159),
-    [sym_ifdef_directive] = STATE(159),
-    [sym_ifndef_directive] = STATE(159),
-    [sym_finish_directive] = STATE(159),
-    [sym_ignore_directive] = STATE(159),
-    [sym_unignore_directive] = STATE(159),
-    [sym_lists_directive] = STATE(159),
-    [sym_unlists_directive] = STATE(159),
-    [sym_subscribe_directive] = STATE(159),
-    [sym_unsubscribe_directive] = STATE(159),
-    [sym_macro_directive] = STATE(159),
-    [sym_unmacro_directive] = STATE(159),
-    [sym_mailboxes_directive] = STATE(159),
-    [sym_named_mailboxes_directive] = STATE(159),
-    [sym_unmailboxes_directive] = STATE(159),
-    [sym_mailto_allow_directive] = STATE(159),
-    [sym_unmailto_allow_directive] = STATE(159),
-    [sym_echo_directive] = STATE(159),
-    [sym_cd_directive] = STATE(159),
-    [sym_mbox_hook_directive] = STATE(159),
-    [sym_message_hook_directive] = STATE(159),
-    [sym_mime_lookup_directive] = STATE(159),
-    [sym_unmime_lookup_directive] = STATE(159),
-    [sym_mono_directive] = STATE(159),
-    [sym_unmono_directive] = STATE(159),
-    [sym_my_hdr_directive] = STATE(159),
-    [sym_unmy_hdr_directive] = STATE(159),
-    [sym_open_hook_directive] = STATE(159),
-    [sym_close_hook_directive] = STATE(159),
-    [sym_append_hook_directive] = STATE(159),
-    [sym_push_directive] = STATE(159),
-    [sym_reply_hook_directive] = STATE(159),
-    [sym_send_hook_directive] = STATE(159),
-    [sym_send2_hook_directive] = STATE(159),
-    [sym_spam_directive] = STATE(159),
-    [sym_nospam_directive] = STATE(159),
-    [sym_subjectrx_directive] = STATE(159),
-    [sym_unsubjectrx_directive] = STATE(159),
-    [sym_subscribe_to_directive] = STATE(159),
-    [sym_unsubscribe_from_directive] = STATE(159),
-    [sym_timeout_hook_directive] = STATE(159),
-    [sym_startup_hook_directive] = STATE(159),
-    [sym_shutdown_hook_directive] = STATE(159),
-    [sym_unhook_directive] = STATE(159),
-    [sym_set_directive] = STATE(159),
-    [sym_unset_directive] = STATE(159),
-    [sym_reset_directive] = STATE(159),
-    [sym_toggle_directive] = STATE(159),
-    [sym_setenv_directive] = STATE(159),
-    [sym_unsetenv_directive] = STATE(159),
-    [sym_sidebar_pin_directive] = STATE(159),
-    [sym_sidebar_unpin_directive] = STATE(159),
-    [sym_score_directive] = STATE(159),
-    [sym_unscore_directive] = STATE(159),
-    [sym_source_directive] = STATE(159),
-    [sym__space] = STATE(459),
+    [sym_file] = STATE(485),
+    [sym__command] = STATE(98),
+    [sym_account_hook_directive] = STATE(98),
+    [sym_alias_directive] = STATE(98),
+    [sym_unalias_directive] = STATE(98),
+    [sym_alternates_directive] = STATE(98),
+    [sym_unalternates_directive] = STATE(98),
+    [sym_alternative_order_directive] = STATE(98),
+    [sym_unalternative_order_directive] = STATE(98),
+    [sym_attachments_directive] = STATE(98),
+    [sym_unattachments_directive] = STATE(98),
+    [sym_auto_view_directive] = STATE(98),
+    [sym_unauto_view_directive] = STATE(98),
+    [sym_bind_directive] = STATE(98),
+    [sym_unbind_directive] = STATE(98),
+    [sym_charset_hook_directive] = STATE(98),
+    [sym_iconv_hook_directive] = STATE(98),
+    [sym_color_directive] = STATE(98),
+    [sym_uncolor_directive] = STATE(98),
+    [sym_crypt_hook_directive] = STATE(98),
+    [sym_index_format_hook_directive] = STATE(98),
+    [sym_exec_directive] = STATE(98),
+    [sym_fcc_save_hook_directive] = STATE(98),
+    [sym_fcc_hook_directive] = STATE(98),
+    [sym_save_hook_directive] = STATE(98),
+    [sym_folder_hook_directive] = STATE(98),
+    [sym_group_directive] = STATE(98),
+    [sym_ungroup_directive] = STATE(98),
+    [sym_hdr_order_directive] = STATE(98),
+    [sym_unhdr_order_directive] = STATE(98),
+    [sym_ifdef_directive] = STATE(98),
+    [sym_ifndef_directive] = STATE(98),
+    [sym_finish_directive] = STATE(98),
+    [sym_ignore_directive] = STATE(98),
+    [sym_unignore_directive] = STATE(98),
+    [sym_lists_directive] = STATE(98),
+    [sym_unlists_directive] = STATE(98),
+    [sym_subscribe_directive] = STATE(98),
+    [sym_unsubscribe_directive] = STATE(98),
+    [sym_macro_directive] = STATE(98),
+    [sym_unmacro_directive] = STATE(98),
+    [sym_mailboxes_directive] = STATE(98),
+    [sym_named_mailboxes_directive] = STATE(98),
+    [sym_unmailboxes_directive] = STATE(98),
+    [sym_mailto_allow_directive] = STATE(98),
+    [sym_unmailto_allow_directive] = STATE(98),
+    [sym_echo_directive] = STATE(98),
+    [sym_cd_directive] = STATE(98),
+    [sym_mbox_hook_directive] = STATE(98),
+    [sym_message_hook_directive] = STATE(98),
+    [sym_mime_lookup_directive] = STATE(98),
+    [sym_unmime_lookup_directive] = STATE(98),
+    [sym_mono_directive] = STATE(98),
+    [sym_unmono_directive] = STATE(98),
+    [sym_my_hdr_directive] = STATE(98),
+    [sym_unmy_hdr_directive] = STATE(98),
+    [sym_open_hook_directive] = STATE(98),
+    [sym_close_hook_directive] = STATE(98),
+    [sym_append_hook_directive] = STATE(98),
+    [sym_push_directive] = STATE(98),
+    [sym_reply_hook_directive] = STATE(98),
+    [sym_send_hook_directive] = STATE(98),
+    [sym_send2_hook_directive] = STATE(98),
+    [sym_spam_directive] = STATE(98),
+    [sym_nospam_directive] = STATE(98),
+    [sym_subjectrx_directive] = STATE(98),
+    [sym_unsubjectrx_directive] = STATE(98),
+    [sym_subscribe_to_directive] = STATE(98),
+    [sym_unsubscribe_from_directive] = STATE(98),
+    [sym_timeout_hook_directive] = STATE(98),
+    [sym_startup_hook_directive] = STATE(98),
+    [sym_shutdown_hook_directive] = STATE(98),
+    [sym_unhook_directive] = STATE(98),
+    [sym_set_directive] = STATE(98),
+    [sym_unset_directive] = STATE(98),
+    [sym_reset_directive] = STATE(98),
+    [sym_toggle_directive] = STATE(98),
+    [sym_setenv_directive] = STATE(98),
+    [sym_unsetenv_directive] = STATE(98),
+    [sym_sidebar_pin_directive] = STATE(98),
+    [sym_sidebar_unpin_directive] = STATE(98),
+    [sym_score_directive] = STATE(98),
+    [sym_unscore_directive] = STATE(98),
+    [sym_source_directive] = STATE(98),
+    [sym__space] = STATE(452),
     [sym__end] = STATE(3),
     [aux_sym_file_repeat1] = STATE(3),
-    [aux_sym__space_repeat1] = STATE(288),
+    [aux_sym__space_repeat1] = STATE(285),
     [ts_builtin_sym_end] = ACTIONS(3),
     [anon_sym_account_DASHhook] = ACTIONS(5),
     [anon_sym_alias] = ACTIONS(7),
     [anon_sym_unalias] = ACTIONS(9),
     [anon_sym_alternates] = ACTIONS(11),
     [anon_sym_unalternates] = ACTIONS(13),
     [anon_sym_alternative_order] = ACTIONS(15),
@@ -11232,101 +11208,101 @@
     [anon_sym_unscore] = ACTIONS(165),
     [anon_sym_source] = ACTIONS(167),
     [sym_comment] = ACTIONS(169),
     [sym__eol] = ACTIONS(171),
     [aux_sym__space_token1] = ACTIONS(173),
   },
   [2] = {
-    [sym__command] = STATE(159),
-    [sym_account_hook_directive] = STATE(159),
-    [sym_alias_directive] = STATE(159),
-    [sym_unalias_directive] = STATE(159),
-    [sym_alternates_directive] = STATE(159),
-    [sym_unalternates_directive] = STATE(159),
-    [sym_alternative_order_directive] = STATE(159),
-    [sym_unalternative_order_directive] = STATE(159),
-    [sym_attachments_directive] = STATE(159),
-    [sym_unattachments_directive] = STATE(159),
-    [sym_auto_view_directive] = STATE(159),
-    [sym_unauto_view_directive] = STATE(159),
-    [sym_bind_directive] = STATE(159),
-    [sym_unbind_directive] = STATE(159),
-    [sym_charset_hook_directive] = STATE(159),
-    [sym_iconv_hook_directive] = STATE(159),
-    [sym_color_directive] = STATE(159),
-    [sym_uncolor_directive] = STATE(159),
-    [sym_crypt_hook_directive] = STATE(159),
-    [sym_index_format_hook_directive] = STATE(159),
-    [sym_exec_directive] = STATE(159),
-    [sym_fcc_save_hook_directive] = STATE(159),
-    [sym_fcc_hook_directive] = STATE(159),
-    [sym_save_hook_directive] = STATE(159),
-    [sym_folder_hook_directive] = STATE(159),
-    [sym_group_directive] = STATE(159),
-    [sym_ungroup_directive] = STATE(159),
-    [sym_hdr_order_directive] = STATE(159),
-    [sym_unhdr_order_directive] = STATE(159),
-    [sym_ifdef_directive] = STATE(159),
-    [sym_ifndef_directive] = STATE(159),
-    [sym_finish_directive] = STATE(159),
-    [sym_ignore_directive] = STATE(159),
-    [sym_unignore_directive] = STATE(159),
-    [sym_lists_directive] = STATE(159),
-    [sym_unlists_directive] = STATE(159),
-    [sym_subscribe_directive] = STATE(159),
-    [sym_unsubscribe_directive] = STATE(159),
-    [sym_macro_directive] = STATE(159),
-    [sym_unmacro_directive] = STATE(159),
-    [sym_mailboxes_directive] = STATE(159),
-    [sym_named_mailboxes_directive] = STATE(159),
-    [sym_unmailboxes_directive] = STATE(159),
-    [sym_mailto_allow_directive] = STATE(159),
-    [sym_unmailto_allow_directive] = STATE(159),
-    [sym_echo_directive] = STATE(159),
-    [sym_cd_directive] = STATE(159),
-    [sym_mbox_hook_directive] = STATE(159),
-    [sym_message_hook_directive] = STATE(159),
-    [sym_mime_lookup_directive] = STATE(159),
-    [sym_unmime_lookup_directive] = STATE(159),
-    [sym_mono_directive] = STATE(159),
-    [sym_unmono_directive] = STATE(159),
-    [sym_my_hdr_directive] = STATE(159),
-    [sym_unmy_hdr_directive] = STATE(159),
-    [sym_open_hook_directive] = STATE(159),
-    [sym_close_hook_directive] = STATE(159),
-    [sym_append_hook_directive] = STATE(159),
-    [sym_push_directive] = STATE(159),
-    [sym_reply_hook_directive] = STATE(159),
-    [sym_send_hook_directive] = STATE(159),
-    [sym_send2_hook_directive] = STATE(159),
-    [sym_spam_directive] = STATE(159),
-    [sym_nospam_directive] = STATE(159),
-    [sym_subjectrx_directive] = STATE(159),
-    [sym_unsubjectrx_directive] = STATE(159),
-    [sym_subscribe_to_directive] = STATE(159),
-    [sym_unsubscribe_from_directive] = STATE(159),
-    [sym_timeout_hook_directive] = STATE(159),
-    [sym_startup_hook_directive] = STATE(159),
-    [sym_shutdown_hook_directive] = STATE(159),
-    [sym_unhook_directive] = STATE(159),
-    [sym_set_directive] = STATE(159),
-    [sym_unset_directive] = STATE(159),
-    [sym_reset_directive] = STATE(159),
-    [sym_toggle_directive] = STATE(159),
-    [sym_setenv_directive] = STATE(159),
-    [sym_unsetenv_directive] = STATE(159),
-    [sym_sidebar_pin_directive] = STATE(159),
-    [sym_sidebar_unpin_directive] = STATE(159),
-    [sym_score_directive] = STATE(159),
-    [sym_unscore_directive] = STATE(159),
-    [sym_source_directive] = STATE(159),
-    [sym__space] = STATE(459),
+    [sym__command] = STATE(98),
+    [sym_account_hook_directive] = STATE(98),
+    [sym_alias_directive] = STATE(98),
+    [sym_unalias_directive] = STATE(98),
+    [sym_alternates_directive] = STATE(98),
+    [sym_unalternates_directive] = STATE(98),
+    [sym_alternative_order_directive] = STATE(98),
+    [sym_unalternative_order_directive] = STATE(98),
+    [sym_attachments_directive] = STATE(98),
+    [sym_unattachments_directive] = STATE(98),
+    [sym_auto_view_directive] = STATE(98),
+    [sym_unauto_view_directive] = STATE(98),
+    [sym_bind_directive] = STATE(98),
+    [sym_unbind_directive] = STATE(98),
+    [sym_charset_hook_directive] = STATE(98),
+    [sym_iconv_hook_directive] = STATE(98),
+    [sym_color_directive] = STATE(98),
+    [sym_uncolor_directive] = STATE(98),
+    [sym_crypt_hook_directive] = STATE(98),
+    [sym_index_format_hook_directive] = STATE(98),
+    [sym_exec_directive] = STATE(98),
+    [sym_fcc_save_hook_directive] = STATE(98),
+    [sym_fcc_hook_directive] = STATE(98),
+    [sym_save_hook_directive] = STATE(98),
+    [sym_folder_hook_directive] = STATE(98),
+    [sym_group_directive] = STATE(98),
+    [sym_ungroup_directive] = STATE(98),
+    [sym_hdr_order_directive] = STATE(98),
+    [sym_unhdr_order_directive] = STATE(98),
+    [sym_ifdef_directive] = STATE(98),
+    [sym_ifndef_directive] = STATE(98),
+    [sym_finish_directive] = STATE(98),
+    [sym_ignore_directive] = STATE(98),
+    [sym_unignore_directive] = STATE(98),
+    [sym_lists_directive] = STATE(98),
+    [sym_unlists_directive] = STATE(98),
+    [sym_subscribe_directive] = STATE(98),
+    [sym_unsubscribe_directive] = STATE(98),
+    [sym_macro_directive] = STATE(98),
+    [sym_unmacro_directive] = STATE(98),
+    [sym_mailboxes_directive] = STATE(98),
+    [sym_named_mailboxes_directive] = STATE(98),
+    [sym_unmailboxes_directive] = STATE(98),
+    [sym_mailto_allow_directive] = STATE(98),
+    [sym_unmailto_allow_directive] = STATE(98),
+    [sym_echo_directive] = STATE(98),
+    [sym_cd_directive] = STATE(98),
+    [sym_mbox_hook_directive] = STATE(98),
+    [sym_message_hook_directive] = STATE(98),
+    [sym_mime_lookup_directive] = STATE(98),
+    [sym_unmime_lookup_directive] = STATE(98),
+    [sym_mono_directive] = STATE(98),
+    [sym_unmono_directive] = STATE(98),
+    [sym_my_hdr_directive] = STATE(98),
+    [sym_unmy_hdr_directive] = STATE(98),
+    [sym_open_hook_directive] = STATE(98),
+    [sym_close_hook_directive] = STATE(98),
+    [sym_append_hook_directive] = STATE(98),
+    [sym_push_directive] = STATE(98),
+    [sym_reply_hook_directive] = STATE(98),
+    [sym_send_hook_directive] = STATE(98),
+    [sym_send2_hook_directive] = STATE(98),
+    [sym_spam_directive] = STATE(98),
+    [sym_nospam_directive] = STATE(98),
+    [sym_subjectrx_directive] = STATE(98),
+    [sym_unsubjectrx_directive] = STATE(98),
+    [sym_subscribe_to_directive] = STATE(98),
+    [sym_unsubscribe_from_directive] = STATE(98),
+    [sym_timeout_hook_directive] = STATE(98),
+    [sym_startup_hook_directive] = STATE(98),
+    [sym_shutdown_hook_directive] = STATE(98),
+    [sym_unhook_directive] = STATE(98),
+    [sym_set_directive] = STATE(98),
+    [sym_unset_directive] = STATE(98),
+    [sym_reset_directive] = STATE(98),
+    [sym_toggle_directive] = STATE(98),
+    [sym_setenv_directive] = STATE(98),
+    [sym_unsetenv_directive] = STATE(98),
+    [sym_sidebar_pin_directive] = STATE(98),
+    [sym_sidebar_unpin_directive] = STATE(98),
+    [sym_score_directive] = STATE(98),
+    [sym_unscore_directive] = STATE(98),
+    [sym_source_directive] = STATE(98),
+    [sym__space] = STATE(452),
     [sym__end] = STATE(2),
     [aux_sym_file_repeat1] = STATE(2),
-    [aux_sym__space_repeat1] = STATE(288),
+    [aux_sym__space_repeat1] = STATE(285),
     [ts_builtin_sym_end] = ACTIONS(175),
     [anon_sym_account_DASHhook] = ACTIONS(177),
     [anon_sym_alias] = ACTIONS(180),
     [anon_sym_unalias] = ACTIONS(183),
     [anon_sym_alternates] = ACTIONS(186),
     [anon_sym_unalternates] = ACTIONS(189),
     [anon_sym_alternative_order] = ACTIONS(192),
@@ -11407,101 +11383,101 @@
     [anon_sym_unscore] = ACTIONS(417),
     [anon_sym_source] = ACTIONS(420),
     [sym_comment] = ACTIONS(423),
     [sym__eol] = ACTIONS(426),
     [aux_sym__space_token1] = ACTIONS(429),
   },
   [3] = {
-    [sym__command] = STATE(159),
-    [sym_account_hook_directive] = STATE(159),
-    [sym_alias_directive] = STATE(159),
-    [sym_unalias_directive] = STATE(159),
-    [sym_alternates_directive] = STATE(159),
-    [sym_unalternates_directive] = STATE(159),
-    [sym_alternative_order_directive] = STATE(159),
-    [sym_unalternative_order_directive] = STATE(159),
-    [sym_attachments_directive] = STATE(159),
-    [sym_unattachments_directive] = STATE(159),
-    [sym_auto_view_directive] = STATE(159),
-    [sym_unauto_view_directive] = STATE(159),
-    [sym_bind_directive] = STATE(159),
-    [sym_unbind_directive] = STATE(159),
-    [sym_charset_hook_directive] = STATE(159),
-    [sym_iconv_hook_directive] = STATE(159),
-    [sym_color_directive] = STATE(159),
-    [sym_uncolor_directive] = STATE(159),
-    [sym_crypt_hook_directive] = STATE(159),
-    [sym_index_format_hook_directive] = STATE(159),
-    [sym_exec_directive] = STATE(159),
-    [sym_fcc_save_hook_directive] = STATE(159),
-    [sym_fcc_hook_directive] = STATE(159),
-    [sym_save_hook_directive] = STATE(159),
-    [sym_folder_hook_directive] = STATE(159),
-    [sym_group_directive] = STATE(159),
-    [sym_ungroup_directive] = STATE(159),
-    [sym_hdr_order_directive] = STATE(159),
-    [sym_unhdr_order_directive] = STATE(159),
-    [sym_ifdef_directive] = STATE(159),
-    [sym_ifndef_directive] = STATE(159),
-    [sym_finish_directive] = STATE(159),
-    [sym_ignore_directive] = STATE(159),
-    [sym_unignore_directive] = STATE(159),
-    [sym_lists_directive] = STATE(159),
-    [sym_unlists_directive] = STATE(159),
-    [sym_subscribe_directive] = STATE(159),
-    [sym_unsubscribe_directive] = STATE(159),
-    [sym_macro_directive] = STATE(159),
-    [sym_unmacro_directive] = STATE(159),
-    [sym_mailboxes_directive] = STATE(159),
-    [sym_named_mailboxes_directive] = STATE(159),
-    [sym_unmailboxes_directive] = STATE(159),
-    [sym_mailto_allow_directive] = STATE(159),
-    [sym_unmailto_allow_directive] = STATE(159),
-    [sym_echo_directive] = STATE(159),
-    [sym_cd_directive] = STATE(159),
-    [sym_mbox_hook_directive] = STATE(159),
-    [sym_message_hook_directive] = STATE(159),
-    [sym_mime_lookup_directive] = STATE(159),
-    [sym_unmime_lookup_directive] = STATE(159),
-    [sym_mono_directive] = STATE(159),
-    [sym_unmono_directive] = STATE(159),
-    [sym_my_hdr_directive] = STATE(159),
-    [sym_unmy_hdr_directive] = STATE(159),
-    [sym_open_hook_directive] = STATE(159),
-    [sym_close_hook_directive] = STATE(159),
-    [sym_append_hook_directive] = STATE(159),
-    [sym_push_directive] = STATE(159),
-    [sym_reply_hook_directive] = STATE(159),
-    [sym_send_hook_directive] = STATE(159),
-    [sym_send2_hook_directive] = STATE(159),
-    [sym_spam_directive] = STATE(159),
-    [sym_nospam_directive] = STATE(159),
-    [sym_subjectrx_directive] = STATE(159),
-    [sym_unsubjectrx_directive] = STATE(159),
-    [sym_subscribe_to_directive] = STATE(159),
-    [sym_unsubscribe_from_directive] = STATE(159),
-    [sym_timeout_hook_directive] = STATE(159),
-    [sym_startup_hook_directive] = STATE(159),
-    [sym_shutdown_hook_directive] = STATE(159),
-    [sym_unhook_directive] = STATE(159),
-    [sym_set_directive] = STATE(159),
-    [sym_unset_directive] = STATE(159),
-    [sym_reset_directive] = STATE(159),
-    [sym_toggle_directive] = STATE(159),
-    [sym_setenv_directive] = STATE(159),
-    [sym_unsetenv_directive] = STATE(159),
-    [sym_sidebar_pin_directive] = STATE(159),
-    [sym_sidebar_unpin_directive] = STATE(159),
-    [sym_score_directive] = STATE(159),
-    [sym_unscore_directive] = STATE(159),
-    [sym_source_directive] = STATE(159),
-    [sym__space] = STATE(459),
+    [sym__command] = STATE(98),
+    [sym_account_hook_directive] = STATE(98),
+    [sym_alias_directive] = STATE(98),
+    [sym_unalias_directive] = STATE(98),
+    [sym_alternates_directive] = STATE(98),
+    [sym_unalternates_directive] = STATE(98),
+    [sym_alternative_order_directive] = STATE(98),
+    [sym_unalternative_order_directive] = STATE(98),
+    [sym_attachments_directive] = STATE(98),
+    [sym_unattachments_directive] = STATE(98),
+    [sym_auto_view_directive] = STATE(98),
+    [sym_unauto_view_directive] = STATE(98),
+    [sym_bind_directive] = STATE(98),
+    [sym_unbind_directive] = STATE(98),
+    [sym_charset_hook_directive] = STATE(98),
+    [sym_iconv_hook_directive] = STATE(98),
+    [sym_color_directive] = STATE(98),
+    [sym_uncolor_directive] = STATE(98),
+    [sym_crypt_hook_directive] = STATE(98),
+    [sym_index_format_hook_directive] = STATE(98),
+    [sym_exec_directive] = STATE(98),
+    [sym_fcc_save_hook_directive] = STATE(98),
+    [sym_fcc_hook_directive] = STATE(98),
+    [sym_save_hook_directive] = STATE(98),
+    [sym_folder_hook_directive] = STATE(98),
+    [sym_group_directive] = STATE(98),
+    [sym_ungroup_directive] = STATE(98),
+    [sym_hdr_order_directive] = STATE(98),
+    [sym_unhdr_order_directive] = STATE(98),
+    [sym_ifdef_directive] = STATE(98),
+    [sym_ifndef_directive] = STATE(98),
+    [sym_finish_directive] = STATE(98),
+    [sym_ignore_directive] = STATE(98),
+    [sym_unignore_directive] = STATE(98),
+    [sym_lists_directive] = STATE(98),
+    [sym_unlists_directive] = STATE(98),
+    [sym_subscribe_directive] = STATE(98),
+    [sym_unsubscribe_directive] = STATE(98),
+    [sym_macro_directive] = STATE(98),
+    [sym_unmacro_directive] = STATE(98),
+    [sym_mailboxes_directive] = STATE(98),
+    [sym_named_mailboxes_directive] = STATE(98),
+    [sym_unmailboxes_directive] = STATE(98),
+    [sym_mailto_allow_directive] = STATE(98),
+    [sym_unmailto_allow_directive] = STATE(98),
+    [sym_echo_directive] = STATE(98),
+    [sym_cd_directive] = STATE(98),
+    [sym_mbox_hook_directive] = STATE(98),
+    [sym_message_hook_directive] = STATE(98),
+    [sym_mime_lookup_directive] = STATE(98),
+    [sym_unmime_lookup_directive] = STATE(98),
+    [sym_mono_directive] = STATE(98),
+    [sym_unmono_directive] = STATE(98),
+    [sym_my_hdr_directive] = STATE(98),
+    [sym_unmy_hdr_directive] = STATE(98),
+    [sym_open_hook_directive] = STATE(98),
+    [sym_close_hook_directive] = STATE(98),
+    [sym_append_hook_directive] = STATE(98),
+    [sym_push_directive] = STATE(98),
+    [sym_reply_hook_directive] = STATE(98),
+    [sym_send_hook_directive] = STATE(98),
+    [sym_send2_hook_directive] = STATE(98),
+    [sym_spam_directive] = STATE(98),
+    [sym_nospam_directive] = STATE(98),
+    [sym_subjectrx_directive] = STATE(98),
+    [sym_unsubjectrx_directive] = STATE(98),
+    [sym_subscribe_to_directive] = STATE(98),
+    [sym_unsubscribe_from_directive] = STATE(98),
+    [sym_timeout_hook_directive] = STATE(98),
+    [sym_startup_hook_directive] = STATE(98),
+    [sym_shutdown_hook_directive] = STATE(98),
+    [sym_unhook_directive] = STATE(98),
+    [sym_set_directive] = STATE(98),
+    [sym_unset_directive] = STATE(98),
+    [sym_reset_directive] = STATE(98),
+    [sym_toggle_directive] = STATE(98),
+    [sym_setenv_directive] = STATE(98),
+    [sym_unsetenv_directive] = STATE(98),
+    [sym_sidebar_pin_directive] = STATE(98),
+    [sym_sidebar_unpin_directive] = STATE(98),
+    [sym_score_directive] = STATE(98),
+    [sym_unscore_directive] = STATE(98),
+    [sym_source_directive] = STATE(98),
+    [sym__space] = STATE(452),
     [sym__end] = STATE(2),
     [aux_sym_file_repeat1] = STATE(2),
-    [aux_sym__space_repeat1] = STATE(288),
+    [aux_sym__space_repeat1] = STATE(285),
     [ts_builtin_sym_end] = ACTIONS(432),
     [anon_sym_account_DASHhook] = ACTIONS(5),
     [anon_sym_alias] = ACTIONS(7),
     [anon_sym_unalias] = ACTIONS(9),
     [anon_sym_alternates] = ACTIONS(11),
     [anon_sym_unalternates] = ACTIONS(13),
     [anon_sym_alternative_order] = ACTIONS(15),
@@ -11582,97 +11558,97 @@
     [anon_sym_unscore] = ACTIONS(165),
     [anon_sym_source] = ACTIONS(167),
     [sym_comment] = ACTIONS(169),
     [sym__eol] = ACTIONS(434),
     [aux_sym__space_token1] = ACTIONS(173),
   },
   [4] = {
-    [sym__command] = STATE(331),
-    [sym_account_hook_directive] = STATE(331),
-    [sym_alias_directive] = STATE(331),
-    [sym_unalias_directive] = STATE(331),
-    [sym_alternates_directive] = STATE(331),
-    [sym_unalternates_directive] = STATE(331),
-    [sym_alternative_order_directive] = STATE(331),
-    [sym_unalternative_order_directive] = STATE(331),
-    [sym_attachments_directive] = STATE(331),
-    [sym_unattachments_directive] = STATE(331),
-    [sym_auto_view_directive] = STATE(331),
-    [sym_unauto_view_directive] = STATE(331),
-    [sym_bind_directive] = STATE(331),
-    [sym_unbind_directive] = STATE(331),
-    [sym_charset_hook_directive] = STATE(331),
-    [sym_iconv_hook_directive] = STATE(331),
-    [sym_color_directive] = STATE(331),
-    [sym_uncolor_directive] = STATE(331),
-    [sym_crypt_hook_directive] = STATE(331),
-    [sym_index_format_hook_directive] = STATE(331),
-    [sym_exec_directive] = STATE(331),
-    [sym_fcc_save_hook_directive] = STATE(331),
-    [sym_fcc_hook_directive] = STATE(331),
-    [sym_save_hook_directive] = STATE(331),
-    [sym_folder_hook_directive] = STATE(331),
-    [sym_group_directive] = STATE(331),
-    [sym_ungroup_directive] = STATE(331),
-    [sym_hdr_order_directive] = STATE(331),
-    [sym_unhdr_order_directive] = STATE(331),
-    [sym_ifdef_directive] = STATE(331),
-    [sym_ifndef_directive] = STATE(331),
-    [sym_finish_directive] = STATE(331),
-    [sym_ignore_directive] = STATE(331),
-    [sym_unignore_directive] = STATE(331),
-    [sym_lists_directive] = STATE(331),
-    [sym_unlists_directive] = STATE(331),
-    [sym_subscribe_directive] = STATE(331),
-    [sym_unsubscribe_directive] = STATE(331),
-    [sym_macro_directive] = STATE(331),
-    [sym_unmacro_directive] = STATE(331),
-    [sym_mailboxes_directive] = STATE(331),
-    [sym_named_mailboxes_directive] = STATE(331),
-    [sym_unmailboxes_directive] = STATE(331),
-    [sym_mailto_allow_directive] = STATE(331),
-    [sym_unmailto_allow_directive] = STATE(331),
-    [sym_echo_directive] = STATE(331),
-    [sym_cd_directive] = STATE(331),
-    [sym_mbox_hook_directive] = STATE(331),
-    [sym_message_hook_directive] = STATE(331),
-    [sym_mime_lookup_directive] = STATE(331),
-    [sym_unmime_lookup_directive] = STATE(331),
-    [sym_mono_directive] = STATE(331),
-    [sym_unmono_directive] = STATE(331),
-    [sym_my_hdr_directive] = STATE(331),
-    [sym_unmy_hdr_directive] = STATE(331),
-    [sym_open_hook_directive] = STATE(331),
-    [sym_close_hook_directive] = STATE(331),
-    [sym_append_hook_directive] = STATE(331),
-    [sym_push_directive] = STATE(331),
-    [sym_reply_hook_directive] = STATE(331),
-    [sym_send_hook_directive] = STATE(331),
-    [sym_send2_hook_directive] = STATE(331),
-    [sym_spam_directive] = STATE(331),
-    [sym_nospam_directive] = STATE(331),
-    [sym_subjectrx_directive] = STATE(331),
-    [sym_unsubjectrx_directive] = STATE(331),
-    [sym_subscribe_to_directive] = STATE(331),
-    [sym_unsubscribe_from_directive] = STATE(331),
-    [sym_timeout_hook_directive] = STATE(331),
-    [sym_startup_hook_directive] = STATE(331),
-    [sym_shutdown_hook_directive] = STATE(331),
-    [sym_unhook_directive] = STATE(331),
-    [sym_set_directive] = STATE(331),
-    [sym_unset_directive] = STATE(331),
-    [sym_reset_directive] = STATE(331),
-    [sym_toggle_directive] = STATE(331),
-    [sym_setenv_directive] = STATE(331),
-    [sym_unsetenv_directive] = STATE(331),
-    [sym_sidebar_pin_directive] = STATE(331),
-    [sym_sidebar_unpin_directive] = STATE(331),
-    [sym_score_directive] = STATE(331),
-    [sym_unscore_directive] = STATE(331),
-    [sym_source_directive] = STATE(331),
+    [sym__command] = STATE(327),
+    [sym_account_hook_directive] = STATE(327),
+    [sym_alias_directive] = STATE(327),
+    [sym_unalias_directive] = STATE(327),
+    [sym_alternates_directive] = STATE(327),
+    [sym_unalternates_directive] = STATE(327),
+    [sym_alternative_order_directive] = STATE(327),
+    [sym_unalternative_order_directive] = STATE(327),
+    [sym_attachments_directive] = STATE(327),
+    [sym_unattachments_directive] = STATE(327),
+    [sym_auto_view_directive] = STATE(327),
+    [sym_unauto_view_directive] = STATE(327),
+    [sym_bind_directive] = STATE(327),
+    [sym_unbind_directive] = STATE(327),
+    [sym_charset_hook_directive] = STATE(327),
+    [sym_iconv_hook_directive] = STATE(327),
+    [sym_color_directive] = STATE(327),
+    [sym_uncolor_directive] = STATE(327),
+    [sym_crypt_hook_directive] = STATE(327),
+    [sym_index_format_hook_directive] = STATE(327),
+    [sym_exec_directive] = STATE(327),
+    [sym_fcc_save_hook_directive] = STATE(327),
+    [sym_fcc_hook_directive] = STATE(327),
+    [sym_save_hook_directive] = STATE(327),
+    [sym_folder_hook_directive] = STATE(327),
+    [sym_group_directive] = STATE(327),
+    [sym_ungroup_directive] = STATE(327),
+    [sym_hdr_order_directive] = STATE(327),
+    [sym_unhdr_order_directive] = STATE(327),
+    [sym_ifdef_directive] = STATE(327),
+    [sym_ifndef_directive] = STATE(327),
+    [sym_finish_directive] = STATE(327),
+    [sym_ignore_directive] = STATE(327),
+    [sym_unignore_directive] = STATE(327),
+    [sym_lists_directive] = STATE(327),
+    [sym_unlists_directive] = STATE(327),
+    [sym_subscribe_directive] = STATE(327),
+    [sym_unsubscribe_directive] = STATE(327),
+    [sym_macro_directive] = STATE(327),
+    [sym_unmacro_directive] = STATE(327),
+    [sym_mailboxes_directive] = STATE(327),
+    [sym_named_mailboxes_directive] = STATE(327),
+    [sym_unmailboxes_directive] = STATE(327),
+    [sym_mailto_allow_directive] = STATE(327),
+    [sym_unmailto_allow_directive] = STATE(327),
+    [sym_echo_directive] = STATE(327),
+    [sym_cd_directive] = STATE(327),
+    [sym_mbox_hook_directive] = STATE(327),
+    [sym_message_hook_directive] = STATE(327),
+    [sym_mime_lookup_directive] = STATE(327),
+    [sym_unmime_lookup_directive] = STATE(327),
+    [sym_mono_directive] = STATE(327),
+    [sym_unmono_directive] = STATE(327),
+    [sym_my_hdr_directive] = STATE(327),
+    [sym_unmy_hdr_directive] = STATE(327),
+    [sym_open_hook_directive] = STATE(327),
+    [sym_close_hook_directive] = STATE(327),
+    [sym_append_hook_directive] = STATE(327),
+    [sym_push_directive] = STATE(327),
+    [sym_reply_hook_directive] = STATE(327),
+    [sym_send_hook_directive] = STATE(327),
+    [sym_send2_hook_directive] = STATE(327),
+    [sym_spam_directive] = STATE(327),
+    [sym_nospam_directive] = STATE(327),
+    [sym_subjectrx_directive] = STATE(327),
+    [sym_unsubjectrx_directive] = STATE(327),
+    [sym_subscribe_to_directive] = STATE(327),
+    [sym_unsubscribe_from_directive] = STATE(327),
+    [sym_timeout_hook_directive] = STATE(327),
+    [sym_startup_hook_directive] = STATE(327),
+    [sym_shutdown_hook_directive] = STATE(327),
+    [sym_unhook_directive] = STATE(327),
+    [sym_set_directive] = STATE(327),
+    [sym_unset_directive] = STATE(327),
+    [sym_reset_directive] = STATE(327),
+    [sym_toggle_directive] = STATE(327),
+    [sym_setenv_directive] = STATE(327),
+    [sym_unsetenv_directive] = STATE(327),
+    [sym_sidebar_pin_directive] = STATE(327),
+    [sym_sidebar_unpin_directive] = STATE(327),
+    [sym_score_directive] = STATE(327),
+    [sym_unscore_directive] = STATE(327),
+    [sym_source_directive] = STATE(327),
     [anon_sym_account_DASHhook] = ACTIONS(436),
     [anon_sym_alias] = ACTIONS(438),
     [anon_sym_unalias] = ACTIONS(440),
     [anon_sym_alternates] = ACTIONS(442),
     [anon_sym_unalternates] = ACTIONS(444),
     [anon_sym_alternative_order] = ACTIONS(446),
     [anon_sym_unalternative_order] = ACTIONS(448),
@@ -11749,97 +11725,97 @@
     [anon_sym_sidebar_pin] = ACTIONS(582),
     [anon_sym_sidebar_unpin] = ACTIONS(584),
     [anon_sym_score] = ACTIONS(586),
     [anon_sym_unscore] = ACTIONS(588),
     [anon_sym_source] = ACTIONS(590),
   },
   [5] = {
-    [sym__command] = STATE(340),
-    [sym_account_hook_directive] = STATE(340),
-    [sym_alias_directive] = STATE(340),
-    [sym_unalias_directive] = STATE(340),
-    [sym_alternates_directive] = STATE(340),
-    [sym_unalternates_directive] = STATE(340),
-    [sym_alternative_order_directive] = STATE(340),
-    [sym_unalternative_order_directive] = STATE(340),
-    [sym_attachments_directive] = STATE(340),
-    [sym_unattachments_directive] = STATE(340),
-    [sym_auto_view_directive] = STATE(340),
-    [sym_unauto_view_directive] = STATE(340),
-    [sym_bind_directive] = STATE(340),
-    [sym_unbind_directive] = STATE(340),
-    [sym_charset_hook_directive] = STATE(340),
-    [sym_iconv_hook_directive] = STATE(340),
-    [sym_color_directive] = STATE(340),
-    [sym_uncolor_directive] = STATE(340),
-    [sym_crypt_hook_directive] = STATE(340),
-    [sym_index_format_hook_directive] = STATE(340),
-    [sym_exec_directive] = STATE(340),
-    [sym_fcc_save_hook_directive] = STATE(340),
-    [sym_fcc_hook_directive] = STATE(340),
-    [sym_save_hook_directive] = STATE(340),
-    [sym_folder_hook_directive] = STATE(340),
-    [sym_group_directive] = STATE(340),
-    [sym_ungroup_directive] = STATE(340),
-    [sym_hdr_order_directive] = STATE(340),
-    [sym_unhdr_order_directive] = STATE(340),
-    [sym_ifdef_directive] = STATE(340),
-    [sym_ifndef_directive] = STATE(340),
-    [sym_finish_directive] = STATE(340),
-    [sym_ignore_directive] = STATE(340),
-    [sym_unignore_directive] = STATE(340),
-    [sym_lists_directive] = STATE(340),
-    [sym_unlists_directive] = STATE(340),
-    [sym_subscribe_directive] = STATE(340),
-    [sym_unsubscribe_directive] = STATE(340),
-    [sym_macro_directive] = STATE(340),
-    [sym_unmacro_directive] = STATE(340),
-    [sym_mailboxes_directive] = STATE(340),
-    [sym_named_mailboxes_directive] = STATE(340),
-    [sym_unmailboxes_directive] = STATE(340),
-    [sym_mailto_allow_directive] = STATE(340),
-    [sym_unmailto_allow_directive] = STATE(340),
-    [sym_echo_directive] = STATE(340),
-    [sym_cd_directive] = STATE(340),
-    [sym_mbox_hook_directive] = STATE(340),
-    [sym_message_hook_directive] = STATE(340),
-    [sym_mime_lookup_directive] = STATE(340),
-    [sym_unmime_lookup_directive] = STATE(340),
-    [sym_mono_directive] = STATE(340),
-    [sym_unmono_directive] = STATE(340),
-    [sym_my_hdr_directive] = STATE(340),
-    [sym_unmy_hdr_directive] = STATE(340),
-    [sym_open_hook_directive] = STATE(340),
-    [sym_close_hook_directive] = STATE(340),
-    [sym_append_hook_directive] = STATE(340),
-    [sym_push_directive] = STATE(340),
-    [sym_reply_hook_directive] = STATE(340),
-    [sym_send_hook_directive] = STATE(340),
-    [sym_send2_hook_directive] = STATE(340),
-    [sym_spam_directive] = STATE(340),
-    [sym_nospam_directive] = STATE(340),
-    [sym_subjectrx_directive] = STATE(340),
-    [sym_unsubjectrx_directive] = STATE(340),
-    [sym_subscribe_to_directive] = STATE(340),
-    [sym_unsubscribe_from_directive] = STATE(340),
-    [sym_timeout_hook_directive] = STATE(340),
-    [sym_startup_hook_directive] = STATE(340),
-    [sym_shutdown_hook_directive] = STATE(340),
-    [sym_unhook_directive] = STATE(340),
-    [sym_set_directive] = STATE(340),
-    [sym_unset_directive] = STATE(340),
-    [sym_reset_directive] = STATE(340),
-    [sym_toggle_directive] = STATE(340),
-    [sym_setenv_directive] = STATE(340),
-    [sym_unsetenv_directive] = STATE(340),
-    [sym_sidebar_pin_directive] = STATE(340),
-    [sym_sidebar_unpin_directive] = STATE(340),
-    [sym_score_directive] = STATE(340),
-    [sym_unscore_directive] = STATE(340),
-    [sym_source_directive] = STATE(340),
+    [sym__command] = STATE(326),
+    [sym_account_hook_directive] = STATE(326),
+    [sym_alias_directive] = STATE(326),
+    [sym_unalias_directive] = STATE(326),
+    [sym_alternates_directive] = STATE(326),
+    [sym_unalternates_directive] = STATE(326),
+    [sym_alternative_order_directive] = STATE(326),
+    [sym_unalternative_order_directive] = STATE(326),
+    [sym_attachments_directive] = STATE(326),
+    [sym_unattachments_directive] = STATE(326),
+    [sym_auto_view_directive] = STATE(326),
+    [sym_unauto_view_directive] = STATE(326),
+    [sym_bind_directive] = STATE(326),
+    [sym_unbind_directive] = STATE(326),
+    [sym_charset_hook_directive] = STATE(326),
+    [sym_iconv_hook_directive] = STATE(326),
+    [sym_color_directive] = STATE(326),
+    [sym_uncolor_directive] = STATE(326),
+    [sym_crypt_hook_directive] = STATE(326),
+    [sym_index_format_hook_directive] = STATE(326),
+    [sym_exec_directive] = STATE(326),
+    [sym_fcc_save_hook_directive] = STATE(326),
+    [sym_fcc_hook_directive] = STATE(326),
+    [sym_save_hook_directive] = STATE(326),
+    [sym_folder_hook_directive] = STATE(326),
+    [sym_group_directive] = STATE(326),
+    [sym_ungroup_directive] = STATE(326),
+    [sym_hdr_order_directive] = STATE(326),
+    [sym_unhdr_order_directive] = STATE(326),
+    [sym_ifdef_directive] = STATE(326),
+    [sym_ifndef_directive] = STATE(326),
+    [sym_finish_directive] = STATE(326),
+    [sym_ignore_directive] = STATE(326),
+    [sym_unignore_directive] = STATE(326),
+    [sym_lists_directive] = STATE(326),
+    [sym_unlists_directive] = STATE(326),
+    [sym_subscribe_directive] = STATE(326),
+    [sym_unsubscribe_directive] = STATE(326),
+    [sym_macro_directive] = STATE(326),
+    [sym_unmacro_directive] = STATE(326),
+    [sym_mailboxes_directive] = STATE(326),
+    [sym_named_mailboxes_directive] = STATE(326),
+    [sym_unmailboxes_directive] = STATE(326),
+    [sym_mailto_allow_directive] = STATE(326),
+    [sym_unmailto_allow_directive] = STATE(326),
+    [sym_echo_directive] = STATE(326),
+    [sym_cd_directive] = STATE(326),
+    [sym_mbox_hook_directive] = STATE(326),
+    [sym_message_hook_directive] = STATE(326),
+    [sym_mime_lookup_directive] = STATE(326),
+    [sym_unmime_lookup_directive] = STATE(326),
+    [sym_mono_directive] = STATE(326),
+    [sym_unmono_directive] = STATE(326),
+    [sym_my_hdr_directive] = STATE(326),
+    [sym_unmy_hdr_directive] = STATE(326),
+    [sym_open_hook_directive] = STATE(326),
+    [sym_close_hook_directive] = STATE(326),
+    [sym_append_hook_directive] = STATE(326),
+    [sym_push_directive] = STATE(326),
+    [sym_reply_hook_directive] = STATE(326),
+    [sym_send_hook_directive] = STATE(326),
+    [sym_send2_hook_directive] = STATE(326),
+    [sym_spam_directive] = STATE(326),
+    [sym_nospam_directive] = STATE(326),
+    [sym_subjectrx_directive] = STATE(326),
+    [sym_unsubjectrx_directive] = STATE(326),
+    [sym_subscribe_to_directive] = STATE(326),
+    [sym_unsubscribe_from_directive] = STATE(326),
+    [sym_timeout_hook_directive] = STATE(326),
+    [sym_startup_hook_directive] = STATE(326),
+    [sym_shutdown_hook_directive] = STATE(326),
+    [sym_unhook_directive] = STATE(326),
+    [sym_set_directive] = STATE(326),
+    [sym_unset_directive] = STATE(326),
+    [sym_reset_directive] = STATE(326),
+    [sym_toggle_directive] = STATE(326),
+    [sym_setenv_directive] = STATE(326),
+    [sym_unsetenv_directive] = STATE(326),
+    [sym_sidebar_pin_directive] = STATE(326),
+    [sym_sidebar_unpin_directive] = STATE(326),
+    [sym_score_directive] = STATE(326),
+    [sym_unscore_directive] = STATE(326),
+    [sym_source_directive] = STATE(326),
     [anon_sym_account_DASHhook] = ACTIONS(436),
     [anon_sym_alias] = ACTIONS(438),
     [anon_sym_unalias] = ACTIONS(440),
     [anon_sym_alternates] = ACTIONS(442),
     [anon_sym_unalternates] = ACTIONS(444),
     [anon_sym_alternative_order] = ACTIONS(446),
     [anon_sym_unalternative_order] = ACTIONS(448),
@@ -11916,97 +11892,97 @@
     [anon_sym_sidebar_pin] = ACTIONS(582),
     [anon_sym_sidebar_unpin] = ACTIONS(584),
     [anon_sym_score] = ACTIONS(586),
     [anon_sym_unscore] = ACTIONS(588),
     [anon_sym_source] = ACTIONS(590),
   },
   [6] = {
-    [sym__command] = STATE(339),
-    [sym_account_hook_directive] = STATE(339),
-    [sym_alias_directive] = STATE(339),
-    [sym_unalias_directive] = STATE(339),
-    [sym_alternates_directive] = STATE(339),
-    [sym_unalternates_directive] = STATE(339),
-    [sym_alternative_order_directive] = STATE(339),
-    [sym_unalternative_order_directive] = STATE(339),
-    [sym_attachments_directive] = STATE(339),
-    [sym_unattachments_directive] = STATE(339),
-    [sym_auto_view_directive] = STATE(339),
-    [sym_unauto_view_directive] = STATE(339),
-    [sym_bind_directive] = STATE(339),
-    [sym_unbind_directive] = STATE(339),
-    [sym_charset_hook_directive] = STATE(339),
-    [sym_iconv_hook_directive] = STATE(339),
-    [sym_color_directive] = STATE(339),
-    [sym_uncolor_directive] = STATE(339),
-    [sym_crypt_hook_directive] = STATE(339),
-    [sym_index_format_hook_directive] = STATE(339),
-    [sym_exec_directive] = STATE(339),
-    [sym_fcc_save_hook_directive] = STATE(339),
-    [sym_fcc_hook_directive] = STATE(339),
-    [sym_save_hook_directive] = STATE(339),
-    [sym_folder_hook_directive] = STATE(339),
-    [sym_group_directive] = STATE(339),
-    [sym_ungroup_directive] = STATE(339),
-    [sym_hdr_order_directive] = STATE(339),
-    [sym_unhdr_order_directive] = STATE(339),
-    [sym_ifdef_directive] = STATE(339),
-    [sym_ifndef_directive] = STATE(339),
-    [sym_finish_directive] = STATE(339),
-    [sym_ignore_directive] = STATE(339),
-    [sym_unignore_directive] = STATE(339),
-    [sym_lists_directive] = STATE(339),
-    [sym_unlists_directive] = STATE(339),
-    [sym_subscribe_directive] = STATE(339),
-    [sym_unsubscribe_directive] = STATE(339),
-    [sym_macro_directive] = STATE(339),
-    [sym_unmacro_directive] = STATE(339),
-    [sym_mailboxes_directive] = STATE(339),
-    [sym_named_mailboxes_directive] = STATE(339),
-    [sym_unmailboxes_directive] = STATE(339),
-    [sym_mailto_allow_directive] = STATE(339),
-    [sym_unmailto_allow_directive] = STATE(339),
-    [sym_echo_directive] = STATE(339),
-    [sym_cd_directive] = STATE(339),
-    [sym_mbox_hook_directive] = STATE(339),
-    [sym_message_hook_directive] = STATE(339),
-    [sym_mime_lookup_directive] = STATE(339),
-    [sym_unmime_lookup_directive] = STATE(339),
-    [sym_mono_directive] = STATE(339),
-    [sym_unmono_directive] = STATE(339),
-    [sym_my_hdr_directive] = STATE(339),
-    [sym_unmy_hdr_directive] = STATE(339),
-    [sym_open_hook_directive] = STATE(339),
-    [sym_close_hook_directive] = STATE(339),
-    [sym_append_hook_directive] = STATE(339),
-    [sym_push_directive] = STATE(339),
-    [sym_reply_hook_directive] = STATE(339),
-    [sym_send_hook_directive] = STATE(339),
-    [sym_send2_hook_directive] = STATE(339),
-    [sym_spam_directive] = STATE(339),
-    [sym_nospam_directive] = STATE(339),
-    [sym_subjectrx_directive] = STATE(339),
-    [sym_unsubjectrx_directive] = STATE(339),
-    [sym_subscribe_to_directive] = STATE(339),
-    [sym_unsubscribe_from_directive] = STATE(339),
-    [sym_timeout_hook_directive] = STATE(339),
-    [sym_startup_hook_directive] = STATE(339),
-    [sym_shutdown_hook_directive] = STATE(339),
-    [sym_unhook_directive] = STATE(339),
-    [sym_set_directive] = STATE(339),
-    [sym_unset_directive] = STATE(339),
-    [sym_reset_directive] = STATE(339),
-    [sym_toggle_directive] = STATE(339),
-    [sym_setenv_directive] = STATE(339),
-    [sym_unsetenv_directive] = STATE(339),
-    [sym_sidebar_pin_directive] = STATE(339),
-    [sym_sidebar_unpin_directive] = STATE(339),
-    [sym_score_directive] = STATE(339),
-    [sym_unscore_directive] = STATE(339),
-    [sym_source_directive] = STATE(339),
+    [sym__command] = STATE(325),
+    [sym_account_hook_directive] = STATE(325),
+    [sym_alias_directive] = STATE(325),
+    [sym_unalias_directive] = STATE(325),
+    [sym_alternates_directive] = STATE(325),
+    [sym_unalternates_directive] = STATE(325),
+    [sym_alternative_order_directive] = STATE(325),
+    [sym_unalternative_order_directive] = STATE(325),
+    [sym_attachments_directive] = STATE(325),
+    [sym_unattachments_directive] = STATE(325),
+    [sym_auto_view_directive] = STATE(325),
+    [sym_unauto_view_directive] = STATE(325),
+    [sym_bind_directive] = STATE(325),
+    [sym_unbind_directive] = STATE(325),
+    [sym_charset_hook_directive] = STATE(325),
+    [sym_iconv_hook_directive] = STATE(325),
+    [sym_color_directive] = STATE(325),
+    [sym_uncolor_directive] = STATE(325),
+    [sym_crypt_hook_directive] = STATE(325),
+    [sym_index_format_hook_directive] = STATE(325),
+    [sym_exec_directive] = STATE(325),
+    [sym_fcc_save_hook_directive] = STATE(325),
+    [sym_fcc_hook_directive] = STATE(325),
+    [sym_save_hook_directive] = STATE(325),
+    [sym_folder_hook_directive] = STATE(325),
+    [sym_group_directive] = STATE(325),
+    [sym_ungroup_directive] = STATE(325),
+    [sym_hdr_order_directive] = STATE(325),
+    [sym_unhdr_order_directive] = STATE(325),
+    [sym_ifdef_directive] = STATE(325),
+    [sym_ifndef_directive] = STATE(325),
+    [sym_finish_directive] = STATE(325),
+    [sym_ignore_directive] = STATE(325),
+    [sym_unignore_directive] = STATE(325),
+    [sym_lists_directive] = STATE(325),
+    [sym_unlists_directive] = STATE(325),
+    [sym_subscribe_directive] = STATE(325),
+    [sym_unsubscribe_directive] = STATE(325),
+    [sym_macro_directive] = STATE(325),
+    [sym_unmacro_directive] = STATE(325),
+    [sym_mailboxes_directive] = STATE(325),
+    [sym_named_mailboxes_directive] = STATE(325),
+    [sym_unmailboxes_directive] = STATE(325),
+    [sym_mailto_allow_directive] = STATE(325),
+    [sym_unmailto_allow_directive] = STATE(325),
+    [sym_echo_directive] = STATE(325),
+    [sym_cd_directive] = STATE(325),
+    [sym_mbox_hook_directive] = STATE(325),
+    [sym_message_hook_directive] = STATE(325),
+    [sym_mime_lookup_directive] = STATE(325),
+    [sym_unmime_lookup_directive] = STATE(325),
+    [sym_mono_directive] = STATE(325),
+    [sym_unmono_directive] = STATE(325),
+    [sym_my_hdr_directive] = STATE(325),
+    [sym_unmy_hdr_directive] = STATE(325),
+    [sym_open_hook_directive] = STATE(325),
+    [sym_close_hook_directive] = STATE(325),
+    [sym_append_hook_directive] = STATE(325),
+    [sym_push_directive] = STATE(325),
+    [sym_reply_hook_directive] = STATE(325),
+    [sym_send_hook_directive] = STATE(325),
+    [sym_send2_hook_directive] = STATE(325),
+    [sym_spam_directive] = STATE(325),
+    [sym_nospam_directive] = STATE(325),
+    [sym_subjectrx_directive] = STATE(325),
+    [sym_unsubjectrx_directive] = STATE(325),
+    [sym_subscribe_to_directive] = STATE(325),
+    [sym_unsubscribe_from_directive] = STATE(325),
+    [sym_timeout_hook_directive] = STATE(325),
+    [sym_startup_hook_directive] = STATE(325),
+    [sym_shutdown_hook_directive] = STATE(325),
+    [sym_unhook_directive] = STATE(325),
+    [sym_set_directive] = STATE(325),
+    [sym_unset_directive] = STATE(325),
+    [sym_reset_directive] = STATE(325),
+    [sym_toggle_directive] = STATE(325),
+    [sym_setenv_directive] = STATE(325),
+    [sym_unsetenv_directive] = STATE(325),
+    [sym_sidebar_pin_directive] = STATE(325),
+    [sym_sidebar_unpin_directive] = STATE(325),
+    [sym_score_directive] = STATE(325),
+    [sym_unscore_directive] = STATE(325),
+    [sym_source_directive] = STATE(325),
     [anon_sym_account_DASHhook] = ACTIONS(436),
     [anon_sym_alias] = ACTIONS(438),
     [anon_sym_unalias] = ACTIONS(440),
     [anon_sym_alternates] = ACTIONS(442),
     [anon_sym_unalternates] = ACTIONS(444),
     [anon_sym_alternative_order] = ACTIONS(446),
     [anon_sym_unalternative_order] = ACTIONS(448),
@@ -12083,97 +12059,97 @@
     [anon_sym_sidebar_pin] = ACTIONS(582),
     [anon_sym_sidebar_unpin] = ACTIONS(584),
     [anon_sym_score] = ACTIONS(586),
     [anon_sym_unscore] = ACTIONS(588),
     [anon_sym_source] = ACTIONS(590),
   },
   [7] = {
-    [sym__command] = STATE(312),
-    [sym_account_hook_directive] = STATE(312),
-    [sym_alias_directive] = STATE(312),
-    [sym_unalias_directive] = STATE(312),
-    [sym_alternates_directive] = STATE(312),
-    [sym_unalternates_directive] = STATE(312),
-    [sym_alternative_order_directive] = STATE(312),
-    [sym_unalternative_order_directive] = STATE(312),
-    [sym_attachments_directive] = STATE(312),
-    [sym_unattachments_directive] = STATE(312),
-    [sym_auto_view_directive] = STATE(312),
-    [sym_unauto_view_directive] = STATE(312),
-    [sym_bind_directive] = STATE(312),
-    [sym_unbind_directive] = STATE(312),
-    [sym_charset_hook_directive] = STATE(312),
-    [sym_iconv_hook_directive] = STATE(312),
-    [sym_color_directive] = STATE(312),
-    [sym_uncolor_directive] = STATE(312),
-    [sym_crypt_hook_directive] = STATE(312),
-    [sym_index_format_hook_directive] = STATE(312),
-    [sym_exec_directive] = STATE(312),
-    [sym_fcc_save_hook_directive] = STATE(312),
-    [sym_fcc_hook_directive] = STATE(312),
-    [sym_save_hook_directive] = STATE(312),
-    [sym_folder_hook_directive] = STATE(312),
-    [sym_group_directive] = STATE(312),
-    [sym_ungroup_directive] = STATE(312),
-    [sym_hdr_order_directive] = STATE(312),
-    [sym_unhdr_order_directive] = STATE(312),
-    [sym_ifdef_directive] = STATE(312),
-    [sym_ifndef_directive] = STATE(312),
-    [sym_finish_directive] = STATE(312),
-    [sym_ignore_directive] = STATE(312),
-    [sym_unignore_directive] = STATE(312),
-    [sym_lists_directive] = STATE(312),
-    [sym_unlists_directive] = STATE(312),
-    [sym_subscribe_directive] = STATE(312),
-    [sym_unsubscribe_directive] = STATE(312),
-    [sym_macro_directive] = STATE(312),
-    [sym_unmacro_directive] = STATE(312),
-    [sym_mailboxes_directive] = STATE(312),
-    [sym_named_mailboxes_directive] = STATE(312),
-    [sym_unmailboxes_directive] = STATE(312),
-    [sym_mailto_allow_directive] = STATE(312),
-    [sym_unmailto_allow_directive] = STATE(312),
-    [sym_echo_directive] = STATE(312),
-    [sym_cd_directive] = STATE(312),
-    [sym_mbox_hook_directive] = STATE(312),
-    [sym_message_hook_directive] = STATE(312),
-    [sym_mime_lookup_directive] = STATE(312),
-    [sym_unmime_lookup_directive] = STATE(312),
-    [sym_mono_directive] = STATE(312),
-    [sym_unmono_directive] = STATE(312),
-    [sym_my_hdr_directive] = STATE(312),
-    [sym_unmy_hdr_directive] = STATE(312),
-    [sym_open_hook_directive] = STATE(312),
-    [sym_close_hook_directive] = STATE(312),
-    [sym_append_hook_directive] = STATE(312),
-    [sym_push_directive] = STATE(312),
-    [sym_reply_hook_directive] = STATE(312),
-    [sym_send_hook_directive] = STATE(312),
-    [sym_send2_hook_directive] = STATE(312),
-    [sym_spam_directive] = STATE(312),
-    [sym_nospam_directive] = STATE(312),
-    [sym_subjectrx_directive] = STATE(312),
-    [sym_unsubjectrx_directive] = STATE(312),
-    [sym_subscribe_to_directive] = STATE(312),
-    [sym_unsubscribe_from_directive] = STATE(312),
-    [sym_timeout_hook_directive] = STATE(312),
-    [sym_startup_hook_directive] = STATE(312),
-    [sym_shutdown_hook_directive] = STATE(312),
-    [sym_unhook_directive] = STATE(312),
-    [sym_set_directive] = STATE(312),
-    [sym_unset_directive] = STATE(312),
-    [sym_reset_directive] = STATE(312),
-    [sym_toggle_directive] = STATE(312),
-    [sym_setenv_directive] = STATE(312),
-    [sym_unsetenv_directive] = STATE(312),
-    [sym_sidebar_pin_directive] = STATE(312),
-    [sym_sidebar_unpin_directive] = STATE(312),
-    [sym_score_directive] = STATE(312),
-    [sym_unscore_directive] = STATE(312),
-    [sym_source_directive] = STATE(312),
+    [sym__command] = STATE(318),
+    [sym_account_hook_directive] = STATE(318),
+    [sym_alias_directive] = STATE(318),
+    [sym_unalias_directive] = STATE(318),
+    [sym_alternates_directive] = STATE(318),
+    [sym_unalternates_directive] = STATE(318),
+    [sym_alternative_order_directive] = STATE(318),
+    [sym_unalternative_order_directive] = STATE(318),
+    [sym_attachments_directive] = STATE(318),
+    [sym_unattachments_directive] = STATE(318),
+    [sym_auto_view_directive] = STATE(318),
+    [sym_unauto_view_directive] = STATE(318),
+    [sym_bind_directive] = STATE(318),
+    [sym_unbind_directive] = STATE(318),
+    [sym_charset_hook_directive] = STATE(318),
+    [sym_iconv_hook_directive] = STATE(318),
+    [sym_color_directive] = STATE(318),
+    [sym_uncolor_directive] = STATE(318),
+    [sym_crypt_hook_directive] = STATE(318),
+    [sym_index_format_hook_directive] = STATE(318),
+    [sym_exec_directive] = STATE(318),
+    [sym_fcc_save_hook_directive] = STATE(318),
+    [sym_fcc_hook_directive] = STATE(318),
+    [sym_save_hook_directive] = STATE(318),
+    [sym_folder_hook_directive] = STATE(318),
+    [sym_group_directive] = STATE(318),
+    [sym_ungroup_directive] = STATE(318),
+    [sym_hdr_order_directive] = STATE(318),
+    [sym_unhdr_order_directive] = STATE(318),
+    [sym_ifdef_directive] = STATE(318),
+    [sym_ifndef_directive] = STATE(318),
+    [sym_finish_directive] = STATE(318),
+    [sym_ignore_directive] = STATE(318),
+    [sym_unignore_directive] = STATE(318),
+    [sym_lists_directive] = STATE(318),
+    [sym_unlists_directive] = STATE(318),
+    [sym_subscribe_directive] = STATE(318),
+    [sym_unsubscribe_directive] = STATE(318),
+    [sym_macro_directive] = STATE(318),
+    [sym_unmacro_directive] = STATE(318),
+    [sym_mailboxes_directive] = STATE(318),
+    [sym_named_mailboxes_directive] = STATE(318),
+    [sym_unmailboxes_directive] = STATE(318),
+    [sym_mailto_allow_directive] = STATE(318),
+    [sym_unmailto_allow_directive] = STATE(318),
+    [sym_echo_directive] = STATE(318),
+    [sym_cd_directive] = STATE(318),
+    [sym_mbox_hook_directive] = STATE(318),
+    [sym_message_hook_directive] = STATE(318),
+    [sym_mime_lookup_directive] = STATE(318),
+    [sym_unmime_lookup_directive] = STATE(318),
+    [sym_mono_directive] = STATE(318),
+    [sym_unmono_directive] = STATE(318),
+    [sym_my_hdr_directive] = STATE(318),
+    [sym_unmy_hdr_directive] = STATE(318),
+    [sym_open_hook_directive] = STATE(318),
+    [sym_close_hook_directive] = STATE(318),
+    [sym_append_hook_directive] = STATE(318),
+    [sym_push_directive] = STATE(318),
+    [sym_reply_hook_directive] = STATE(318),
+    [sym_send_hook_directive] = STATE(318),
+    [sym_send2_hook_directive] = STATE(318),
+    [sym_spam_directive] = STATE(318),
+    [sym_nospam_directive] = STATE(318),
+    [sym_subjectrx_directive] = STATE(318),
+    [sym_unsubjectrx_directive] = STATE(318),
+    [sym_subscribe_to_directive] = STATE(318),
+    [sym_unsubscribe_from_directive] = STATE(318),
+    [sym_timeout_hook_directive] = STATE(318),
+    [sym_startup_hook_directive] = STATE(318),
+    [sym_shutdown_hook_directive] = STATE(318),
+    [sym_unhook_directive] = STATE(318),
+    [sym_set_directive] = STATE(318),
+    [sym_unset_directive] = STATE(318),
+    [sym_reset_directive] = STATE(318),
+    [sym_toggle_directive] = STATE(318),
+    [sym_setenv_directive] = STATE(318),
+    [sym_unsetenv_directive] = STATE(318),
+    [sym_sidebar_pin_directive] = STATE(318),
+    [sym_sidebar_unpin_directive] = STATE(318),
+    [sym_score_directive] = STATE(318),
+    [sym_unscore_directive] = STATE(318),
+    [sym_source_directive] = STATE(318),
     [anon_sym_account_DASHhook] = ACTIONS(436),
     [anon_sym_alias] = ACTIONS(438),
     [anon_sym_unalias] = ACTIONS(440),
     [anon_sym_alternates] = ACTIONS(442),
     [anon_sym_unalternates] = ACTIONS(444),
     [anon_sym_alternative_order] = ACTIONS(446),
     [anon_sym_unalternative_order] = ACTIONS(448),
@@ -12250,97 +12226,97 @@
     [anon_sym_sidebar_pin] = ACTIONS(582),
     [anon_sym_sidebar_unpin] = ACTIONS(584),
     [anon_sym_score] = ACTIONS(586),
     [anon_sym_unscore] = ACTIONS(588),
     [anon_sym_source] = ACTIONS(590),
   },
   [8] = {
-    [sym__command] = STATE(359),
-    [sym_account_hook_directive] = STATE(359),
-    [sym_alias_directive] = STATE(359),
-    [sym_unalias_directive] = STATE(359),
-    [sym_alternates_directive] = STATE(359),
-    [sym_unalternates_directive] = STATE(359),
-    [sym_alternative_order_directive] = STATE(359),
-    [sym_unalternative_order_directive] = STATE(359),
-    [sym_attachments_directive] = STATE(359),
-    [sym_unattachments_directive] = STATE(359),
-    [sym_auto_view_directive] = STATE(359),
-    [sym_unauto_view_directive] = STATE(359),
-    [sym_bind_directive] = STATE(359),
-    [sym_unbind_directive] = STATE(359),
-    [sym_charset_hook_directive] = STATE(359),
-    [sym_iconv_hook_directive] = STATE(359),
-    [sym_color_directive] = STATE(359),
-    [sym_uncolor_directive] = STATE(359),
-    [sym_crypt_hook_directive] = STATE(359),
-    [sym_index_format_hook_directive] = STATE(359),
-    [sym_exec_directive] = STATE(359),
-    [sym_fcc_save_hook_directive] = STATE(359),
-    [sym_fcc_hook_directive] = STATE(359),
-    [sym_save_hook_directive] = STATE(359),
-    [sym_folder_hook_directive] = STATE(359),
-    [sym_group_directive] = STATE(359),
-    [sym_ungroup_directive] = STATE(359),
-    [sym_hdr_order_directive] = STATE(359),
-    [sym_unhdr_order_directive] = STATE(359),
-    [sym_ifdef_directive] = STATE(359),
-    [sym_ifndef_directive] = STATE(359),
-    [sym_finish_directive] = STATE(359),
-    [sym_ignore_directive] = STATE(359),
-    [sym_unignore_directive] = STATE(359),
-    [sym_lists_directive] = STATE(359),
-    [sym_unlists_directive] = STATE(359),
-    [sym_subscribe_directive] = STATE(359),
-    [sym_unsubscribe_directive] = STATE(359),
-    [sym_macro_directive] = STATE(359),
-    [sym_unmacro_directive] = STATE(359),
-    [sym_mailboxes_directive] = STATE(359),
-    [sym_named_mailboxes_directive] = STATE(359),
-    [sym_unmailboxes_directive] = STATE(359),
-    [sym_mailto_allow_directive] = STATE(359),
-    [sym_unmailto_allow_directive] = STATE(359),
-    [sym_echo_directive] = STATE(359),
-    [sym_cd_directive] = STATE(359),
-    [sym_mbox_hook_directive] = STATE(359),
-    [sym_message_hook_directive] = STATE(359),
-    [sym_mime_lookup_directive] = STATE(359),
-    [sym_unmime_lookup_directive] = STATE(359),
-    [sym_mono_directive] = STATE(359),
-    [sym_unmono_directive] = STATE(359),
-    [sym_my_hdr_directive] = STATE(359),
-    [sym_unmy_hdr_directive] = STATE(359),
-    [sym_open_hook_directive] = STATE(359),
-    [sym_close_hook_directive] = STATE(359),
-    [sym_append_hook_directive] = STATE(359),
-    [sym_push_directive] = STATE(359),
-    [sym_reply_hook_directive] = STATE(359),
-    [sym_send_hook_directive] = STATE(359),
-    [sym_send2_hook_directive] = STATE(359),
-    [sym_spam_directive] = STATE(359),
-    [sym_nospam_directive] = STATE(359),
-    [sym_subjectrx_directive] = STATE(359),
-    [sym_unsubjectrx_directive] = STATE(359),
-    [sym_subscribe_to_directive] = STATE(359),
-    [sym_unsubscribe_from_directive] = STATE(359),
-    [sym_timeout_hook_directive] = STATE(359),
-    [sym_startup_hook_directive] = STATE(359),
-    [sym_shutdown_hook_directive] = STATE(359),
-    [sym_unhook_directive] = STATE(359),
-    [sym_set_directive] = STATE(359),
-    [sym_unset_directive] = STATE(359),
-    [sym_reset_directive] = STATE(359),
-    [sym_toggle_directive] = STATE(359),
-    [sym_setenv_directive] = STATE(359),
-    [sym_unsetenv_directive] = STATE(359),
-    [sym_sidebar_pin_directive] = STATE(359),
-    [sym_sidebar_unpin_directive] = STATE(359),
-    [sym_score_directive] = STATE(359),
-    [sym_unscore_directive] = STATE(359),
-    [sym_source_directive] = STATE(359),
+    [sym__command] = STATE(319),
+    [sym_account_hook_directive] = STATE(319),
+    [sym_alias_directive] = STATE(319),
+    [sym_unalias_directive] = STATE(319),
+    [sym_alternates_directive] = STATE(319),
+    [sym_unalternates_directive] = STATE(319),
+    [sym_alternative_order_directive] = STATE(319),
+    [sym_unalternative_order_directive] = STATE(319),
+    [sym_attachments_directive] = STATE(319),
+    [sym_unattachments_directive] = STATE(319),
+    [sym_auto_view_directive] = STATE(319),
+    [sym_unauto_view_directive] = STATE(319),
+    [sym_bind_directive] = STATE(319),
+    [sym_unbind_directive] = STATE(319),
+    [sym_charset_hook_directive] = STATE(319),
+    [sym_iconv_hook_directive] = STATE(319),
+    [sym_color_directive] = STATE(319),
+    [sym_uncolor_directive] = STATE(319),
+    [sym_crypt_hook_directive] = STATE(319),
+    [sym_index_format_hook_directive] = STATE(319),
+    [sym_exec_directive] = STATE(319),
+    [sym_fcc_save_hook_directive] = STATE(319),
+    [sym_fcc_hook_directive] = STATE(319),
+    [sym_save_hook_directive] = STATE(319),
+    [sym_folder_hook_directive] = STATE(319),
+    [sym_group_directive] = STATE(319),
+    [sym_ungroup_directive] = STATE(319),
+    [sym_hdr_order_directive] = STATE(319),
+    [sym_unhdr_order_directive] = STATE(319),
+    [sym_ifdef_directive] = STATE(319),
+    [sym_ifndef_directive] = STATE(319),
+    [sym_finish_directive] = STATE(319),
+    [sym_ignore_directive] = STATE(319),
+    [sym_unignore_directive] = STATE(319),
+    [sym_lists_directive] = STATE(319),
+    [sym_unlists_directive] = STATE(319),
+    [sym_subscribe_directive] = STATE(319),
+    [sym_unsubscribe_directive] = STATE(319),
+    [sym_macro_directive] = STATE(319),
+    [sym_unmacro_directive] = STATE(319),
+    [sym_mailboxes_directive] = STATE(319),
+    [sym_named_mailboxes_directive] = STATE(319),
+    [sym_unmailboxes_directive] = STATE(319),
+    [sym_mailto_allow_directive] = STATE(319),
+    [sym_unmailto_allow_directive] = STATE(319),
+    [sym_echo_directive] = STATE(319),
+    [sym_cd_directive] = STATE(319),
+    [sym_mbox_hook_directive] = STATE(319),
+    [sym_message_hook_directive] = STATE(319),
+    [sym_mime_lookup_directive] = STATE(319),
+    [sym_unmime_lookup_directive] = STATE(319),
+    [sym_mono_directive] = STATE(319),
+    [sym_unmono_directive] = STATE(319),
+    [sym_my_hdr_directive] = STATE(319),
+    [sym_unmy_hdr_directive] = STATE(319),
+    [sym_open_hook_directive] = STATE(319),
+    [sym_close_hook_directive] = STATE(319),
+    [sym_append_hook_directive] = STATE(319),
+    [sym_push_directive] = STATE(319),
+    [sym_reply_hook_directive] = STATE(319),
+    [sym_send_hook_directive] = STATE(319),
+    [sym_send2_hook_directive] = STATE(319),
+    [sym_spam_directive] = STATE(319),
+    [sym_nospam_directive] = STATE(319),
+    [sym_subjectrx_directive] = STATE(319),
+    [sym_unsubjectrx_directive] = STATE(319),
+    [sym_subscribe_to_directive] = STATE(319),
+    [sym_unsubscribe_from_directive] = STATE(319),
+    [sym_timeout_hook_directive] = STATE(319),
+    [sym_startup_hook_directive] = STATE(319),
+    [sym_shutdown_hook_directive] = STATE(319),
+    [sym_unhook_directive] = STATE(319),
+    [sym_set_directive] = STATE(319),
+    [sym_unset_directive] = STATE(319),
+    [sym_reset_directive] = STATE(319),
+    [sym_toggle_directive] = STATE(319),
+    [sym_setenv_directive] = STATE(319),
+    [sym_unsetenv_directive] = STATE(319),
+    [sym_sidebar_pin_directive] = STATE(319),
+    [sym_sidebar_unpin_directive] = STATE(319),
+    [sym_score_directive] = STATE(319),
+    [sym_unscore_directive] = STATE(319),
+    [sym_source_directive] = STATE(319),
     [anon_sym_account_DASHhook] = ACTIONS(436),
     [anon_sym_alias] = ACTIONS(438),
     [anon_sym_unalias] = ACTIONS(440),
     [anon_sym_alternates] = ACTIONS(442),
     [anon_sym_unalternates] = ACTIONS(444),
     [anon_sym_alternative_order] = ACTIONS(446),
     [anon_sym_unalternative_order] = ACTIONS(448),
@@ -12417,97 +12393,97 @@
     [anon_sym_sidebar_pin] = ACTIONS(582),
     [anon_sym_sidebar_unpin] = ACTIONS(584),
     [anon_sym_score] = ACTIONS(586),
     [anon_sym_unscore] = ACTIONS(588),
     [anon_sym_source] = ACTIONS(590),
   },
   [9] = {
-    [sym__command] = STATE(338),
-    [sym_account_hook_directive] = STATE(338),
-    [sym_alias_directive] = STATE(338),
-    [sym_unalias_directive] = STATE(338),
-    [sym_alternates_directive] = STATE(338),
-    [sym_unalternates_directive] = STATE(338),
-    [sym_alternative_order_directive] = STATE(338),
-    [sym_unalternative_order_directive] = STATE(338),
-    [sym_attachments_directive] = STATE(338),
-    [sym_unattachments_directive] = STATE(338),
-    [sym_auto_view_directive] = STATE(338),
-    [sym_unauto_view_directive] = STATE(338),
-    [sym_bind_directive] = STATE(338),
-    [sym_unbind_directive] = STATE(338),
-    [sym_charset_hook_directive] = STATE(338),
-    [sym_iconv_hook_directive] = STATE(338),
-    [sym_color_directive] = STATE(338),
-    [sym_uncolor_directive] = STATE(338),
-    [sym_crypt_hook_directive] = STATE(338),
-    [sym_index_format_hook_directive] = STATE(338),
-    [sym_exec_directive] = STATE(338),
-    [sym_fcc_save_hook_directive] = STATE(338),
-    [sym_fcc_hook_directive] = STATE(338),
-    [sym_save_hook_directive] = STATE(338),
-    [sym_folder_hook_directive] = STATE(338),
-    [sym_group_directive] = STATE(338),
-    [sym_ungroup_directive] = STATE(338),
-    [sym_hdr_order_directive] = STATE(338),
-    [sym_unhdr_order_directive] = STATE(338),
-    [sym_ifdef_directive] = STATE(338),
-    [sym_ifndef_directive] = STATE(338),
-    [sym_finish_directive] = STATE(338),
-    [sym_ignore_directive] = STATE(338),
-    [sym_unignore_directive] = STATE(338),
-    [sym_lists_directive] = STATE(338),
-    [sym_unlists_directive] = STATE(338),
-    [sym_subscribe_directive] = STATE(338),
-    [sym_unsubscribe_directive] = STATE(338),
-    [sym_macro_directive] = STATE(338),
-    [sym_unmacro_directive] = STATE(338),
-    [sym_mailboxes_directive] = STATE(338),
-    [sym_named_mailboxes_directive] = STATE(338),
-    [sym_unmailboxes_directive] = STATE(338),
-    [sym_mailto_allow_directive] = STATE(338),
-    [sym_unmailto_allow_directive] = STATE(338),
-    [sym_echo_directive] = STATE(338),
-    [sym_cd_directive] = STATE(338),
-    [sym_mbox_hook_directive] = STATE(338),
-    [sym_message_hook_directive] = STATE(338),
-    [sym_mime_lookup_directive] = STATE(338),
-    [sym_unmime_lookup_directive] = STATE(338),
-    [sym_mono_directive] = STATE(338),
-    [sym_unmono_directive] = STATE(338),
-    [sym_my_hdr_directive] = STATE(338),
-    [sym_unmy_hdr_directive] = STATE(338),
-    [sym_open_hook_directive] = STATE(338),
-    [sym_close_hook_directive] = STATE(338),
-    [sym_append_hook_directive] = STATE(338),
-    [sym_push_directive] = STATE(338),
-    [sym_reply_hook_directive] = STATE(338),
-    [sym_send_hook_directive] = STATE(338),
-    [sym_send2_hook_directive] = STATE(338),
-    [sym_spam_directive] = STATE(338),
-    [sym_nospam_directive] = STATE(338),
-    [sym_subjectrx_directive] = STATE(338),
-    [sym_unsubjectrx_directive] = STATE(338),
-    [sym_subscribe_to_directive] = STATE(338),
-    [sym_unsubscribe_from_directive] = STATE(338),
-    [sym_timeout_hook_directive] = STATE(338),
-    [sym_startup_hook_directive] = STATE(338),
-    [sym_shutdown_hook_directive] = STATE(338),
-    [sym_unhook_directive] = STATE(338),
-    [sym_set_directive] = STATE(338),
-    [sym_unset_directive] = STATE(338),
-    [sym_reset_directive] = STATE(338),
-    [sym_toggle_directive] = STATE(338),
-    [sym_setenv_directive] = STATE(338),
-    [sym_unsetenv_directive] = STATE(338),
-    [sym_sidebar_pin_directive] = STATE(338),
-    [sym_sidebar_unpin_directive] = STATE(338),
-    [sym_score_directive] = STATE(338),
-    [sym_unscore_directive] = STATE(338),
-    [sym_source_directive] = STATE(338),
+    [sym__command] = STATE(315),
+    [sym_account_hook_directive] = STATE(315),
+    [sym_alias_directive] = STATE(315),
+    [sym_unalias_directive] = STATE(315),
+    [sym_alternates_directive] = STATE(315),
+    [sym_unalternates_directive] = STATE(315),
+    [sym_alternative_order_directive] = STATE(315),
+    [sym_unalternative_order_directive] = STATE(315),
+    [sym_attachments_directive] = STATE(315),
+    [sym_unattachments_directive] = STATE(315),
+    [sym_auto_view_directive] = STATE(315),
+    [sym_unauto_view_directive] = STATE(315),
+    [sym_bind_directive] = STATE(315),
+    [sym_unbind_directive] = STATE(315),
+    [sym_charset_hook_directive] = STATE(315),
+    [sym_iconv_hook_directive] = STATE(315),
+    [sym_color_directive] = STATE(315),
+    [sym_uncolor_directive] = STATE(315),
+    [sym_crypt_hook_directive] = STATE(315),
+    [sym_index_format_hook_directive] = STATE(315),
+    [sym_exec_directive] = STATE(315),
+    [sym_fcc_save_hook_directive] = STATE(315),
+    [sym_fcc_hook_directive] = STATE(315),
+    [sym_save_hook_directive] = STATE(315),
+    [sym_folder_hook_directive] = STATE(315),
+    [sym_group_directive] = STATE(315),
+    [sym_ungroup_directive] = STATE(315),
+    [sym_hdr_order_directive] = STATE(315),
+    [sym_unhdr_order_directive] = STATE(315),
+    [sym_ifdef_directive] = STATE(315),
+    [sym_ifndef_directive] = STATE(315),
+    [sym_finish_directive] = STATE(315),
+    [sym_ignore_directive] = STATE(315),
+    [sym_unignore_directive] = STATE(315),
+    [sym_lists_directive] = STATE(315),
+    [sym_unlists_directive] = STATE(315),
+    [sym_subscribe_directive] = STATE(315),
+    [sym_unsubscribe_directive] = STATE(315),
+    [sym_macro_directive] = STATE(315),
+    [sym_unmacro_directive] = STATE(315),
+    [sym_mailboxes_directive] = STATE(315),
+    [sym_named_mailboxes_directive] = STATE(315),
+    [sym_unmailboxes_directive] = STATE(315),
+    [sym_mailto_allow_directive] = STATE(315),
+    [sym_unmailto_allow_directive] = STATE(315),
+    [sym_echo_directive] = STATE(315),
+    [sym_cd_directive] = STATE(315),
+    [sym_mbox_hook_directive] = STATE(315),
+    [sym_message_hook_directive] = STATE(315),
+    [sym_mime_lookup_directive] = STATE(315),
+    [sym_unmime_lookup_directive] = STATE(315),
+    [sym_mono_directive] = STATE(315),
+    [sym_unmono_directive] = STATE(315),
+    [sym_my_hdr_directive] = STATE(315),
+    [sym_unmy_hdr_directive] = STATE(315),
+    [sym_open_hook_directive] = STATE(315),
+    [sym_close_hook_directive] = STATE(315),
+    [sym_append_hook_directive] = STATE(315),
+    [sym_push_directive] = STATE(315),
+    [sym_reply_hook_directive] = STATE(315),
+    [sym_send_hook_directive] = STATE(315),
+    [sym_send2_hook_directive] = STATE(315),
+    [sym_spam_directive] = STATE(315),
+    [sym_nospam_directive] = STATE(315),
+    [sym_subjectrx_directive] = STATE(315),
+    [sym_unsubjectrx_directive] = STATE(315),
+    [sym_subscribe_to_directive] = STATE(315),
+    [sym_unsubscribe_from_directive] = STATE(315),
+    [sym_timeout_hook_directive] = STATE(315),
+    [sym_startup_hook_directive] = STATE(315),
+    [sym_shutdown_hook_directive] = STATE(315),
+    [sym_unhook_directive] = STATE(315),
+    [sym_set_directive] = STATE(315),
+    [sym_unset_directive] = STATE(315),
+    [sym_reset_directive] = STATE(315),
+    [sym_toggle_directive] = STATE(315),
+    [sym_setenv_directive] = STATE(315),
+    [sym_unsetenv_directive] = STATE(315),
+    [sym_sidebar_pin_directive] = STATE(315),
+    [sym_sidebar_unpin_directive] = STATE(315),
+    [sym_score_directive] = STATE(315),
+    [sym_unscore_directive] = STATE(315),
+    [sym_source_directive] = STATE(315),
     [anon_sym_account_DASHhook] = ACTIONS(436),
     [anon_sym_alias] = ACTIONS(438),
     [anon_sym_unalias] = ACTIONS(440),
     [anon_sym_alternates] = ACTIONS(442),
     [anon_sym_unalternates] = ACTIONS(444),
     [anon_sym_alternative_order] = ACTIONS(446),
     [anon_sym_unalternative_order] = ACTIONS(448),
@@ -12584,97 +12560,97 @@
     [anon_sym_sidebar_pin] = ACTIONS(582),
     [anon_sym_sidebar_unpin] = ACTIONS(584),
     [anon_sym_score] = ACTIONS(586),
     [anon_sym_unscore] = ACTIONS(588),
     [anon_sym_source] = ACTIONS(590),
   },
   [10] = {
-    [sym__command] = STATE(375),
-    [sym_account_hook_directive] = STATE(375),
-    [sym_alias_directive] = STATE(375),
-    [sym_unalias_directive] = STATE(375),
-    [sym_alternates_directive] = STATE(375),
-    [sym_unalternates_directive] = STATE(375),
-    [sym_alternative_order_directive] = STATE(375),
-    [sym_unalternative_order_directive] = STATE(375),
-    [sym_attachments_directive] = STATE(375),
-    [sym_unattachments_directive] = STATE(375),
-    [sym_auto_view_directive] = STATE(375),
-    [sym_unauto_view_directive] = STATE(375),
-    [sym_bind_directive] = STATE(375),
-    [sym_unbind_directive] = STATE(375),
-    [sym_charset_hook_directive] = STATE(375),
-    [sym_iconv_hook_directive] = STATE(375),
-    [sym_color_directive] = STATE(375),
-    [sym_uncolor_directive] = STATE(375),
-    [sym_crypt_hook_directive] = STATE(375),
-    [sym_index_format_hook_directive] = STATE(375),
-    [sym_exec_directive] = STATE(375),
-    [sym_fcc_save_hook_directive] = STATE(375),
-    [sym_fcc_hook_directive] = STATE(375),
-    [sym_save_hook_directive] = STATE(375),
-    [sym_folder_hook_directive] = STATE(375),
-    [sym_group_directive] = STATE(375),
-    [sym_ungroup_directive] = STATE(375),
-    [sym_hdr_order_directive] = STATE(375),
-    [sym_unhdr_order_directive] = STATE(375),
-    [sym_ifdef_directive] = STATE(375),
-    [sym_ifndef_directive] = STATE(375),
-    [sym_finish_directive] = STATE(375),
-    [sym_ignore_directive] = STATE(375),
-    [sym_unignore_directive] = STATE(375),
-    [sym_lists_directive] = STATE(375),
-    [sym_unlists_directive] = STATE(375),
-    [sym_subscribe_directive] = STATE(375),
-    [sym_unsubscribe_directive] = STATE(375),
-    [sym_macro_directive] = STATE(375),
-    [sym_unmacro_directive] = STATE(375),
-    [sym_mailboxes_directive] = STATE(375),
-    [sym_named_mailboxes_directive] = STATE(375),
-    [sym_unmailboxes_directive] = STATE(375),
-    [sym_mailto_allow_directive] = STATE(375),
-    [sym_unmailto_allow_directive] = STATE(375),
-    [sym_echo_directive] = STATE(375),
-    [sym_cd_directive] = STATE(375),
-    [sym_mbox_hook_directive] = STATE(375),
-    [sym_message_hook_directive] = STATE(375),
-    [sym_mime_lookup_directive] = STATE(375),
-    [sym_unmime_lookup_directive] = STATE(375),
-    [sym_mono_directive] = STATE(375),
-    [sym_unmono_directive] = STATE(375),
-    [sym_my_hdr_directive] = STATE(375),
-    [sym_unmy_hdr_directive] = STATE(375),
-    [sym_open_hook_directive] = STATE(375),
-    [sym_close_hook_directive] = STATE(375),
-    [sym_append_hook_directive] = STATE(375),
-    [sym_push_directive] = STATE(375),
-    [sym_reply_hook_directive] = STATE(375),
-    [sym_send_hook_directive] = STATE(375),
-    [sym_send2_hook_directive] = STATE(375),
-    [sym_spam_directive] = STATE(375),
-    [sym_nospam_directive] = STATE(375),
-    [sym_subjectrx_directive] = STATE(375),
-    [sym_unsubjectrx_directive] = STATE(375),
-    [sym_subscribe_to_directive] = STATE(375),
-    [sym_unsubscribe_from_directive] = STATE(375),
-    [sym_timeout_hook_directive] = STATE(375),
-    [sym_startup_hook_directive] = STATE(375),
-    [sym_shutdown_hook_directive] = STATE(375),
-    [sym_unhook_directive] = STATE(375),
-    [sym_set_directive] = STATE(375),
-    [sym_unset_directive] = STATE(375),
-    [sym_reset_directive] = STATE(375),
-    [sym_toggle_directive] = STATE(375),
-    [sym_setenv_directive] = STATE(375),
-    [sym_unsetenv_directive] = STATE(375),
-    [sym_sidebar_pin_directive] = STATE(375),
-    [sym_sidebar_unpin_directive] = STATE(375),
-    [sym_score_directive] = STATE(375),
-    [sym_unscore_directive] = STATE(375),
-    [sym_source_directive] = STATE(375),
+    [sym__command] = STATE(352),
+    [sym_account_hook_directive] = STATE(352),
+    [sym_alias_directive] = STATE(352),
+    [sym_unalias_directive] = STATE(352),
+    [sym_alternates_directive] = STATE(352),
+    [sym_unalternates_directive] = STATE(352),
+    [sym_alternative_order_directive] = STATE(352),
+    [sym_unalternative_order_directive] = STATE(352),
+    [sym_attachments_directive] = STATE(352),
+    [sym_unattachments_directive] = STATE(352),
+    [sym_auto_view_directive] = STATE(352),
+    [sym_unauto_view_directive] = STATE(352),
+    [sym_bind_directive] = STATE(352),
+    [sym_unbind_directive] = STATE(352),
+    [sym_charset_hook_directive] = STATE(352),
+    [sym_iconv_hook_directive] = STATE(352),
+    [sym_color_directive] = STATE(352),
+    [sym_uncolor_directive] = STATE(352),
+    [sym_crypt_hook_directive] = STATE(352),
+    [sym_index_format_hook_directive] = STATE(352),
+    [sym_exec_directive] = STATE(352),
+    [sym_fcc_save_hook_directive] = STATE(352),
+    [sym_fcc_hook_directive] = STATE(352),
+    [sym_save_hook_directive] = STATE(352),
+    [sym_folder_hook_directive] = STATE(352),
+    [sym_group_directive] = STATE(352),
+    [sym_ungroup_directive] = STATE(352),
+    [sym_hdr_order_directive] = STATE(352),
+    [sym_unhdr_order_directive] = STATE(352),
+    [sym_ifdef_directive] = STATE(352),
+    [sym_ifndef_directive] = STATE(352),
+    [sym_finish_directive] = STATE(352),
+    [sym_ignore_directive] = STATE(352),
+    [sym_unignore_directive] = STATE(352),
+    [sym_lists_directive] = STATE(352),
+    [sym_unlists_directive] = STATE(352),
+    [sym_subscribe_directive] = STATE(352),
+    [sym_unsubscribe_directive] = STATE(352),
+    [sym_macro_directive] = STATE(352),
+    [sym_unmacro_directive] = STATE(352),
+    [sym_mailboxes_directive] = STATE(352),
+    [sym_named_mailboxes_directive] = STATE(352),
+    [sym_unmailboxes_directive] = STATE(352),
+    [sym_mailto_allow_directive] = STATE(352),
+    [sym_unmailto_allow_directive] = STATE(352),
+    [sym_echo_directive] = STATE(352),
+    [sym_cd_directive] = STATE(352),
+    [sym_mbox_hook_directive] = STATE(352),
+    [sym_message_hook_directive] = STATE(352),
+    [sym_mime_lookup_directive] = STATE(352),
+    [sym_unmime_lookup_directive] = STATE(352),
+    [sym_mono_directive] = STATE(352),
+    [sym_unmono_directive] = STATE(352),
+    [sym_my_hdr_directive] = STATE(352),
+    [sym_unmy_hdr_directive] = STATE(352),
+    [sym_open_hook_directive] = STATE(352),
+    [sym_close_hook_directive] = STATE(352),
+    [sym_append_hook_directive] = STATE(352),
+    [sym_push_directive] = STATE(352),
+    [sym_reply_hook_directive] = STATE(352),
+    [sym_send_hook_directive] = STATE(352),
+    [sym_send2_hook_directive] = STATE(352),
+    [sym_spam_directive] = STATE(352),
+    [sym_nospam_directive] = STATE(352),
+    [sym_subjectrx_directive] = STATE(352),
+    [sym_unsubjectrx_directive] = STATE(352),
+    [sym_subscribe_to_directive] = STATE(352),
+    [sym_unsubscribe_from_directive] = STATE(352),
+    [sym_timeout_hook_directive] = STATE(352),
+    [sym_startup_hook_directive] = STATE(352),
+    [sym_shutdown_hook_directive] = STATE(352),
+    [sym_unhook_directive] = STATE(352),
+    [sym_set_directive] = STATE(352),
+    [sym_unset_directive] = STATE(352),
+    [sym_reset_directive] = STATE(352),
+    [sym_toggle_directive] = STATE(352),
+    [sym_setenv_directive] = STATE(352),
+    [sym_unsetenv_directive] = STATE(352),
+    [sym_sidebar_pin_directive] = STATE(352),
+    [sym_sidebar_unpin_directive] = STATE(352),
+    [sym_score_directive] = STATE(352),
+    [sym_unscore_directive] = STATE(352),
+    [sym_source_directive] = STATE(352),
     [anon_sym_account_DASHhook] = ACTIONS(436),
     [anon_sym_alias] = ACTIONS(438),
     [anon_sym_unalias] = ACTIONS(440),
     [anon_sym_alternates] = ACTIONS(442),
     [anon_sym_unalternates] = ACTIONS(444),
     [anon_sym_alternative_order] = ACTIONS(446),
     [anon_sym_unalternative_order] = ACTIONS(448),
@@ -12751,97 +12727,97 @@
     [anon_sym_sidebar_pin] = ACTIONS(582),
     [anon_sym_sidebar_unpin] = ACTIONS(584),
     [anon_sym_score] = ACTIONS(586),
     [anon_sym_unscore] = ACTIONS(588),
     [anon_sym_source] = ACTIONS(590),
   },
   [11] = {
-    [sym__command] = STATE(410),
-    [sym_account_hook_directive] = STATE(410),
-    [sym_alias_directive] = STATE(410),
-    [sym_unalias_directive] = STATE(410),
-    [sym_alternates_directive] = STATE(410),
-    [sym_unalternates_directive] = STATE(410),
-    [sym_alternative_order_directive] = STATE(410),
-    [sym_unalternative_order_directive] = STATE(410),
-    [sym_attachments_directive] = STATE(410),
-    [sym_unattachments_directive] = STATE(410),
-    [sym_auto_view_directive] = STATE(410),
-    [sym_unauto_view_directive] = STATE(410),
-    [sym_bind_directive] = STATE(410),
-    [sym_unbind_directive] = STATE(410),
-    [sym_charset_hook_directive] = STATE(410),
-    [sym_iconv_hook_directive] = STATE(410),
-    [sym_color_directive] = STATE(410),
-    [sym_uncolor_directive] = STATE(410),
-    [sym_crypt_hook_directive] = STATE(410),
-    [sym_index_format_hook_directive] = STATE(410),
-    [sym_exec_directive] = STATE(410),
-    [sym_fcc_save_hook_directive] = STATE(410),
-    [sym_fcc_hook_directive] = STATE(410),
-    [sym_save_hook_directive] = STATE(410),
-    [sym_folder_hook_directive] = STATE(410),
-    [sym_group_directive] = STATE(410),
-    [sym_ungroup_directive] = STATE(410),
-    [sym_hdr_order_directive] = STATE(410),
-    [sym_unhdr_order_directive] = STATE(410),
-    [sym_ifdef_directive] = STATE(410),
-    [sym_ifndef_directive] = STATE(410),
-    [sym_finish_directive] = STATE(410),
-    [sym_ignore_directive] = STATE(410),
-    [sym_unignore_directive] = STATE(410),
-    [sym_lists_directive] = STATE(410),
-    [sym_unlists_directive] = STATE(410),
-    [sym_subscribe_directive] = STATE(410),
-    [sym_unsubscribe_directive] = STATE(410),
-    [sym_macro_directive] = STATE(410),
-    [sym_unmacro_directive] = STATE(410),
-    [sym_mailboxes_directive] = STATE(410),
-    [sym_named_mailboxes_directive] = STATE(410),
-    [sym_unmailboxes_directive] = STATE(410),
-    [sym_mailto_allow_directive] = STATE(410),
-    [sym_unmailto_allow_directive] = STATE(410),
-    [sym_echo_directive] = STATE(410),
-    [sym_cd_directive] = STATE(410),
-    [sym_mbox_hook_directive] = STATE(410),
-    [sym_message_hook_directive] = STATE(410),
-    [sym_mime_lookup_directive] = STATE(410),
-    [sym_unmime_lookup_directive] = STATE(410),
-    [sym_mono_directive] = STATE(410),
-    [sym_unmono_directive] = STATE(410),
-    [sym_my_hdr_directive] = STATE(410),
-    [sym_unmy_hdr_directive] = STATE(410),
-    [sym_open_hook_directive] = STATE(410),
-    [sym_close_hook_directive] = STATE(410),
-    [sym_append_hook_directive] = STATE(410),
-    [sym_push_directive] = STATE(410),
-    [sym_reply_hook_directive] = STATE(410),
-    [sym_send_hook_directive] = STATE(410),
-    [sym_send2_hook_directive] = STATE(410),
-    [sym_spam_directive] = STATE(410),
-    [sym_nospam_directive] = STATE(410),
-    [sym_subjectrx_directive] = STATE(410),
-    [sym_unsubjectrx_directive] = STATE(410),
-    [sym_subscribe_to_directive] = STATE(410),
-    [sym_unsubscribe_from_directive] = STATE(410),
-    [sym_timeout_hook_directive] = STATE(410),
-    [sym_startup_hook_directive] = STATE(410),
-    [sym_shutdown_hook_directive] = STATE(410),
-    [sym_unhook_directive] = STATE(410),
-    [sym_set_directive] = STATE(410),
-    [sym_unset_directive] = STATE(410),
-    [sym_reset_directive] = STATE(410),
-    [sym_toggle_directive] = STATE(410),
-    [sym_setenv_directive] = STATE(410),
-    [sym_unsetenv_directive] = STATE(410),
-    [sym_sidebar_pin_directive] = STATE(410),
-    [sym_sidebar_unpin_directive] = STATE(410),
-    [sym_score_directive] = STATE(410),
-    [sym_unscore_directive] = STATE(410),
-    [sym_source_directive] = STATE(410),
+    [sym__command] = STATE(441),
+    [sym_account_hook_directive] = STATE(441),
+    [sym_alias_directive] = STATE(441),
+    [sym_unalias_directive] = STATE(441),
+    [sym_alternates_directive] = STATE(441),
+    [sym_unalternates_directive] = STATE(441),
+    [sym_alternative_order_directive] = STATE(441),
+    [sym_unalternative_order_directive] = STATE(441),
+    [sym_attachments_directive] = STATE(441),
+    [sym_unattachments_directive] = STATE(441),
+    [sym_auto_view_directive] = STATE(441),
+    [sym_unauto_view_directive] = STATE(441),
+    [sym_bind_directive] = STATE(441),
+    [sym_unbind_directive] = STATE(441),
+    [sym_charset_hook_directive] = STATE(441),
+    [sym_iconv_hook_directive] = STATE(441),
+    [sym_color_directive] = STATE(441),
+    [sym_uncolor_directive] = STATE(441),
+    [sym_crypt_hook_directive] = STATE(441),
+    [sym_index_format_hook_directive] = STATE(441),
+    [sym_exec_directive] = STATE(441),
+    [sym_fcc_save_hook_directive] = STATE(441),
+    [sym_fcc_hook_directive] = STATE(441),
+    [sym_save_hook_directive] = STATE(441),
+    [sym_folder_hook_directive] = STATE(441),
+    [sym_group_directive] = STATE(441),
+    [sym_ungroup_directive] = STATE(441),
+    [sym_hdr_order_directive] = STATE(441),
+    [sym_unhdr_order_directive] = STATE(441),
+    [sym_ifdef_directive] = STATE(441),
+    [sym_ifndef_directive] = STATE(441),
+    [sym_finish_directive] = STATE(441),
+    [sym_ignore_directive] = STATE(441),
+    [sym_unignore_directive] = STATE(441),
+    [sym_lists_directive] = STATE(441),
+    [sym_unlists_directive] = STATE(441),
+    [sym_subscribe_directive] = STATE(441),
+    [sym_unsubscribe_directive] = STATE(441),
+    [sym_macro_directive] = STATE(441),
+    [sym_unmacro_directive] = STATE(441),
+    [sym_mailboxes_directive] = STATE(441),
+    [sym_named_mailboxes_directive] = STATE(441),
+    [sym_unmailboxes_directive] = STATE(441),
+    [sym_mailto_allow_directive] = STATE(441),
+    [sym_unmailto_allow_directive] = STATE(441),
+    [sym_echo_directive] = STATE(441),
+    [sym_cd_directive] = STATE(441),
+    [sym_mbox_hook_directive] = STATE(441),
+    [sym_message_hook_directive] = STATE(441),
+    [sym_mime_lookup_directive] = STATE(441),
+    [sym_unmime_lookup_directive] = STATE(441),
+    [sym_mono_directive] = STATE(441),
+    [sym_unmono_directive] = STATE(441),
+    [sym_my_hdr_directive] = STATE(441),
+    [sym_unmy_hdr_directive] = STATE(441),
+    [sym_open_hook_directive] = STATE(441),
+    [sym_close_hook_directive] = STATE(441),
+    [sym_append_hook_directive] = STATE(441),
+    [sym_push_directive] = STATE(441),
+    [sym_reply_hook_directive] = STATE(441),
+    [sym_send_hook_directive] = STATE(441),
+    [sym_send2_hook_directive] = STATE(441),
+    [sym_spam_directive] = STATE(441),
+    [sym_nospam_directive] = STATE(441),
+    [sym_subjectrx_directive] = STATE(441),
+    [sym_unsubjectrx_directive] = STATE(441),
+    [sym_subscribe_to_directive] = STATE(441),
+    [sym_unsubscribe_from_directive] = STATE(441),
+    [sym_timeout_hook_directive] = STATE(441),
+    [sym_startup_hook_directive] = STATE(441),
+    [sym_shutdown_hook_directive] = STATE(441),
+    [sym_unhook_directive] = STATE(441),
+    [sym_set_directive] = STATE(441),
+    [sym_unset_directive] = STATE(441),
+    [sym_reset_directive] = STATE(441),
+    [sym_toggle_directive] = STATE(441),
+    [sym_setenv_directive] = STATE(441),
+    [sym_unsetenv_directive] = STATE(441),
+    [sym_sidebar_pin_directive] = STATE(441),
+    [sym_sidebar_unpin_directive] = STATE(441),
+    [sym_score_directive] = STATE(441),
+    [sym_unscore_directive] = STATE(441),
+    [sym_source_directive] = STATE(441),
     [anon_sym_account_DASHhook] = ACTIONS(436),
     [anon_sym_alias] = ACTIONS(438),
     [anon_sym_unalias] = ACTIONS(440),
     [anon_sym_alternates] = ACTIONS(442),
     [anon_sym_unalternates] = ACTIONS(444),
     [anon_sym_alternative_order] = ACTIONS(446),
     [anon_sym_unalternative_order] = ACTIONS(448),
@@ -12918,97 +12894,97 @@
     [anon_sym_sidebar_pin] = ACTIONS(582),
     [anon_sym_sidebar_unpin] = ACTIONS(584),
     [anon_sym_score] = ACTIONS(586),
     [anon_sym_unscore] = ACTIONS(588),
     [anon_sym_source] = ACTIONS(590),
   },
   [12] = {
-    [sym__command] = STATE(413),
-    [sym_account_hook_directive] = STATE(413),
-    [sym_alias_directive] = STATE(413),
-    [sym_unalias_directive] = STATE(413),
-    [sym_alternates_directive] = STATE(413),
-    [sym_unalternates_directive] = STATE(413),
-    [sym_alternative_order_directive] = STATE(413),
-    [sym_unalternative_order_directive] = STATE(413),
-    [sym_attachments_directive] = STATE(413),
-    [sym_unattachments_directive] = STATE(413),
-    [sym_auto_view_directive] = STATE(413),
-    [sym_unauto_view_directive] = STATE(413),
-    [sym_bind_directive] = STATE(413),
-    [sym_unbind_directive] = STATE(413),
-    [sym_charset_hook_directive] = STATE(413),
-    [sym_iconv_hook_directive] = STATE(413),
-    [sym_color_directive] = STATE(413),
-    [sym_uncolor_directive] = STATE(413),
-    [sym_crypt_hook_directive] = STATE(413),
-    [sym_index_format_hook_directive] = STATE(413),
-    [sym_exec_directive] = STATE(413),
-    [sym_fcc_save_hook_directive] = STATE(413),
-    [sym_fcc_hook_directive] = STATE(413),
-    [sym_save_hook_directive] = STATE(413),
-    [sym_folder_hook_directive] = STATE(413),
-    [sym_group_directive] = STATE(413),
-    [sym_ungroup_directive] = STATE(413),
-    [sym_hdr_order_directive] = STATE(413),
-    [sym_unhdr_order_directive] = STATE(413),
-    [sym_ifdef_directive] = STATE(413),
-    [sym_ifndef_directive] = STATE(413),
-    [sym_finish_directive] = STATE(413),
-    [sym_ignore_directive] = STATE(413),
-    [sym_unignore_directive] = STATE(413),
-    [sym_lists_directive] = STATE(413),
-    [sym_unlists_directive] = STATE(413),
-    [sym_subscribe_directive] = STATE(413),
-    [sym_unsubscribe_directive] = STATE(413),
-    [sym_macro_directive] = STATE(413),
-    [sym_unmacro_directive] = STATE(413),
-    [sym_mailboxes_directive] = STATE(413),
-    [sym_named_mailboxes_directive] = STATE(413),
-    [sym_unmailboxes_directive] = STATE(413),
-    [sym_mailto_allow_directive] = STATE(413),
-    [sym_unmailto_allow_directive] = STATE(413),
-    [sym_echo_directive] = STATE(413),
-    [sym_cd_directive] = STATE(413),
-    [sym_mbox_hook_directive] = STATE(413),
-    [sym_message_hook_directive] = STATE(413),
-    [sym_mime_lookup_directive] = STATE(413),
-    [sym_unmime_lookup_directive] = STATE(413),
-    [sym_mono_directive] = STATE(413),
-    [sym_unmono_directive] = STATE(413),
-    [sym_my_hdr_directive] = STATE(413),
-    [sym_unmy_hdr_directive] = STATE(413),
-    [sym_open_hook_directive] = STATE(413),
-    [sym_close_hook_directive] = STATE(413),
-    [sym_append_hook_directive] = STATE(413),
-    [sym_push_directive] = STATE(413),
-    [sym_reply_hook_directive] = STATE(413),
-    [sym_send_hook_directive] = STATE(413),
-    [sym_send2_hook_directive] = STATE(413),
-    [sym_spam_directive] = STATE(413),
-    [sym_nospam_directive] = STATE(413),
-    [sym_subjectrx_directive] = STATE(413),
-    [sym_unsubjectrx_directive] = STATE(413),
-    [sym_subscribe_to_directive] = STATE(413),
-    [sym_unsubscribe_from_directive] = STATE(413),
-    [sym_timeout_hook_directive] = STATE(413),
-    [sym_startup_hook_directive] = STATE(413),
-    [sym_shutdown_hook_directive] = STATE(413),
-    [sym_unhook_directive] = STATE(413),
-    [sym_set_directive] = STATE(413),
-    [sym_unset_directive] = STATE(413),
-    [sym_reset_directive] = STATE(413),
-    [sym_toggle_directive] = STATE(413),
-    [sym_setenv_directive] = STATE(413),
-    [sym_unsetenv_directive] = STATE(413),
-    [sym_sidebar_pin_directive] = STATE(413),
-    [sym_sidebar_unpin_directive] = STATE(413),
-    [sym_score_directive] = STATE(413),
-    [sym_unscore_directive] = STATE(413),
-    [sym_source_directive] = STATE(413),
+    [sym__command] = STATE(442),
+    [sym_account_hook_directive] = STATE(442),
+    [sym_alias_directive] = STATE(442),
+    [sym_unalias_directive] = STATE(442),
+    [sym_alternates_directive] = STATE(442),
+    [sym_unalternates_directive] = STATE(442),
+    [sym_alternative_order_directive] = STATE(442),
+    [sym_unalternative_order_directive] = STATE(442),
+    [sym_attachments_directive] = STATE(442),
+    [sym_unattachments_directive] = STATE(442),
+    [sym_auto_view_directive] = STATE(442),
+    [sym_unauto_view_directive] = STATE(442),
+    [sym_bind_directive] = STATE(442),
+    [sym_unbind_directive] = STATE(442),
+    [sym_charset_hook_directive] = STATE(442),
+    [sym_iconv_hook_directive] = STATE(442),
+    [sym_color_directive] = STATE(442),
+    [sym_uncolor_directive] = STATE(442),
+    [sym_crypt_hook_directive] = STATE(442),
+    [sym_index_format_hook_directive] = STATE(442),
+    [sym_exec_directive] = STATE(442),
+    [sym_fcc_save_hook_directive] = STATE(442),
+    [sym_fcc_hook_directive] = STATE(442),
+    [sym_save_hook_directive] = STATE(442),
+    [sym_folder_hook_directive] = STATE(442),
+    [sym_group_directive] = STATE(442),
+    [sym_ungroup_directive] = STATE(442),
+    [sym_hdr_order_directive] = STATE(442),
+    [sym_unhdr_order_directive] = STATE(442),
+    [sym_ifdef_directive] = STATE(442),
+    [sym_ifndef_directive] = STATE(442),
+    [sym_finish_directive] = STATE(442),
+    [sym_ignore_directive] = STATE(442),
+    [sym_unignore_directive] = STATE(442),
+    [sym_lists_directive] = STATE(442),
+    [sym_unlists_directive] = STATE(442),
+    [sym_subscribe_directive] = STATE(442),
+    [sym_unsubscribe_directive] = STATE(442),
+    [sym_macro_directive] = STATE(442),
+    [sym_unmacro_directive] = STATE(442),
+    [sym_mailboxes_directive] = STATE(442),
+    [sym_named_mailboxes_directive] = STATE(442),
+    [sym_unmailboxes_directive] = STATE(442),
+    [sym_mailto_allow_directive] = STATE(442),
+    [sym_unmailto_allow_directive] = STATE(442),
+    [sym_echo_directive] = STATE(442),
+    [sym_cd_directive] = STATE(442),
+    [sym_mbox_hook_directive] = STATE(442),
+    [sym_message_hook_directive] = STATE(442),
+    [sym_mime_lookup_directive] = STATE(442),
+    [sym_unmime_lookup_directive] = STATE(442),
+    [sym_mono_directive] = STATE(442),
+    [sym_unmono_directive] = STATE(442),
+    [sym_my_hdr_directive] = STATE(442),
+    [sym_unmy_hdr_directive] = STATE(442),
+    [sym_open_hook_directive] = STATE(442),
+    [sym_close_hook_directive] = STATE(442),
+    [sym_append_hook_directive] = STATE(442),
+    [sym_push_directive] = STATE(442),
+    [sym_reply_hook_directive] = STATE(442),
+    [sym_send_hook_directive] = STATE(442),
+    [sym_send2_hook_directive] = STATE(442),
+    [sym_spam_directive] = STATE(442),
+    [sym_nospam_directive] = STATE(442),
+    [sym_subjectrx_directive] = STATE(442),
+    [sym_unsubjectrx_directive] = STATE(442),
+    [sym_subscribe_to_directive] = STATE(442),
+    [sym_unsubscribe_from_directive] = STATE(442),
+    [sym_timeout_hook_directive] = STATE(442),
+    [sym_startup_hook_directive] = STATE(442),
+    [sym_shutdown_hook_directive] = STATE(442),
+    [sym_unhook_directive] = STATE(442),
+    [sym_set_directive] = STATE(442),
+    [sym_unset_directive] = STATE(442),
+    [sym_reset_directive] = STATE(442),
+    [sym_toggle_directive] = STATE(442),
+    [sym_setenv_directive] = STATE(442),
+    [sym_unsetenv_directive] = STATE(442),
+    [sym_sidebar_pin_directive] = STATE(442),
+    [sym_sidebar_unpin_directive] = STATE(442),
+    [sym_score_directive] = STATE(442),
+    [sym_unscore_directive] = STATE(442),
+    [sym_source_directive] = STATE(442),
     [anon_sym_account_DASHhook] = ACTIONS(436),
     [anon_sym_alias] = ACTIONS(438),
     [anon_sym_unalias] = ACTIONS(440),
     [anon_sym_alternates] = ACTIONS(442),
     [anon_sym_unalternates] = ACTIONS(444),
     [anon_sym_alternative_order] = ACTIONS(446),
     [anon_sym_unalternative_order] = ACTIONS(448),
@@ -13085,97 +13061,97 @@
     [anon_sym_sidebar_pin] = ACTIONS(582),
     [anon_sym_sidebar_unpin] = ACTIONS(584),
     [anon_sym_score] = ACTIONS(586),
     [anon_sym_unscore] = ACTIONS(588),
     [anon_sym_source] = ACTIONS(590),
   },
   [13] = {
-    [sym__command] = STATE(310),
-    [sym_account_hook_directive] = STATE(310),
-    [sym_alias_directive] = STATE(310),
-    [sym_unalias_directive] = STATE(310),
-    [sym_alternates_directive] = STATE(310),
-    [sym_unalternates_directive] = STATE(310),
-    [sym_alternative_order_directive] = STATE(310),
-    [sym_unalternative_order_directive] = STATE(310),
-    [sym_attachments_directive] = STATE(310),
-    [sym_unattachments_directive] = STATE(310),
-    [sym_auto_view_directive] = STATE(310),
-    [sym_unauto_view_directive] = STATE(310),
-    [sym_bind_directive] = STATE(310),
-    [sym_unbind_directive] = STATE(310),
-    [sym_charset_hook_directive] = STATE(310),
-    [sym_iconv_hook_directive] = STATE(310),
-    [sym_color_directive] = STATE(310),
-    [sym_uncolor_directive] = STATE(310),
-    [sym_crypt_hook_directive] = STATE(310),
-    [sym_index_format_hook_directive] = STATE(310),
-    [sym_exec_directive] = STATE(310),
-    [sym_fcc_save_hook_directive] = STATE(310),
-    [sym_fcc_hook_directive] = STATE(310),
-    [sym_save_hook_directive] = STATE(310),
-    [sym_folder_hook_directive] = STATE(310),
-    [sym_group_directive] = STATE(310),
-    [sym_ungroup_directive] = STATE(310),
-    [sym_hdr_order_directive] = STATE(310),
-    [sym_unhdr_order_directive] = STATE(310),
-    [sym_ifdef_directive] = STATE(310),
-    [sym_ifndef_directive] = STATE(310),
-    [sym_finish_directive] = STATE(310),
-    [sym_ignore_directive] = STATE(310),
-    [sym_unignore_directive] = STATE(310),
-    [sym_lists_directive] = STATE(310),
-    [sym_unlists_directive] = STATE(310),
-    [sym_subscribe_directive] = STATE(310),
-    [sym_unsubscribe_directive] = STATE(310),
-    [sym_macro_directive] = STATE(310),
-    [sym_unmacro_directive] = STATE(310),
-    [sym_mailboxes_directive] = STATE(310),
-    [sym_named_mailboxes_directive] = STATE(310),
-    [sym_unmailboxes_directive] = STATE(310),
-    [sym_mailto_allow_directive] = STATE(310),
-    [sym_unmailto_allow_directive] = STATE(310),
-    [sym_echo_directive] = STATE(310),
-    [sym_cd_directive] = STATE(310),
-    [sym_mbox_hook_directive] = STATE(310),
-    [sym_message_hook_directive] = STATE(310),
-    [sym_mime_lookup_directive] = STATE(310),
-    [sym_unmime_lookup_directive] = STATE(310),
-    [sym_mono_directive] = STATE(310),
-    [sym_unmono_directive] = STATE(310),
-    [sym_my_hdr_directive] = STATE(310),
-    [sym_unmy_hdr_directive] = STATE(310),
-    [sym_open_hook_directive] = STATE(310),
-    [sym_close_hook_directive] = STATE(310),
-    [sym_append_hook_directive] = STATE(310),
-    [sym_push_directive] = STATE(310),
-    [sym_reply_hook_directive] = STATE(310),
-    [sym_send_hook_directive] = STATE(310),
-    [sym_send2_hook_directive] = STATE(310),
-    [sym_spam_directive] = STATE(310),
-    [sym_nospam_directive] = STATE(310),
-    [sym_subjectrx_directive] = STATE(310),
-    [sym_unsubjectrx_directive] = STATE(310),
-    [sym_subscribe_to_directive] = STATE(310),
-    [sym_unsubscribe_from_directive] = STATE(310),
-    [sym_timeout_hook_directive] = STATE(310),
-    [sym_startup_hook_directive] = STATE(310),
-    [sym_shutdown_hook_directive] = STATE(310),
-    [sym_unhook_directive] = STATE(310),
-    [sym_set_directive] = STATE(310),
-    [sym_unset_directive] = STATE(310),
-    [sym_reset_directive] = STATE(310),
-    [sym_toggle_directive] = STATE(310),
-    [sym_setenv_directive] = STATE(310),
-    [sym_unsetenv_directive] = STATE(310),
-    [sym_sidebar_pin_directive] = STATE(310),
-    [sym_sidebar_unpin_directive] = STATE(310),
-    [sym_score_directive] = STATE(310),
-    [sym_unscore_directive] = STATE(310),
-    [sym_source_directive] = STATE(310),
+    [sym__command] = STATE(446),
+    [sym_account_hook_directive] = STATE(446),
+    [sym_alias_directive] = STATE(446),
+    [sym_unalias_directive] = STATE(446),
+    [sym_alternates_directive] = STATE(446),
+    [sym_unalternates_directive] = STATE(446),
+    [sym_alternative_order_directive] = STATE(446),
+    [sym_unalternative_order_directive] = STATE(446),
+    [sym_attachments_directive] = STATE(446),
+    [sym_unattachments_directive] = STATE(446),
+    [sym_auto_view_directive] = STATE(446),
+    [sym_unauto_view_directive] = STATE(446),
+    [sym_bind_directive] = STATE(446),
+    [sym_unbind_directive] = STATE(446),
+    [sym_charset_hook_directive] = STATE(446),
+    [sym_iconv_hook_directive] = STATE(446),
+    [sym_color_directive] = STATE(446),
+    [sym_uncolor_directive] = STATE(446),
+    [sym_crypt_hook_directive] = STATE(446),
+    [sym_index_format_hook_directive] = STATE(446),
+    [sym_exec_directive] = STATE(446),
+    [sym_fcc_save_hook_directive] = STATE(446),
+    [sym_fcc_hook_directive] = STATE(446),
+    [sym_save_hook_directive] = STATE(446),
+    [sym_folder_hook_directive] = STATE(446),
+    [sym_group_directive] = STATE(446),
+    [sym_ungroup_directive] = STATE(446),
+    [sym_hdr_order_directive] = STATE(446),
+    [sym_unhdr_order_directive] = STATE(446),
+    [sym_ifdef_directive] = STATE(446),
+    [sym_ifndef_directive] = STATE(446),
+    [sym_finish_directive] = STATE(446),
+    [sym_ignore_directive] = STATE(446),
+    [sym_unignore_directive] = STATE(446),
+    [sym_lists_directive] = STATE(446),
+    [sym_unlists_directive] = STATE(446),
+    [sym_subscribe_directive] = STATE(446),
+    [sym_unsubscribe_directive] = STATE(446),
+    [sym_macro_directive] = STATE(446),
+    [sym_unmacro_directive] = STATE(446),
+    [sym_mailboxes_directive] = STATE(446),
+    [sym_named_mailboxes_directive] = STATE(446),
+    [sym_unmailboxes_directive] = STATE(446),
+    [sym_mailto_allow_directive] = STATE(446),
+    [sym_unmailto_allow_directive] = STATE(446),
+    [sym_echo_directive] = STATE(446),
+    [sym_cd_directive] = STATE(446),
+    [sym_mbox_hook_directive] = STATE(446),
+    [sym_message_hook_directive] = STATE(446),
+    [sym_mime_lookup_directive] = STATE(446),
+    [sym_unmime_lookup_directive] = STATE(446),
+    [sym_mono_directive] = STATE(446),
+    [sym_unmono_directive] = STATE(446),
+    [sym_my_hdr_directive] = STATE(446),
+    [sym_unmy_hdr_directive] = STATE(446),
+    [sym_open_hook_directive] = STATE(446),
+    [sym_close_hook_directive] = STATE(446),
+    [sym_append_hook_directive] = STATE(446),
+    [sym_push_directive] = STATE(446),
+    [sym_reply_hook_directive] = STATE(446),
+    [sym_send_hook_directive] = STATE(446),
+    [sym_send2_hook_directive] = STATE(446),
+    [sym_spam_directive] = STATE(446),
+    [sym_nospam_directive] = STATE(446),
+    [sym_subjectrx_directive] = STATE(446),
+    [sym_unsubjectrx_directive] = STATE(446),
+    [sym_subscribe_to_directive] = STATE(446),
+    [sym_unsubscribe_from_directive] = STATE(446),
+    [sym_timeout_hook_directive] = STATE(446),
+    [sym_startup_hook_directive] = STATE(446),
+    [sym_shutdown_hook_directive] = STATE(446),
+    [sym_unhook_directive] = STATE(446),
+    [sym_set_directive] = STATE(446),
+    [sym_unset_directive] = STATE(446),
+    [sym_reset_directive] = STATE(446),
+    [sym_toggle_directive] = STATE(446),
+    [sym_setenv_directive] = STATE(446),
+    [sym_unsetenv_directive] = STATE(446),
+    [sym_sidebar_pin_directive] = STATE(446),
+    [sym_sidebar_unpin_directive] = STATE(446),
+    [sym_score_directive] = STATE(446),
+    [sym_unscore_directive] = STATE(446),
+    [sym_source_directive] = STATE(446),
     [anon_sym_account_DASHhook] = ACTIONS(436),
     [anon_sym_alias] = ACTIONS(438),
     [anon_sym_unalias] = ACTIONS(440),
     [anon_sym_alternates] = ACTIONS(442),
     [anon_sym_unalternates] = ACTIONS(444),
     [anon_sym_alternative_order] = ACTIONS(446),
     [anon_sym_unalternative_order] = ACTIONS(448),
@@ -13252,97 +13228,97 @@
     [anon_sym_sidebar_pin] = ACTIONS(582),
     [anon_sym_sidebar_unpin] = ACTIONS(584),
     [anon_sym_score] = ACTIONS(586),
     [anon_sym_unscore] = ACTIONS(588),
     [anon_sym_source] = ACTIONS(590),
   },
   [14] = {
-    [sym__command] = STATE(318),
-    [sym_account_hook_directive] = STATE(318),
-    [sym_alias_directive] = STATE(318),
-    [sym_unalias_directive] = STATE(318),
-    [sym_alternates_directive] = STATE(318),
-    [sym_unalternates_directive] = STATE(318),
-    [sym_alternative_order_directive] = STATE(318),
-    [sym_unalternative_order_directive] = STATE(318),
-    [sym_attachments_directive] = STATE(318),
-    [sym_unattachments_directive] = STATE(318),
-    [sym_auto_view_directive] = STATE(318),
-    [sym_unauto_view_directive] = STATE(318),
-    [sym_bind_directive] = STATE(318),
-    [sym_unbind_directive] = STATE(318),
-    [sym_charset_hook_directive] = STATE(318),
-    [sym_iconv_hook_directive] = STATE(318),
-    [sym_color_directive] = STATE(318),
-    [sym_uncolor_directive] = STATE(318),
-    [sym_crypt_hook_directive] = STATE(318),
-    [sym_index_format_hook_directive] = STATE(318),
-    [sym_exec_directive] = STATE(318),
-    [sym_fcc_save_hook_directive] = STATE(318),
-    [sym_fcc_hook_directive] = STATE(318),
-    [sym_save_hook_directive] = STATE(318),
-    [sym_folder_hook_directive] = STATE(318),
-    [sym_group_directive] = STATE(318),
-    [sym_ungroup_directive] = STATE(318),
-    [sym_hdr_order_directive] = STATE(318),
-    [sym_unhdr_order_directive] = STATE(318),
-    [sym_ifdef_directive] = STATE(318),
-    [sym_ifndef_directive] = STATE(318),
-    [sym_finish_directive] = STATE(318),
-    [sym_ignore_directive] = STATE(318),
-    [sym_unignore_directive] = STATE(318),
-    [sym_lists_directive] = STATE(318),
-    [sym_unlists_directive] = STATE(318),
-    [sym_subscribe_directive] = STATE(318),
-    [sym_unsubscribe_directive] = STATE(318),
-    [sym_macro_directive] = STATE(318),
-    [sym_unmacro_directive] = STATE(318),
-    [sym_mailboxes_directive] = STATE(318),
-    [sym_named_mailboxes_directive] = STATE(318),
-    [sym_unmailboxes_directive] = STATE(318),
-    [sym_mailto_allow_directive] = STATE(318),
-    [sym_unmailto_allow_directive] = STATE(318),
-    [sym_echo_directive] = STATE(318),
-    [sym_cd_directive] = STATE(318),
-    [sym_mbox_hook_directive] = STATE(318),
-    [sym_message_hook_directive] = STATE(318),
-    [sym_mime_lookup_directive] = STATE(318),
-    [sym_unmime_lookup_directive] = STATE(318),
-    [sym_mono_directive] = STATE(318),
-    [sym_unmono_directive] = STATE(318),
-    [sym_my_hdr_directive] = STATE(318),
-    [sym_unmy_hdr_directive] = STATE(318),
-    [sym_open_hook_directive] = STATE(318),
-    [sym_close_hook_directive] = STATE(318),
-    [sym_append_hook_directive] = STATE(318),
-    [sym_push_directive] = STATE(318),
-    [sym_reply_hook_directive] = STATE(318),
-    [sym_send_hook_directive] = STATE(318),
-    [sym_send2_hook_directive] = STATE(318),
-    [sym_spam_directive] = STATE(318),
-    [sym_nospam_directive] = STATE(318),
-    [sym_subjectrx_directive] = STATE(318),
-    [sym_unsubjectrx_directive] = STATE(318),
-    [sym_subscribe_to_directive] = STATE(318),
-    [sym_unsubscribe_from_directive] = STATE(318),
-    [sym_timeout_hook_directive] = STATE(318),
-    [sym_startup_hook_directive] = STATE(318),
-    [sym_shutdown_hook_directive] = STATE(318),
-    [sym_unhook_directive] = STATE(318),
-    [sym_set_directive] = STATE(318),
-    [sym_unset_directive] = STATE(318),
-    [sym_reset_directive] = STATE(318),
-    [sym_toggle_directive] = STATE(318),
-    [sym_setenv_directive] = STATE(318),
-    [sym_unsetenv_directive] = STATE(318),
-    [sym_sidebar_pin_directive] = STATE(318),
-    [sym_sidebar_unpin_directive] = STATE(318),
-    [sym_score_directive] = STATE(318),
-    [sym_unscore_directive] = STATE(318),
-    [sym_source_directive] = STATE(318),
+    [sym__command] = STATE(415),
+    [sym_account_hook_directive] = STATE(415),
+    [sym_alias_directive] = STATE(415),
+    [sym_unalias_directive] = STATE(415),
+    [sym_alternates_directive] = STATE(415),
+    [sym_unalternates_directive] = STATE(415),
+    [sym_alternative_order_directive] = STATE(415),
+    [sym_unalternative_order_directive] = STATE(415),
+    [sym_attachments_directive] = STATE(415),
+    [sym_unattachments_directive] = STATE(415),
+    [sym_auto_view_directive] = STATE(415),
+    [sym_unauto_view_directive] = STATE(415),
+    [sym_bind_directive] = STATE(415),
+    [sym_unbind_directive] = STATE(415),
+    [sym_charset_hook_directive] = STATE(415),
+    [sym_iconv_hook_directive] = STATE(415),
+    [sym_color_directive] = STATE(415),
+    [sym_uncolor_directive] = STATE(415),
+    [sym_crypt_hook_directive] = STATE(415),
+    [sym_index_format_hook_directive] = STATE(415),
+    [sym_exec_directive] = STATE(415),
+    [sym_fcc_save_hook_directive] = STATE(415),
+    [sym_fcc_hook_directive] = STATE(415),
+    [sym_save_hook_directive] = STATE(415),
+    [sym_folder_hook_directive] = STATE(415),
+    [sym_group_directive] = STATE(415),
+    [sym_ungroup_directive] = STATE(415),
+    [sym_hdr_order_directive] = STATE(415),
+    [sym_unhdr_order_directive] = STATE(415),
+    [sym_ifdef_directive] = STATE(415),
+    [sym_ifndef_directive] = STATE(415),
+    [sym_finish_directive] = STATE(415),
+    [sym_ignore_directive] = STATE(415),
+    [sym_unignore_directive] = STATE(415),
+    [sym_lists_directive] = STATE(415),
+    [sym_unlists_directive] = STATE(415),
+    [sym_subscribe_directive] = STATE(415),
+    [sym_unsubscribe_directive] = STATE(415),
+    [sym_macro_directive] = STATE(415),
+    [sym_unmacro_directive] = STATE(415),
+    [sym_mailboxes_directive] = STATE(415),
+    [sym_named_mailboxes_directive] = STATE(415),
+    [sym_unmailboxes_directive] = STATE(415),
+    [sym_mailto_allow_directive] = STATE(415),
+    [sym_unmailto_allow_directive] = STATE(415),
+    [sym_echo_directive] = STATE(415),
+    [sym_cd_directive] = STATE(415),
+    [sym_mbox_hook_directive] = STATE(415),
+    [sym_message_hook_directive] = STATE(415),
+    [sym_mime_lookup_directive] = STATE(415),
+    [sym_unmime_lookup_directive] = STATE(415),
+    [sym_mono_directive] = STATE(415),
+    [sym_unmono_directive] = STATE(415),
+    [sym_my_hdr_directive] = STATE(415),
+    [sym_unmy_hdr_directive] = STATE(415),
+    [sym_open_hook_directive] = STATE(415),
+    [sym_close_hook_directive] = STATE(415),
+    [sym_append_hook_directive] = STATE(415),
+    [sym_push_directive] = STATE(415),
+    [sym_reply_hook_directive] = STATE(415),
+    [sym_send_hook_directive] = STATE(415),
+    [sym_send2_hook_directive] = STATE(415),
+    [sym_spam_directive] = STATE(415),
+    [sym_nospam_directive] = STATE(415),
+    [sym_subjectrx_directive] = STATE(415),
+    [sym_unsubjectrx_directive] = STATE(415),
+    [sym_subscribe_to_directive] = STATE(415),
+    [sym_unsubscribe_from_directive] = STATE(415),
+    [sym_timeout_hook_directive] = STATE(415),
+    [sym_startup_hook_directive] = STATE(415),
+    [sym_shutdown_hook_directive] = STATE(415),
+    [sym_unhook_directive] = STATE(415),
+    [sym_set_directive] = STATE(415),
+    [sym_unset_directive] = STATE(415),
+    [sym_reset_directive] = STATE(415),
+    [sym_toggle_directive] = STATE(415),
+    [sym_setenv_directive] = STATE(415),
+    [sym_unsetenv_directive] = STATE(415),
+    [sym_sidebar_pin_directive] = STATE(415),
+    [sym_sidebar_unpin_directive] = STATE(415),
+    [sym_score_directive] = STATE(415),
+    [sym_unscore_directive] = STATE(415),
+    [sym_source_directive] = STATE(415),
     [anon_sym_account_DASHhook] = ACTIONS(436),
     [anon_sym_alias] = ACTIONS(438),
     [anon_sym_unalias] = ACTIONS(440),
     [anon_sym_alternates] = ACTIONS(442),
     [anon_sym_unalternates] = ACTIONS(444),
     [anon_sym_alternative_order] = ACTIONS(446),
     [anon_sym_unalternative_order] = ACTIONS(448),
@@ -13419,97 +13395,97 @@
     [anon_sym_sidebar_pin] = ACTIONS(582),
     [anon_sym_sidebar_unpin] = ACTIONS(584),
     [anon_sym_score] = ACTIONS(586),
     [anon_sym_unscore] = ACTIONS(588),
     [anon_sym_source] = ACTIONS(590),
   },
   [15] = {
-    [sym__command] = STATE(319),
-    [sym_account_hook_directive] = STATE(319),
-    [sym_alias_directive] = STATE(319),
-    [sym_unalias_directive] = STATE(319),
-    [sym_alternates_directive] = STATE(319),
-    [sym_unalternates_directive] = STATE(319),
-    [sym_alternative_order_directive] = STATE(319),
-    [sym_unalternative_order_directive] = STATE(319),
-    [sym_attachments_directive] = STATE(319),
-    [sym_unattachments_directive] = STATE(319),
-    [sym_auto_view_directive] = STATE(319),
-    [sym_unauto_view_directive] = STATE(319),
-    [sym_bind_directive] = STATE(319),
-    [sym_unbind_directive] = STATE(319),
-    [sym_charset_hook_directive] = STATE(319),
-    [sym_iconv_hook_directive] = STATE(319),
-    [sym_color_directive] = STATE(319),
-    [sym_uncolor_directive] = STATE(319),
-    [sym_crypt_hook_directive] = STATE(319),
-    [sym_index_format_hook_directive] = STATE(319),
-    [sym_exec_directive] = STATE(319),
-    [sym_fcc_save_hook_directive] = STATE(319),
-    [sym_fcc_hook_directive] = STATE(319),
-    [sym_save_hook_directive] = STATE(319),
-    [sym_folder_hook_directive] = STATE(319),
-    [sym_group_directive] = STATE(319),
-    [sym_ungroup_directive] = STATE(319),
-    [sym_hdr_order_directive] = STATE(319),
-    [sym_unhdr_order_directive] = STATE(319),
-    [sym_ifdef_directive] = STATE(319),
-    [sym_ifndef_directive] = STATE(319),
-    [sym_finish_directive] = STATE(319),
-    [sym_ignore_directive] = STATE(319),
-    [sym_unignore_directive] = STATE(319),
-    [sym_lists_directive] = STATE(319),
-    [sym_unlists_directive] = STATE(319),
-    [sym_subscribe_directive] = STATE(319),
-    [sym_unsubscribe_directive] = STATE(319),
-    [sym_macro_directive] = STATE(319),
-    [sym_unmacro_directive] = STATE(319),
-    [sym_mailboxes_directive] = STATE(319),
-    [sym_named_mailboxes_directive] = STATE(319),
-    [sym_unmailboxes_directive] = STATE(319),
-    [sym_mailto_allow_directive] = STATE(319),
-    [sym_unmailto_allow_directive] = STATE(319),
-    [sym_echo_directive] = STATE(319),
-    [sym_cd_directive] = STATE(319),
-    [sym_mbox_hook_directive] = STATE(319),
-    [sym_message_hook_directive] = STATE(319),
-    [sym_mime_lookup_directive] = STATE(319),
-    [sym_unmime_lookup_directive] = STATE(319),
-    [sym_mono_directive] = STATE(319),
-    [sym_unmono_directive] = STATE(319),
-    [sym_my_hdr_directive] = STATE(319),
-    [sym_unmy_hdr_directive] = STATE(319),
-    [sym_open_hook_directive] = STATE(319),
-    [sym_close_hook_directive] = STATE(319),
-    [sym_append_hook_directive] = STATE(319),
-    [sym_push_directive] = STATE(319),
-    [sym_reply_hook_directive] = STATE(319),
-    [sym_send_hook_directive] = STATE(319),
-    [sym_send2_hook_directive] = STATE(319),
-    [sym_spam_directive] = STATE(319),
-    [sym_nospam_directive] = STATE(319),
-    [sym_subjectrx_directive] = STATE(319),
-    [sym_unsubjectrx_directive] = STATE(319),
-    [sym_subscribe_to_directive] = STATE(319),
-    [sym_unsubscribe_from_directive] = STATE(319),
-    [sym_timeout_hook_directive] = STATE(319),
-    [sym_startup_hook_directive] = STATE(319),
-    [sym_shutdown_hook_directive] = STATE(319),
-    [sym_unhook_directive] = STATE(319),
-    [sym_set_directive] = STATE(319),
-    [sym_unset_directive] = STATE(319),
-    [sym_reset_directive] = STATE(319),
-    [sym_toggle_directive] = STATE(319),
-    [sym_setenv_directive] = STATE(319),
-    [sym_unsetenv_directive] = STATE(319),
-    [sym_sidebar_pin_directive] = STATE(319),
-    [sym_sidebar_unpin_directive] = STATE(319),
-    [sym_score_directive] = STATE(319),
-    [sym_unscore_directive] = STATE(319),
-    [sym_source_directive] = STATE(319),
+    [sym__command] = STATE(371),
+    [sym_account_hook_directive] = STATE(371),
+    [sym_alias_directive] = STATE(371),
+    [sym_unalias_directive] = STATE(371),
+    [sym_alternates_directive] = STATE(371),
+    [sym_unalternates_directive] = STATE(371),
+    [sym_alternative_order_directive] = STATE(371),
+    [sym_unalternative_order_directive] = STATE(371),
+    [sym_attachments_directive] = STATE(371),
+    [sym_unattachments_directive] = STATE(371),
+    [sym_auto_view_directive] = STATE(371),
+    [sym_unauto_view_directive] = STATE(371),
+    [sym_bind_directive] = STATE(371),
+    [sym_unbind_directive] = STATE(371),
+    [sym_charset_hook_directive] = STATE(371),
+    [sym_iconv_hook_directive] = STATE(371),
+    [sym_color_directive] = STATE(371),
+    [sym_uncolor_directive] = STATE(371),
+    [sym_crypt_hook_directive] = STATE(371),
+    [sym_index_format_hook_directive] = STATE(371),
+    [sym_exec_directive] = STATE(371),
+    [sym_fcc_save_hook_directive] = STATE(371),
+    [sym_fcc_hook_directive] = STATE(371),
+    [sym_save_hook_directive] = STATE(371),
+    [sym_folder_hook_directive] = STATE(371),
+    [sym_group_directive] = STATE(371),
+    [sym_ungroup_directive] = STATE(371),
+    [sym_hdr_order_directive] = STATE(371),
+    [sym_unhdr_order_directive] = STATE(371),
+    [sym_ifdef_directive] = STATE(371),
+    [sym_ifndef_directive] = STATE(371),
+    [sym_finish_directive] = STATE(371),
+    [sym_ignore_directive] = STATE(371),
+    [sym_unignore_directive] = STATE(371),
+    [sym_lists_directive] = STATE(371),
+    [sym_unlists_directive] = STATE(371),
+    [sym_subscribe_directive] = STATE(371),
+    [sym_unsubscribe_directive] = STATE(371),
+    [sym_macro_directive] = STATE(371),
+    [sym_unmacro_directive] = STATE(371),
+    [sym_mailboxes_directive] = STATE(371),
+    [sym_named_mailboxes_directive] = STATE(371),
+    [sym_unmailboxes_directive] = STATE(371),
+    [sym_mailto_allow_directive] = STATE(371),
+    [sym_unmailto_allow_directive] = STATE(371),
+    [sym_echo_directive] = STATE(371),
+    [sym_cd_directive] = STATE(371),
+    [sym_mbox_hook_directive] = STATE(371),
+    [sym_message_hook_directive] = STATE(371),
+    [sym_mime_lookup_directive] = STATE(371),
+    [sym_unmime_lookup_directive] = STATE(371),
+    [sym_mono_directive] = STATE(371),
+    [sym_unmono_directive] = STATE(371),
+    [sym_my_hdr_directive] = STATE(371),
+    [sym_unmy_hdr_directive] = STATE(371),
+    [sym_open_hook_directive] = STATE(371),
+    [sym_close_hook_directive] = STATE(371),
+    [sym_append_hook_directive] = STATE(371),
+    [sym_push_directive] = STATE(371),
+    [sym_reply_hook_directive] = STATE(371),
+    [sym_send_hook_directive] = STATE(371),
+    [sym_send2_hook_directive] = STATE(371),
+    [sym_spam_directive] = STATE(371),
+    [sym_nospam_directive] = STATE(371),
+    [sym_subjectrx_directive] = STATE(371),
+    [sym_unsubjectrx_directive] = STATE(371),
+    [sym_subscribe_to_directive] = STATE(371),
+    [sym_unsubscribe_from_directive] = STATE(371),
+    [sym_timeout_hook_directive] = STATE(371),
+    [sym_startup_hook_directive] = STATE(371),
+    [sym_shutdown_hook_directive] = STATE(371),
+    [sym_unhook_directive] = STATE(371),
+    [sym_set_directive] = STATE(371),
+    [sym_unset_directive] = STATE(371),
+    [sym_reset_directive] = STATE(371),
+    [sym_toggle_directive] = STATE(371),
+    [sym_setenv_directive] = STATE(371),
+    [sym_unsetenv_directive] = STATE(371),
+    [sym_sidebar_pin_directive] = STATE(371),
+    [sym_sidebar_unpin_directive] = STATE(371),
+    [sym_score_directive] = STATE(371),
+    [sym_unscore_directive] = STATE(371),
+    [sym_source_directive] = STATE(371),
     [anon_sym_account_DASHhook] = ACTIONS(436),
     [anon_sym_alias] = ACTIONS(438),
     [anon_sym_unalias] = ACTIONS(440),
     [anon_sym_alternates] = ACTIONS(442),
     [anon_sym_unalternates] = ACTIONS(444),
     [anon_sym_alternative_order] = ACTIONS(446),
     [anon_sym_unalternative_order] = ACTIONS(448),
@@ -13862,103 +13838,103 @@
     [anon_sym_sidebar_unpin] = ACTIONS(600),
     [anon_sym_score] = ACTIONS(600),
     [anon_sym_unscore] = ACTIONS(600),
     [sym_int] = ACTIONS(600),
     [anon_sym_source] = ACTIONS(600),
   },
   [19] = {
-    [ts_builtin_sym_end] = ACTIONS(175),
-    [anon_sym_account_DASHhook] = ACTIONS(604),
-    [anon_sym_alias] = ACTIONS(604),
-    [anon_sym_unalias] = ACTIONS(604),
-    [anon_sym_alternates] = ACTIONS(604),
-    [anon_sym_unalternates] = ACTIONS(604),
-    [anon_sym_alternative_order] = ACTIONS(604),
-    [anon_sym_unalternative_order] = ACTIONS(604),
-    [anon_sym_attachments] = ACTIONS(604),
-    [anon_sym_unattachments] = ACTIONS(604),
-    [anon_sym_auto_view] = ACTIONS(604),
-    [anon_sym_unauto_view] = ACTIONS(604),
-    [anon_sym_bind] = ACTIONS(604),
-    [anon_sym_unbind] = ACTIONS(604),
-    [anon_sym_charset_DASHhook] = ACTIONS(604),
-    [anon_sym_iconv_DASHhook] = ACTIONS(604),
-    [anon_sym_color] = ACTIONS(604),
-    [anon_sym_uncolor] = ACTIONS(604),
-    [anon_sym_crypt_DASHhook] = ACTIONS(604),
-    [anon_sym_index_DASHformat_DASHhook] = ACTIONS(604),
-    [anon_sym_exec] = ACTIONS(604),
-    [anon_sym_fcc_DASHsave_DASHhook] = ACTIONS(604),
-    [anon_sym_fcc_DASHhook] = ACTIONS(604),
-    [anon_sym_save_DASHhook] = ACTIONS(604),
-    [anon_sym_folder_DASHhook] = ACTIONS(604),
-    [anon_sym_group] = ACTIONS(604),
-    [anon_sym_ungroup] = ACTIONS(604),
-    [anon_sym_hdr_order] = ACTIONS(604),
-    [anon_sym_unhdr_order] = ACTIONS(604),
-    [anon_sym_ifdef] = ACTIONS(604),
-    [anon_sym_ifndef] = ACTIONS(604),
-    [anon_sym_finish] = ACTIONS(604),
-    [anon_sym_ignore] = ACTIONS(604),
-    [anon_sym_unignore] = ACTIONS(604),
-    [anon_sym_lists] = ACTIONS(604),
-    [anon_sym_unlists] = ACTIONS(604),
-    [anon_sym_subscribe] = ACTIONS(604),
-    [anon_sym_unsubscribe] = ACTIONS(604),
-    [anon_sym_macro] = ACTIONS(604),
-    [anon_sym_unmacro] = ACTIONS(604),
-    [anon_sym_mailboxes] = ACTIONS(604),
-    [anon_sym_named_DASHmailboxes] = ACTIONS(604),
-    [anon_sym_unmailboxes] = ACTIONS(604),
-    [anon_sym_mailto_allow] = ACTIONS(604),
-    [anon_sym_unmailto_allow] = ACTIONS(604),
-    [anon_sym_echo] = ACTIONS(604),
-    [anon_sym_cd] = ACTIONS(604),
-    [anon_sym_mbox_DASHhook] = ACTIONS(604),
-    [anon_sym_message_DASHhook] = ACTIONS(604),
-    [anon_sym_mime_lookup] = ACTIONS(604),
-    [anon_sym_unmime_lookup] = ACTIONS(604),
-    [anon_sym_mono] = ACTIONS(604),
-    [anon_sym_unmono] = ACTIONS(604),
-    [anon_sym_my_hdr] = ACTIONS(604),
-    [anon_sym_unmy_hdr] = ACTIONS(604),
-    [anon_sym_open_DASHhook] = ACTIONS(604),
-    [anon_sym_close_DASHhook] = ACTIONS(604),
-    [anon_sym_append_DASHhook] = ACTIONS(604),
-    [anon_sym_push] = ACTIONS(604),
-    [anon_sym_reply_DASHhook] = ACTIONS(604),
-    [anon_sym_send_DASHhook] = ACTIONS(604),
-    [anon_sym_send2_DASHhook] = ACTIONS(604),
-    [anon_sym_spam] = ACTIONS(604),
-    [anon_sym_nospam] = ACTIONS(604),
-    [anon_sym_subjectrx] = ACTIONS(604),
-    [anon_sym_unsubjectrx] = ACTIONS(604),
-    [anon_sym_subscribe_DASHto] = ACTIONS(604),
-    [anon_sym_unsubscribe_DASHfrom] = ACTIONS(604),
-    [anon_sym_timeout_DASHhook] = ACTIONS(604),
-    [anon_sym_startup_DASHhook] = ACTIONS(604),
-    [anon_sym_shutdown_DASHhook] = ACTIONS(604),
-    [anon_sym_unhook] = ACTIONS(604),
-    [anon_sym_set] = ACTIONS(604),
-    [anon_sym_unset] = ACTIONS(604),
-    [anon_sym_reset] = ACTIONS(604),
-    [anon_sym_toggle] = ACTIONS(604),
-    [anon_sym_setenv] = ACTIONS(604),
-    [anon_sym_unsetenv] = ACTIONS(604),
-    [anon_sym_sidebar_pin] = ACTIONS(604),
-    [anon_sym_sidebar_unpin] = ACTIONS(604),
-    [anon_sym_score] = ACTIONS(604),
-    [anon_sym_unscore] = ACTIONS(604),
-    [anon_sym_source] = ACTIONS(604),
-    [sym_comment] = ACTIONS(604),
-    [sym__eol] = ACTIONS(604),
-    [aux_sym__space_token1] = ACTIONS(604),
+    [ts_builtin_sym_end] = ACTIONS(604),
+    [anon_sym_account_DASHhook] = ACTIONS(606),
+    [anon_sym_alias] = ACTIONS(606),
+    [anon_sym_unalias] = ACTIONS(606),
+    [anon_sym_alternates] = ACTIONS(606),
+    [anon_sym_unalternates] = ACTIONS(606),
+    [anon_sym_alternative_order] = ACTIONS(606),
+    [anon_sym_unalternative_order] = ACTIONS(606),
+    [anon_sym_attachments] = ACTIONS(606),
+    [anon_sym_unattachments] = ACTIONS(606),
+    [anon_sym_auto_view] = ACTIONS(606),
+    [anon_sym_unauto_view] = ACTIONS(606),
+    [anon_sym_bind] = ACTIONS(606),
+    [anon_sym_unbind] = ACTIONS(606),
+    [anon_sym_charset_DASHhook] = ACTIONS(606),
+    [anon_sym_iconv_DASHhook] = ACTIONS(606),
+    [anon_sym_color] = ACTIONS(606),
+    [anon_sym_uncolor] = ACTIONS(606),
+    [anon_sym_crypt_DASHhook] = ACTIONS(606),
+    [anon_sym_index_DASHformat_DASHhook] = ACTIONS(606),
+    [anon_sym_exec] = ACTIONS(606),
+    [anon_sym_fcc_DASHsave_DASHhook] = ACTIONS(606),
+    [anon_sym_fcc_DASHhook] = ACTIONS(606),
+    [anon_sym_save_DASHhook] = ACTIONS(606),
+    [anon_sym_folder_DASHhook] = ACTIONS(606),
+    [anon_sym_group] = ACTIONS(606),
+    [anon_sym_ungroup] = ACTIONS(606),
+    [anon_sym_hdr_order] = ACTIONS(606),
+    [anon_sym_unhdr_order] = ACTIONS(606),
+    [anon_sym_ifdef] = ACTIONS(606),
+    [anon_sym_ifndef] = ACTIONS(606),
+    [anon_sym_finish] = ACTIONS(606),
+    [anon_sym_ignore] = ACTIONS(606),
+    [anon_sym_unignore] = ACTIONS(606),
+    [anon_sym_lists] = ACTIONS(606),
+    [anon_sym_unlists] = ACTIONS(606),
+    [anon_sym_subscribe] = ACTIONS(606),
+    [anon_sym_unsubscribe] = ACTIONS(606),
+    [anon_sym_macro] = ACTIONS(606),
+    [anon_sym_unmacro] = ACTIONS(606),
+    [anon_sym_mailboxes] = ACTIONS(606),
+    [anon_sym_named_DASHmailboxes] = ACTIONS(606),
+    [anon_sym_unmailboxes] = ACTIONS(606),
+    [anon_sym_mailto_allow] = ACTIONS(606),
+    [anon_sym_unmailto_allow] = ACTIONS(606),
+    [anon_sym_echo] = ACTIONS(606),
+    [anon_sym_cd] = ACTIONS(606),
+    [anon_sym_mbox_DASHhook] = ACTIONS(606),
+    [anon_sym_message_DASHhook] = ACTIONS(606),
+    [anon_sym_mime_lookup] = ACTIONS(606),
+    [anon_sym_unmime_lookup] = ACTIONS(606),
+    [anon_sym_mono] = ACTIONS(606),
+    [anon_sym_unmono] = ACTIONS(606),
+    [anon_sym_my_hdr] = ACTIONS(606),
+    [anon_sym_unmy_hdr] = ACTIONS(606),
+    [anon_sym_open_DASHhook] = ACTIONS(606),
+    [anon_sym_close_DASHhook] = ACTIONS(606),
+    [anon_sym_append_DASHhook] = ACTIONS(606),
+    [anon_sym_push] = ACTIONS(606),
+    [anon_sym_reply_DASHhook] = ACTIONS(606),
+    [anon_sym_send_DASHhook] = ACTIONS(606),
+    [anon_sym_send2_DASHhook] = ACTIONS(606),
+    [anon_sym_spam] = ACTIONS(606),
+    [anon_sym_nospam] = ACTIONS(606),
+    [anon_sym_subjectrx] = ACTIONS(606),
+    [anon_sym_unsubjectrx] = ACTIONS(606),
+    [anon_sym_subscribe_DASHto] = ACTIONS(606),
+    [anon_sym_unsubscribe_DASHfrom] = ACTIONS(606),
+    [anon_sym_timeout_DASHhook] = ACTIONS(606),
+    [anon_sym_startup_DASHhook] = ACTIONS(606),
+    [anon_sym_shutdown_DASHhook] = ACTIONS(606),
+    [anon_sym_unhook] = ACTIONS(606),
+    [anon_sym_set] = ACTIONS(606),
+    [anon_sym_unset] = ACTIONS(606),
+    [anon_sym_reset] = ACTIONS(606),
+    [anon_sym_toggle] = ACTIONS(606),
+    [anon_sym_setenv] = ACTIONS(606),
+    [anon_sym_unsetenv] = ACTIONS(606),
+    [anon_sym_sidebar_pin] = ACTIONS(606),
+    [anon_sym_sidebar_unpin] = ACTIONS(606),
+    [anon_sym_score] = ACTIONS(606),
+    [anon_sym_unscore] = ACTIONS(606),
+    [anon_sym_source] = ACTIONS(606),
+    [sym_comment] = ACTIONS(606),
+    [sym__eol] = ACTIONS(606),
+    [aux_sym__space_token1] = ACTIONS(606),
   },
   [20] = {
-    [ts_builtin_sym_end] = ACTIONS(606),
+    [ts_builtin_sym_end] = ACTIONS(175),
     [anon_sym_account_DASHhook] = ACTIONS(608),
     [anon_sym_alias] = ACTIONS(608),
     [anon_sym_unalias] = ACTIONS(608),
     [anon_sym_alternates] = ACTIONS(608),
     [anon_sym_unalternates] = ACTIONS(608),
     [anon_sym_alternative_order] = ACTIONS(608),
     [anon_sym_unalternative_order] = ACTIONS(608),
@@ -14471,20 +14447,19 @@
   [0] = 7,
     ACTIONS(632), 1,
       anon_sym_SQUOTE,
     ACTIONS(634), 1,
       anon_sym_DQUOTE,
     ACTIONS(636), 1,
       anon_sym_BQUOTE,
+    ACTIONS(638), 1,
+      sym__word,
     STATE(18), 1,
       sym__string,
-    ACTIONS(638), 2,
-      anon_sym_LF,
-      sym__word,
-    STATE(171), 2,
+    STATE(153), 2,
       sym_pattern,
       sym_object,
     ACTIONS(630), 39,
       anon_sym_index,
       anon_sym_attach_headers,
       anon_sym_attachment,
       anon_sym_body,
@@ -14519,18 +14494,18 @@
       anon_sym_sidebar_divider,
       anon_sym_sidebar_flagged,
       anon_sym_sidebar_highlight,
       anon_sym_sidebar_indicator,
       anon_sym_sidebar_new,
       anon_sym_sidebar_ordinary,
       anon_sym_sidebar_spool_file,
-  [62] = 4,
+  [61] = 4,
     ACTIONS(640), 1,
       anon_sym_compose,
-    STATE(29), 1,
+    STATE(30), 1,
       sym_object,
     ACTIONS(630), 2,
       anon_sym_index,
       anon_sym_index_tag,
     ACTIONS(642), 37,
       anon_sym_attach_headers,
       anon_sym_attachment,
@@ -14565,49 +14540,22 @@
       anon_sym_sidebar_divider,
       anon_sym_sidebar_flagged,
       anon_sym_sidebar_highlight,
       anon_sym_sidebar_indicator,
       anon_sym_sidebar_new,
       anon_sym_sidebar_ordinary,
       anon_sym_sidebar_spool_file,
-  [112] = 6,
-    STATE(46), 1,
-      sym_attribute,
-    STATE(49), 1,
+  [111] = 6,
+    STATE(39), 1,
       sym_foreground,
-    STATE(50), 1,
+    STATE(40), 1,
       sym__attributes,
-    STATE(57), 1,
-      sym_color,
-    ACTIONS(644), 5,
-      anon_sym_bold,
-      anon_sym_underline,
-      anon_sym_none,
-      anon_sym_reverse,
-      anon_sym_standout,
-    ACTIONS(646), 11,
-      anon_sym_default,
-      anon_sym_black,
-      anon_sym_red,
-      anon_sym_green,
-      anon_sym_yellow,
-      anon_sym_blue,
-      anon_sym_magenta,
-      anon_sym_cyan,
-      anon_sym_white,
-      aux_sym_color_token1,
-      aux_sym_color_token2,
-  [145] = 6,
     STATE(41), 1,
-      sym__attributes,
-    STATE(44), 1,
-      sym_foreground,
-    STATE(46), 1,
       sym_attribute,
-    STATE(57), 1,
+    STATE(53), 1,
       sym_color,
     ACTIONS(644), 5,
       anon_sym_bold,
       anon_sym_underline,
       anon_sym_none,
       anon_sym_reverse,
       anon_sym_standout,
@@ -14619,18 +14567,18 @@
       anon_sym_yellow,
       anon_sym_blue,
       anon_sym_magenta,
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
-  [178] = 3,
+  [144] = 3,
     ACTIONS(650), 1,
       anon_sym_STAR,
-    STATE(401), 1,
+    STATE(439), 1,
       sym_hook_type,
     ACTIONS(648), 18,
       anon_sym_account_DASHhook,
       anon_sym_charset_DASHhook,
       anon_sym_iconv_DASHhook,
       anon_sym_crypt_DASHhook,
       anon_sym_fcc_DASHhook,
@@ -14643,37 +14591,43 @@
       anon_sym_append_DASHhook,
       anon_sym_reply_DASHhook,
       anon_sym_send_DASHhook,
       anon_sym_send2_DASHhook,
       anon_sym_timeout_DASHhook,
       anon_sym_startup_DASHhook,
       anon_sym_shutdown_DASHhook,
-  [205] = 4,
-    ACTIONS(654), 1,
-      anon_sym_STAR,
-    STATE(250), 1,
-      sym_map,
-    STATE(252), 1,
-      sym__maps,
-    ACTIONS(652), 13,
-      anon_sym_alias,
-      anon_sym_attach,
-      anon_sym_browser,
-      anon_sym_compose,
-      anon_sym_editor,
-      anon_sym_generic,
-      anon_sym_index,
-      anon_sym_mix,
-      anon_sym_pager,
-      anon_sym_pgp,
-      anon_sym_postpone,
-      anon_sym_query,
-      anon_sym_smime,
-  [230] = 1,
-    ACTIONS(656), 16,
+  [171] = 6,
+    STATE(41), 1,
+      sym_attribute,
+    STATE(43), 1,
+      sym__attributes,
+    STATE(44), 1,
+      sym_foreground,
+    STATE(53), 1,
+      sym_color,
+    ACTIONS(644), 5,
+      anon_sym_bold,
+      anon_sym_underline,
+      anon_sym_none,
+      anon_sym_reverse,
+      anon_sym_standout,
+    ACTIONS(646), 11,
+      anon_sym_default,
+      anon_sym_black,
+      anon_sym_red,
+      anon_sym_green,
+      anon_sym_yellow,
+      anon_sym_blue,
+      anon_sym_magenta,
+      anon_sym_cyan,
+      anon_sym_white,
+      aux_sym_color_token1,
+      aux_sym_color_token2,
+  [204] = 1,
+    ACTIONS(652), 16,
       anon_sym_bold,
       anon_sym_underline,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
@@ -14682,16 +14636,16 @@
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
       anon_sym_none,
       anon_sym_reverse,
       anon_sym_standout,
-  [249] = 1,
-    ACTIONS(658), 16,
+  [223] = 1,
+    ACTIONS(654), 16,
       anon_sym_bold,
       anon_sym_underline,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
@@ -14700,5581 +14654,5441 @@
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
       anon_sym_none,
       anon_sym_reverse,
       anon_sym_standout,
-  [268] = 4,
+  [242] = 4,
+    ACTIONS(658), 1,
+      anon_sym_STAR,
+    STATE(217), 1,
+      sym__maps,
+    STATE(233), 1,
+      sym_map,
+    ACTIONS(656), 13,
+      anon_sym_alias,
+      anon_sym_attach,
+      anon_sym_browser,
+      anon_sym_compose,
+      anon_sym_editor,
+      anon_sym_generic,
+      anon_sym_index,
+      anon_sym_mix,
+      anon_sym_pager,
+      anon_sym_pgp,
+      anon_sym_postpone,
+      anon_sym_query,
+      anon_sym_smime,
+  [267] = 4,
     ACTIONS(660), 1,
       anon_sym_STAR,
-    STATE(191), 1,
+    STATE(171), 1,
       sym__maps,
-    STATE(250), 1,
+    STATE(233), 1,
       sym_map,
-    ACTIONS(652), 13,
+    ACTIONS(656), 13,
       anon_sym_alias,
       anon_sym_attach,
       anon_sym_browser,
       anon_sym_compose,
       anon_sym_editor,
       anon_sym_generic,
       anon_sym_index,
       anon_sym_mix,
       anon_sym_pager,
       anon_sym_pgp,
       anon_sym_postpone,
       anon_sym_query,
       anon_sym_smime,
-  [293] = 3,
-    STATE(185), 1,
+  [292] = 3,
+    STATE(232), 1,
       sym__maps,
-    STATE(250), 1,
+    STATE(233), 1,
       sym_map,
-    ACTIONS(652), 13,
+    ACTIONS(656), 13,
       anon_sym_alias,
       anon_sym_attach,
       anon_sym_browser,
       anon_sym_compose,
       anon_sym_editor,
       anon_sym_generic,
       anon_sym_index,
       anon_sym_mix,
       anon_sym_pager,
       anon_sym_pgp,
       anon_sym_postpone,
       anon_sym_query,
       anon_sym_smime,
-  [315] = 3,
-    STATE(190), 1,
+  [314] = 3,
+    STATE(170), 1,
       sym__maps,
-    STATE(250), 1,
+    STATE(233), 1,
       sym_map,
-    ACTIONS(652), 13,
+    ACTIONS(656), 13,
       anon_sym_alias,
       anon_sym_attach,
       anon_sym_browser,
       anon_sym_compose,
       anon_sym_editor,
       anon_sym_generic,
       anon_sym_index,
       anon_sym_mix,
       anon_sym_pager,
       anon_sym_pgp,
       anon_sym_postpone,
       anon_sym_query,
       anon_sym_smime,
-  [337] = 2,
-    STATE(304), 1,
+  [336] = 2,
+    STATE(288), 1,
       sym_map,
-    ACTIONS(652), 13,
+    ACTIONS(656), 13,
       anon_sym_alias,
       anon_sym_attach,
       anon_sym_browser,
       anon_sym_compose,
       anon_sym_editor,
       anon_sym_generic,
       anon_sym_index,
       anon_sym_mix,
       anon_sym_pager,
       anon_sym_pgp,
       anon_sym_postpone,
       anon_sym_query,
       anon_sym_smime,
-  [356] = 9,
+  [355] = 3,
     ACTIONS(662), 1,
       anon_sym_SPACE,
-    ACTIONS(666), 1,
-      sym_int,
-    ACTIONS(668), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(670), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(672), 1,
-      anon_sym_BQUOTE,
-    STATE(216), 1,
-      sym__string,
-    STATE(217), 1,
-      sym_quadoption,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-    ACTIONS(664), 4,
-      anon_sym_yes,
-      anon_sym_no,
-      anon_sym_ask_DASHyes,
-      anon_sym_ask_DASHno,
-  [388] = 9,
-    ACTIONS(668), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(670), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(672), 1,
-      anon_sym_BQUOTE,
-    ACTIONS(676), 1,
-      anon_sym_SPACE,
-    ACTIONS(678), 1,
-      sym_int,
-    STATE(224), 1,
-      sym__string,
-    STATE(226), 1,
-      sym_quadoption,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-    ACTIONS(664), 4,
-      anon_sym_yes,
-      anon_sym_no,
-      anon_sym_ask_DASHyes,
-      anon_sym_ask_DASHno,
-  [420] = 9,
-    ACTIONS(668), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(670), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(672), 1,
-      anon_sym_BQUOTE,
-    ACTIONS(680), 1,
-      anon_sym_SPACE,
-    ACTIONS(682), 1,
-      sym_int,
-    STATE(284), 1,
-      sym__string,
-    STATE(286), 1,
-      sym_quadoption,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-    ACTIONS(664), 4,
-      anon_sym_yes,
-      anon_sym_no,
-      anon_sym_ask_DASHyes,
-      anon_sym_ask_DASHno,
-  [452] = 3,
-    STATE(47), 1,
+    STATE(38), 1,
+      aux_sym__attributes_repeat1,
+    ACTIONS(665), 11,
+      anon_sym_default,
+      anon_sym_black,
+      anon_sym_red,
+      anon_sym_green,
+      anon_sym_yellow,
+      anon_sym_blue,
+      anon_sym_magenta,
+      anon_sym_cyan,
+      anon_sym_white,
+      aux_sym_color_token1,
+      aux_sym_color_token2,
+  [375] = 3,
+    STATE(403), 1,
+      sym_background,
+    STATE(422), 1,
+      sym_color,
+    ACTIONS(667), 11,
+      anon_sym_default,
+      anon_sym_black,
+      anon_sym_red,
+      anon_sym_green,
+      anon_sym_yellow,
+      anon_sym_blue,
+      anon_sym_magenta,
+      anon_sym_cyan,
+      anon_sym_white,
+      aux_sym_color_token1,
+      aux_sym_color_token2,
+  [395] = 3,
+    STATE(46), 1,
       sym_foreground,
-    STATE(57), 1,
+    STATE(53), 1,
       sym_color,
     ACTIONS(646), 11,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
       anon_sym_blue,
       anon_sym_magenta,
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
-  [472] = 9,
-    ACTIONS(668), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(670), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(672), 1,
-      anon_sym_BQUOTE,
-    ACTIONS(684), 1,
+  [415] = 3,
+    ACTIONS(669), 1,
       anon_sym_SPACE,
-    ACTIONS(686), 1,
-      sym_int,
-    STATE(282), 1,
-      sym__string,
-    STATE(283), 1,
-      sym_quadoption,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-    ACTIONS(664), 4,
-      anon_sym_yes,
-      anon_sym_no,
-      anon_sym_ask_DASHyes,
-      anon_sym_ask_DASHno,
-  [504] = 3,
-    ACTIONS(688), 1,
-      anon_sym_SPACE,
-    STATE(43), 1,
+    STATE(42), 1,
       aux_sym__attributes_repeat1,
-    ACTIONS(691), 11,
+    ACTIONS(671), 11,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
       anon_sym_blue,
       anon_sym_magenta,
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
-  [524] = 3,
-    STATE(177), 1,
-      sym_background,
-    STATE(234), 1,
-      sym_color,
-    ACTIONS(693), 11,
+  [435] = 3,
+    ACTIONS(669), 1,
+      anon_sym_SPACE,
+    STATE(38), 1,
+      aux_sym__attributes_repeat1,
+    ACTIONS(673), 11,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
       anon_sym_blue,
       anon_sym_magenta,
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
-  [544] = 3,
-    STATE(416), 1,
+  [455] = 3,
+    STATE(45), 1,
+      sym_foreground,
+    STATE(53), 1,
       sym_color,
-    STATE(419), 1,
-      sym_background,
-    ACTIONS(695), 11,
+    ACTIONS(646), 11,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
       anon_sym_blue,
       anon_sym_magenta,
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
-  [564] = 3,
-    ACTIONS(697), 1,
-      anon_sym_SPACE,
-    STATE(48), 1,
-      aux_sym__attributes_repeat1,
-    ACTIONS(699), 11,
+  [475] = 3,
+    STATE(73), 1,
+      sym_background,
+    STATE(85), 1,
+      sym_color,
+    ACTIONS(675), 11,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
       anon_sym_blue,
       anon_sym_magenta,
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
-  [584] = 3,
-    STATE(183), 1,
+  [495] = 3,
+    STATE(72), 1,
       sym_background,
-    STATE(234), 1,
+    STATE(85), 1,
       sym_color,
-    ACTIONS(693), 11,
+    ACTIONS(675), 11,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
       anon_sym_blue,
       anon_sym_magenta,
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
-  [604] = 3,
-    ACTIONS(697), 1,
-      anon_sym_SPACE,
-    STATE(43), 1,
-      aux_sym__attributes_repeat1,
-    ACTIONS(701), 11,
+  [515] = 3,
+    STATE(419), 1,
+      sym_background,
+    STATE(422), 1,
+      sym_color,
+    ACTIONS(667), 11,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
       anon_sym_blue,
       anon_sym_magenta,
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
-  [624] = 3,
-    STATE(403), 1,
-      sym_background,
-    STATE(416), 1,
-      sym_color,
-    ACTIONS(695), 11,
+  [535] = 9,
+    ACTIONS(677), 1,
+      anon_sym_SPACE,
+    ACTIONS(681), 1,
+      sym_int,
+    ACTIONS(683), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(685), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(687), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(689), 1,
+      sym__word,
+    STATE(261), 1,
+      sym_quadoption,
+    STATE(262), 1,
+      sym__string,
+    ACTIONS(679), 4,
+      anon_sym_yes,
+      anon_sym_no,
+      anon_sym_ask_DASHyes,
+      anon_sym_ask_DASHno,
+  [566] = 2,
+    ACTIONS(691), 1,
+      anon_sym_SPACE,
+    ACTIONS(665), 11,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
       anon_sym_blue,
       anon_sym_magenta,
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
-  [644] = 3,
-    STATE(45), 1,
-      sym_foreground,
-    STATE(57), 1,
-      sym_color,
-    ACTIONS(646), 11,
+  [583] = 2,
+    ACTIONS(693), 1,
+      anon_sym_SPACE,
+    ACTIONS(695), 11,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
       anon_sym_blue,
       anon_sym_magenta,
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
-  [664] = 8,
-    ACTIONS(668), 1,
+  [600] = 9,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    ACTIONS(703), 1,
+    ACTIONS(689), 1,
+      sym__word,
+    ACTIONS(697), 1,
+      anon_sym_SPACE,
+    ACTIONS(699), 1,
       sym_int,
-    STATE(184), 1,
-      sym__string,
-    STATE(212), 1,
+    STATE(263), 1,
       sym_quadoption,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-    ACTIONS(664), 4,
+    STATE(266), 1,
+      sym__string,
+    ACTIONS(679), 4,
       anon_sym_yes,
       anon_sym_no,
       anon_sym_ask_DASHyes,
       anon_sym_ask_DASHno,
-  [693] = 8,
-    ACTIONS(668), 1,
+  [631] = 9,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    ACTIONS(686), 1,
+    ACTIONS(689), 1,
+      sym__word,
+    ACTIONS(701), 1,
+      anon_sym_SPACE,
+    ACTIONS(703), 1,
       sym_int,
-    STATE(281), 1,
-      sym__string,
-    STATE(283), 1,
+    STATE(215), 1,
       sym_quadoption,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-    ACTIONS(664), 4,
+    STATE(218), 1,
+      sym__string,
+    ACTIONS(679), 4,
       anon_sym_yes,
       anon_sym_no,
       anon_sym_ask_DASHyes,
       anon_sym_ask_DASHno,
-  [722] = 8,
-    ACTIONS(668), 1,
+  [662] = 9,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
+    ACTIONS(689), 1,
+      sym__word,
     ACTIONS(705), 1,
+      anon_sym_SPACE,
+    ACTIONS(707), 1,
       sym_int,
-    STATE(279), 1,
+    STATE(240), 1,
       sym__string,
-    STATE(280), 1,
+    STATE(241), 1,
       sym_quadoption,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-    ACTIONS(664), 4,
+    ACTIONS(679), 4,
       anon_sym_yes,
       anon_sym_no,
       anon_sym_ask_DASHyes,
       anon_sym_ask_DASHno,
-  [751] = 2,
-    ACTIONS(707), 1,
-      anon_sym_SPACE,
-    ACTIONS(691), 11,
+  [693] = 1,
+    ACTIONS(709), 11,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
       anon_sym_blue,
       anon_sym_magenta,
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
-  [768] = 8,
-    ACTIONS(666), 1,
-      sym_int,
-    ACTIONS(668), 1,
+  [707] = 8,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    STATE(215), 1,
+    ACTIONS(689), 1,
+      sym__word,
+    ACTIONS(707), 1,
+      sym_int,
+    STATE(239), 1,
       sym__string,
-    STATE(217), 1,
+    STATE(241), 1,
       sym_quadoption,
-    ACTIONS(674), 2,
-      anon_sym_LF,
+    ACTIONS(679), 4,
+      anon_sym_yes,
+      anon_sym_no,
+      anon_sym_ask_DASHyes,
+      anon_sym_ask_DASHno,
+  [735] = 8,
+    ACTIONS(683), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(685), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(687), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(689), 1,
       sym__word,
-    ACTIONS(664), 4,
+    ACTIONS(699), 1,
+      sym_int,
+    STATE(263), 1,
+      sym_quadoption,
+    STATE(267), 1,
+      sym__string,
+    ACTIONS(679), 4,
       anon_sym_yes,
       anon_sym_no,
       anon_sym_ask_DASHyes,
       anon_sym_ask_DASHno,
-  [797] = 2,
-    ACTIONS(709), 1,
-      anon_sym_SPACE,
-    ACTIONS(711), 11,
-      anon_sym_default,
-      anon_sym_black,
-      anon_sym_red,
-      anon_sym_green,
-      anon_sym_yellow,
-      anon_sym_blue,
-      anon_sym_magenta,
-      anon_sym_cyan,
-      anon_sym_white,
-      aux_sym_color_token1,
-      aux_sym_color_token2,
-  [814] = 1,
+  [763] = 8,
+    ACTIONS(683), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(685), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(687), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(689), 1,
+      sym__word,
+    ACTIONS(711), 1,
+      sym_int,
+    STATE(268), 1,
+      sym_quadoption,
+    STATE(269), 1,
+      sym__string,
+    ACTIONS(679), 4,
+      anon_sym_yes,
+      anon_sym_no,
+      anon_sym_ask_DASHyes,
+      anon_sym_ask_DASHno,
+  [791] = 1,
     ACTIONS(713), 11,
       anon_sym_default,
       anon_sym_black,
       anon_sym_red,
       anon_sym_green,
       anon_sym_yellow,
       anon_sym_blue,
       anon_sym_magenta,
       anon_sym_cyan,
       anon_sym_white,
       aux_sym_color_token1,
       aux_sym_color_token2,
-  [828] = 1,
-    ACTIONS(715), 11,
-      anon_sym_default,
-      anon_sym_black,
-      anon_sym_red,
-      anon_sym_green,
-      anon_sym_yellow,
-      anon_sym_blue,
-      anon_sym_magenta,
-      anon_sym_cyan,
-      anon_sym_white,
-      aux_sym_color_token1,
-      aux_sym_color_token2,
-  [842] = 10,
+  [805] = 8,
+    ACTIONS(683), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(685), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(687), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(689), 1,
+      sym__word,
+    ACTIONS(715), 1,
+      sym_int,
+    STATE(161), 1,
+      sym__string,
+    STATE(231), 1,
+      sym_quadoption,
+    ACTIONS(679), 4,
+      anon_sym_yes,
+      anon_sym_no,
+      anon_sym_ask_DASHyes,
+      anon_sym_ask_DASHno,
+  [833] = 9,
     ACTIONS(717), 1,
       anon_sym_DASHgroup,
     ACTIONS(719), 1,
       anon_sym_STAR,
     ACTIONS(721), 1,
       anon_sym_SQUOTE,
     ACTIONS(723), 1,
       anon_sym_DQUOTE,
     ACTIONS(725), 1,
       anon_sym_BQUOTE,
     ACTIONS(727), 1,
-      anon_sym_LF,
-    ACTIONS(729), 1,
       sym__word,
-    STATE(80), 1,
+    STATE(75), 1,
       sym__group,
-    STATE(235), 1,
+    STATE(192), 1,
       sym__regex,
-    STATE(368), 1,
+    STATE(367), 1,
       sym__regexes,
-  [873] = 8,
+  [861] = 8,
+    ACTIONS(729), 1,
+      anon_sym_STAR,
     ACTIONS(733), 1,
-      anon_sym_QMARK,
-    ACTIONS(735), 1,
       anon_sym_SQUOTE,
-    ACTIONS(737), 1,
+    ACTIONS(735), 1,
       anon_sym_DQUOTE,
-    ACTIONS(739), 1,
+    ACTIONS(737), 1,
       anon_sym_BQUOTE,
-    STATE(454), 1,
+    ACTIONS(739), 1,
+      sym__word,
+    STATE(459), 1,
       sym_disposition,
-    STATE(490), 1,
+    STATE(480), 1,
       sym__string,
     ACTIONS(731), 2,
       anon_sym_PLUS,
       anon_sym_DASH,
-    ACTIONS(741), 2,
-      anon_sym_LF,
-      sym__word,
-  [900] = 8,
-    ACTIONS(735), 1,
+  [887] = 8,
+    ACTIONS(733), 1,
       anon_sym_SQUOTE,
-    ACTIONS(737), 1,
+    ACTIONS(735), 1,
       anon_sym_DQUOTE,
-    ACTIONS(739), 1,
+    ACTIONS(737), 1,
       anon_sym_BQUOTE,
+    ACTIONS(739), 1,
+      sym__word,
     ACTIONS(743), 1,
-      anon_sym_STAR,
-    STATE(452), 1,
+      anon_sym_QMARK,
+    STATE(454), 1,
       sym_disposition,
-    STATE(490), 1,
+    STATE(480), 1,
       sym__string,
     ACTIONS(741), 2,
-      anon_sym_LF,
-      sym__word,
-    ACTIONS(745), 2,
       anon_sym_PLUS,
       anon_sym_DASH,
-  [927] = 8,
-    ACTIONS(668), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(670), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(672), 1,
-      anon_sym_BQUOTE,
-    ACTIONS(747), 1,
-      anon_sym_STAR,
-    STATE(259), 1,
-      sym_header,
-    STATE(278), 1,
-      sym__string,
-    STATE(391), 1,
-      sym__headers,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-  [953] = 4,
-    ACTIONS(749), 1,
+  [913] = 4,
+    ACTIONS(745), 1,
       anon_sym_LT,
-    STATE(63), 1,
+    STATE(69), 1,
       aux_sym_key_repeat1,
-    ACTIONS(752), 2,
+    ACTIONS(747), 2,
       aux_sym_key_token2,
       aux_sym_key_token3,
-    ACTIONS(755), 5,
+    ACTIONS(749), 4,
       anon_sym_SQUOTE,
       anon_sym_DQUOTE,
       anon_sym_BQUOTE,
-      anon_sym_LF,
       sym__word,
-  [971] = 9,
-    ACTIONS(721), 1,
+  [930] = 8,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(723), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(725), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    ACTIONS(727), 1,
-      anon_sym_LF,
-    ACTIONS(729), 1,
+    ACTIONS(689), 1,
       sym__word,
-    ACTIONS(757), 1,
-      anon_sym_DASHgroup,
-    STATE(106), 1,
-      sym__group,
-    STATE(235), 1,
-      sym__regex,
-    STATE(372), 1,
-      sym__regexes,
-  [999] = 8,
-    ACTIONS(668), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(670), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(672), 1,
-      anon_sym_BQUOTE,
-    ACTIONS(759), 1,
+    ACTIONS(751), 1,
       anon_sym_STAR,
-    STATE(192), 1,
+    STATE(172), 1,
       sym_mailbox,
-    STATE(273), 1,
+    STATE(302), 1,
       sym__string,
-    STATE(405), 1,
+    STATE(360), 1,
       sym__mailboxes,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-  [1025] = 8,
-    ACTIONS(668), 1,
+  [955] = 8,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    ACTIONS(761), 1,
-      anon_sym_STAR,
-    STATE(198), 1,
-      sym_header_field,
-    STATE(275), 1,
-      sym__string,
-    STATE(409), 1,
-      sym__header_fields,
-    ACTIONS(674), 2,
-      anon_sym_LF,
+    ACTIONS(689), 1,
       sym__word,
-  [1051] = 8,
-    ACTIONS(668), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(670), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(672), 1,
-      anon_sym_BQUOTE,
-    ACTIONS(763), 1,
+    ACTIONS(753), 1,
       anon_sym_STAR,
-    STATE(198), 1,
+    STATE(179), 1,
       sym_header_field,
-    STATE(275), 1,
+    STATE(297), 1,
       sym__string,
-    STATE(412), 1,
+    STATE(363), 1,
       sym__header_fields,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-  [1077] = 4,
-    ACTIONS(765), 1,
+  [980] = 7,
+    ACTIONS(755), 1,
+      anon_sym_DASHgroup,
+    ACTIONS(757), 1,
+      anon_sym_STAR,
+    ACTIONS(759), 1,
       anon_sym_LT,
-    STATE(63), 1,
+    STATE(92), 1,
       aux_sym_key_repeat1,
-    ACTIONS(767), 2,
+    STATE(107), 1,
+      sym__group,
+    STATE(334), 1,
+      sym_key,
+    ACTIONS(761), 2,
       aux_sym_key_token2,
       aux_sym_key_token3,
-    ACTIONS(769), 5,
+  [1003] = 8,
+    ACTIONS(721), 1,
       anon_sym_SQUOTE,
+    ACTIONS(723), 1,
       anon_sym_DQUOTE,
+    ACTIONS(725), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
+    ACTIONS(727), 1,
       sym__word,
-  [1095] = 8,
-    ACTIONS(668), 1,
+    ACTIONS(763), 1,
+      anon_sym_DASHgroup,
+    STATE(112), 1,
+      sym__group,
+    STATE(192), 1,
+      sym__regex,
+    STATE(349), 1,
+      sym__regexes,
+  [1028] = 8,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    ACTIONS(771), 1,
+    ACTIONS(689), 1,
+      sym__word,
+    ACTIONS(765), 1,
       anon_sym_STAR,
-    STATE(192), 1,
-      sym_mailbox,
-    STATE(273), 1,
+    STATE(179), 1,
+      sym_header_field,
+    STATE(297), 1,
       sym__string,
-    STATE(376), 1,
-      sym__mailboxes,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-  [1121] = 7,
+    STATE(362), 1,
+      sym__header_fields,
+  [1053] = 4,
+    ACTIONS(767), 1,
+      anon_sym_SPACE,
+    STATE(174), 1,
+      aux_sym__options2_repeat1,
+    ACTIONS(769), 3,
+      anon_sym_PLUS_EQ,
+      anon_sym_DASH_EQ,
+      anon_sym_EQ,
+    ACTIONS(771), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [1070] = 4,
     ACTIONS(773), 1,
-      anon_sym_STAR,
-    ACTIONS(775), 1,
+      anon_sym_LT,
+    STATE(69), 1,
+      aux_sym_key_repeat1,
+    ACTIONS(776), 2,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+    ACTIONS(779), 4,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
       anon_sym_BQUOTE,
-    STATE(382), 1,
-      sym__string,
-    STATE(421), 1,
-      sym_pattern,
-    ACTIONS(781), 2,
-      anon_sym_LF,
       sym__word,
-  [1144] = 7,
-    ACTIONS(668), 1,
+  [1087] = 8,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    STATE(259), 1,
+    ACTIONS(689), 1,
+      sym__word,
+    ACTIONS(781), 1,
+      anon_sym_STAR,
+    STATE(195), 1,
       sym_header,
-    STATE(278), 1,
+    STATE(287), 1,
       sym__string,
-    STATE(439), 1,
+    STATE(417), 1,
       sym__headers,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-  [1167] = 8,
-    ACTIONS(721), 1,
+  [1112] = 8,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(723), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(725), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    ACTIONS(727), 1,
-      anon_sym_LF,
-    ACTIONS(729), 1,
+    ACTIONS(689), 1,
       sym__word,
     ACTIONS(783), 1,
       anon_sym_STAR,
-    STATE(235), 1,
-      sym__regex,
-    STATE(322), 1,
-      sym__regexes,
-  [1192] = 7,
-    ACTIONS(775), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(777), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(779), 1,
-      anon_sym_BQUOTE,
-    STATE(247), 1,
-      sym_address,
-    STATE(290), 1,
+    STATE(172), 1,
+      sym_mailbox,
+    STATE(302), 1,
       sym__string,
-    STATE(345), 1,
-      sym__addresses,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [1215] = 7,
-    ACTIONS(668), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(670), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(672), 1,
-      anon_sym_BQUOTE,
+    STATE(426), 1,
+      sym__mailboxes,
+  [1137] = 6,
     ACTIONS(785), 1,
-      anon_sym_STAR,
-    STATE(187), 1,
-      sym__string,
-    STATE(398), 1,
-      sym__strings,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-  [1238] = 1,
-    ACTIONS(787), 8,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
       anon_sym_SQUOTE,
+    ACTIONS(787), 1,
       anon_sym_DQUOTE,
+    ACTIONS(789), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
+    ACTIONS(791), 1,
       sym__word,
-  [1249] = 7,
-    ACTIONS(775), 1,
+    STATE(420), 1,
+      sym__regex,
+    ACTIONS(793), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [1158] = 6,
+    ACTIONS(785), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(787), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
-      anon_sym_BQUOTE,
-    STATE(247), 1,
-      sym_address,
-    STATE(290), 1,
-      sym__string,
-    STATE(356), 1,
-      sym__addresses,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [1272] = 7,
     ACTIONS(789), 1,
-      anon_sym_BANG,
-    ACTIONS(791), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(793), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(795), 1,
       anon_sym_BQUOTE,
-    STATE(163), 1,
-      sym_pattern,
-    STATE(204), 1,
-      sym__string,
-    ACTIONS(797), 2,
-      anon_sym_LF,
+    ACTIONS(791), 1,
       sym__word,
-  [1295] = 7,
+    STATE(407), 1,
+      sym__regex,
+    ACTIONS(795), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [1179] = 7,
+    ACTIONS(797), 1,
+      anon_sym_BANG,
     ACTIONS(799), 1,
-      anon_sym_DASHgroup,
-    ACTIONS(801), 1,
-      anon_sym_STAR,
-    ACTIONS(803), 1,
-      anon_sym_LT,
-    STATE(97), 1,
-      aux_sym_key_repeat1,
-    STATE(179), 1,
-      sym__group,
-    STATE(402), 1,
-      sym_key,
-    ACTIONS(805), 2,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [1318] = 7,
-    ACTIONS(668), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(801), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(803), 1,
       anon_sym_BQUOTE,
-    STATE(192), 1,
-      sym_mailbox,
-    STATE(273), 1,
-      sym__string,
-    STATE(377), 1,
-      sym__mailboxes,
-    ACTIONS(674), 2,
-      anon_sym_LF,
+    ACTIONS(805), 1,
       sym__word,
-  [1341] = 8,
+    STATE(202), 1,
+      sym_pattern,
+    STATE(272), 1,
+      sym__string,
+  [1201] = 7,
     ACTIONS(721), 1,
       anon_sym_SQUOTE,
     ACTIONS(723), 1,
       anon_sym_DQUOTE,
     ACTIONS(725), 1,
       anon_sym_BQUOTE,
     ACTIONS(727), 1,
-      anon_sym_LF,
-    ACTIONS(729), 1,
       sym__word,
     ACTIONS(807), 1,
       anon_sym_STAR,
-    STATE(235), 1,
+    STATE(192), 1,
       sym__regex,
-    STATE(353), 1,
+    STATE(398), 1,
       sym__regexes,
-  [1366] = 4,
+  [1223] = 6,
+    ACTIONS(745), 1,
+      anon_sym_LT,
     ACTIONS(809), 1,
-      anon_sym_SPACE,
-    STATE(244), 1,
-      aux_sym__options2_repeat1,
-    ACTIONS(811), 3,
-      anon_sym_PLUS_EQ,
-      anon_sym_DASH_EQ,
-      anon_sym_EQ,
-    ACTIONS(813), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [1383] = 7,
-    ACTIONS(775), 1,
+      anon_sym_DASHgroup,
+    STATE(62), 1,
+      aux_sym_key_repeat1,
+    STATE(91), 1,
+      sym_key,
+    STATE(169), 1,
+      sym__group,
+    ACTIONS(811), 2,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [1243] = 7,
+    ACTIONS(813), 1,
+      anon_sym_STAR,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    ACTIONS(815), 1,
-      anon_sym_STAR,
-    STATE(371), 1,
+    ACTIONS(821), 1,
+      sym__word,
+    STATE(320), 1,
       sym_pattern,
-    STATE(382), 1,
+    STATE(391), 1,
       sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [1406] = 7,
-    ACTIONS(775), 1,
+  [1265] = 1,
+    ACTIONS(823), 7,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
       anon_sym_BQUOTE,
-    ACTIONS(817), 1,
-      anon_sym_STAR,
-    STATE(333), 1,
-      sym_pattern,
-    STATE(382), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
       sym__word,
-  [1429] = 8,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [1275] = 7,
     ACTIONS(721), 1,
       anon_sym_SQUOTE,
     ACTIONS(723), 1,
       anon_sym_DQUOTE,
     ACTIONS(725), 1,
       anon_sym_BQUOTE,
     ACTIONS(727), 1,
-      anon_sym_LF,
-    ACTIONS(729), 1,
       sym__word,
-    ACTIONS(819), 1,
+    ACTIONS(825), 1,
       anon_sym_STAR,
-    STATE(235), 1,
+    STATE(192), 1,
       sym__regex,
-    STATE(325), 1,
+    STATE(348), 1,
       sym__regexes,
-  [1454] = 7,
-    ACTIONS(775), 1,
+  [1297] = 7,
+    ACTIONS(721), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(723), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(725), 1,
       anon_sym_BQUOTE,
-    ACTIONS(821), 1,
-      anon_sym_STAR,
-    STATE(429), 1,
-      sym_header_field,
-    STATE(444), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(727), 1,
       sym__word,
-  [1477] = 7,
-    ACTIONS(668), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(670), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(672), 1,
-      anon_sym_BQUOTE,
+    ACTIONS(827), 1,
+      anon_sym_STAR,
     STATE(192), 1,
-      sym_mailbox,
-    STATE(273), 1,
-      sym__string,
-    STATE(400), 1,
-      sym__mailboxes,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-  [1500] = 7,
-    ACTIONS(775), 1,
+      sym__regex,
+    STATE(345), 1,
+      sym__regexes,
+  [1319] = 7,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(247), 1,
+    ACTIONS(821), 1,
+      sym__word,
+    STATE(246), 1,
       sym_address,
-    STATE(290), 1,
+    STATE(251), 1,
       sym__string,
-    STATE(314), 1,
+    STATE(313), 1,
       sym__addresses,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [1523] = 6,
-    ACTIONS(775), 1,
+  [1341] = 7,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    STATE(432), 1,
-      sym_message,
-    STATE(433), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(689), 1,
       sym__word,
-  [1543] = 6,
-    ACTIONS(791), 1,
+    ACTIONS(829), 1,
+      anon_sym_STAR,
+    STATE(163), 1,
+      sym__string,
+    STATE(316), 1,
+      sym__strings,
+  [1363] = 7,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(793), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(795), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(145), 1,
+    ACTIONS(821), 1,
+      sym__word,
+    ACTIONS(831), 1,
+      anon_sym_STAR,
+    STATE(372), 1,
       sym_pattern,
-    STATE(204), 1,
+    STATE(391), 1,
       sym__string,
-    ACTIONS(797), 2,
-      anon_sym_LF,
-      sym__word,
-  [1563] = 6,
-    ACTIONS(668), 1,
+  [1385] = 7,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(273), 1,
-      sym__string,
-    STATE(289), 1,
-      sym_mailbox,
-    ACTIONS(674), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [1583] = 6,
-    ACTIONS(775), 1,
+    STATE(246), 1,
+      sym_address,
+    STATE(251), 1,
+      sym__string,
+    STATE(343), 1,
+      sym__addresses,
+  [1407] = 1,
+    ACTIONS(833), 7,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
       anon_sym_BQUOTE,
-    STATE(341), 1,
-      sym_format,
-    STATE(342), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
       sym__word,
-  [1603] = 6,
-    ACTIONS(765), 1,
-      anon_sym_LT,
-    ACTIONS(823), 1,
-      anon_sym_DASHgroup,
-    STATE(68), 1,
-      aux_sym_key_repeat1,
-    STATE(73), 1,
-      sym_key,
-    STATE(219), 1,
-      sym__group,
-    ACTIONS(825), 2,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [1623] = 6,
-    ACTIONS(827), 1,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [1417] = 7,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(829), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(831), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    STATE(152), 1,
-      sym__string,
-    STATE(165), 1,
-      sym_group_name,
-    ACTIONS(833), 2,
-      anon_sym_LF,
+    ACTIONS(689), 1,
       sym__word,
-  [1643] = 6,
-    ACTIONS(632), 1,
+    STATE(172), 1,
+      sym_mailbox,
+    STATE(302), 1,
+      sym__string,
+    STATE(427), 1,
+      sym__mailboxes,
+  [1439] = 7,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(634), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(636), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(18), 1,
-      sym__string,
-    STATE(479), 1,
-      sym_pattern,
-    ACTIONS(638), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [1663] = 6,
     ACTIONS(835), 1,
+      anon_sym_STAR,
+    STATE(405), 1,
+      sym_header_field,
+    STATE(444), 1,
+      sym__string,
+  [1461] = 7,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(837), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(839), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(350), 1,
-      sym__string,
-    STATE(358), 1,
-      sym_group_name,
-    ACTIONS(841), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [1683] = 6,
-    ACTIONS(632), 1,
+    ACTIONS(837), 1,
+      anon_sym_STAR,
+    STATE(391), 1,
+      sym__string,
+    STATE(424), 1,
+      sym_pattern,
+  [1483] = 7,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(634), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(636), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    STATE(360), 1,
-      sym__string,
-    STATE(362), 1,
-      sym_group_name,
-    ACTIONS(638), 2,
-      anon_sym_LF,
+    ACTIONS(689), 1,
       sym__word,
-  [1703] = 4,
-    ACTIONS(803), 1,
+    STATE(172), 1,
+      sym_mailbox,
+    STATE(302), 1,
+      sym__string,
+    STATE(341), 1,
+      sym__mailboxes,
+  [1505] = 4,
+    ACTIONS(839), 1,
       anon_sym_LT,
-    STATE(98), 1,
+    STATE(90), 1,
       aux_sym_key_repeat1,
-    ACTIONS(843), 2,
+    ACTIONS(842), 2,
       aux_sym_key_token2,
       aux_sym_key_token3,
-    ACTIONS(769), 3,
+    ACTIONS(779), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [1719] = 4,
-    ACTIONS(845), 1,
+  [1521] = 7,
+    ACTIONS(815), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(817), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(819), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(821), 1,
+      sym__word,
+    STATE(246), 1,
+      sym_address,
+    STATE(251), 1,
+      sym__string,
+    STATE(410), 1,
+      sym__addresses,
+  [1543] = 4,
+    ACTIONS(759), 1,
       anon_sym_LT,
-    STATE(98), 1,
+    STATE(90), 1,
       aux_sym_key_repeat1,
-    ACTIONS(848), 2,
+    ACTIONS(845), 2,
       aux_sym_key_token2,
       aux_sym_key_token3,
-    ACTIONS(755), 3,
+    ACTIONS(749), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [1735] = 6,
-    ACTIONS(791), 1,
+  [1559] = 1,
+    ACTIONS(847), 7,
+      anon_sym_LT,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
       anon_sym_SQUOTE,
-    ACTIONS(793), 1,
       anon_sym_DQUOTE,
-    ACTIONS(795), 1,
       anon_sym_BQUOTE,
-    STATE(193), 1,
-      sym__string,
-    STATE(194), 1,
-      sym_group_name,
-    ACTIONS(797), 2,
-      anon_sym_LF,
       sym__word,
-  [1755] = 6,
-    ACTIONS(775), 1,
+  [1569] = 7,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    STATE(415), 1,
-      sym_uri,
-    STATE(417), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(689), 1,
       sym__word,
-  [1775] = 6,
-    ACTIONS(851), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(853), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(855), 1,
-      anon_sym_BQUOTE,
-    STATE(276), 1,
+    STATE(195), 1,
+      sym_header,
+    STATE(287), 1,
       sym__string,
-    STATE(277), 1,
-      sym_group_name,
-    ACTIONS(857), 2,
-      anon_sym_LF,
-      sym__word,
-  [1795] = 6,
-    ACTIONS(775), 1,
+    STATE(412), 1,
+      sym__headers,
+  [1591] = 6,
+    ACTIONS(632), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(634), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(636), 1,
       anon_sym_BQUOTE,
-    STATE(417), 1,
-      sym__string,
-    STATE(418), 1,
-      sym_uri,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(638), 1,
       sym__word,
-  [1815] = 6,
-    ACTIONS(791), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(793), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(795), 1,
-      anon_sym_BQUOTE,
-    STATE(90), 1,
-      sym_description,
-    STATE(195), 1,
+    STATE(365), 1,
       sym__string,
-    ACTIONS(797), 2,
-      anon_sym_LF,
-      sym__word,
-  [1835] = 6,
-    ACTIONS(775), 1,
+    STATE(366), 1,
+      sym_group_name,
+  [1610] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(335), 1,
-      sym__string,
-    STATE(337), 1,
-      sym_shell_command,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [1855] = 6,
-    ACTIONS(775), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(777), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(779), 1,
-      anon_sym_BQUOTE,
-    STATE(335), 1,
+    STATE(330), 1,
+      sym_replacement,
+    STATE(331), 1,
       sym__string,
-    STATE(336), 1,
-      sym_shell_command,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [1875] = 7,
-    ACTIONS(721), 1,
+  [1629] = 2,
+    STATE(48), 1,
+      sym_attribute,
+    ACTIONS(644), 5,
+      anon_sym_bold,
+      anon_sym_underline,
+      anon_sym_none,
+      anon_sym_reverse,
+      anon_sym_standout,
+  [1640] = 6,
+    ACTIONS(169), 1,
+      sym_comment,
+    ACTIONS(173), 1,
+      aux_sym__space_token1,
+    ACTIONS(849), 1,
+      sym__eol,
+    STATE(20), 1,
+      sym__end,
+    STATE(285), 1,
+      aux_sym__space_repeat1,
+    STATE(452), 1,
+      sym__space,
+  [1659] = 6,
+    ACTIONS(799), 1,
       anon_sym_SQUOTE,
-    ACTIONS(723), 1,
+    ACTIONS(801), 1,
       anon_sym_DQUOTE,
-    ACTIONS(725), 1,
+    ACTIONS(803), 1,
       anon_sym_BQUOTE,
-    ACTIONS(727), 1,
-      anon_sym_LF,
-    ACTIONS(729), 1,
+    ACTIONS(805), 1,
       sym__word,
-    STATE(235), 1,
-      sym__regex,
-    STATE(332), 1,
-      sym__regexes,
-  [1897] = 7,
-    ACTIONS(859), 1,
-      anon_sym_STAR,
-    ACTIONS(861), 1,
+    STATE(139), 1,
+      sym_pattern,
+    STATE(272), 1,
+      sym__string,
+  [1678] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(863), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(865), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    ACTIONS(867), 1,
-      anon_sym_LF,
-    ACTIONS(869), 1,
+    ACTIONS(821), 1,
       sym__word,
-    STATE(422), 1,
-      sym__regex,
-  [1919] = 6,
-    ACTIONS(775), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(777), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(779), 1,
-      anon_sym_BQUOTE,
-    STATE(334), 1,
-      sym_shell_command,
-    STATE(335), 1,
+    STATE(251), 1,
       sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [1939] = 6,
-    ACTIONS(668), 1,
+    STATE(256), 1,
+      sym_address,
+  [1697] = 6,
+    ACTIONS(851), 1,
+      anon_sym_DASHgroup,
+    ACTIONS(853), 1,
+      anon_sym_STAR,
+    ACTIONS(855), 1,
+      anon_sym_DASHrx,
+    ACTIONS(857), 1,
+      anon_sym_DASHaddr,
+    STATE(293), 1,
+      sym__group,
+    STATE(401), 1,
+      sym__rx_addr,
+  [1716] = 6,
+    ACTIONS(859), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(672), 1,
-      anon_sym_BQUOTE,
-    STATE(258), 1,
-      sym_mailbox,
-    STATE(273), 1,
-      sym__string,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-  [1959] = 7,
     ACTIONS(861), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(863), 1,
       anon_sym_DQUOTE,
-    ACTIONS(865), 1,
+    ACTIONS(863), 1,
       anon_sym_BQUOTE,
-    ACTIONS(869), 1,
+    ACTIONS(865), 1,
       sym__word,
-    ACTIONS(871), 1,
-      anon_sym_STAR,
-    ACTIONS(873), 1,
-      anon_sym_LF,
-    STATE(425), 1,
-      sym__regex,
-  [1981] = 6,
-    ACTIONS(791), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(793), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(795), 1,
-      anon_sym_BQUOTE,
-    STATE(129), 1,
-      sym_alias,
-    STATE(253), 1,
+    STATE(413), 1,
       sym__string,
-    ACTIONS(797), 2,
-      anon_sym_LF,
-      sym__word,
-  [2001] = 6,
+    STATE(414), 1,
+      sym_group_name,
+  [1735] = 1,
+    ACTIONS(847), 6,
+      anon_sym_LT,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [1744] = 6,
     ACTIONS(632), 1,
       anon_sym_SQUOTE,
     ACTIONS(634), 1,
       anon_sym_DQUOTE,
     ACTIONS(636), 1,
       anon_sym_BQUOTE,
-    STATE(5), 1,
-      sym_pattern,
-    STATE(18), 1,
-      sym__string,
-    ACTIONS(638), 2,
-      anon_sym_LF,
+    ACTIONS(638), 1,
       sym__word,
-  [2021] = 6,
-    ACTIONS(775), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(777), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(779), 1,
-      anon_sym_BQUOTE,
-    STATE(290), 1,
+    STATE(8), 1,
+      sym_symbol,
+    STATE(23), 1,
       sym__string,
-    STATE(293), 1,
-      sym_address,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [2041] = 6,
+  [1763] = 6,
     ACTIONS(632), 1,
       anon_sym_SQUOTE,
     ACTIONS(634), 1,
       anon_sym_DQUOTE,
     ACTIONS(636), 1,
       anon_sym_BQUOTE,
-    STATE(6), 1,
-      sym_pattern,
-    STATE(18), 1,
-      sym__string,
-    ACTIONS(638), 2,
-      anon_sym_LF,
+    ACTIONS(638), 1,
       sym__word,
-  [2061] = 6,
-    ACTIONS(632), 1,
+    STATE(9), 1,
+      sym_symbol,
+    STATE(23), 1,
+      sym__string,
+  [1782] = 3,
+    ACTIONS(871), 1,
+      sym_option,
+    ACTIONS(867), 2,
+      anon_sym_QMARK,
+      anon_sym_AMP,
+    ACTIONS(869), 3,
+      anon_sym_PLUS_EQ,
+      anon_sym_DASH_EQ,
+      anon_sym_EQ,
+  [1795] = 5,
+    ACTIONS(759), 1,
+      anon_sym_LT,
+    ACTIONS(873), 1,
+      anon_sym_STAR,
+    STATE(92), 1,
+      aux_sym_key_repeat1,
+    STATE(406), 1,
+      sym_key,
+    ACTIONS(761), 2,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [1812] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(634), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(636), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(9), 1,
-      sym_pattern,
-    STATE(18), 1,
-      sym__string,
-    ACTIONS(638), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [2081] = 6,
-    ACTIONS(735), 1,
+    STATE(384), 1,
+      sym_mailbox,
+    STATE(445), 1,
+      sym__string,
+  [1831] = 6,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(737), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(739), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    STATE(460), 1,
-      sym_disposition,
-    STATE(490), 1,
-      sym__string,
-    ACTIONS(741), 2,
-      anon_sym_LF,
+    ACTIONS(689), 1,
       sym__word,
-  [2101] = 6,
-    ACTIONS(791), 1,
+    STATE(270), 1,
+      sym_header_field,
+    STATE(297), 1,
+      sym__string,
+  [1850] = 6,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(793), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(795), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    STATE(131), 1,
-      sym_charset,
-    STATE(261), 1,
-      sym__string,
-    ACTIONS(797), 2,
-      anon_sym_LF,
+    ACTIONS(689), 1,
       sym__word,
-  [2121] = 6,
-    ACTIONS(827), 1,
+    STATE(273), 1,
+      sym_mailbox,
+    STATE(302), 1,
+      sym__string,
+  [1869] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(829), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(831), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(70), 1,
-      sym_pattern,
-    STATE(154), 1,
-      sym__string,
-    ACTIONS(833), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [2141] = 7,
+    STATE(376), 1,
+      sym_sequence,
+    STATE(377), 1,
+      sym__string,
+  [1888] = 6,
     ACTIONS(721), 1,
       anon_sym_SQUOTE,
     ACTIONS(723), 1,
       anon_sym_DQUOTE,
     ACTIONS(725), 1,
       anon_sym_BQUOTE,
     ACTIONS(727), 1,
-      anon_sym_LF,
-    ACTIONS(729), 1,
       sym__word,
-    STATE(235), 1,
+    STATE(192), 1,
       sym__regex,
-    STATE(323), 1,
+    STATE(400), 1,
       sym__regexes,
-  [2163] = 6,
-    ACTIONS(875), 1,
+  [1907] = 6,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(877), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(879), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    STATE(77), 1,
-      sym_name,
-    STATE(153), 1,
-      sym__string,
-    ACTIONS(881), 2,
-      anon_sym_LF,
+    ACTIONS(689), 1,
       sym__word,
-  [2183] = 6,
-    ACTIONS(735), 1,
+    STATE(277), 1,
+      sym_header,
+    STATE(287), 1,
+      sym__string,
+  [1926] = 6,
+    ACTIONS(875), 1,
+      anon_sym_DASHnoregex,
+    ACTIONS(877), 1,
       anon_sym_SQUOTE,
-    ACTIONS(737), 1,
+    ACTIONS(879), 1,
       anon_sym_DQUOTE,
-    ACTIONS(739), 1,
+    ACTIONS(881), 1,
       anon_sym_BQUOTE,
-    STATE(462), 1,
-      sym_disposition,
-    STATE(490), 1,
-      sym__string,
-    ACTIONS(741), 2,
-      anon_sym_LF,
+    ACTIONS(883), 1,
       sym__word,
-  [2203] = 6,
-    ACTIONS(775), 1,
+    STATE(10), 1,
+      sym__regex,
+  [1945] = 6,
+    ACTIONS(799), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(801), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(803), 1,
       anon_sym_BQUOTE,
-    STATE(384), 1,
-      sym_mailbox,
-    STATE(445), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(805), 1,
       sym__word,
-  [2223] = 6,
-    ACTIONS(668), 1,
+    STATE(204), 1,
+      sym_pattern,
+    STATE(272), 1,
+      sym__string,
+  [1964] = 6,
+    ACTIONS(799), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(801), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(803), 1,
       anon_sym_BQUOTE,
-    STATE(275), 1,
-      sym__string,
-    STATE(305), 1,
-      sym_header_field,
-    ACTIONS(674), 2,
-      anon_sym_LF,
+    ACTIONS(805), 1,
       sym__word,
-  [2243] = 6,
-    ACTIONS(668), 1,
+    STATE(150), 1,
+      sym_description,
+    STATE(300), 1,
+      sym__string,
+  [1983] = 6,
+    ACTIONS(733), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(735), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(737), 1,
       anon_sym_BQUOTE,
-    STATE(273), 1,
-      sym__string,
-    STATE(301), 1,
-      sym_mailbox,
-    ACTIONS(674), 2,
-      anon_sym_LF,
+    ACTIONS(739), 1,
       sym__word,
-  [2263] = 6,
-    ACTIONS(775), 1,
+    STATE(460), 1,
+      sym_disposition,
+    STATE(480), 1,
+      sym__string,
+  [2002] = 6,
+    ACTIONS(885), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(887), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(889), 1,
       anon_sym_BQUOTE,
-    STATE(378), 1,
-      sym_sequence,
-    STATE(379), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(891), 1,
       sym__word,
-  [2283] = 7,
-    ACTIONS(721), 1,
+    STATE(184), 1,
+      sym__string,
+    STATE(185), 1,
+      sym_group_name,
+  [2021] = 6,
+    ACTIONS(799), 1,
       anon_sym_SQUOTE,
-    ACTIONS(723), 1,
+    ACTIONS(801), 1,
       anon_sym_DQUOTE,
-    ACTIONS(725), 1,
+    ACTIONS(803), 1,
       anon_sym_BQUOTE,
-    ACTIONS(727), 1,
-      anon_sym_LF,
-    ACTIONS(729), 1,
+    ACTIONS(805), 1,
       sym__word,
-    STATE(235), 1,
-      sym__regex,
-    STATE(320), 1,
-      sym__regexes,
-  [2305] = 6,
-    ACTIONS(668), 1,
+    STATE(138), 1,
+      sym_pattern,
+    STATE(272), 1,
+      sym__string,
+  [2040] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(278), 1,
-      sym__string,
-    STATE(309), 1,
-      sym_header,
-    ACTIONS(674), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [2325] = 6,
-    ACTIONS(775), 1,
+    STATE(328), 1,
+      sym_format,
+    STATE(329), 1,
+      sym__string,
+  [2059] = 6,
+    ACTIONS(733), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(735), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(737), 1,
       anon_sym_BQUOTE,
-    STATE(343), 1,
-      sym_replacement,
-    STATE(344), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(739), 1,
       sym__word,
-  [2345] = 6,
-    ACTIONS(775), 1,
+    STATE(461), 1,
+      sym_disposition,
+    STATE(480), 1,
+      sym__string,
+  [2078] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(441), 1,
-      sym_charset,
-    STATE(447), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [2365] = 6,
-    ACTIONS(775), 1,
+    STATE(364), 1,
+      sym_message,
+    STATE(378), 1,
+      sym__string,
+  [2097] = 6,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    STATE(330), 1,
+    ACTIONS(689), 1,
+      sym__word,
+    STATE(257), 1,
       sym_mailbox,
-    STATE(445), 1,
+    STATE(302), 1,
       sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [2385] = 6,
-    ACTIONS(775), 1,
+  [2116] = 6,
+    ACTIONS(799), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(801), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(803), 1,
       anon_sym_BQUOTE,
-    STATE(440), 1,
-      sym_charset,
-    STATE(447), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(805), 1,
       sym__word,
-  [2405] = 6,
-    ACTIONS(791), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(793), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(795), 1,
-      anon_sym_BQUOTE,
-    STATE(178), 1,
+    STATE(137), 1,
       sym_pattern,
-    STATE(204), 1,
+    STATE(272), 1,
       sym__string,
-    ACTIONS(797), 2,
-      anon_sym_LF,
-      sym__word,
-  [2425] = 6,
-    ACTIONS(791), 1,
+  [2135] = 6,
+    ACTIONS(893), 1,
       anon_sym_SQUOTE,
-    ACTIONS(793), 1,
+    ACTIONS(895), 1,
       anon_sym_DQUOTE,
-    ACTIONS(795), 1,
+    ACTIONS(897), 1,
       anon_sym_BQUOTE,
-    STATE(143), 1,
-      sym_pattern,
-    STATE(204), 1,
-      sym__string,
-    ACTIONS(797), 2,
-      anon_sym_LF,
+    ACTIONS(899), 1,
       sym__word,
-  [2445] = 6,
-    ACTIONS(791), 1,
+    STATE(74), 1,
+      sym_name,
+    STATE(167), 1,
+      sym__string,
+  [2154] = 6,
+    ACTIONS(885), 1,
       anon_sym_SQUOTE,
-    ACTIONS(793), 1,
+    ACTIONS(887), 1,
       anon_sym_DQUOTE,
-    ACTIONS(795), 1,
+    ACTIONS(889), 1,
       anon_sym_BQUOTE,
-    STATE(144), 1,
+    ACTIONS(891), 1,
+      sym__word,
+    STATE(83), 1,
       sym_pattern,
-    STATE(204), 1,
+    STATE(200), 1,
       sym__string,
-    ACTIONS(797), 2,
-      anon_sym_LF,
-      sym__word,
-  [2465] = 7,
-    ACTIONS(883), 1,
-      anon_sym_DASHnoregex,
+  [2173] = 6,
     ACTIONS(885), 1,
       anon_sym_SQUOTE,
     ACTIONS(887), 1,
       anon_sym_DQUOTE,
     ACTIONS(889), 1,
       anon_sym_BQUOTE,
     ACTIONS(891), 1,
-      anon_sym_LF,
-    ACTIONS(893), 1,
       sym__word,
-    STATE(7), 1,
-      sym__regex,
-  [2487] = 6,
-    ACTIONS(827), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(829), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(831), 1,
-      anon_sym_BQUOTE,
-    STATE(83), 1,
+    STATE(77), 1,
       sym_pattern,
-    STATE(154), 1,
+    STATE(200), 1,
       sym__string,
-    ACTIONS(833), 2,
-      anon_sym_LF,
-      sym__word,
-  [2507] = 6,
+  [2192] = 6,
     ACTIONS(632), 1,
       anon_sym_SQUOTE,
     ACTIONS(634), 1,
       anon_sym_DQUOTE,
     ACTIONS(636), 1,
       anon_sym_BQUOTE,
-    STATE(14), 1,
-      sym_symbol,
-    STATE(22), 1,
-      sym__string,
-    ACTIONS(638), 2,
-      anon_sym_LF,
+    ACTIONS(638), 1,
       sym__word,
-  [2527] = 6,
-    ACTIONS(775), 1,
+    STATE(18), 1,
+      sym__string,
+    STATE(466), 1,
+      sym_pattern,
+  [2211] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(411), 1,
-      sym__string,
-    STATE(414), 1,
-      sym_keyid,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [2547] = 6,
-    ACTIONS(632), 1,
+    STATE(383), 1,
+      sym_charset,
+    STATE(447), 1,
+      sym__string,
+  [2230] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(634), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(636), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(4), 1,
-      sym_pattern,
-    STATE(18), 1,
-      sym__string,
-    ACTIONS(638), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [2567] = 6,
-    ACTIONS(632), 1,
+    STATE(382), 1,
+      sym_charset,
+    STATE(447), 1,
+      sym__string,
+  [2249] = 2,
+    STATE(28), 1,
+      sym_composeobject,
+    ACTIONS(901), 5,
+      anon_sym_header,
+      anon_sym_security_encrypt,
+      anon_sym_security_sign,
+      anon_sym_security_both,
+      anon_sym_security_none,
+  [2260] = 6,
+    ACTIONS(799), 1,
       anon_sym_SQUOTE,
-    ACTIONS(634), 1,
+    ACTIONS(801), 1,
       anon_sym_DQUOTE,
-    ACTIONS(636), 1,
+    ACTIONS(803), 1,
       anon_sym_BQUOTE,
-    STATE(15), 1,
-      sym_symbol,
-    STATE(22), 1,
-      sym__string,
-    ACTIONS(638), 2,
-      anon_sym_LF,
+    ACTIONS(805), 1,
       sym__word,
-  [2587] = 7,
-    ACTIONS(895), 1,
-      anon_sym_DASHnoregex,
-    ACTIONS(897), 1,
+    STATE(130), 1,
+      sym_charset,
+    STATE(284), 1,
+      sym__string,
+  [2279] = 6,
+    ACTIONS(799), 1,
       anon_sym_SQUOTE,
-    ACTIONS(899), 1,
+    ACTIONS(801), 1,
       anon_sym_DQUOTE,
-    ACTIONS(901), 1,
+    ACTIONS(803), 1,
       anon_sym_BQUOTE,
-    ACTIONS(903), 1,
-      anon_sym_LF,
-    ACTIONS(905), 1,
+    ACTIONS(805), 1,
       sym__word,
-    STATE(130), 1,
-      sym__regex,
-  [2609] = 6,
-    ACTIONS(775), 1,
+    STATE(129), 1,
+      sym_alias,
+    STATE(286), 1,
+      sym__string,
+  [2298] = 6,
+    ACTIONS(799), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(801), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(803), 1,
       anon_sym_BQUOTE,
-    STATE(434), 1,
-      sym_directory,
-    STATE(437), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(805), 1,
       sym__word,
-  [2629] = 6,
-    ACTIONS(775), 1,
+    STATE(123), 1,
+      sym_description,
+    STATE(300), 1,
+      sym__string,
+  [2317] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(396), 1,
-      sym_mailbox,
-    STATE(445), 1,
+    ACTIONS(821), 1,
+      sym__word,
+    STATE(369), 1,
       sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    STATE(370), 1,
+      sym_keyid,
+  [2336] = 6,
+    ACTIONS(632), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(634), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(636), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(638), 1,
       sym__word,
-  [2649] = 6,
-    ACTIONS(775), 1,
+    STATE(7), 1,
+      sym_pattern,
+    STATE(18), 1,
+      sym__string,
+  [2355] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(392), 1,
+    ACTIONS(821), 1,
+      sym__word,
+    STATE(361), 1,
       sym_mailbox,
     STATE(445), 1,
       sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [2669] = 6,
-    ACTIONS(775), 1,
+  [2374] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(438), 1,
+    ACTIONS(821), 1,
+      sym__word,
+    STATE(358), 1,
       sym_mailbox,
     STATE(445), 1,
       sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [2689] = 6,
-    ACTIONS(668), 1,
+  [2393] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(670), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(672), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(187), 1,
-      sym__string,
-    STATE(363), 1,
-      sym__strings,
-    ACTIONS(674), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [2709] = 6,
-    ACTIONS(791), 1,
+    STATE(357), 1,
+      sym_mailbox,
+    STATE(445), 1,
+      sym__string,
+  [2412] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(793), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(795), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(109), 1,
-      sym_description,
-    STATE(195), 1,
-      sym__string,
-    ACTIONS(797), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [2729] = 7,
+    STATE(443), 1,
+      sym__string,
+    STATE(448), 1,
+      sym_uri,
+  [2431] = 6,
     ACTIONS(721), 1,
       anon_sym_SQUOTE,
     ACTIONS(723), 1,
       anon_sym_DQUOTE,
     ACTIONS(725), 1,
       anon_sym_BQUOTE,
     ACTIONS(727), 1,
-      anon_sym_LF,
-    ACTIONS(729), 1,
       sym__word,
-    STATE(235), 1,
+    STATE(192), 1,
       sym__regex,
-    STATE(313), 1,
+    STATE(312), 1,
       sym__regexes,
-  [2751] = 6,
-    ACTIONS(897), 1,
+  [2450] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(899), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(901), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    ACTIONS(905), 1,
+    ACTIONS(821), 1,
       sym__word,
-    ACTIONS(907), 1,
-      anon_sym_LF,
-    STATE(105), 1,
-      sym__regex,
-  [2770] = 5,
-    ACTIONS(668), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(670), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(672), 1,
-      anon_sym_BQUOTE,
-    STATE(303), 1,
+    STATE(438), 1,
+      sym_uri,
+    STATE(443), 1,
       sym__string,
-    ACTIONS(674), 2,
-      anon_sym_LF,
-      sym__word,
-  [2787] = 6,
-    ACTIONS(885), 1,
+  [2469] = 6,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
-    ACTIONS(887), 1,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
-    ACTIONS(889), 1,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-    ACTIONS(893), 1,
+    ACTIONS(689), 1,
       sym__word,
-    ACTIONS(909), 1,
-      anon_sym_LF,
-    STATE(10), 1,
-      sym__regex,
-  [2806] = 1,
-    ACTIONS(911), 6,
-      anon_sym_STAR,
-      anon_sym_SQUOTE,
-      anon_sym_DQUOTE,
-      anon_sym_BQUOTE,
-      anon_sym_LF,
-      sym__word,
-  [2815] = 1,
-    ACTIONS(913), 6,
-      anon_sym_BANG,
-      anon_sym_SQUOTE,
-      anon_sym_DQUOTE,
-      anon_sym_BQUOTE,
-      anon_sym_LF,
-      sym__word,
-  [2824] = 1,
-    ACTIONS(602), 6,
-      anon_sym_STAR,
+    STATE(163), 1,
+      sym__string,
+    STATE(394), 1,
+      sym__strings,
+  [2488] = 6,
+    ACTIONS(903), 1,
       anon_sym_SQUOTE,
+    ACTIONS(905), 1,
       anon_sym_DQUOTE,
+    ACTIONS(907), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
+    ACTIONS(909), 1,
       sym__word,
-  [2833] = 6,
-    ACTIONS(915), 1,
-      anon_sym_DASHgroup,
-    ACTIONS(917), 1,
-      anon_sym_STAR,
-    ACTIONS(919), 1,
-      anon_sym_DASHrx,
-    ACTIONS(921), 1,
-      anon_sym_DASHaddr,
-    STATE(285), 1,
-      sym__group,
-    STATE(311), 1,
-      sym__rx_addr,
-  [2852] = 1,
-    ACTIONS(594), 6,
-      anon_sym_STAR,
+    STATE(276), 1,
+      sym_group_name,
+    STATE(278), 1,
+      sym__string,
+  [2507] = 6,
+    ACTIONS(799), 1,
       anon_sym_SQUOTE,
+    ACTIONS(801), 1,
       anon_sym_DQUOTE,
+    ACTIONS(803), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
+    ACTIONS(805), 1,
       sym__word,
-  [2861] = 6,
+    STATE(289), 1,
+      sym_group_name,
+    STATE(290), 1,
+      sym__string,
+  [2526] = 6,
     ACTIONS(721), 1,
       anon_sym_SQUOTE,
     ACTIONS(723), 1,
       anon_sym_DQUOTE,
     ACTIONS(725), 1,
       anon_sym_BQUOTE,
-    ACTIONS(729), 1,
+    ACTIONS(727), 1,
       sym__word,
-    ACTIONS(923), 1,
-      anon_sym_LF,
-    STATE(308), 1,
+    STATE(192), 1,
       sym__regex,
-  [2880] = 5,
-    ACTIONS(775), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(777), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(779), 1,
-      anon_sym_BQUOTE,
-    STATE(430), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [2897] = 6,
-    ACTIONS(169), 1,
-      sym_comment,
-    ACTIONS(173), 1,
-      aux_sym__space_token1,
-    ACTIONS(925), 1,
-      sym__eol,
-    STATE(19), 1,
-      sym__end,
-    STATE(288), 1,
-      aux_sym__space_repeat1,
-    STATE(459), 1,
-      sym__space,
-  [2916] = 6,
-    ACTIONS(897), 1,
+    STATE(337), 1,
+      sym__regexes,
+  [2545] = 6,
+    ACTIONS(785), 1,
       anon_sym_SQUOTE,
-    ACTIONS(899), 1,
+    ACTIONS(787), 1,
       anon_sym_DQUOTE,
-    ACTIONS(901), 1,
+    ACTIONS(789), 1,
       anon_sym_BQUOTE,
-    ACTIONS(905), 1,
+    ACTIONS(791), 1,
       sym__word,
-    ACTIONS(927), 1,
-      anon_sym_LF,
-    STATE(108), 1,
+    ACTIONS(911), 1,
+      anon_sym_STAR,
+    STATE(430), 1,
       sym__regex,
-  [2935] = 2,
-    STATE(28), 1,
-      sym_composeobject,
-    ACTIONS(929), 5,
-      anon_sym_header,
-      anon_sym_security_encrypt,
-      anon_sym_security_sign,
-      anon_sym_security_both,
-      anon_sym_security_none,
-  [2946] = 6,
-    ACTIONS(897), 1,
+  [2564] = 6,
+    ACTIONS(721), 1,
       anon_sym_SQUOTE,
-    ACTIONS(899), 1,
+    ACTIONS(723), 1,
       anon_sym_DQUOTE,
-    ACTIONS(901), 1,
+    ACTIONS(725), 1,
       anon_sym_BQUOTE,
-    ACTIONS(905), 1,
+    ACTIONS(727), 1,
       sym__word,
-    ACTIONS(931), 1,
-      anon_sym_LF,
-    STATE(122), 1,
+    STATE(192), 1,
       sym__regex,
-  [2965] = 5,
-    ACTIONS(775), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(777), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(779), 1,
-      anon_sym_BQUOTE,
-    STATE(373), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [2982] = 1,
-    ACTIONS(598), 6,
-      anon_sym_BANG,
-      anon_sym_SQUOTE,
-      anon_sym_DQUOTE,
-      anon_sym_BQUOTE,
-      anon_sym_LF,
-      sym__word,
-  [2991] = 1,
-    ACTIONS(933), 6,
-      anon_sym_STAR,
+    STATE(346), 1,
+      sym__regexes,
+  [2583] = 6,
+    ACTIONS(785), 1,
       anon_sym_SQUOTE,
+    ACTIONS(787), 1,
       anon_sym_DQUOTE,
+    ACTIONS(789), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
+    ACTIONS(791), 1,
       sym__word,
-  [3000] = 1,
-    ACTIONS(598), 6,
+    ACTIONS(913), 1,
       anon_sym_STAR,
+    STATE(421), 1,
+      sym__regex,
+  [2602] = 6,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
-      sym__word,
-  [3009] = 6,
-    ACTIONS(861), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(863), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(865), 1,
-      anon_sym_BQUOTE,
-    ACTIONS(869), 1,
+    ACTIONS(689), 1,
       sym__word,
-    ACTIONS(935), 1,
-      anon_sym_LF,
-    STATE(385), 1,
-      sym__regex,
-  [3028] = 3,
-    ACTIONS(941), 1,
-      sym_option,
-    ACTIONS(937), 2,
-      anon_sym_QMARK,
-      anon_sym_AMP,
-    ACTIONS(939), 3,
-      anon_sym_PLUS_EQ,
-      anon_sym_DASH_EQ,
-      anon_sym_EQ,
-  [3041] = 6,
-    ACTIONS(897), 1,
+    STATE(178), 1,
+      sym_mailbox,
+    STATE(302), 1,
+      sym__string,
+  [2621] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(899), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(901), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    ACTIONS(905), 1,
+    ACTIONS(821), 1,
       sym__word,
-    ACTIONS(943), 1,
-      anon_sym_LF,
-    STATE(138), 1,
-      sym__regex,
-  [3060] = 6,
-    ACTIONS(897), 1,
+    STATE(317), 1,
+      sym_mailbox,
+    STATE(445), 1,
+      sym__string,
+  [2640] = 6,
+    ACTIONS(632), 1,
       anon_sym_SQUOTE,
-    ACTIONS(899), 1,
+    ACTIONS(634), 1,
       anon_sym_DQUOTE,
-    ACTIONS(901), 1,
+    ACTIONS(636), 1,
       anon_sym_BQUOTE,
-    ACTIONS(905), 1,
+    ACTIONS(638), 1,
       sym__word,
-    ACTIONS(945), 1,
-      anon_sym_LF,
-    STATE(104), 1,
-      sym__regex,
-  [3079] = 2,
-    STATE(167), 1,
+    STATE(4), 1,
+      sym_pattern,
+    STATE(18), 1,
+      sym__string,
+  [2659] = 2,
+    STATE(176), 1,
       sym_attribute,
-    ACTIONS(947), 5,
+    ACTIONS(915), 5,
       anon_sym_bold,
       anon_sym_underline,
       anon_sym_none,
       anon_sym_reverse,
       anon_sym_standout,
-  [3090] = 5,
-    ACTIONS(775), 1,
+  [2670] = 6,
+    ACTIONS(632), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(634), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(636), 1,
       anon_sym_BQUOTE,
-    STATE(428), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(638), 1,
       sym__word,
-  [3107] = 6,
-    ACTIONS(897), 1,
+    STATE(5), 1,
+      sym_pattern,
+    STATE(18), 1,
+      sym__string,
+  [2689] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(899), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(901), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    ACTIONS(905), 1,
+    ACTIONS(821), 1,
       sym__word,
-    ACTIONS(949), 1,
-      anon_sym_LF,
-    STATE(91), 1,
-      sym__regex,
-  [3126] = 1,
-    ACTIONS(594), 6,
-      anon_sym_BANG,
+    STATE(321), 1,
+      sym_shell_command,
+    STATE(322), 1,
+      sym__string,
+  [2708] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [3135] = 2,
-    STATE(54), 1,
-      sym_attribute,
-    ACTIONS(644), 5,
-      anon_sym_bold,
-      anon_sym_underline,
-      anon_sym_none,
-      anon_sym_reverse,
-      anon_sym_standout,
-  [3146] = 6,
-    ACTIONS(897), 1,
+    STATE(322), 1,
+      sym__string,
+    STATE(323), 1,
+      sym_shell_command,
+  [2727] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(899), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(901), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    ACTIONS(905), 1,
+    ACTIONS(821), 1,
       sym__word,
-    ACTIONS(951), 1,
-      anon_sym_LF,
-    STATE(128), 1,
-      sym__regex,
-  [3165] = 6,
-    ACTIONS(861), 1,
+    STATE(322), 1,
+      sym__string,
+    STATE(324), 1,
+      sym_shell_command,
+  [2746] = 6,
+    ACTIONS(917), 1,
+      anon_sym_DASHnoregex,
+    ACTIONS(919), 1,
       anon_sym_SQUOTE,
-    ACTIONS(863), 1,
+    ACTIONS(921), 1,
       anon_sym_DQUOTE,
-    ACTIONS(865), 1,
+    ACTIONS(923), 1,
       anon_sym_BQUOTE,
-    ACTIONS(869), 1,
+    ACTIONS(925), 1,
       sym__word,
-    ACTIONS(953), 1,
-      anon_sym_LF,
-    STATE(407), 1,
+    STATE(151), 1,
       sym__regex,
-  [3184] = 5,
-    ACTIONS(775), 1,
+  [2765] = 6,
+    ACTIONS(815), 1,
       anon_sym_SQUOTE,
-    ACTIONS(777), 1,
+    ACTIONS(817), 1,
       anon_sym_DQUOTE,
-    ACTIONS(779), 1,
+    ACTIONS(819), 1,
       anon_sym_BQUOTE,
-    STATE(408), 1,
-      sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
+    ACTIONS(821), 1,
       sym__word,
-  [3201] = 5,
-    ACTIONS(803), 1,
-      anon_sym_LT,
-    ACTIONS(955), 1,
-      anon_sym_STAR,
-    STATE(97), 1,
-      aux_sym_key_repeat1,
-    STATE(390), 1,
-      sym_key,
-    ACTIONS(805), 2,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [3218] = 1,
-    ACTIONS(787), 6,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [3227] = 5,
-    ACTIONS(775), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(777), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(779), 1,
-      anon_sym_BQUOTE,
-    STATE(370), 1,
+    STATE(388), 1,
+      sym_directory,
+    STATE(389), 1,
       sym__string,
-    ACTIONS(781), 2,
-      anon_sym_LF,
-      sym__word,
-  [3244] = 5,
+  [2784] = 6,
     ACTIONS(632), 1,
       anon_sym_SQUOTE,
     ACTIONS(634), 1,
       anon_sym_DQUOTE,
     ACTIONS(636), 1,
       anon_sym_BQUOTE,
-    STATE(8), 1,
-      sym__string,
-    ACTIONS(638), 2,
-      anon_sym_LF,
+    ACTIONS(638), 1,
       sym__word,
-  [3261] = 6,
-    ACTIONS(861), 1,
-      anon_sym_SQUOTE,
-    ACTIONS(863), 1,
-      anon_sym_DQUOTE,
-    ACTIONS(865), 1,
-      anon_sym_BQUOTE,
-    ACTIONS(869), 1,
-      sym__word,
-    ACTIONS(957), 1,
-      anon_sym_LF,
-    STATE(420), 1,
-      sym__regex,
-  [3280] = 3,
-    ACTIONS(959), 1,
+    STATE(6), 1,
+      sym_pattern,
+    STATE(18), 1,
+      sym__string,
+  [2803] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
-    STATE(206), 1,
+    STATE(223), 1,
       aux_sym__options3_repeat1,
-    ACTIONS(961), 3,
+    ACTIONS(929), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3292] = 4,
-    ACTIONS(963), 1,
-      anon_sym_LT,
-    STATE(197), 1,
-      aux_sym_key_repeat1,
-    STATE(484), 1,
-      sym_key,
-    ACTIONS(965), 2,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [3306] = 5,
-    ACTIONS(915), 1,
-      anon_sym_DASHgroup,
-    ACTIONS(919), 1,
-      anon_sym_DASHrx,
-    ACTIONS(921), 1,
-      anon_sym_DASHaddr,
-    STATE(427), 1,
-      sym__group,
-    STATE(435), 1,
-      sym__rx_addr,
-  [3322] = 3,
-    ACTIONS(967), 1,
+  [2815] = 3,
+    ACTIONS(931), 1,
       anon_sym_SPACE,
-    STATE(249), 1,
+    STATE(162), 1,
       aux_sym__strings_repeat1,
-    ACTIONS(969), 3,
+    ACTIONS(934), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3334] = 1,
-    ACTIONS(594), 5,
+  [2827] = 3,
+    ACTIONS(936), 1,
+      anon_sym_SPACE,
+    STATE(188), 1,
+      aux_sym__strings_repeat1,
+    ACTIONS(938), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [2839] = 3,
+    ACTIONS(940), 1,
+      anon_sym_SPACE,
+    STATE(164), 1,
+      aux_sym__regexes_repeat1,
+    ACTIONS(943), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [2851] = 3,
+    ACTIONS(945), 1,
+      anon_sym_COMMA,
+    STATE(243), 1,
+      aux_sym__addresses_repeat1,
+    ACTIONS(947), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [2863] = 5,
+    ACTIONS(877), 1,
       anon_sym_SQUOTE,
+    ACTIONS(879), 1,
       anon_sym_DQUOTE,
+    ACTIONS(881), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
+    ACTIONS(883), 1,
       sym__word,
-  [3342] = 4,
-    ACTIONS(755), 1,
-      sym_function,
-    ACTIONS(971), 1,
+    STATE(15), 1,
+      sym__regex,
+  [2879] = 1,
+    ACTIONS(949), 5,
+      anon_sym_BANG,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [2887] = 3,
+    ACTIONS(951), 1,
+      anon_sym_SPACE,
+    STATE(201), 1,
+      aux_sym__functions_repeat1,
+    ACTIONS(953), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [2899] = 4,
+    ACTIONS(745), 1,
       anon_sym_LT,
-    STATE(189), 1,
+    STATE(62), 1,
       aux_sym_key_repeat1,
-    ACTIONS(974), 2,
+    STATE(84), 1,
+      sym_key,
+    ACTIONS(811), 2,
       aux_sym_key_token2,
       aux_sym_key_token3,
-  [3356] = 4,
-    ACTIONS(765), 1,
+  [2913] = 4,
+    ACTIONS(745), 1,
       anon_sym_LT,
-    STATE(68), 1,
+    STATE(62), 1,
       aux_sym_key_repeat1,
-    STATE(125), 1,
+    STATE(111), 1,
       sym_key,
-    ACTIONS(825), 2,
+    ACTIONS(811), 2,
       aux_sym_key_token2,
       aux_sym_key_token3,
-  [3370] = 4,
-    ACTIONS(803), 1,
+  [2927] = 4,
+    ACTIONS(759), 1,
       anon_sym_LT,
-    STATE(97), 1,
+    STATE(92), 1,
       aux_sym_key_repeat1,
-    STATE(326), 1,
+    STATE(350), 1,
       sym_key,
-    ACTIONS(805), 2,
+    ACTIONS(761), 2,
       aux_sym_key_token2,
       aux_sym_key_token3,
-  [3384] = 3,
-    ACTIONS(977), 1,
+  [2941] = 3,
+    ACTIONS(955), 1,
       anon_sym_SPACE,
-    STATE(257), 1,
+    STATE(180), 1,
       aux_sym__mailboxes_repeat1,
-    ACTIONS(979), 3,
+    ACTIONS(957), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [2953] = 3,
+    ACTIONS(959), 1,
+      anon_sym_SPACE,
+    STATE(234), 1,
+      aux_sym__options_repeat1,
+    ACTIONS(961), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [2965] = 3,
+    ACTIONS(963), 1,
+      anon_sym_SPACE,
+    STATE(226), 1,
+      aux_sym__options2_repeat1,
+    ACTIONS(965), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [2977] = 3,
+    ACTIONS(963), 1,
+      anon_sym_SPACE,
+    STATE(212), 1,
+      aux_sym__options2_repeat1,
+    ACTIONS(965), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3396] = 1,
-    ACTIONS(911), 5,
+  [2989] = 5,
+    ACTIONS(785), 1,
       anon_sym_SQUOTE,
+    ACTIONS(787), 1,
       anon_sym_DQUOTE,
+    ACTIONS(789), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
+    ACTIONS(791), 1,
       sym__word,
-  [3404] = 1,
-    ACTIONS(933), 5,
+    STATE(385), 1,
+      sym__regex,
+  [3005] = 3,
+    ACTIONS(967), 1,
+      anon_sym_SPACE,
+    STATE(211), 1,
+      aux_sym__header_fields_repeat1,
+    ACTIONS(969), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [3017] = 3,
+    ACTIONS(971), 1,
+      anon_sym_SPACE,
+    STATE(210), 1,
+      aux_sym_named_mailboxes_directive_repeat1,
+    ACTIONS(973), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [3029] = 3,
+    ACTIONS(967), 1,
+      anon_sym_SPACE,
+    STATE(177), 1,
+      aux_sym__header_fields_repeat1,
+    ACTIONS(975), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [3041] = 3,
+    ACTIONS(955), 1,
+      anon_sym_SPACE,
+    STATE(209), 1,
+      aux_sym__mailboxes_repeat1,
+    ACTIONS(977), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [3053] = 1,
+    ACTIONS(598), 5,
+      anon_sym_BANG,
       anon_sym_SQUOTE,
       anon_sym_DQUOTE,
       anon_sym_BQUOTE,
-      anon_sym_LF,
       sym__word,
-  [3412] = 1,
-    ACTIONS(981), 5,
+  [3061] = 1,
+    ACTIONS(594), 5,
+      anon_sym_BANG,
       anon_sym_SQUOTE,
       anon_sym_DQUOTE,
       anon_sym_BQUOTE,
-      anon_sym_LF,
       sym__word,
-  [3420] = 4,
-    ACTIONS(985), 1,
-      sym_option,
-    STATE(395), 1,
-      sym__options2,
-    STATE(397), 1,
-      sym__options3,
-    ACTIONS(983), 2,
-      anon_sym_QMARK,
-      anon_sym_AMP,
-  [3434] = 4,
-    ACTIONS(769), 1,
-      sym_function,
-    ACTIONS(963), 1,
-      anon_sym_LT,
-    STATE(189), 1,
-      aux_sym_key_repeat1,
-    ACTIONS(987), 2,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [3448] = 3,
-    ACTIONS(989), 1,
-      anon_sym_SPACE,
-    STATE(246), 1,
-      aux_sym__header_fields_repeat1,
-    ACTIONS(991), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [3460] = 1,
+  [3069] = 1,
     ACTIONS(598), 5,
+      anon_sym_STAR,
       anon_sym_SQUOTE,
       anon_sym_DQUOTE,
       anon_sym_BQUOTE,
-      anon_sym_LF,
       sym__word,
-  [3468] = 1,
-    ACTIONS(628), 5,
+  [3077] = 1,
+    ACTIONS(979), 5,
+      anon_sym_STAR,
       anon_sym_SQUOTE,
       anon_sym_DQUOTE,
       anon_sym_BQUOTE,
-      anon_sym_LF,
       sym__word,
-  [3476] = 1,
-    ACTIONS(624), 5,
+  [3085] = 1,
+    ACTIONS(981), 5,
+      anon_sym_STAR,
       anon_sym_SQUOTE,
       anon_sym_DQUOTE,
       anon_sym_BQUOTE,
-      anon_sym_LF,
       sym__word,
-  [3484] = 1,
-    ACTIONS(993), 5,
+  [3093] = 5,
+    ACTIONS(919), 1,
       anon_sym_SQUOTE,
+    ACTIONS(921), 1,
       anon_sym_DQUOTE,
+    ACTIONS(923), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
+    ACTIONS(925), 1,
       sym__word,
-  [3492] = 1,
-    ACTIONS(711), 5,
+    STATE(108), 1,
+      sym__regex,
+  [3109] = 1,
+    ACTIONS(594), 5,
+      anon_sym_STAR,
       anon_sym_SQUOTE,
       anon_sym_DQUOTE,
       anon_sym_BQUOTE,
-      anon_sym_LF,
       sym__word,
-  [3500] = 1,
-    ACTIONS(602), 5,
+  [3117] = 3,
+    ACTIONS(936), 1,
+      anon_sym_SPACE,
+    STATE(162), 1,
+      aux_sym__strings_repeat1,
+    ACTIONS(983), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [3129] = 5,
+    ACTIONS(919), 1,
       anon_sym_SQUOTE,
+    ACTIONS(921), 1,
       anon_sym_DQUOTE,
+    ACTIONS(923), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
+    ACTIONS(925), 1,
       sym__word,
-  [3508] = 1,
-    ACTIONS(620), 5,
+    STATE(135), 1,
+      sym__regex,
+  [3145] = 5,
+    ACTIONS(683), 1,
       anon_sym_SQUOTE,
+    ACTIONS(685), 1,
       anon_sym_DQUOTE,
+    ACTIONS(687), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
+    ACTIONS(689), 1,
       sym__word,
-  [3516] = 3,
-    ACTIONS(959), 1,
+    STATE(275), 1,
+      sym__string,
+  [3161] = 3,
+    ACTIONS(985), 1,
       anon_sym_SPACE,
     STATE(208), 1,
-      aux_sym__options3_repeat1,
-    ACTIONS(995), 3,
+      aux_sym__headers_repeat1,
+    ACTIONS(987), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3528] = 3,
-    ACTIONS(959), 1,
+  [3173] = 3,
+    ACTIONS(989), 1,
       anon_sym_SPACE,
-    STATE(208), 1,
-      aux_sym__options3_repeat1,
-    ACTIONS(997), 3,
+    STATE(235), 1,
+      aux_sym__regexes_repeat1,
+    ACTIONS(991), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3540] = 3,
+  [3185] = 4,
+    ACTIONS(779), 1,
+      sym_function,
+    ACTIONS(993), 1,
+      anon_sym_LT,
+    STATE(193), 1,
+      aux_sym_key_repeat1,
+    ACTIONS(996), 2,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [3199] = 3,
     ACTIONS(999), 1,
       anon_sym_SPACE,
-    STATE(208), 1,
-      aux_sym__options3_repeat1,
+    STATE(194), 1,
+      aux_sym__mimes_repeat1,
     ACTIONS(1002), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3552] = 3,
-    ACTIONS(959), 1,
+  [3211] = 3,
+    ACTIONS(985), 1,
       anon_sym_SPACE,
-    STATE(208), 1,
-      aux_sym__options3_repeat1,
+    STATE(191), 1,
+      aux_sym__headers_repeat1,
     ACTIONS(1004), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3564] = 3,
-    ACTIONS(959), 1,
+  [3223] = 3,
+    ACTIONS(1006), 1,
       anon_sym_SPACE,
-    STATE(208), 1,
-      aux_sym__options3_repeat1,
-    ACTIONS(1004), 3,
+    STATE(247), 1,
+      aux_sym__mime_types_repeat1,
+    ACTIONS(1008), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3576] = 3,
-    ACTIONS(959), 1,
+  [3235] = 3,
+    ACTIONS(1010), 1,
+      anon_sym_COMMA,
+    STATE(197), 1,
+      aux_sym__maps_repeat1,
+    ACTIONS(1013), 3,
+      anon_sym_LT,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [3247] = 5,
+    ACTIONS(851), 1,
+      anon_sym_DASHgroup,
+    ACTIONS(855), 1,
+      anon_sym_DASHrx,
+    ACTIONS(857), 1,
+      anon_sym_DASHaddr,
+    STATE(354), 1,
+      sym__group,
+    STATE(390), 1,
+      sym__rx_addr,
+  [3263] = 4,
+    ACTIONS(749), 1,
+      sym_function,
+    ACTIONS(1015), 1,
+      anon_sym_LT,
+    STATE(193), 1,
+      aux_sym_key_repeat1,
+    ACTIONS(1017), 2,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [3277] = 1,
+    ACTIONS(602), 5,
+      anon_sym_STAR,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [3285] = 3,
+    ACTIONS(951), 1,
       anon_sym_SPACE,
-    STATE(208), 1,
-      aux_sym__options3_repeat1,
-    ACTIONS(961), 3,
+    STATE(205), 1,
+      aux_sym__functions_repeat1,
+    ACTIONS(1019), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3588] = 3,
-    ACTIONS(959), 1,
+  [3297] = 5,
+    ACTIONS(815), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(817), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(819), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(821), 1,
+      sym__word,
+    STATE(368), 1,
+      sym__string,
+  [3313] = 5,
+    ACTIONS(815), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(817), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(819), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(821), 1,
+      sym__word,
+    STATE(423), 1,
+      sym__string,
+  [3329] = 5,
+    ACTIONS(815), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(817), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(819), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(821), 1,
+      sym__word,
+    STATE(408), 1,
+      sym__string,
+  [3345] = 3,
+    ACTIONS(1021), 1,
       anon_sym_SPACE,
-    STATE(207), 1,
-      aux_sym__options3_repeat1,
-    ACTIONS(1006), 3,
+    STATE(205), 1,
+      aux_sym__functions_repeat1,
+    ACTIONS(1024), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3600] = 3,
-    ACTIONS(959), 1,
+  [3357] = 2,
+    ACTIONS(1028), 1,
+      anon_sym_SLASH,
+    ACTIONS(1026), 4,
       anon_sym_SPACE,
-    STATE(208), 1,
-      aux_sym__options3_repeat1,
-    ACTIONS(1008), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3612] = 3,
-    ACTIONS(959), 1,
+  [3367] = 3,
+    ACTIONS(1030), 1,
+      anon_sym_SPACE,
+    STATE(219), 1,
+      aux_sym__mimes_repeat1,
+    ACTIONS(1032), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [3379] = 3,
+    ACTIONS(1034), 1,
       anon_sym_SPACE,
     STATE(208), 1,
-      aux_sym__options3_repeat1,
-    ACTIONS(1010), 3,
+      aux_sym__headers_repeat1,
+    ACTIONS(1037), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3624] = 3,
-    ACTIONS(959), 1,
+  [3391] = 3,
+    ACTIONS(1039), 1,
       anon_sym_SPACE,
     STATE(209), 1,
-      aux_sym__options3_repeat1,
-    ACTIONS(1010), 3,
+      aux_sym__mailboxes_repeat1,
+    ACTIONS(1042), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3636] = 3,
-    ACTIONS(959), 1,
+  [3403] = 3,
+    ACTIONS(971), 1,
       anon_sym_SPACE,
-    STATE(210), 1,
-      aux_sym__options3_repeat1,
-    ACTIONS(1010), 3,
+    STATE(244), 1,
+      aux_sym_named_mailboxes_directive_repeat1,
+    ACTIONS(1044), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3648] = 3,
-    ACTIONS(959), 1,
+  [3415] = 3,
+    ACTIONS(1046), 1,
       anon_sym_SPACE,
     STATE(211), 1,
-      aux_sym__options3_repeat1,
-    ACTIONS(1012), 3,
+      aux_sym__header_fields_repeat1,
+    ACTIONS(1049), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3660] = 3,
-    ACTIONS(1014), 1,
+  [3427] = 3,
+    ACTIONS(963), 1,
       anon_sym_SPACE,
-    STATE(218), 1,
-      aux_sym_named_mailboxes_directive_repeat1,
-    ACTIONS(1017), 3,
+    STATE(226), 1,
+      aux_sym__options2_repeat1,
+    ACTIONS(1051), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3672] = 4,
-    ACTIONS(765), 1,
+  [3439] = 3,
+    ACTIONS(1053), 1,
+      anon_sym_COMMA,
+    STATE(197), 1,
+      aux_sym__maps_repeat1,
+    ACTIONS(1055), 3,
       anon_sym_LT,
-    STATE(68), 1,
-      aux_sym_key_repeat1,
-    STATE(76), 1,
-      sym_key,
-    ACTIONS(825), 2,
       aux_sym_key_token2,
       aux_sym_key_token3,
-  [3686] = 3,
-    ACTIONS(1019), 1,
+  [3451] = 5,
+    ACTIONS(632), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(634), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(636), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(638), 1,
+      sym__word,
+    STATE(14), 1,
+      sym__string,
+  [3467] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
-    STATE(220), 1,
-      aux_sym__mime_types_repeat1,
-    ACTIONS(1022), 3,
+    STATE(238), 1,
+      aux_sym__options3_repeat1,
+    ACTIONS(1057), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3698] = 3,
-    ACTIONS(1024), 1,
-      anon_sym_COMMA,
-    STATE(221), 1,
-      aux_sym__addresses_repeat1,
-    ACTIONS(1027), 3,
+  [3479] = 3,
+    ACTIONS(1006), 1,
+      anon_sym_SPACE,
+    STATE(196), 1,
+      aux_sym__mime_types_repeat1,
+    ACTIONS(1059), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3710] = 3,
-    ACTIONS(1029), 1,
+  [3491] = 4,
+    ACTIONS(759), 1,
+      anon_sym_LT,
+    STATE(92), 1,
+      aux_sym_key_repeat1,
+    STATE(387), 1,
+      sym_key,
+    ACTIONS(761), 2,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [3505] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
-    STATE(222), 1,
-      aux_sym__options_repeat1,
-    ACTIONS(1032), 3,
+    STATE(237), 1,
+      aux_sym__options3_repeat1,
+    ACTIONS(1061), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3722] = 3,
-    ACTIONS(1034), 1,
+  [3517] = 3,
+    ACTIONS(1030), 1,
       anon_sym_SPACE,
-    STATE(223), 1,
-      aux_sym__options2_repeat1,
-    ACTIONS(1037), 3,
+    STATE(194), 1,
+      aux_sym__mimes_repeat1,
+    ACTIONS(1063), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3734] = 3,
+  [3529] = 3,
     ACTIONS(959), 1,
       anon_sym_SPACE,
-    STATE(213), 1,
+    STATE(173), 1,
+      aux_sym__options_repeat1,
+    ACTIONS(1065), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [3541] = 5,
+    ACTIONS(815), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(817), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(819), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(821), 1,
+      sym__word,
+    STATE(402), 1,
+      sym__string,
+  [3557] = 5,
+    ACTIONS(919), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(921), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(923), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(925), 1,
+      sym__word,
+    STATE(155), 1,
+      sym__regex,
+  [3573] = 3,
+    ACTIONS(927), 1,
+      anon_sym_SPACE,
+    STATE(225), 1,
       aux_sym__options3_repeat1,
-    ACTIONS(1039), 3,
+    ACTIONS(1067), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3746] = 3,
-    ACTIONS(1041), 1,
+  [3585] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
-    STATE(243), 1,
-      aux_sym__options_repeat1,
-    ACTIONS(1043), 3,
+    STATE(225), 1,
+      aux_sym__options3_repeat1,
+    ACTIONS(1069), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3758] = 3,
-    ACTIONS(959), 1,
+  [3597] = 3,
+    ACTIONS(1071), 1,
       anon_sym_SPACE,
-    STATE(214), 1,
+    STATE(225), 1,
       aux_sym__options3_repeat1,
-    ACTIONS(1045), 3,
+    ACTIONS(1074), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3770] = 3,
-    ACTIONS(1047), 1,
+  [3609] = 3,
+    ACTIONS(1076), 1,
       anon_sym_SPACE,
-    STATE(223), 1,
+    STATE(226), 1,
       aux_sym__options2_repeat1,
-    ACTIONS(1049), 3,
+    ACTIONS(1079), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3782] = 3,
-    ACTIONS(1051), 1,
+  [3621] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
-    STATE(228), 1,
-      aux_sym__header_fields_repeat1,
-    ACTIONS(1054), 3,
+    STATE(225), 1,
+      aux_sym__options3_repeat1,
+    ACTIONS(1081), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3794] = 3,
-    ACTIONS(1056), 1,
+  [3633] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
-    STATE(218), 1,
-      aux_sym_named_mailboxes_directive_repeat1,
-    ACTIONS(1058), 3,
+    STATE(225), 1,
+      aux_sym__options3_repeat1,
+    ACTIONS(1081), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3806] = 3,
-    ACTIONS(1060), 1,
+  [3645] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
-    STATE(230), 1,
-      aux_sym__mailboxes_repeat1,
-    ACTIONS(1063), 3,
+    STATE(225), 1,
+      aux_sym__options3_repeat1,
+    ACTIONS(929), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3818] = 3,
-    ACTIONS(1065), 1,
+  [3657] = 5,
+    ACTIONS(919), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(921), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(923), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(925), 1,
+      sym__word,
+    STATE(156), 1,
+      sym__regex,
+  [3673] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
-    STATE(231), 1,
-      aux_sym__strings_repeat1,
-    ACTIONS(1068), 3,
+    STATE(224), 1,
+      aux_sym__options3_repeat1,
+    ACTIONS(1083), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3830] = 3,
-    ACTIONS(1070), 1,
+  [3685] = 4,
+    ACTIONS(1015), 1,
+      anon_sym_LT,
+    STATE(199), 1,
+      aux_sym_key_repeat1,
+    STATE(477), 1,
+      sym_key,
+    ACTIONS(1085), 2,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [3699] = 3,
+    ACTIONS(1053), 1,
+      anon_sym_COMMA,
+    STATE(213), 1,
+      aux_sym__maps_repeat1,
+    ACTIONS(1087), 3,
+      anon_sym_LT,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [3711] = 3,
+    ACTIONS(1089), 1,
       anon_sym_SPACE,
-    STATE(232), 1,
-      aux_sym__headers_repeat1,
-    ACTIONS(1073), 3,
+    STATE(234), 1,
+      aux_sym__options_repeat1,
+    ACTIONS(1092), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3842] = 3,
-    ACTIONS(1075), 1,
+  [3723] = 3,
+    ACTIONS(989), 1,
       anon_sym_SPACE,
-    STATE(233), 1,
-      aux_sym__functions_repeat1,
-    ACTIONS(1078), 3,
+    STATE(164), 1,
+      aux_sym__regexes_repeat1,
+    ACTIONS(1094), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3854] = 1,
-    ACTIONS(1080), 5,
+  [3735] = 5,
+    ACTIONS(721), 1,
       anon_sym_SQUOTE,
+    ACTIONS(723), 1,
       anon_sym_DQUOTE,
+    ACTIONS(725), 1,
       anon_sym_BQUOTE,
-      anon_sym_LF,
+    ACTIONS(727), 1,
       sym__word,
-  [3862] = 3,
-    ACTIONS(1082), 1,
-      anon_sym_SPACE,
-    STATE(255), 1,
-      aux_sym__regexes_repeat1,
-    ACTIONS(1084), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [3874] = 2,
-    ACTIONS(1088), 1,
-      anon_sym_SLASH,
-    ACTIONS(1086), 4,
+    STATE(308), 1,
+      sym__regex,
+  [3751] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
+    STATE(225), 1,
+      aux_sym__options3_repeat1,
+    ACTIONS(1096), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3884] = 3,
-    ACTIONS(1090), 1,
+  [3763] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
-    STATE(260), 1,
-      aux_sym__mimes_repeat1,
-    ACTIONS(1092), 3,
+    STATE(225), 1,
+      aux_sym__options3_repeat1,
+    ACTIONS(1098), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3896] = 3,
-    ACTIONS(1094), 1,
-      anon_sym_COMMA,
-    STATE(238), 1,
-      aux_sym__maps_repeat1,
-    ACTIONS(1097), 3,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [3908] = 3,
-    ACTIONS(1099), 1,
+  [3775] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
-    STATE(220), 1,
-      aux_sym__mime_types_repeat1,
-    ACTIONS(1101), 3,
+    STATE(227), 1,
+      aux_sym__options3_repeat1,
+    ACTIONS(1098), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3920] = 3,
-    ACTIONS(1103), 1,
+  [3787] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
-    STATE(240), 1,
-      aux_sym__mimes_repeat1,
-    ACTIONS(1106), 3,
+    STATE(228), 1,
+      aux_sym__options3_repeat1,
+    ACTIONS(1098), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3932] = 3,
-    ACTIONS(1108), 1,
+  [3799] = 3,
+    ACTIONS(927), 1,
       anon_sym_SPACE,
-    STATE(241), 1,
-      aux_sym__regexes_repeat1,
-    ACTIONS(1111), 3,
+    STATE(229), 1,
+      aux_sym__options3_repeat1,
+    ACTIONS(1100), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3944] = 3,
-    ACTIONS(1113), 1,
+  [3811] = 5,
+    ACTIONS(919), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(921), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(923), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(925), 1,
+      sym__word,
+    STATE(157), 1,
+      sym__regex,
+  [3827] = 3,
+    ACTIONS(1102), 1,
       anon_sym_COMMA,
-    STATE(221), 1,
+    STATE(243), 1,
       aux_sym__addresses_repeat1,
-    ACTIONS(1115), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [3956] = 3,
-    ACTIONS(1041), 1,
-      anon_sym_SPACE,
-    STATE(222), 1,
-      aux_sym__options_repeat1,
-    ACTIONS(1117), 3,
+    ACTIONS(1105), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3968] = 3,
-    ACTIONS(1047), 1,
+  [3839] = 3,
+    ACTIONS(1107), 1,
       anon_sym_SPACE,
-    STATE(223), 1,
-      aux_sym__options2_repeat1,
-    ACTIONS(1119), 3,
+    STATE(244), 1,
+      aux_sym_named_mailboxes_directive_repeat1,
+    ACTIONS(1110), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3980] = 3,
-    ACTIONS(1047), 1,
-      anon_sym_SPACE,
-    STATE(227), 1,
-      aux_sym__options2_repeat1,
-    ACTIONS(1119), 3,
+  [3851] = 5,
+    ACTIONS(815), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(817), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(819), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(821), 1,
+      sym__word,
+    STATE(416), 1,
+      sym__string,
+  [3867] = 3,
+    ACTIONS(945), 1,
+      anon_sym_COMMA,
+    STATE(165), 1,
+      aux_sym__addresses_repeat1,
+    ACTIONS(1112), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [3992] = 3,
-    ACTIONS(989), 1,
+  [3879] = 3,
+    ACTIONS(1114), 1,
       anon_sym_SPACE,
-    STATE(228), 1,
-      aux_sym__header_fields_repeat1,
-    ACTIONS(1121), 3,
+    STATE(247), 1,
+      aux_sym__mime_types_repeat1,
+    ACTIONS(1117), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4004] = 3,
-    ACTIONS(1113), 1,
+  [3891] = 5,
+    ACTIONS(919), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(921), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(923), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(925), 1,
+      sym__word,
+    STATE(120), 1,
+      sym__regex,
+  [3907] = 5,
+    ACTIONS(919), 1,
+      anon_sym_SQUOTE,
+    ACTIONS(921), 1,
+      anon_sym_DQUOTE,
+    ACTIONS(923), 1,
+      anon_sym_BQUOTE,
+    ACTIONS(925), 1,
+      sym__word,
+    STATE(96), 1,
+      sym__regex,
+  [3923] = 4,
+    ACTIONS(1121), 1,
+      sym_option,
+    STATE(435), 1,
+      sym__options2,
+    STATE(436), 1,
+      sym__options3,
+    ACTIONS(1119), 2,
+      anon_sym_QMARK,
+      anon_sym_AMP,
+  [3937] = 1,
+    ACTIONS(1123), 4,
       anon_sym_COMMA,
-    STATE(242), 1,
-      aux_sym__addresses_repeat1,
-    ACTIONS(1123), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4016] = 3,
-    ACTIONS(1125), 1,
+  [3944] = 1,
+    ACTIONS(1117), 4,
       anon_sym_SPACE,
-    STATE(233), 1,
-      aux_sym__functions_repeat1,
-    ACTIONS(1127), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4028] = 3,
-    ACTIONS(967), 1,
+  [3951] = 1,
+    ACTIONS(1125), 4,
       anon_sym_SPACE,
-    STATE(231), 1,
-      aux_sym__strings_repeat1,
-    ACTIONS(1129), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4040] = 3,
-    ACTIONS(1131), 1,
+  [3958] = 3,
+    ACTIONS(1129), 1,
+      aux_sym__space_token1,
+    STATE(254), 1,
+      aux_sym__space_repeat1,
+    ACTIONS(1127), 2,
+      sym_comment,
+      sym__eol,
+  [3969] = 1,
+    ACTIONS(1132), 4,
       anon_sym_COMMA,
-    STATE(251), 1,
-      aux_sym__maps_repeat1,
-    ACTIONS(1133), 3,
       anon_sym_LT,
       aux_sym_key_token2,
       aux_sym_key_token3,
-  [4052] = 3,
-    ACTIONS(1131), 1,
+  [3976] = 1,
+    ACTIONS(1105), 4,
       anon_sym_COMMA,
-    STATE(238), 1,
-      aux_sym__maps_repeat1,
-    ACTIONS(1135), 3,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [4064] = 4,
-    ACTIONS(803), 1,
-      anon_sym_LT,
-    STATE(97), 1,
-      aux_sym_key_repeat1,
-    STATE(442), 1,
-      sym_key,
-    ACTIONS(805), 2,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [4078] = 1,
-    ACTIONS(1137), 5,
-      anon_sym_SQUOTE,
-      anon_sym_DQUOTE,
-      anon_sym_BQUOTE,
-      anon_sym_LF,
-      sym__word,
-  [4086] = 3,
-    ACTIONS(1125), 1,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [3983] = 1,
+    ACTIONS(1134), 4,
       anon_sym_SPACE,
-    STATE(248), 1,
-      aux_sym__functions_repeat1,
-    ACTIONS(1139), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4098] = 3,
-    ACTIONS(1082), 1,
+  [3990] = 1,
+    ACTIONS(1092), 4,
       anon_sym_SPACE,
-    STATE(241), 1,
-      aux_sym__regexes_repeat1,
-    ACTIONS(1141), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4110] = 3,
-    ACTIONS(1143), 1,
+  [3997] = 2,
+    ACTIONS(1136), 1,
+      anon_sym_SPACE,
+    ACTIONS(1138), 3,
+      anon_sym_PLUS_EQ,
+      anon_sym_DASH_EQ,
+      anon_sym_EQ,
+  [4006] = 4,
+    ACTIONS(1140), 1,
+      anon_sym_STAR,
+    ACTIONS(1142), 1,
+      sym_mime_type,
+    STATE(207), 1,
+      sym_mime,
+    STATE(397), 1,
+      sym__mimes,
+  [4019] = 1,
+    ACTIONS(1144), 4,
       anon_sym_SPACE,
-    STATE(232), 1,
-      aux_sym__headers_repeat1,
-    ACTIONS(1145), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4122] = 3,
-    ACTIONS(977), 1,
+  [4026] = 1,
+    ACTIONS(1146), 4,
       anon_sym_SPACE,
-    STATE(230), 1,
-      aux_sym__mailboxes_repeat1,
-    ACTIONS(1147), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4134] = 3,
-    ACTIONS(1056), 1,
+  [4033] = 1,
+    ACTIONS(1148), 4,
       anon_sym_SPACE,
-    STATE(229), 1,
-      aux_sym_named_mailboxes_directive_repeat1,
-    ACTIONS(1149), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4146] = 3,
-    ACTIONS(1143), 1,
+  [4040] = 1,
+    ACTIONS(1150), 4,
       anon_sym_SPACE,
-    STATE(256), 1,
-      aux_sym__headers_repeat1,
-    ACTIONS(1151), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4158] = 3,
-    ACTIONS(1090), 1,
+  [4047] = 1,
+    ACTIONS(1079), 4,
       anon_sym_SPACE,
-    STATE(240), 1,
-      aux_sym__mimes_repeat1,
-    ACTIONS(1153), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4170] = 1,
-    ACTIONS(1155), 5,
-      anon_sym_SQUOTE,
-      anon_sym_DQUOTE,
-      anon_sym_BQUOTE,
-      anon_sym_LF,
-      sym__word,
-  [4178] = 3,
-    ACTIONS(1099), 1,
+  [4054] = 1,
+    ACTIONS(1152), 4,
       anon_sym_SPACE,
-    STATE(239), 1,
-      aux_sym__mime_types_repeat1,
-    ACTIONS(1157), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4190] = 1,
-    ACTIONS(787), 4,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-      sym_function,
-  [4197] = 1,
-    ACTIONS(1159), 4,
+  [4061] = 1,
+    ACTIONS(1152), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4204] = 4,
-    ACTIONS(1161), 1,
-      anon_sym_STAR,
-    ACTIONS(1163), 1,
-      sym_mime_type,
-    STATE(237), 1,
-      sym_mime,
-    STATE(355), 1,
-      sym__mimes,
-  [4217] = 4,
-    ACTIONS(1163), 1,
-      sym_mime_type,
-    ACTIONS(1165), 1,
-      anon_sym_STAR,
-    STATE(237), 1,
-      sym_mime,
-    STATE(327), 1,
-      sym__mimes,
-  [4230] = 1,
-    ACTIONS(594), 4,
-      anon_sym_STAR,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [4237] = 1,
-    ACTIONS(598), 4,
-      anon_sym_STAR,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [4244] = 1,
-    ACTIONS(594), 4,
-      anon_sym_COMMA,
+  [4068] = 1,
+    ACTIONS(1154), 4,
+      anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4251] = 1,
-    ACTIONS(598), 4,
-      anon_sym_COMMA,
+  [4075] = 1,
+    ACTIONS(1156), 4,
+      anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4258] = 1,
-    ACTIONS(594), 4,
+  [4082] = 1,
+    ACTIONS(1049), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4265] = 1,
-    ACTIONS(598), 4,
+  [4089] = 1,
+    ACTIONS(616), 4,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [4096] = 1,
+    ACTIONS(602), 4,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [4103] = 1,
+    ACTIONS(1042), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4272] = 1,
-    ACTIONS(1167), 4,
+  [4110] = 1,
+    ACTIONS(1158), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4279] = 4,
-    ACTIONS(1163), 1,
-      sym_mime_type,
-    ACTIONS(1169), 1,
-      anon_sym_STAR,
-    STATE(237), 1,
-      sym_mime,
-    STATE(446), 1,
-      sym__mimes,
-  [4292] = 1,
-    ACTIONS(1171), 4,
+  [4117] = 1,
+    ACTIONS(1160), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4299] = 1,
-    ACTIONS(911), 4,
+  [4124] = 1,
+    ACTIONS(981), 4,
       anon_sym_STAR,
       anon_sym_LT,
       aux_sym_key_token2,
       aux_sym_key_token3,
-  [4306] = 1,
-    ACTIONS(933), 4,
+  [4131] = 1,
+    ACTIONS(1037), 4,
+      anon_sym_SPACE,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [4138] = 1,
+    ACTIONS(979), 4,
       anon_sym_STAR,
       anon_sym_LT,
       aux_sym_key_token2,
       aux_sym_key_token3,
-  [4313] = 1,
-    ACTIONS(1173), 4,
+  [4145] = 1,
+    ACTIONS(695), 4,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [4152] = 1,
+    ACTIONS(624), 4,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [4159] = 1,
+    ACTIONS(1024), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4320] = 1,
-    ACTIONS(1175), 4,
-      anon_sym_SPACE,
+  [4166] = 1,
+    ACTIONS(628), 4,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [4173] = 1,
+    ACTIONS(594), 4,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [4180] = 1,
+    ACTIONS(1162), 4,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [4187] = 3,
+    ACTIONS(1166), 1,
+      aux_sym__space_token1,
+    STATE(254), 1,
+      aux_sym__space_repeat1,
+    ACTIONS(1164), 2,
       sym_comment,
       sym__eol,
-      aux_sym__space_token1,
-  [4327] = 1,
-    ACTIONS(1177), 4,
+  [4198] = 1,
+    ACTIONS(1168), 4,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [4205] = 1,
+    ACTIONS(1170), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4334] = 1,
-    ACTIONS(1179), 4,
+  [4212] = 1,
+    ACTIONS(1013), 4,
+      anon_sym_COMMA,
+      anon_sym_LT,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [4219] = 1,
+    ACTIONS(981), 4,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [4226] = 1,
+    ACTIONS(979), 4,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [4233] = 1,
+    ACTIONS(1002), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4341] = 1,
-    ACTIONS(1179), 4,
+  [4240] = 1,
+    ACTIONS(598), 4,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [4247] = 4,
+    ACTIONS(855), 1,
+      anon_sym_DASHrx,
+    ACTIONS(857), 1,
+      anon_sym_DASHaddr,
+    ACTIONS(1172), 1,
+      anon_sym_STAR,
+    STATE(437), 1,
+      sym__rx_addr,
+  [4260] = 1,
+    ACTIONS(847), 4,
+      anon_sym_LT,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+      sym_function,
+  [4267] = 4,
+    ACTIONS(1142), 1,
+      sym_mime_type,
+    ACTIONS(1174), 1,
+      anon_sym_STAR,
+    STATE(207), 1,
+      sym_mime,
+    STATE(411), 1,
+      sym__mimes,
+  [4280] = 1,
+    ACTIONS(616), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4348] = 1,
-    ACTIONS(1181), 4,
+  [4287] = 1,
+    ACTIONS(1176), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4355] = 1,
-    ACTIONS(1183), 4,
+  [4294] = 1,
+    ACTIONS(594), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4362] = 4,
-    ACTIONS(919), 1,
-      anon_sym_DASHrx,
-    ACTIONS(921), 1,
-      anon_sym_DASHaddr,
-    ACTIONS(1185), 1,
-      anon_sym_STAR,
-    STATE(317), 1,
-      sym__rx_addr,
-  [4375] = 1,
-    ACTIONS(1187), 4,
+  [4301] = 1,
+    ACTIONS(598), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4382] = 2,
-    ACTIONS(1189), 1,
-      anon_sym_SPACE,
-    ACTIONS(1191), 3,
-      anon_sym_PLUS_EQ,
-      anon_sym_DASH_EQ,
-      anon_sym_EQ,
-  [4391] = 3,
-    ACTIONS(1195), 1,
-      aux_sym__space_token1,
-    STATE(298), 1,
-      aux_sym__space_repeat1,
-    ACTIONS(1193), 2,
+  [4308] = 1,
+    ACTIONS(1178), 4,
+      anon_sym_SQUOTE,
+      anon_sym_DQUOTE,
+      anon_sym_BQUOTE,
+      sym__word,
+  [4315] = 1,
+    ACTIONS(594), 4,
+      anon_sym_COMMA,
       sym_comment,
       sym__eol,
-  [4402] = 1,
-    ACTIONS(1197), 4,
+      aux_sym__space_token1,
+  [4322] = 1,
+    ACTIONS(1180), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4409] = 1,
-    ACTIONS(1199), 4,
+  [4329] = 1,
+    ACTIONS(598), 4,
       anon_sym_COMMA,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4416] = 1,
-    ACTIONS(1201), 4,
+  [4336] = 1,
+    ACTIONS(594), 4,
+      anon_sym_STAR,
+      anon_sym_LT,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [4343] = 1,
+    ACTIONS(598), 4,
+      anon_sym_STAR,
+      anon_sym_LT,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [4350] = 1,
+    ACTIONS(624), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4423] = 1,
-    ACTIONS(1022), 4,
+  [4357] = 1,
+    ACTIONS(628), 4,
       anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4430] = 1,
-    ACTIONS(1027), 4,
-      anon_sym_COMMA,
+  [4364] = 1,
+    ACTIONS(1182), 4,
+      anon_sym_SPACE,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4437] = 1,
-    ACTIONS(1032), 4,
-      anon_sym_SPACE,
+  [4371] = 4,
+    ACTIONS(1142), 1,
+      sym_mime_type,
+    ACTIONS(1184), 1,
+      anon_sym_STAR,
+    STATE(207), 1,
+      sym_mime,
+    STATE(351), 1,
+      sym__mimes,
+  [4384] = 1,
+    ACTIONS(1186), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4444] = 1,
-    ACTIONS(1203), 4,
-      anon_sym_SPACE,
+  [4390] = 3,
+    ACTIONS(1142), 1,
+      sym_mime_type,
+    STATE(207), 1,
+      sym_mime,
+    STATE(396), 1,
+      sym__mimes,
+  [4400] = 1,
+    ACTIONS(1188), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4451] = 1,
-    ACTIONS(1037), 4,
-      anon_sym_SPACE,
+  [4406] = 1,
+    ACTIONS(1190), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4458] = 1,
-    ACTIONS(1106), 4,
-      anon_sym_SPACE,
+  [4412] = 3,
+    ACTIONS(1142), 1,
+      sym_mime_type,
+    STATE(207), 1,
+      sym_mime,
+    STATE(373), 1,
+      sym__mimes,
+  [4422] = 1,
+    ACTIONS(1192), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4465] = 3,
-    ACTIONS(1207), 1,
+  [4428] = 1,
+    ACTIONS(1194), 3,
+      sym_comment,
+      sym__eol,
       aux_sym__space_token1,
-    STATE(298), 1,
-      aux_sym__space_repeat1,
-    ACTIONS(1205), 2,
+  [4434] = 1,
+    ACTIONS(1196), 3,
       sym_comment,
       sym__eol,
-  [4476] = 1,
-    ACTIONS(1210), 4,
-      anon_sym_COMMA,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [4483] = 1,
-    ACTIONS(620), 4,
-      anon_sym_SPACE,
+      aux_sym__space_token1,
+  [4440] = 1,
+    ACTIONS(1198), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4490] = 1,
-    ACTIONS(1063), 4,
-      anon_sym_SPACE,
+  [4446] = 1,
+    ACTIONS(1200), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4497] = 1,
-    ACTIONS(1078), 4,
-      anon_sym_SPACE,
+  [4452] = 1,
+    ACTIONS(1202), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4504] = 1,
-    ACTIONS(1212), 4,
-      anon_sym_SPACE,
+  [4458] = 1,
+    ACTIONS(1204), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4511] = 1,
-    ACTIONS(1097), 4,
-      anon_sym_COMMA,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [4518] = 1,
-    ACTIONS(1054), 4,
-      anon_sym_SPACE,
+  [4464] = 1,
+    ACTIONS(1206), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4525] = 1,
-    ACTIONS(624), 4,
-      anon_sym_SPACE,
+  [4470] = 1,
+    ACTIONS(1208), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4532] = 1,
-    ACTIONS(628), 4,
-      anon_sym_SPACE,
+  [4476] = 1,
+    ACTIONS(1210), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4539] = 1,
-    ACTIONS(1214), 4,
-      anon_sym_SPACE,
+  [4482] = 1,
+    ACTIONS(1212), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4546] = 1,
-    ACTIONS(1073), 4,
-      anon_sym_SPACE,
+  [4488] = 1,
+    ACTIONS(1214), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4553] = 1,
+  [4494] = 1,
     ACTIONS(1216), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4559] = 1,
+  [4500] = 1,
     ACTIONS(1218), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4565] = 1,
+  [4506] = 1,
     ACTIONS(1220), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4571] = 1,
+  [4512] = 1,
     ACTIONS(1222), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4577] = 1,
+  [4518] = 1,
     ACTIONS(1224), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4583] = 1,
+  [4524] = 1,
     ACTIONS(1226), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4589] = 1,
+  [4530] = 3,
+    ACTIONS(1142), 1,
+      sym_mime_type,
+    STATE(207), 1,
+      sym_mime,
+    STATE(409), 1,
+      sym__mimes,
+  [4540] = 1,
     ACTIONS(1228), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4595] = 1,
+  [4546] = 1,
     ACTIONS(1230), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4601] = 1,
+  [4552] = 1,
     ACTIONS(1232), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4607] = 1,
+  [4558] = 1,
     ACTIONS(1234), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4613] = 1,
+  [4564] = 1,
     ACTIONS(1236), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4619] = 1,
+  [4570] = 1,
     ACTIONS(1238), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4625] = 1,
+  [4576] = 1,
     ACTIONS(1240), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4631] = 1,
+  [4582] = 1,
     ACTIONS(1242), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4637] = 1,
+  [4588] = 1,
+    ACTIONS(598), 3,
+      anon_sym_LT,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [4594] = 1,
     ACTIONS(1244), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4643] = 1,
+  [4600] = 1,
+    ACTIONS(594), 3,
+      anon_sym_LT,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [4606] = 1,
     ACTIONS(1246), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4649] = 1,
+  [4612] = 1,
     ACTIONS(1248), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4655] = 1,
+  [4618] = 1,
     ACTIONS(1250), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4661] = 3,
-    ACTIONS(1163), 1,
-      sym_mime_type,
-    STATE(237), 1,
-      sym_mime,
-    STATE(329), 1,
-      sym__mimes,
-  [4671] = 1,
+  [4624] = 1,
     ACTIONS(1252), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4677] = 1,
+  [4630] = 1,
     ACTIONS(1254), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4683] = 1,
+  [4636] = 1,
     ACTIONS(1256), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4689] = 1,
+  [4642] = 1,
     ACTIONS(1258), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4695] = 1,
+  [4648] = 1,
     ACTIONS(1260), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4701] = 1,
+  [4654] = 1,
     ACTIONS(1262), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4707] = 1,
+  [4660] = 3,
+    ACTIONS(855), 1,
+      anon_sym_DASHrx,
+    ACTIONS(857), 1,
+      anon_sym_DASHaddr,
+    STATE(332), 1,
+      sym__rx_addr,
+  [4670] = 1,
     ACTIONS(1264), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4713] = 1,
+  [4676] = 1,
     ACTIONS(1266), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4719] = 1,
+  [4682] = 1,
     ACTIONS(1268), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4725] = 1,
+  [4688] = 1,
     ACTIONS(1270), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4731] = 1,
+  [4694] = 1,
     ACTIONS(1272), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4737] = 1,
+  [4700] = 1,
     ACTIONS(1274), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4743] = 1,
+  [4706] = 1,
     ACTIONS(1276), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4749] = 1,
+  [4712] = 1,
     ACTIONS(1278), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4755] = 1,
+  [4718] = 1,
     ACTIONS(1280), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4761] = 1,
+  [4724] = 1,
     ACTIONS(1282), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4767] = 1,
+  [4730] = 1,
     ACTIONS(1284), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [4773] = 1,
+      anon_sym_STAR,
+      anon_sym_DASHrx,
+      anon_sym_DASHaddr,
+  [4736] = 1,
     ACTIONS(1286), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [4779] = 1,
-    ACTIONS(594), 3,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [4785] = 1,
-    ACTIONS(598), 3,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [4791] = 1,
+      anon_sym_STAR,
+      anon_sym_DASHrx,
+      anon_sym_DASHaddr,
+  [4742] = 1,
     ACTIONS(1288), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4797] = 1,
-    ACTIONS(911), 3,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [4803] = 1,
+  [4748] = 1,
     ACTIONS(1290), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4809] = 1,
+  [4754] = 1,
     ACTIONS(1292), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4815] = 1,
+  [4760] = 1,
     ACTIONS(1294), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4821] = 1,
+  [4766] = 1,
     ACTIONS(1296), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4827] = 1,
+  [4772] = 1,
     ACTIONS(1298), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4833] = 1,
+  [4778] = 1,
     ACTIONS(1300), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4839] = 1,
+  [4784] = 1,
     ACTIONS(1302), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4845] = 1,
-    ACTIONS(933), 3,
-      anon_sym_LT,
-      aux_sym_key_token2,
-      aux_sym_key_token3,
-  [4851] = 1,
+  [4790] = 1,
     ACTIONS(1304), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4857] = 1,
+  [4796] = 1,
     ACTIONS(1306), 3,
-      anon_sym_STAR,
-      anon_sym_DASHrx,
-      anon_sym_DASHaddr,
-  [4863] = 1,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [4802] = 1,
     ACTIONS(1308), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4869] = 1,
+  [4808] = 1,
     ACTIONS(1310), 3,
-      anon_sym_STAR,
-      anon_sym_DASHrx,
-      anon_sym_DASHaddr,
-  [4875] = 1,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [4814] = 1,
+    ACTIONS(628), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [4820] = 1,
+    ACTIONS(624), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [4826] = 1,
     ACTIONS(1312), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4881] = 1,
+  [4832] = 1,
     ACTIONS(1314), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4887] = 1,
+  [4838] = 1,
     ACTIONS(1316), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4893] = 1,
+  [4844] = 1,
     ACTIONS(1318), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4899] = 1,
-    ACTIONS(628), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [4905] = 1,
+  [4850] = 1,
     ACTIONS(1320), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4911] = 1,
+  [4856] = 2,
+    ACTIONS(871), 1,
+      sym_option,
+    ACTIONS(867), 2,
+      anon_sym_QMARK,
+      anon_sym_AMP,
+  [4864] = 1,
     ACTIONS(1322), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4917] = 1,
+  [4870] = 1,
     ACTIONS(1324), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4923] = 1,
+  [4876] = 1,
     ACTIONS(1326), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4929] = 1,
+  [4882] = 1,
     ACTIONS(1328), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4935] = 1,
+  [4888] = 1,
+    ACTIONS(602), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [4894] = 1,
     ACTIONS(1330), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4941] = 1,
-    ACTIONS(624), 3,
+  [4900] = 1,
+    ACTIONS(616), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4947] = 1,
+  [4906] = 1,
     ACTIONS(1332), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4953] = 1,
+  [4912] = 1,
     ACTIONS(1334), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4959] = 1,
+  [4918] = 1,
     ACTIONS(1336), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4965] = 1,
+  [4924] = 1,
     ACTIONS(1338), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4971] = 1,
+  [4930] = 1,
     ACTIONS(1340), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4977] = 1,
+  [4936] = 1,
     ACTIONS(1342), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4983] = 1,
+  [4942] = 1,
     ACTIONS(1344), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4989] = 1,
-    ACTIONS(602), 3,
+  [4948] = 1,
+    ACTIONS(1346), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [4995] = 1,
-    ACTIONS(620), 3,
+  [4954] = 1,
+    ACTIONS(1348), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5001] = 1,
-    ACTIONS(1346), 3,
+  [4960] = 1,
+    ACTIONS(793), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5007] = 1,
-    ACTIONS(1348), 3,
+  [4966] = 1,
+    ACTIONS(823), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5013] = 2,
-    ACTIONS(941), 1,
-      sym_option,
-    ACTIONS(937), 2,
-      anon_sym_QMARK,
-      anon_sym_AMP,
-  [5021] = 1,
+  [4972] = 1,
     ACTIONS(1350), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5027] = 3,
-    ACTIONS(1163), 1,
-      sym_mime_type,
-    STATE(237), 1,
-      sym_mime,
-    STATE(448), 1,
-      sym__mimes,
-  [5037] = 3,
-    ACTIONS(1163), 1,
-      sym_mime_type,
-    STATE(237), 1,
-      sym_mime,
-    STATE(357), 1,
-      sym__mimes,
-  [5047] = 1,
+  [4978] = 1,
     ACTIONS(1352), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5053] = 1,
+  [4984] = 1,
     ACTIONS(1354), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5059] = 1,
+  [4990] = 1,
     ACTIONS(1356), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5065] = 1,
+  [4996] = 1,
     ACTIONS(1358), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5071] = 1,
+  [5002] = 1,
     ACTIONS(1360), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5077] = 1,
+  [5008] = 1,
     ACTIONS(1362), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5083] = 1,
+  [5014] = 1,
     ACTIONS(1364), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5089] = 1,
+  [5020] = 1,
+    ACTIONS(979), 3,
+      anon_sym_LT,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [5026] = 1,
+    ACTIONS(981), 3,
+      anon_sym_LT,
+      aux_sym_key_token2,
+      aux_sym_key_token3,
+  [5032] = 1,
     ACTIONS(1366), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5095] = 1,
+  [5038] = 1,
     ACTIONS(1368), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5101] = 1,
-    ACTIONS(993), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5107] = 1,
+  [5044] = 1,
     ACTIONS(1370), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5113] = 1,
+  [5050] = 1,
     ACTIONS(1372), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5119] = 1,
+  [5056] = 1,
     ACTIONS(1374), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5125] = 1,
+  [5062] = 1,
     ACTIONS(1376), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5131] = 1,
+  [5068] = 1,
     ACTIONS(1378), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5137] = 1,
+  [5074] = 1,
+    ACTIONS(833), 3,
+      sym_comment,
+      sym__eol,
+      aux_sym__space_token1,
+  [5080] = 1,
     ACTIONS(1380), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5143] = 1,
+  [5086] = 1,
     ACTIONS(1382), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5149] = 1,
+  [5092] = 1,
     ACTIONS(1384), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5155] = 1,
+  [5098] = 1,
     ACTIONS(1386), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5161] = 1,
+  [5104] = 1,
     ACTIONS(1388), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5167] = 1,
+  [5110] = 1,
     ACTIONS(1390), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5173] = 1,
+  [5116] = 1,
     ACTIONS(1392), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5179] = 1,
+  [5122] = 1,
     ACTIONS(1394), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5185] = 1,
+  [5128] = 1,
     ACTIONS(1396), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5191] = 1,
+      anon_sym_PLUS_EQ,
+      anon_sym_DASH_EQ,
+      anon_sym_EQ,
+  [5134] = 1,
     ACTIONS(1398), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5197] = 1,
+  [5140] = 1,
     ACTIONS(1400), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5203] = 1,
-    ACTIONS(1080), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5209] = 1,
+  [5146] = 1,
     ACTIONS(1402), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5215] = 1,
+  [5152] = 1,
     ACTIONS(1404), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5221] = 1,
+  [5158] = 1,
     ACTIONS(1406), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5227] = 1,
+  [5164] = 1,
     ACTIONS(1408), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5233] = 1,
+  [5170] = 1,
     ACTIONS(1410), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5239] = 1,
+  [5176] = 1,
     ACTIONS(1412), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5245] = 1,
+  [5182] = 1,
     ACTIONS(1414), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5251] = 1,
+  [5188] = 1,
     ACTIONS(1416), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5257] = 1,
+  [5194] = 1,
     ACTIONS(1418), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5263] = 1,
+  [5200] = 1,
     ACTIONS(1420), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5269] = 3,
-    ACTIONS(919), 1,
-      anon_sym_DASHrx,
-    ACTIONS(921), 1,
-      anon_sym_DASHaddr,
-    STATE(315), 1,
-      sym__rx_addr,
-  [5279] = 1,
-    ACTIONS(1422), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5285] = 1,
-    ACTIONS(1424), 3,
+  [5206] = 1,
+    ACTIONS(1176), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5291] = 1,
-    ACTIONS(1426), 3,
+  [5212] = 1,
+    ACTIONS(1180), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5297] = 1,
-    ACTIONS(1428), 3,
-      anon_sym_PLUS_EQ,
-      anon_sym_DASH_EQ,
-      anon_sym_EQ,
-  [5303] = 1,
-    ACTIONS(1430), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5309] = 1,
-    ACTIONS(1432), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5315] = 1,
-    ACTIONS(1434), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5321] = 1,
-    ACTIONS(1436), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5327] = 1,
-    ACTIONS(1438), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5333] = 1,
-    ACTIONS(1440), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5339] = 1,
-    ACTIONS(1442), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5345] = 1,
-    ACTIONS(1444), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5351] = 1,
-    ACTIONS(1446), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5357] = 1,
-    ACTIONS(1448), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5363] = 1,
-    ACTIONS(1450), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5369] = 1,
-    ACTIONS(1452), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5375] = 1,
-    ACTIONS(1171), 3,
-      sym_comment,
-      sym__eol,
-      aux_sym__space_token1,
-  [5381] = 1,
-    ACTIONS(1167), 3,
+  [5218] = 1,
+    ACTIONS(1422), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5387] = 1,
-    ACTIONS(1454), 3,
+  [5224] = 1,
+    ACTIONS(1162), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5393] = 1,
-    ACTIONS(1155), 3,
+  [5230] = 1,
+    ACTIONS(1424), 3,
       sym_comment,
       sym__eol,
       aux_sym__space_token1,
-  [5399] = 1,
-    ACTIONS(1456), 3,
+  [5236] = 2,
+    ACTIONS(1426), 1,
+      sym_function,
+    STATE(336), 1,
+      sym__functions,
+  [5243] = 2,
+    ACTIONS(1428), 1,
+      anon_sym_DASHgroup,
+    STATE(79), 1,
+      sym__group,
+  [5250] = 2,
+    ACTIONS(1430), 1,
+      anon_sym_DASHgroup,
+    STATE(148), 1,
+      sym__group,
+  [5257] = 2,
+    ACTIONS(1432), 1,
       sym_comment,
+    ACTIONS(1434), 1,
       sym__eol,
-      aux_sym__space_token1,
-  [5405] = 2,
-    ACTIONS(1458), 1,
+  [5264] = 2,
+    ACTIONS(1428), 1,
       anon_sym_DASHgroup,
-    STATE(119), 1,
+    STATE(80), 1,
       sym__group,
-  [5412] = 2,
-    ACTIONS(1460), 1,
+  [5271] = 2,
+    ACTIONS(1436), 1,
+      sym_mime_type,
+    STATE(310), 1,
+      sym__mime_types,
+  [5278] = 2,
+    ACTIONS(1430), 1,
+      anon_sym_DASHgroup,
+    STATE(146), 1,
+      sym__group,
+  [5285] = 2,
+    ACTIONS(1438), 1,
       anon_sym_QMARK,
-    ACTIONS(1462), 1,
+    ACTIONS(1440), 1,
       sym_option,
-  [5419] = 2,
-    ACTIONS(1464), 1,
+  [5292] = 2,
+    ACTIONS(1442), 1,
       sym_option,
-    STATE(387), 1,
+    STATE(432), 1,
       sym__options,
-  [5426] = 2,
-    ACTIONS(1466), 1,
+  [5299] = 2,
+    ACTIONS(1142), 1,
       sym_mime_type,
-    STATE(443), 1,
-      sym__mime_types,
-  [5433] = 2,
-    ACTIONS(1464), 1,
-      sym_option,
-    STATE(393), 1,
-      sym__options,
-  [5440] = 2,
-    ACTIONS(1466), 1,
+    STATE(291), 1,
+      sym_mime,
+  [5306] = 2,
+    ACTIONS(1436), 1,
       sym_mime_type,
-    STATE(406), 1,
+    STATE(392), 1,
       sym__mime_types,
-  [5447] = 2,
-    ACTIONS(1163), 1,
-      sym_mime_type,
-    STATE(297), 1,
-      sym_mime,
-  [5454] = 2,
-    ACTIONS(1468), 1,
-      sym_function,
-    STATE(423), 1,
-      sym__functions,
-  [5461] = 2,
-    ACTIONS(1464), 1,
-      sym_option,
-    STATE(394), 1,
-      sym__options,
-  [5468] = 2,
-    ACTIONS(1470), 1,
-      anon_sym_DASHgroup,
-    STATE(72), 1,
-      sym__group,
-  [5475] = 2,
-    ACTIONS(1472), 1,
-      sym_comment,
-    ACTIONS(1474), 1,
-      sym__eol,
-  [5482] = 2,
-    ACTIONS(1466), 1,
+  [5313] = 2,
+    ACTIONS(1436), 1,
       sym_mime_type,
-    STATE(361), 1,
+    STATE(353), 1,
       sym__mime_types,
-  [5489] = 2,
-    ACTIONS(1458), 1,
-      anon_sym_DASHgroup,
-    STATE(126), 1,
-      sym__group,
-  [5496] = 2,
-    ACTIONS(1466), 1,
+  [5320] = 2,
+    ACTIONS(1436), 1,
       sym_mime_type,
-    STATE(364), 1,
+    STATE(356), 1,
       sym__mime_types,
-  [5503] = 2,
-    ACTIONS(1470), 1,
-      anon_sym_DASHgroup,
-    STATE(84), 1,
-      sym__group,
-  [5510] = 1,
-    ACTIONS(1476), 1,
-      anon_sym_DQUOTE,
-  [5514] = 1,
-    ACTIONS(1478), 1,
-      anon_sym_BQUOTE,
-  [5518] = 1,
-    ACTIONS(1480), 1,
+  [5327] = 2,
+    ACTIONS(1442), 1,
       sym_option,
-  [5522] = 1,
-    ACTIONS(1482), 1,
-      aux_sym__string_token1,
-  [5526] = 1,
-    ACTIONS(1484), 1,
-      aux_sym__string_token2,
-  [5530] = 1,
-    ACTIONS(1486), 1,
-      aux_sym__string_token3,
-  [5534] = 1,
-    ACTIONS(1488), 1,
-      aux_sym_key_token1,
-  [5538] = 1,
-    ACTIONS(1490), 1,
-      aux_sym__string_token2,
-  [5542] = 1,
-    ACTIONS(1492), 1,
-      sym_option,
-  [5546] = 1,
-    ACTIONS(1494), 1,
-      sym_function,
-  [5550] = 1,
-    ACTIONS(1496), 1,
-      aux_sym__string_token1,
-  [5554] = 1,
-    ACTIONS(1498), 1,
-      sym_option,
-  [5558] = 1,
-    ACTIONS(1500), 1,
+    STATE(434), 1,
+      sym__options,
+  [5334] = 2,
+    ACTIONS(1442), 1,
       sym_option,
-  [5562] = 1,
-    ACTIONS(1500), 1,
-      aux_sym_setenv_directive_token1,
-  [5566] = 1,
-    ACTIONS(1502), 1,
-      aux_sym__string_token3,
-  [5570] = 1,
-    ACTIONS(1504), 1,
+    STATE(433), 1,
+      sym__options,
+  [5341] = 1,
+    ACTIONS(1444), 1,
+      anon_sym_DQUOTE,
+  [5345] = 1,
+    ACTIONS(1446), 1,
+      anon_sym_BQUOTE,
+  [5349] = 1,
+    ACTIONS(1448), 1,
       sym_int,
-  [5574] = 1,
-    ACTIONS(1506), 1,
+  [5353] = 1,
+    ACTIONS(1450), 1,
       sym__eol,
-  [5578] = 1,
-    ACTIONS(1508), 1,
+  [5357] = 1,
+    ACTIONS(1452), 1,
       anon_sym_SQUOTE,
-  [5582] = 1,
-    ACTIONS(1510), 1,
-      sym_mime_type,
-  [5586] = 1,
-    ACTIONS(1508), 1,
+  [5361] = 1,
+    ACTIONS(1452), 1,
+      anon_sym_DQUOTE,
+  [5365] = 1,
+    ACTIONS(1452), 1,
       anon_sym_BQUOTE,
-  [5590] = 1,
-    ACTIONS(1512), 1,
+  [5369] = 1,
+    ACTIONS(1454), 1,
+      sym_option,
+  [5373] = 1,
+    ACTIONS(1456), 1,
+      anon_sym_GT,
+  [5377] = 1,
+    ACTIONS(1458), 1,
+      anon_sym_SQUOTE,
+  [5381] = 1,
+    ACTIONS(1458), 1,
+      anon_sym_DQUOTE,
+  [5385] = 1,
+    ACTIONS(1460), 1,
+      anon_sym_BQUOTE,
+  [5389] = 1,
+    ACTIONS(1462), 1,
+      sym_mime_type,
+  [5393] = 1,
+    ACTIONS(1464), 1,
       sym_function,
-  [5594] = 1,
+  [5397] = 1,
+    ACTIONS(1466), 1,
+      sym_option,
+  [5401] = 1,
     ACTIONS(592), 1,
       sym_mime_type,
-  [5598] = 1,
-    ACTIONS(1514), 1,
+  [5405] = 1,
+    ACTIONS(1468), 1,
       sym_mime_type,
-  [5602] = 1,
-    ACTIONS(1474), 1,
+  [5409] = 1,
+    ACTIONS(596), 1,
+      sym_mime_type,
+  [5413] = 1,
+    ACTIONS(1470), 1,
+      sym_option,
+  [5417] = 1,
+    ACTIONS(1472), 1,
+      sym_function,
+  [5421] = 1,
+    ACTIONS(1434), 1,
       sym__eol,
-  [5606] = 1,
-    ACTIONS(1516), 1,
+  [5425] = 1,
+    ACTIONS(1474), 1,
+      ts_builtin_sym_end,
+  [5429] = 1,
+    ACTIONS(1476), 1,
       sym_option,
-  [5610] = 1,
-    ACTIONS(1518), 1,
-      anon_sym_GT,
-  [5614] = 1,
-    ACTIONS(1520), 1,
+  [5433] = 1,
+    ACTIONS(1478), 1,
+      aux_sym__string_token1,
+  [5437] = 1,
+    ACTIONS(1480), 1,
       sym_mime_type,
-  [5618] = 1,
-    ACTIONS(1522), 1,
+  [5441] = 1,
+    ACTIONS(1482), 1,
+      aux_sym__string_token2,
+  [5445] = 1,
+    ACTIONS(1484), 1,
+      aux_sym__string_token3,
+  [5449] = 1,
+    ACTIONS(1486), 1,
+      aux_sym_key_token1,
+  [5453] = 1,
+    ACTIONS(1488), 1,
       sym_option,
-  [5622] = 1,
-    ACTIONS(1524), 1,
-      anon_sym_BQUOTE,
-  [5626] = 1,
-    ACTIONS(1526), 1,
-      anon_sym_DQUOTE,
-  [5630] = 1,
-    ACTIONS(1528), 1,
+  [5457] = 1,
+    ACTIONS(1490), 1,
+      aux_sym__string_token1,
+  [5461] = 1,
+    ACTIONS(1492), 1,
       anon_sym_SQUOTE,
-  [5634] = 1,
-    ACTIONS(1528), 1,
+  [5465] = 1,
+    ACTIONS(1492), 1,
       anon_sym_DQUOTE,
-  [5638] = 1,
-    ACTIONS(1528), 1,
+  [5469] = 1,
+    ACTIONS(1492), 1,
       anon_sym_BQUOTE,
-  [5642] = 1,
-    ACTIONS(1530), 1,
+  [5473] = 1,
+    ACTIONS(1494), 1,
       anon_sym_GT,
-  [5646] = 1,
-    ACTIONS(1532), 1,
+  [5477] = 1,
+    ACTIONS(1496), 1,
       anon_sym_SQUOTE,
-  [5650] = 1,
-    ACTIONS(1532), 1,
+  [5481] = 1,
+    ACTIONS(1496), 1,
       anon_sym_DQUOTE,
-  [5654] = 1,
-    ACTIONS(1534), 1,
+  [5485] = 1,
+    ACTIONS(1498), 1,
       anon_sym_BQUOTE,
-  [5658] = 1,
-    ACTIONS(1508), 1,
-      anon_sym_DQUOTE,
-  [5662] = 1,
-    ACTIONS(1536), 1,
+  [5489] = 1,
+    ACTIONS(1500), 1,
+      aux_sym__string_token2,
+  [5493] = 1,
+    ACTIONS(1502), 1,
       anon_sym_SQUOTE,
-  [5666] = 1,
-    ACTIONS(1536), 1,
+  [5497] = 1,
+    ACTIONS(1502), 1,
       anon_sym_DQUOTE,
-  [5670] = 1,
-    ACTIONS(1536), 1,
+  [5501] = 1,
+    ACTIONS(1502), 1,
       anon_sym_BQUOTE,
-  [5674] = 1,
-    ACTIONS(1538), 1,
+  [5505] = 1,
+    ACTIONS(1504), 1,
       anon_sym_GT,
-  [5678] = 1,
-    ACTIONS(1476), 1,
+  [5509] = 1,
+    ACTIONS(1444), 1,
       anon_sym_SQUOTE,
-  [5682] = 1,
-    ACTIONS(596), 1,
-      sym_mime_type,
-  [5686] = 1,
-    ACTIONS(1540), 1,
+  [5513] = 1,
+    ACTIONS(1506), 1,
+      sym_option,
+  [5517] = 1,
+    ACTIONS(1508), 1,
       anon_sym_BQUOTE,
-  [5690] = 1,
-    ACTIONS(1526), 1,
-      anon_sym_SQUOTE,
-  [5694] = 1,
-    ACTIONS(1542), 1,
+  [5521] = 1,
+    ACTIONS(1510), 1,
+      aux_sym__string_token3,
+  [5525] = 1,
+    ACTIONS(1512), 1,
       anon_sym_SQUOTE,
-  [5698] = 1,
-    ACTIONS(1542), 1,
+  [5529] = 1,
+    ACTIONS(1512), 1,
       anon_sym_DQUOTE,
-  [5702] = 1,
-    ACTIONS(1542), 1,
+  [5533] = 1,
+    ACTIONS(1512), 1,
       anon_sym_BQUOTE,
-  [5706] = 1,
-    ACTIONS(1544), 1,
+  [5537] = 1,
+    ACTIONS(1514), 1,
       anon_sym_SQUOTE,
-  [5710] = 1,
-    ACTIONS(1544), 1,
+  [5541] = 1,
+    ACTIONS(1514), 1,
       anon_sym_DQUOTE,
-  [5714] = 1,
-    ACTIONS(1546), 1,
-      ts_builtin_sym_end,
-  [5718] = 1,
-    ACTIONS(1548), 1,
+  [5545] = 1,
+    ACTIONS(1476), 1,
+      aux_sym_setenv_directive_token1,
+  [5549] = 1,
+    ACTIONS(1516), 1,
       anon_sym_SQUOTE,
-  [5722] = 1,
-    ACTIONS(1548), 1,
+  [5553] = 1,
+    ACTIONS(1516), 1,
       anon_sym_DQUOTE,
-  [5726] = 1,
-    ACTIONS(1548), 1,
+  [5557] = 1,
+    ACTIONS(1516), 1,
       anon_sym_BQUOTE,
-  [5730] = 1,
-    ACTIONS(1550), 1,
+  [5561] = 1,
+    ACTIONS(1518), 1,
       anon_sym_SQUOTE,
-  [5734] = 1,
-    ACTIONS(1550), 1,
+  [5565] = 1,
+    ACTIONS(1518), 1,
       anon_sym_DQUOTE,
-  [5738] = 1,
-    ACTIONS(1550), 1,
+  [5569] = 1,
+    ACTIONS(1518), 1,
       anon_sym_BQUOTE,
-  [5742] = 1,
-    ACTIONS(1552), 1,
+  [5573] = 1,
+    ACTIONS(1520), 1,
       anon_sym_SQUOTE,
-  [5746] = 1,
-    ACTIONS(1552), 1,
+  [5577] = 1,
+    ACTIONS(1520), 1,
       anon_sym_DQUOTE,
-  [5750] = 1,
-    ACTIONS(1552), 1,
+  [5581] = 1,
+    ACTIONS(1520), 1,
       anon_sym_BQUOTE,
-  [5754] = 1,
-    ACTIONS(1554), 1,
+  [5585] = 1,
+    ACTIONS(1522), 1,
       anon_sym_SQUOTE,
-  [5758] = 1,
-    ACTIONS(1554), 1,
+  [5589] = 1,
+    ACTIONS(1522), 1,
       anon_sym_DQUOTE,
-  [5762] = 1,
-    ACTIONS(1554), 1,
+  [5593] = 1,
+    ACTIONS(1522), 1,
       anon_sym_BQUOTE,
-  [5766] = 1,
-    ACTIONS(1556), 1,
+  [5597] = 1,
+    ACTIONS(1524), 1,
       anon_sym_SQUOTE,
-  [5770] = 1,
-    ACTIONS(1556), 1,
+  [5601] = 1,
+    ACTIONS(1524), 1,
       anon_sym_DQUOTE,
-  [5774] = 1,
-    ACTIONS(1556), 1,
+  [5605] = 1,
+    ACTIONS(1524), 1,
       anon_sym_BQUOTE,
-  [5778] = 1,
-    ACTIONS(1558), 1,
+  [5609] = 1,
+    ACTIONS(1526), 1,
       aux_sym__string_token1,
-  [5782] = 1,
-    ACTIONS(1560), 1,
+  [5613] = 1,
+    ACTIONS(1528), 1,
       aux_sym__string_token2,
-  [5786] = 1,
-    ACTIONS(1562), 1,
+  [5617] = 1,
+    ACTIONS(1530), 1,
       aux_sym__string_token3,
-  [5790] = 1,
-    ACTIONS(1564), 1,
+  [5621] = 1,
+    ACTIONS(1532), 1,
       aux_sym_key_token1,
-  [5794] = 1,
-    ACTIONS(1566), 1,
+  [5625] = 1,
+    ACTIONS(1534), 1,
       aux_sym__string_token1,
-  [5798] = 1,
-    ACTIONS(1568), 1,
+  [5629] = 1,
+    ACTIONS(1536), 1,
       aux_sym__string_token2,
-  [5802] = 1,
-    ACTIONS(1570), 1,
+  [5633] = 1,
+    ACTIONS(1538), 1,
       aux_sym__string_token3,
-  [5806] = 1,
-    ACTIONS(1572), 1,
+  [5637] = 1,
+    ACTIONS(1540), 1,
       aux_sym__string_token1,
-  [5810] = 1,
-    ACTIONS(1574), 1,
+  [5641] = 1,
+    ACTIONS(1542), 1,
       aux_sym__string_token2,
-  [5814] = 1,
-    ACTIONS(1576), 1,
+  [5645] = 1,
+    ACTIONS(1544), 1,
       aux_sym__string_token3,
-  [5818] = 1,
-    ACTIONS(1578), 1,
+  [5649] = 1,
+    ACTIONS(1546), 1,
       aux_sym_key_token1,
-  [5822] = 1,
-    ACTIONS(1580), 1,
+  [5653] = 1,
+    ACTIONS(1548), 1,
       aux_sym__string_token1,
-  [5826] = 1,
-    ACTIONS(1582), 1,
+  [5657] = 1,
+    ACTIONS(1550), 1,
       aux_sym__string_token2,
-  [5830] = 1,
-    ACTIONS(1584), 1,
+  [5661] = 1,
+    ACTIONS(1552), 1,
       aux_sym__string_token3,
-  [5834] = 1,
-    ACTIONS(1586), 1,
+  [5665] = 1,
+    ACTIONS(1554), 1,
       aux_sym__string_token1,
-  [5838] = 1,
-    ACTIONS(1588), 1,
+  [5669] = 1,
+    ACTIONS(1556), 1,
       aux_sym__string_token2,
-  [5842] = 1,
-    ACTIONS(1590), 1,
+  [5673] = 1,
+    ACTIONS(1558), 1,
       aux_sym__string_token3,
-  [5846] = 1,
-    ACTIONS(1592), 1,
+  [5677] = 1,
+    ACTIONS(1560), 1,
       aux_sym__string_token1,
-  [5850] = 1,
-    ACTIONS(1594), 1,
+  [5681] = 1,
+    ACTIONS(1562), 1,
       aux_sym__string_token2,
-  [5854] = 1,
-    ACTIONS(1596), 1,
+  [5685] = 1,
+    ACTIONS(1564), 1,
       aux_sym__string_token3,
-  [5858] = 1,
-    ACTIONS(1598), 1,
+  [5689] = 1,
+    ACTIONS(1566), 1,
       aux_sym__string_token1,
-  [5862] = 1,
-    ACTIONS(1600), 1,
+  [5693] = 1,
+    ACTIONS(1568), 1,
       aux_sym__string_token2,
-  [5866] = 1,
-    ACTIONS(1602), 1,
+  [5697] = 1,
+    ACTIONS(1570), 1,
       aux_sym__string_token3,
-  [5870] = 1,
-    ACTIONS(1604), 1,
+  [5701] = 1,
+    ACTIONS(1572), 1,
       aux_sym__string_token1,
-  [5874] = 1,
-    ACTIONS(1606), 1,
+  [5705] = 1,
+    ACTIONS(1574), 1,
       aux_sym__string_token2,
-  [5878] = 1,
-    ACTIONS(1608), 1,
+  [5709] = 1,
+    ACTIONS(1576), 1,
       aux_sym__string_token3,
-  [5882] = 1,
-    ACTIONS(1610), 1,
+  [5713] = 1,
+    ACTIONS(1578), 1,
       aux_sym__string_token1,
-  [5886] = 1,
-    ACTIONS(1612), 1,
+  [5717] = 1,
+    ACTIONS(1580), 1,
       aux_sym__string_token2,
-  [5890] = 1,
-    ACTIONS(1614), 1,
+  [5721] = 1,
+    ACTIONS(1582), 1,
       aux_sym__string_token3,
-  [5894] = 1,
-    ACTIONS(1616), 1,
+  [5725] = 1,
+    ACTIONS(1584), 1,
       aux_sym__string_token1,
-  [5898] = 1,
-    ACTIONS(1618), 1,
+  [5729] = 1,
+    ACTIONS(1586), 1,
       aux_sym__string_token2,
-  [5902] = 1,
-    ACTIONS(1620), 1,
+  [5733] = 1,
+    ACTIONS(1588), 1,
       aux_sym__string_token3,
-  [5906] = 1,
-    ACTIONS(1622), 1,
+  [5737] = 1,
+    ACTIONS(1590), 1,
       aux_sym__string_token1,
-  [5910] = 1,
-    ACTIONS(1624), 1,
+  [5741] = 1,
+    ACTIONS(1592), 1,
       aux_sym__string_token2,
-  [5914] = 1,
-    ACTIONS(1626), 1,
+  [5745] = 1,
+    ACTIONS(1594), 1,
       aux_sym__string_token3,
 };
 
 static const uint32_t ts_small_parse_table_map[] = {
   [SMALL_STATE(26)] = 0,
-  [SMALL_STATE(27)] = 62,
-  [SMALL_STATE(28)] = 112,
-  [SMALL_STATE(29)] = 145,
-  [SMALL_STATE(30)] = 178,
-  [SMALL_STATE(31)] = 205,
-  [SMALL_STATE(32)] = 230,
-  [SMALL_STATE(33)] = 249,
-  [SMALL_STATE(34)] = 268,
-  [SMALL_STATE(35)] = 293,
-  [SMALL_STATE(36)] = 315,
-  [SMALL_STATE(37)] = 337,
-  [SMALL_STATE(38)] = 356,
-  [SMALL_STATE(39)] = 388,
-  [SMALL_STATE(40)] = 420,
-  [SMALL_STATE(41)] = 452,
-  [SMALL_STATE(42)] = 472,
-  [SMALL_STATE(43)] = 504,
-  [SMALL_STATE(44)] = 524,
-  [SMALL_STATE(45)] = 544,
-  [SMALL_STATE(46)] = 564,
-  [SMALL_STATE(47)] = 584,
-  [SMALL_STATE(48)] = 604,
-  [SMALL_STATE(49)] = 624,
-  [SMALL_STATE(50)] = 644,
-  [SMALL_STATE(51)] = 664,
-  [SMALL_STATE(52)] = 693,
-  [SMALL_STATE(53)] = 722,
-  [SMALL_STATE(54)] = 751,
-  [SMALL_STATE(55)] = 768,
-  [SMALL_STATE(56)] = 797,
-  [SMALL_STATE(57)] = 814,
-  [SMALL_STATE(58)] = 828,
-  [SMALL_STATE(59)] = 842,
-  [SMALL_STATE(60)] = 873,
-  [SMALL_STATE(61)] = 900,
-  [SMALL_STATE(62)] = 927,
-  [SMALL_STATE(63)] = 953,
-  [SMALL_STATE(64)] = 971,
-  [SMALL_STATE(65)] = 999,
-  [SMALL_STATE(66)] = 1025,
-  [SMALL_STATE(67)] = 1051,
-  [SMALL_STATE(68)] = 1077,
-  [SMALL_STATE(69)] = 1095,
-  [SMALL_STATE(70)] = 1121,
-  [SMALL_STATE(71)] = 1144,
-  [SMALL_STATE(72)] = 1167,
-  [SMALL_STATE(73)] = 1192,
-  [SMALL_STATE(74)] = 1215,
-  [SMALL_STATE(75)] = 1238,
-  [SMALL_STATE(76)] = 1249,
-  [SMALL_STATE(77)] = 1272,
-  [SMALL_STATE(78)] = 1295,
-  [SMALL_STATE(79)] = 1318,
-  [SMALL_STATE(80)] = 1341,
-  [SMALL_STATE(81)] = 1366,
-  [SMALL_STATE(82)] = 1383,
-  [SMALL_STATE(83)] = 1406,
-  [SMALL_STATE(84)] = 1429,
-  [SMALL_STATE(85)] = 1454,
-  [SMALL_STATE(86)] = 1477,
-  [SMALL_STATE(87)] = 1500,
-  [SMALL_STATE(88)] = 1523,
-  [SMALL_STATE(89)] = 1543,
-  [SMALL_STATE(90)] = 1563,
-  [SMALL_STATE(91)] = 1583,
-  [SMALL_STATE(92)] = 1603,
-  [SMALL_STATE(93)] = 1623,
-  [SMALL_STATE(94)] = 1643,
-  [SMALL_STATE(95)] = 1663,
-  [SMALL_STATE(96)] = 1683,
-  [SMALL_STATE(97)] = 1703,
-  [SMALL_STATE(98)] = 1719,
-  [SMALL_STATE(99)] = 1735,
-  [SMALL_STATE(100)] = 1755,
-  [SMALL_STATE(101)] = 1775,
-  [SMALL_STATE(102)] = 1795,
-  [SMALL_STATE(103)] = 1815,
-  [SMALL_STATE(104)] = 1835,
-  [SMALL_STATE(105)] = 1855,
-  [SMALL_STATE(106)] = 1875,
-  [SMALL_STATE(107)] = 1897,
-  [SMALL_STATE(108)] = 1919,
-  [SMALL_STATE(109)] = 1939,
-  [SMALL_STATE(110)] = 1959,
-  [SMALL_STATE(111)] = 1981,
-  [SMALL_STATE(112)] = 2001,
-  [SMALL_STATE(113)] = 2021,
-  [SMALL_STATE(114)] = 2041,
-  [SMALL_STATE(115)] = 2061,
-  [SMALL_STATE(116)] = 2081,
-  [SMALL_STATE(117)] = 2101,
-  [SMALL_STATE(118)] = 2121,
-  [SMALL_STATE(119)] = 2141,
-  [SMALL_STATE(120)] = 2163,
-  [SMALL_STATE(121)] = 2183,
-  [SMALL_STATE(122)] = 2203,
-  [SMALL_STATE(123)] = 2223,
-  [SMALL_STATE(124)] = 2243,
-  [SMALL_STATE(125)] = 2263,
-  [SMALL_STATE(126)] = 2283,
-  [SMALL_STATE(127)] = 2305,
-  [SMALL_STATE(128)] = 2325,
-  [SMALL_STATE(129)] = 2345,
-  [SMALL_STATE(130)] = 2365,
-  [SMALL_STATE(131)] = 2385,
-  [SMALL_STATE(132)] = 2405,
-  [SMALL_STATE(133)] = 2425,
-  [SMALL_STATE(134)] = 2445,
-  [SMALL_STATE(135)] = 2465,
-  [SMALL_STATE(136)] = 2487,
-  [SMALL_STATE(137)] = 2507,
-  [SMALL_STATE(138)] = 2527,
-  [SMALL_STATE(139)] = 2547,
-  [SMALL_STATE(140)] = 2567,
-  [SMALL_STATE(141)] = 2587,
-  [SMALL_STATE(142)] = 2609,
-  [SMALL_STATE(143)] = 2629,
-  [SMALL_STATE(144)] = 2649,
-  [SMALL_STATE(145)] = 2669,
-  [SMALL_STATE(146)] = 2689,
-  [SMALL_STATE(147)] = 2709,
-  [SMALL_STATE(148)] = 2729,
-  [SMALL_STATE(149)] = 2751,
-  [SMALL_STATE(150)] = 2770,
-  [SMALL_STATE(151)] = 2787,
-  [SMALL_STATE(152)] = 2806,
-  [SMALL_STATE(153)] = 2815,
-  [SMALL_STATE(154)] = 2824,
-  [SMALL_STATE(155)] = 2833,
-  [SMALL_STATE(156)] = 2852,
-  [SMALL_STATE(157)] = 2861,
-  [SMALL_STATE(158)] = 2880,
-  [SMALL_STATE(159)] = 2897,
-  [SMALL_STATE(160)] = 2916,
-  [SMALL_STATE(161)] = 2935,
-  [SMALL_STATE(162)] = 2946,
-  [SMALL_STATE(163)] = 2965,
-  [SMALL_STATE(164)] = 2982,
-  [SMALL_STATE(165)] = 2991,
-  [SMALL_STATE(166)] = 3000,
-  [SMALL_STATE(167)] = 3009,
-  [SMALL_STATE(168)] = 3028,
-  [SMALL_STATE(169)] = 3041,
-  [SMALL_STATE(170)] = 3060,
-  [SMALL_STATE(171)] = 3079,
-  [SMALL_STATE(172)] = 3090,
-  [SMALL_STATE(173)] = 3107,
-  [SMALL_STATE(174)] = 3126,
-  [SMALL_STATE(175)] = 3135,
-  [SMALL_STATE(176)] = 3146,
-  [SMALL_STATE(177)] = 3165,
-  [SMALL_STATE(178)] = 3184,
-  [SMALL_STATE(179)] = 3201,
-  [SMALL_STATE(180)] = 3218,
-  [SMALL_STATE(181)] = 3227,
-  [SMALL_STATE(182)] = 3244,
-  [SMALL_STATE(183)] = 3261,
-  [SMALL_STATE(184)] = 3280,
-  [SMALL_STATE(185)] = 3292,
-  [SMALL_STATE(186)] = 3306,
-  [SMALL_STATE(187)] = 3322,
-  [SMALL_STATE(188)] = 3334,
-  [SMALL_STATE(189)] = 3342,
-  [SMALL_STATE(190)] = 3356,
-  [SMALL_STATE(191)] = 3370,
-  [SMALL_STATE(192)] = 3384,
-  [SMALL_STATE(193)] = 3396,
-  [SMALL_STATE(194)] = 3404,
-  [SMALL_STATE(195)] = 3412,
-  [SMALL_STATE(196)] = 3420,
-  [SMALL_STATE(197)] = 3434,
-  [SMALL_STATE(198)] = 3448,
-  [SMALL_STATE(199)] = 3460,
-  [SMALL_STATE(200)] = 3468,
-  [SMALL_STATE(201)] = 3476,
-  [SMALL_STATE(202)] = 3484,
-  [SMALL_STATE(203)] = 3492,
-  [SMALL_STATE(204)] = 3500,
-  [SMALL_STATE(205)] = 3508,
-  [SMALL_STATE(206)] = 3516,
-  [SMALL_STATE(207)] = 3528,
-  [SMALL_STATE(208)] = 3540,
-  [SMALL_STATE(209)] = 3552,
-  [SMALL_STATE(210)] = 3564,
-  [SMALL_STATE(211)] = 3576,
-  [SMALL_STATE(212)] = 3588,
-  [SMALL_STATE(213)] = 3600,
-  [SMALL_STATE(214)] = 3612,
-  [SMALL_STATE(215)] = 3624,
-  [SMALL_STATE(216)] = 3636,
-  [SMALL_STATE(217)] = 3648,
-  [SMALL_STATE(218)] = 3660,
-  [SMALL_STATE(219)] = 3672,
-  [SMALL_STATE(220)] = 3686,
-  [SMALL_STATE(221)] = 3698,
-  [SMALL_STATE(222)] = 3710,
-  [SMALL_STATE(223)] = 3722,
-  [SMALL_STATE(224)] = 3734,
-  [SMALL_STATE(225)] = 3746,
-  [SMALL_STATE(226)] = 3758,
-  [SMALL_STATE(227)] = 3770,
-  [SMALL_STATE(228)] = 3782,
-  [SMALL_STATE(229)] = 3794,
-  [SMALL_STATE(230)] = 3806,
-  [SMALL_STATE(231)] = 3818,
-  [SMALL_STATE(232)] = 3830,
-  [SMALL_STATE(233)] = 3842,
-  [SMALL_STATE(234)] = 3854,
-  [SMALL_STATE(235)] = 3862,
-  [SMALL_STATE(236)] = 3874,
-  [SMALL_STATE(237)] = 3884,
-  [SMALL_STATE(238)] = 3896,
-  [SMALL_STATE(239)] = 3908,
-  [SMALL_STATE(240)] = 3920,
-  [SMALL_STATE(241)] = 3932,
-  [SMALL_STATE(242)] = 3944,
-  [SMALL_STATE(243)] = 3956,
-  [SMALL_STATE(244)] = 3968,
-  [SMALL_STATE(245)] = 3980,
-  [SMALL_STATE(246)] = 3992,
-  [SMALL_STATE(247)] = 4004,
-  [SMALL_STATE(248)] = 4016,
-  [SMALL_STATE(249)] = 4028,
-  [SMALL_STATE(250)] = 4040,
-  [SMALL_STATE(251)] = 4052,
-  [SMALL_STATE(252)] = 4064,
-  [SMALL_STATE(253)] = 4078,
-  [SMALL_STATE(254)] = 4086,
-  [SMALL_STATE(255)] = 4098,
-  [SMALL_STATE(256)] = 4110,
-  [SMALL_STATE(257)] = 4122,
-  [SMALL_STATE(258)] = 4134,
-  [SMALL_STATE(259)] = 4146,
-  [SMALL_STATE(260)] = 4158,
-  [SMALL_STATE(261)] = 4170,
-  [SMALL_STATE(262)] = 4178,
-  [SMALL_STATE(263)] = 4190,
-  [SMALL_STATE(264)] = 4197,
-  [SMALL_STATE(265)] = 4204,
-  [SMALL_STATE(266)] = 4217,
-  [SMALL_STATE(267)] = 4230,
-  [SMALL_STATE(268)] = 4237,
-  [SMALL_STATE(269)] = 4244,
-  [SMALL_STATE(270)] = 4251,
-  [SMALL_STATE(271)] = 4258,
-  [SMALL_STATE(272)] = 4265,
-  [SMALL_STATE(273)] = 4272,
-  [SMALL_STATE(274)] = 4279,
-  [SMALL_STATE(275)] = 4292,
-  [SMALL_STATE(276)] = 4299,
-  [SMALL_STATE(277)] = 4306,
-  [SMALL_STATE(278)] = 4313,
-  [SMALL_STATE(279)] = 4320,
-  [SMALL_STATE(280)] = 4327,
-  [SMALL_STATE(281)] = 4334,
-  [SMALL_STATE(282)] = 4341,
-  [SMALL_STATE(283)] = 4348,
-  [SMALL_STATE(284)] = 4355,
-  [SMALL_STATE(285)] = 4362,
-  [SMALL_STATE(286)] = 4375,
-  [SMALL_STATE(287)] = 4382,
-  [SMALL_STATE(288)] = 4391,
-  [SMALL_STATE(289)] = 4402,
-  [SMALL_STATE(290)] = 4409,
-  [SMALL_STATE(291)] = 4416,
-  [SMALL_STATE(292)] = 4423,
-  [SMALL_STATE(293)] = 4430,
-  [SMALL_STATE(294)] = 4437,
-  [SMALL_STATE(295)] = 4444,
-  [SMALL_STATE(296)] = 4451,
-  [SMALL_STATE(297)] = 4458,
-  [SMALL_STATE(298)] = 4465,
-  [SMALL_STATE(299)] = 4476,
-  [SMALL_STATE(300)] = 4483,
-  [SMALL_STATE(301)] = 4490,
-  [SMALL_STATE(302)] = 4497,
-  [SMALL_STATE(303)] = 4504,
-  [SMALL_STATE(304)] = 4511,
-  [SMALL_STATE(305)] = 4518,
-  [SMALL_STATE(306)] = 4525,
-  [SMALL_STATE(307)] = 4532,
-  [SMALL_STATE(308)] = 4539,
-  [SMALL_STATE(309)] = 4546,
-  [SMALL_STATE(310)] = 4553,
-  [SMALL_STATE(311)] = 4559,
-  [SMALL_STATE(312)] = 4565,
-  [SMALL_STATE(313)] = 4571,
-  [SMALL_STATE(314)] = 4577,
-  [SMALL_STATE(315)] = 4583,
-  [SMALL_STATE(316)] = 4589,
-  [SMALL_STATE(317)] = 4595,
-  [SMALL_STATE(318)] = 4601,
-  [SMALL_STATE(319)] = 4607,
-  [SMALL_STATE(320)] = 4613,
-  [SMALL_STATE(321)] = 4619,
-  [SMALL_STATE(322)] = 4625,
-  [SMALL_STATE(323)] = 4631,
-  [SMALL_STATE(324)] = 4637,
-  [SMALL_STATE(325)] = 4643,
-  [SMALL_STATE(326)] = 4649,
-  [SMALL_STATE(327)] = 4655,
-  [SMALL_STATE(328)] = 4661,
-  [SMALL_STATE(329)] = 4671,
-  [SMALL_STATE(330)] = 4677,
-  [SMALL_STATE(331)] = 4683,
-  [SMALL_STATE(332)] = 4689,
-  [SMALL_STATE(333)] = 4695,
-  [SMALL_STATE(334)] = 4701,
-  [SMALL_STATE(335)] = 4707,
-  [SMALL_STATE(336)] = 4713,
-  [SMALL_STATE(337)] = 4719,
-  [SMALL_STATE(338)] = 4725,
-  [SMALL_STATE(339)] = 4731,
-  [SMALL_STATE(340)] = 4737,
-  [SMALL_STATE(341)] = 4743,
-  [SMALL_STATE(342)] = 4749,
-  [SMALL_STATE(343)] = 4755,
-  [SMALL_STATE(344)] = 4761,
-  [SMALL_STATE(345)] = 4767,
-  [SMALL_STATE(346)] = 4773,
-  [SMALL_STATE(347)] = 4779,
-  [SMALL_STATE(348)] = 4785,
-  [SMALL_STATE(349)] = 4791,
-  [SMALL_STATE(350)] = 4797,
-  [SMALL_STATE(351)] = 4803,
-  [SMALL_STATE(352)] = 4809,
-  [SMALL_STATE(353)] = 4815,
-  [SMALL_STATE(354)] = 4821,
-  [SMALL_STATE(355)] = 4827,
-  [SMALL_STATE(356)] = 4833,
-  [SMALL_STATE(357)] = 4839,
-  [SMALL_STATE(358)] = 4845,
-  [SMALL_STATE(359)] = 4851,
-  [SMALL_STATE(360)] = 4857,
-  [SMALL_STATE(361)] = 4863,
-  [SMALL_STATE(362)] = 4869,
-  [SMALL_STATE(363)] = 4875,
-  [SMALL_STATE(364)] = 4881,
-  [SMALL_STATE(365)] = 4887,
-  [SMALL_STATE(366)] = 4893,
-  [SMALL_STATE(367)] = 4899,
-  [SMALL_STATE(368)] = 4905,
-  [SMALL_STATE(369)] = 4911,
-  [SMALL_STATE(370)] = 4917,
-  [SMALL_STATE(371)] = 4923,
-  [SMALL_STATE(372)] = 4929,
-  [SMALL_STATE(373)] = 4935,
-  [SMALL_STATE(374)] = 4941,
-  [SMALL_STATE(375)] = 4947,
-  [SMALL_STATE(376)] = 4953,
-  [SMALL_STATE(377)] = 4959,
-  [SMALL_STATE(378)] = 4965,
-  [SMALL_STATE(379)] = 4971,
-  [SMALL_STATE(380)] = 4977,
-  [SMALL_STATE(381)] = 4983,
-  [SMALL_STATE(382)] = 4989,
-  [SMALL_STATE(383)] = 4995,
-  [SMALL_STATE(384)] = 5001,
-  [SMALL_STATE(385)] = 5007,
-  [SMALL_STATE(386)] = 5013,
-  [SMALL_STATE(387)] = 5021,
-  [SMALL_STATE(388)] = 5027,
-  [SMALL_STATE(389)] = 5037,
-  [SMALL_STATE(390)] = 5047,
-  [SMALL_STATE(391)] = 5053,
-  [SMALL_STATE(392)] = 5059,
-  [SMALL_STATE(393)] = 5065,
-  [SMALL_STATE(394)] = 5071,
-  [SMALL_STATE(395)] = 5077,
-  [SMALL_STATE(396)] = 5083,
-  [SMALL_STATE(397)] = 5089,
-  [SMALL_STATE(398)] = 5095,
-  [SMALL_STATE(399)] = 5101,
-  [SMALL_STATE(400)] = 5107,
-  [SMALL_STATE(401)] = 5113,
-  [SMALL_STATE(402)] = 5119,
-  [SMALL_STATE(403)] = 5125,
-  [SMALL_STATE(404)] = 5131,
-  [SMALL_STATE(405)] = 5137,
-  [SMALL_STATE(406)] = 5143,
-  [SMALL_STATE(407)] = 5149,
-  [SMALL_STATE(408)] = 5155,
-  [SMALL_STATE(409)] = 5161,
-  [SMALL_STATE(410)] = 5167,
-  [SMALL_STATE(411)] = 5173,
-  [SMALL_STATE(412)] = 5179,
-  [SMALL_STATE(413)] = 5185,
-  [SMALL_STATE(414)] = 5191,
-  [SMALL_STATE(415)] = 5197,
-  [SMALL_STATE(416)] = 5203,
-  [SMALL_STATE(417)] = 5209,
-  [SMALL_STATE(418)] = 5215,
-  [SMALL_STATE(419)] = 5221,
-  [SMALL_STATE(420)] = 5227,
-  [SMALL_STATE(421)] = 5233,
-  [SMALL_STATE(422)] = 5239,
-  [SMALL_STATE(423)] = 5245,
-  [SMALL_STATE(424)] = 5251,
-  [SMALL_STATE(425)] = 5257,
-  [SMALL_STATE(426)] = 5263,
-  [SMALL_STATE(427)] = 5269,
-  [SMALL_STATE(428)] = 5279,
-  [SMALL_STATE(429)] = 5285,
-  [SMALL_STATE(430)] = 5291,
-  [SMALL_STATE(431)] = 5297,
-  [SMALL_STATE(432)] = 5303,
-  [SMALL_STATE(433)] = 5309,
-  [SMALL_STATE(434)] = 5315,
-  [SMALL_STATE(435)] = 5321,
-  [SMALL_STATE(436)] = 5327,
-  [SMALL_STATE(437)] = 5333,
-  [SMALL_STATE(438)] = 5339,
-  [SMALL_STATE(439)] = 5345,
-  [SMALL_STATE(440)] = 5351,
-  [SMALL_STATE(441)] = 5357,
-  [SMALL_STATE(442)] = 5363,
-  [SMALL_STATE(443)] = 5369,
-  [SMALL_STATE(444)] = 5375,
-  [SMALL_STATE(445)] = 5381,
-  [SMALL_STATE(446)] = 5387,
-  [SMALL_STATE(447)] = 5393,
-  [SMALL_STATE(448)] = 5399,
-  [SMALL_STATE(449)] = 5405,
-  [SMALL_STATE(450)] = 5412,
-  [SMALL_STATE(451)] = 5419,
-  [SMALL_STATE(452)] = 5426,
-  [SMALL_STATE(453)] = 5433,
-  [SMALL_STATE(454)] = 5440,
-  [SMALL_STATE(455)] = 5447,
-  [SMALL_STATE(456)] = 5454,
-  [SMALL_STATE(457)] = 5461,
-  [SMALL_STATE(458)] = 5468,
-  [SMALL_STATE(459)] = 5475,
-  [SMALL_STATE(460)] = 5482,
-  [SMALL_STATE(461)] = 5489,
-  [SMALL_STATE(462)] = 5496,
-  [SMALL_STATE(463)] = 5503,
-  [SMALL_STATE(464)] = 5510,
-  [SMALL_STATE(465)] = 5514,
-  [SMALL_STATE(466)] = 5518,
-  [SMALL_STATE(467)] = 5522,
-  [SMALL_STATE(468)] = 5526,
-  [SMALL_STATE(469)] = 5530,
-  [SMALL_STATE(470)] = 5534,
-  [SMALL_STATE(471)] = 5538,
-  [SMALL_STATE(472)] = 5542,
-  [SMALL_STATE(473)] = 5546,
-  [SMALL_STATE(474)] = 5550,
-  [SMALL_STATE(475)] = 5554,
-  [SMALL_STATE(476)] = 5558,
-  [SMALL_STATE(477)] = 5562,
-  [SMALL_STATE(478)] = 5566,
-  [SMALL_STATE(479)] = 5570,
-  [SMALL_STATE(480)] = 5574,
-  [SMALL_STATE(481)] = 5578,
-  [SMALL_STATE(482)] = 5582,
-  [SMALL_STATE(483)] = 5586,
-  [SMALL_STATE(484)] = 5590,
-  [SMALL_STATE(485)] = 5594,
-  [SMALL_STATE(486)] = 5598,
-  [SMALL_STATE(487)] = 5602,
-  [SMALL_STATE(488)] = 5606,
-  [SMALL_STATE(489)] = 5610,
-  [SMALL_STATE(490)] = 5614,
-  [SMALL_STATE(491)] = 5618,
-  [SMALL_STATE(492)] = 5622,
-  [SMALL_STATE(493)] = 5626,
-  [SMALL_STATE(494)] = 5630,
-  [SMALL_STATE(495)] = 5634,
-  [SMALL_STATE(496)] = 5638,
-  [SMALL_STATE(497)] = 5642,
-  [SMALL_STATE(498)] = 5646,
-  [SMALL_STATE(499)] = 5650,
-  [SMALL_STATE(500)] = 5654,
-  [SMALL_STATE(501)] = 5658,
-  [SMALL_STATE(502)] = 5662,
-  [SMALL_STATE(503)] = 5666,
-  [SMALL_STATE(504)] = 5670,
-  [SMALL_STATE(505)] = 5674,
-  [SMALL_STATE(506)] = 5678,
-  [SMALL_STATE(507)] = 5682,
-  [SMALL_STATE(508)] = 5686,
-  [SMALL_STATE(509)] = 5690,
-  [SMALL_STATE(510)] = 5694,
-  [SMALL_STATE(511)] = 5698,
-  [SMALL_STATE(512)] = 5702,
-  [SMALL_STATE(513)] = 5706,
-  [SMALL_STATE(514)] = 5710,
-  [SMALL_STATE(515)] = 5714,
-  [SMALL_STATE(516)] = 5718,
-  [SMALL_STATE(517)] = 5722,
-  [SMALL_STATE(518)] = 5726,
-  [SMALL_STATE(519)] = 5730,
-  [SMALL_STATE(520)] = 5734,
-  [SMALL_STATE(521)] = 5738,
-  [SMALL_STATE(522)] = 5742,
-  [SMALL_STATE(523)] = 5746,
-  [SMALL_STATE(524)] = 5750,
-  [SMALL_STATE(525)] = 5754,
-  [SMALL_STATE(526)] = 5758,
-  [SMALL_STATE(527)] = 5762,
-  [SMALL_STATE(528)] = 5766,
-  [SMALL_STATE(529)] = 5770,
-  [SMALL_STATE(530)] = 5774,
-  [SMALL_STATE(531)] = 5778,
-  [SMALL_STATE(532)] = 5782,
-  [SMALL_STATE(533)] = 5786,
-  [SMALL_STATE(534)] = 5790,
-  [SMALL_STATE(535)] = 5794,
-  [SMALL_STATE(536)] = 5798,
-  [SMALL_STATE(537)] = 5802,
-  [SMALL_STATE(538)] = 5806,
-  [SMALL_STATE(539)] = 5810,
-  [SMALL_STATE(540)] = 5814,
-  [SMALL_STATE(541)] = 5818,
-  [SMALL_STATE(542)] = 5822,
-  [SMALL_STATE(543)] = 5826,
-  [SMALL_STATE(544)] = 5830,
-  [SMALL_STATE(545)] = 5834,
-  [SMALL_STATE(546)] = 5838,
-  [SMALL_STATE(547)] = 5842,
-  [SMALL_STATE(548)] = 5846,
-  [SMALL_STATE(549)] = 5850,
-  [SMALL_STATE(550)] = 5854,
-  [SMALL_STATE(551)] = 5858,
-  [SMALL_STATE(552)] = 5862,
-  [SMALL_STATE(553)] = 5866,
-  [SMALL_STATE(554)] = 5870,
-  [SMALL_STATE(555)] = 5874,
-  [SMALL_STATE(556)] = 5878,
-  [SMALL_STATE(557)] = 5882,
-  [SMALL_STATE(558)] = 5886,
-  [SMALL_STATE(559)] = 5890,
-  [SMALL_STATE(560)] = 5894,
-  [SMALL_STATE(561)] = 5898,
-  [SMALL_STATE(562)] = 5902,
-  [SMALL_STATE(563)] = 5906,
-  [SMALL_STATE(564)] = 5910,
-  [SMALL_STATE(565)] = 5914,
+  [SMALL_STATE(27)] = 61,
+  [SMALL_STATE(28)] = 111,
+  [SMALL_STATE(29)] = 144,
+  [SMALL_STATE(30)] = 171,
+  [SMALL_STATE(31)] = 204,
+  [SMALL_STATE(32)] = 223,
+  [SMALL_STATE(33)] = 242,
+  [SMALL_STATE(34)] = 267,
+  [SMALL_STATE(35)] = 292,
+  [SMALL_STATE(36)] = 314,
+  [SMALL_STATE(37)] = 336,
+  [SMALL_STATE(38)] = 355,
+  [SMALL_STATE(39)] = 375,
+  [SMALL_STATE(40)] = 395,
+  [SMALL_STATE(41)] = 415,
+  [SMALL_STATE(42)] = 435,
+  [SMALL_STATE(43)] = 455,
+  [SMALL_STATE(44)] = 475,
+  [SMALL_STATE(45)] = 495,
+  [SMALL_STATE(46)] = 515,
+  [SMALL_STATE(47)] = 535,
+  [SMALL_STATE(48)] = 566,
+  [SMALL_STATE(49)] = 583,
+  [SMALL_STATE(50)] = 600,
+  [SMALL_STATE(51)] = 631,
+  [SMALL_STATE(52)] = 662,
+  [SMALL_STATE(53)] = 693,
+  [SMALL_STATE(54)] = 707,
+  [SMALL_STATE(55)] = 735,
+  [SMALL_STATE(56)] = 763,
+  [SMALL_STATE(57)] = 791,
+  [SMALL_STATE(58)] = 805,
+  [SMALL_STATE(59)] = 833,
+  [SMALL_STATE(60)] = 861,
+  [SMALL_STATE(61)] = 887,
+  [SMALL_STATE(62)] = 913,
+  [SMALL_STATE(63)] = 930,
+  [SMALL_STATE(64)] = 955,
+  [SMALL_STATE(65)] = 980,
+  [SMALL_STATE(66)] = 1003,
+  [SMALL_STATE(67)] = 1028,
+  [SMALL_STATE(68)] = 1053,
+  [SMALL_STATE(69)] = 1070,
+  [SMALL_STATE(70)] = 1087,
+  [SMALL_STATE(71)] = 1112,
+  [SMALL_STATE(72)] = 1137,
+  [SMALL_STATE(73)] = 1158,
+  [SMALL_STATE(74)] = 1179,
+  [SMALL_STATE(75)] = 1201,
+  [SMALL_STATE(76)] = 1223,
+  [SMALL_STATE(77)] = 1243,
+  [SMALL_STATE(78)] = 1265,
+  [SMALL_STATE(79)] = 1275,
+  [SMALL_STATE(80)] = 1297,
+  [SMALL_STATE(81)] = 1319,
+  [SMALL_STATE(82)] = 1341,
+  [SMALL_STATE(83)] = 1363,
+  [SMALL_STATE(84)] = 1385,
+  [SMALL_STATE(85)] = 1407,
+  [SMALL_STATE(86)] = 1417,
+  [SMALL_STATE(87)] = 1439,
+  [SMALL_STATE(88)] = 1461,
+  [SMALL_STATE(89)] = 1483,
+  [SMALL_STATE(90)] = 1505,
+  [SMALL_STATE(91)] = 1521,
+  [SMALL_STATE(92)] = 1543,
+  [SMALL_STATE(93)] = 1559,
+  [SMALL_STATE(94)] = 1569,
+  [SMALL_STATE(95)] = 1591,
+  [SMALL_STATE(96)] = 1610,
+  [SMALL_STATE(97)] = 1629,
+  [SMALL_STATE(98)] = 1640,
+  [SMALL_STATE(99)] = 1659,
+  [SMALL_STATE(100)] = 1678,
+  [SMALL_STATE(101)] = 1697,
+  [SMALL_STATE(102)] = 1716,
+  [SMALL_STATE(103)] = 1735,
+  [SMALL_STATE(104)] = 1744,
+  [SMALL_STATE(105)] = 1763,
+  [SMALL_STATE(106)] = 1782,
+  [SMALL_STATE(107)] = 1795,
+  [SMALL_STATE(108)] = 1812,
+  [SMALL_STATE(109)] = 1831,
+  [SMALL_STATE(110)] = 1850,
+  [SMALL_STATE(111)] = 1869,
+  [SMALL_STATE(112)] = 1888,
+  [SMALL_STATE(113)] = 1907,
+  [SMALL_STATE(114)] = 1926,
+  [SMALL_STATE(115)] = 1945,
+  [SMALL_STATE(116)] = 1964,
+  [SMALL_STATE(117)] = 1983,
+  [SMALL_STATE(118)] = 2002,
+  [SMALL_STATE(119)] = 2021,
+  [SMALL_STATE(120)] = 2040,
+  [SMALL_STATE(121)] = 2059,
+  [SMALL_STATE(122)] = 2078,
+  [SMALL_STATE(123)] = 2097,
+  [SMALL_STATE(124)] = 2116,
+  [SMALL_STATE(125)] = 2135,
+  [SMALL_STATE(126)] = 2154,
+  [SMALL_STATE(127)] = 2173,
+  [SMALL_STATE(128)] = 2192,
+  [SMALL_STATE(129)] = 2211,
+  [SMALL_STATE(130)] = 2230,
+  [SMALL_STATE(131)] = 2249,
+  [SMALL_STATE(132)] = 2260,
+  [SMALL_STATE(133)] = 2279,
+  [SMALL_STATE(134)] = 2298,
+  [SMALL_STATE(135)] = 2317,
+  [SMALL_STATE(136)] = 2336,
+  [SMALL_STATE(137)] = 2355,
+  [SMALL_STATE(138)] = 2374,
+  [SMALL_STATE(139)] = 2393,
+  [SMALL_STATE(140)] = 2412,
+  [SMALL_STATE(141)] = 2431,
+  [SMALL_STATE(142)] = 2450,
+  [SMALL_STATE(143)] = 2469,
+  [SMALL_STATE(144)] = 2488,
+  [SMALL_STATE(145)] = 2507,
+  [SMALL_STATE(146)] = 2526,
+  [SMALL_STATE(147)] = 2545,
+  [SMALL_STATE(148)] = 2564,
+  [SMALL_STATE(149)] = 2583,
+  [SMALL_STATE(150)] = 2602,
+  [SMALL_STATE(151)] = 2621,
+  [SMALL_STATE(152)] = 2640,
+  [SMALL_STATE(153)] = 2659,
+  [SMALL_STATE(154)] = 2670,
+  [SMALL_STATE(155)] = 2689,
+  [SMALL_STATE(156)] = 2708,
+  [SMALL_STATE(157)] = 2727,
+  [SMALL_STATE(158)] = 2746,
+  [SMALL_STATE(159)] = 2765,
+  [SMALL_STATE(160)] = 2784,
+  [SMALL_STATE(161)] = 2803,
+  [SMALL_STATE(162)] = 2815,
+  [SMALL_STATE(163)] = 2827,
+  [SMALL_STATE(164)] = 2839,
+  [SMALL_STATE(165)] = 2851,
+  [SMALL_STATE(166)] = 2863,
+  [SMALL_STATE(167)] = 2879,
+  [SMALL_STATE(168)] = 2887,
+  [SMALL_STATE(169)] = 2899,
+  [SMALL_STATE(170)] = 2913,
+  [SMALL_STATE(171)] = 2927,
+  [SMALL_STATE(172)] = 2941,
+  [SMALL_STATE(173)] = 2953,
+  [SMALL_STATE(174)] = 2965,
+  [SMALL_STATE(175)] = 2977,
+  [SMALL_STATE(176)] = 2989,
+  [SMALL_STATE(177)] = 3005,
+  [SMALL_STATE(178)] = 3017,
+  [SMALL_STATE(179)] = 3029,
+  [SMALL_STATE(180)] = 3041,
+  [SMALL_STATE(181)] = 3053,
+  [SMALL_STATE(182)] = 3061,
+  [SMALL_STATE(183)] = 3069,
+  [SMALL_STATE(184)] = 3077,
+  [SMALL_STATE(185)] = 3085,
+  [SMALL_STATE(186)] = 3093,
+  [SMALL_STATE(187)] = 3109,
+  [SMALL_STATE(188)] = 3117,
+  [SMALL_STATE(189)] = 3129,
+  [SMALL_STATE(190)] = 3145,
+  [SMALL_STATE(191)] = 3161,
+  [SMALL_STATE(192)] = 3173,
+  [SMALL_STATE(193)] = 3185,
+  [SMALL_STATE(194)] = 3199,
+  [SMALL_STATE(195)] = 3211,
+  [SMALL_STATE(196)] = 3223,
+  [SMALL_STATE(197)] = 3235,
+  [SMALL_STATE(198)] = 3247,
+  [SMALL_STATE(199)] = 3263,
+  [SMALL_STATE(200)] = 3277,
+  [SMALL_STATE(201)] = 3285,
+  [SMALL_STATE(202)] = 3297,
+  [SMALL_STATE(203)] = 3313,
+  [SMALL_STATE(204)] = 3329,
+  [SMALL_STATE(205)] = 3345,
+  [SMALL_STATE(206)] = 3357,
+  [SMALL_STATE(207)] = 3367,
+  [SMALL_STATE(208)] = 3379,
+  [SMALL_STATE(209)] = 3391,
+  [SMALL_STATE(210)] = 3403,
+  [SMALL_STATE(211)] = 3415,
+  [SMALL_STATE(212)] = 3427,
+  [SMALL_STATE(213)] = 3439,
+  [SMALL_STATE(214)] = 3451,
+  [SMALL_STATE(215)] = 3467,
+  [SMALL_STATE(216)] = 3479,
+  [SMALL_STATE(217)] = 3491,
+  [SMALL_STATE(218)] = 3505,
+  [SMALL_STATE(219)] = 3517,
+  [SMALL_STATE(220)] = 3529,
+  [SMALL_STATE(221)] = 3541,
+  [SMALL_STATE(222)] = 3557,
+  [SMALL_STATE(223)] = 3573,
+  [SMALL_STATE(224)] = 3585,
+  [SMALL_STATE(225)] = 3597,
+  [SMALL_STATE(226)] = 3609,
+  [SMALL_STATE(227)] = 3621,
+  [SMALL_STATE(228)] = 3633,
+  [SMALL_STATE(229)] = 3645,
+  [SMALL_STATE(230)] = 3657,
+  [SMALL_STATE(231)] = 3673,
+  [SMALL_STATE(232)] = 3685,
+  [SMALL_STATE(233)] = 3699,
+  [SMALL_STATE(234)] = 3711,
+  [SMALL_STATE(235)] = 3723,
+  [SMALL_STATE(236)] = 3735,
+  [SMALL_STATE(237)] = 3751,
+  [SMALL_STATE(238)] = 3763,
+  [SMALL_STATE(239)] = 3775,
+  [SMALL_STATE(240)] = 3787,
+  [SMALL_STATE(241)] = 3799,
+  [SMALL_STATE(242)] = 3811,
+  [SMALL_STATE(243)] = 3827,
+  [SMALL_STATE(244)] = 3839,
+  [SMALL_STATE(245)] = 3851,
+  [SMALL_STATE(246)] = 3867,
+  [SMALL_STATE(247)] = 3879,
+  [SMALL_STATE(248)] = 3891,
+  [SMALL_STATE(249)] = 3907,
+  [SMALL_STATE(250)] = 3923,
+  [SMALL_STATE(251)] = 3937,
+  [SMALL_STATE(252)] = 3944,
+  [SMALL_STATE(253)] = 3951,
+  [SMALL_STATE(254)] = 3958,
+  [SMALL_STATE(255)] = 3969,
+  [SMALL_STATE(256)] = 3976,
+  [SMALL_STATE(257)] = 3983,
+  [SMALL_STATE(258)] = 3990,
+  [SMALL_STATE(259)] = 3997,
+  [SMALL_STATE(260)] = 4006,
+  [SMALL_STATE(261)] = 4019,
+  [SMALL_STATE(262)] = 4026,
+  [SMALL_STATE(263)] = 4033,
+  [SMALL_STATE(264)] = 4040,
+  [SMALL_STATE(265)] = 4047,
+  [SMALL_STATE(266)] = 4054,
+  [SMALL_STATE(267)] = 4061,
+  [SMALL_STATE(268)] = 4068,
+  [SMALL_STATE(269)] = 4075,
+  [SMALL_STATE(270)] = 4082,
+  [SMALL_STATE(271)] = 4089,
+  [SMALL_STATE(272)] = 4096,
+  [SMALL_STATE(273)] = 4103,
+  [SMALL_STATE(274)] = 4110,
+  [SMALL_STATE(275)] = 4117,
+  [SMALL_STATE(276)] = 4124,
+  [SMALL_STATE(277)] = 4131,
+  [SMALL_STATE(278)] = 4138,
+  [SMALL_STATE(279)] = 4145,
+  [SMALL_STATE(280)] = 4152,
+  [SMALL_STATE(281)] = 4159,
+  [SMALL_STATE(282)] = 4166,
+  [SMALL_STATE(283)] = 4173,
+  [SMALL_STATE(284)] = 4180,
+  [SMALL_STATE(285)] = 4187,
+  [SMALL_STATE(286)] = 4198,
+  [SMALL_STATE(287)] = 4205,
+  [SMALL_STATE(288)] = 4212,
+  [SMALL_STATE(289)] = 4219,
+  [SMALL_STATE(290)] = 4226,
+  [SMALL_STATE(291)] = 4233,
+  [SMALL_STATE(292)] = 4240,
+  [SMALL_STATE(293)] = 4247,
+  [SMALL_STATE(294)] = 4260,
+  [SMALL_STATE(295)] = 4267,
+  [SMALL_STATE(296)] = 4280,
+  [SMALL_STATE(297)] = 4287,
+  [SMALL_STATE(298)] = 4294,
+  [SMALL_STATE(299)] = 4301,
+  [SMALL_STATE(300)] = 4308,
+  [SMALL_STATE(301)] = 4315,
+  [SMALL_STATE(302)] = 4322,
+  [SMALL_STATE(303)] = 4329,
+  [SMALL_STATE(304)] = 4336,
+  [SMALL_STATE(305)] = 4343,
+  [SMALL_STATE(306)] = 4350,
+  [SMALL_STATE(307)] = 4357,
+  [SMALL_STATE(308)] = 4364,
+  [SMALL_STATE(309)] = 4371,
+  [SMALL_STATE(310)] = 4384,
+  [SMALL_STATE(311)] = 4390,
+  [SMALL_STATE(312)] = 4400,
+  [SMALL_STATE(313)] = 4406,
+  [SMALL_STATE(314)] = 4412,
+  [SMALL_STATE(315)] = 4422,
+  [SMALL_STATE(316)] = 4428,
+  [SMALL_STATE(317)] = 4434,
+  [SMALL_STATE(318)] = 4440,
+  [SMALL_STATE(319)] = 4446,
+  [SMALL_STATE(320)] = 4452,
+  [SMALL_STATE(321)] = 4458,
+  [SMALL_STATE(322)] = 4464,
+  [SMALL_STATE(323)] = 4470,
+  [SMALL_STATE(324)] = 4476,
+  [SMALL_STATE(325)] = 4482,
+  [SMALL_STATE(326)] = 4488,
+  [SMALL_STATE(327)] = 4494,
+  [SMALL_STATE(328)] = 4500,
+  [SMALL_STATE(329)] = 4506,
+  [SMALL_STATE(330)] = 4512,
+  [SMALL_STATE(331)] = 4518,
+  [SMALL_STATE(332)] = 4524,
+  [SMALL_STATE(333)] = 4530,
+  [SMALL_STATE(334)] = 4540,
+  [SMALL_STATE(335)] = 4546,
+  [SMALL_STATE(336)] = 4552,
+  [SMALL_STATE(337)] = 4558,
+  [SMALL_STATE(338)] = 4564,
+  [SMALL_STATE(339)] = 4570,
+  [SMALL_STATE(340)] = 4576,
+  [SMALL_STATE(341)] = 4582,
+  [SMALL_STATE(342)] = 4588,
+  [SMALL_STATE(343)] = 4594,
+  [SMALL_STATE(344)] = 4600,
+  [SMALL_STATE(345)] = 4606,
+  [SMALL_STATE(346)] = 4612,
+  [SMALL_STATE(347)] = 4618,
+  [SMALL_STATE(348)] = 4624,
+  [SMALL_STATE(349)] = 4630,
+  [SMALL_STATE(350)] = 4636,
+  [SMALL_STATE(351)] = 4642,
+  [SMALL_STATE(352)] = 4648,
+  [SMALL_STATE(353)] = 4654,
+  [SMALL_STATE(354)] = 4660,
+  [SMALL_STATE(355)] = 4670,
+  [SMALL_STATE(356)] = 4676,
+  [SMALL_STATE(357)] = 4682,
+  [SMALL_STATE(358)] = 4688,
+  [SMALL_STATE(359)] = 4694,
+  [SMALL_STATE(360)] = 4700,
+  [SMALL_STATE(361)] = 4706,
+  [SMALL_STATE(362)] = 4712,
+  [SMALL_STATE(363)] = 4718,
+  [SMALL_STATE(364)] = 4724,
+  [SMALL_STATE(365)] = 4730,
+  [SMALL_STATE(366)] = 4736,
+  [SMALL_STATE(367)] = 4742,
+  [SMALL_STATE(368)] = 4748,
+  [SMALL_STATE(369)] = 4754,
+  [SMALL_STATE(370)] = 4760,
+  [SMALL_STATE(371)] = 4766,
+  [SMALL_STATE(372)] = 4772,
+  [SMALL_STATE(373)] = 4778,
+  [SMALL_STATE(374)] = 4784,
+  [SMALL_STATE(375)] = 4790,
+  [SMALL_STATE(376)] = 4796,
+  [SMALL_STATE(377)] = 4802,
+  [SMALL_STATE(378)] = 4808,
+  [SMALL_STATE(379)] = 4814,
+  [SMALL_STATE(380)] = 4820,
+  [SMALL_STATE(381)] = 4826,
+  [SMALL_STATE(382)] = 4832,
+  [SMALL_STATE(383)] = 4838,
+  [SMALL_STATE(384)] = 4844,
+  [SMALL_STATE(385)] = 4850,
+  [SMALL_STATE(386)] = 4856,
+  [SMALL_STATE(387)] = 4864,
+  [SMALL_STATE(388)] = 4870,
+  [SMALL_STATE(389)] = 4876,
+  [SMALL_STATE(390)] = 4882,
+  [SMALL_STATE(391)] = 4888,
+  [SMALL_STATE(392)] = 4894,
+  [SMALL_STATE(393)] = 4900,
+  [SMALL_STATE(394)] = 4906,
+  [SMALL_STATE(395)] = 4912,
+  [SMALL_STATE(396)] = 4918,
+  [SMALL_STATE(397)] = 4924,
+  [SMALL_STATE(398)] = 4930,
+  [SMALL_STATE(399)] = 4936,
+  [SMALL_STATE(400)] = 4942,
+  [SMALL_STATE(401)] = 4948,
+  [SMALL_STATE(402)] = 4954,
+  [SMALL_STATE(403)] = 4960,
+  [SMALL_STATE(404)] = 4966,
+  [SMALL_STATE(405)] = 4972,
+  [SMALL_STATE(406)] = 4978,
+  [SMALL_STATE(407)] = 4984,
+  [SMALL_STATE(408)] = 4990,
+  [SMALL_STATE(409)] = 4996,
+  [SMALL_STATE(410)] = 5002,
+  [SMALL_STATE(411)] = 5008,
+  [SMALL_STATE(412)] = 5014,
+  [SMALL_STATE(413)] = 5020,
+  [SMALL_STATE(414)] = 5026,
+  [SMALL_STATE(415)] = 5032,
+  [SMALL_STATE(416)] = 5038,
+  [SMALL_STATE(417)] = 5044,
+  [SMALL_STATE(418)] = 5050,
+  [SMALL_STATE(419)] = 5056,
+  [SMALL_STATE(420)] = 5062,
+  [SMALL_STATE(421)] = 5068,
+  [SMALL_STATE(422)] = 5074,
+  [SMALL_STATE(423)] = 5080,
+  [SMALL_STATE(424)] = 5086,
+  [SMALL_STATE(425)] = 5092,
+  [SMALL_STATE(426)] = 5098,
+  [SMALL_STATE(427)] = 5104,
+  [SMALL_STATE(428)] = 5110,
+  [SMALL_STATE(429)] = 5116,
+  [SMALL_STATE(430)] = 5122,
+  [SMALL_STATE(431)] = 5128,
+  [SMALL_STATE(432)] = 5134,
+  [SMALL_STATE(433)] = 5140,
+  [SMALL_STATE(434)] = 5146,
+  [SMALL_STATE(435)] = 5152,
+  [SMALL_STATE(436)] = 5158,
+  [SMALL_STATE(437)] = 5164,
+  [SMALL_STATE(438)] = 5170,
+  [SMALL_STATE(439)] = 5176,
+  [SMALL_STATE(440)] = 5182,
+  [SMALL_STATE(441)] = 5188,
+  [SMALL_STATE(442)] = 5194,
+  [SMALL_STATE(443)] = 5200,
+  [SMALL_STATE(444)] = 5206,
+  [SMALL_STATE(445)] = 5212,
+  [SMALL_STATE(446)] = 5218,
+  [SMALL_STATE(447)] = 5224,
+  [SMALL_STATE(448)] = 5230,
+  [SMALL_STATE(449)] = 5236,
+  [SMALL_STATE(450)] = 5243,
+  [SMALL_STATE(451)] = 5250,
+  [SMALL_STATE(452)] = 5257,
+  [SMALL_STATE(453)] = 5264,
+  [SMALL_STATE(454)] = 5271,
+  [SMALL_STATE(455)] = 5278,
+  [SMALL_STATE(456)] = 5285,
+  [SMALL_STATE(457)] = 5292,
+  [SMALL_STATE(458)] = 5299,
+  [SMALL_STATE(459)] = 5306,
+  [SMALL_STATE(460)] = 5313,
+  [SMALL_STATE(461)] = 5320,
+  [SMALL_STATE(462)] = 5327,
+  [SMALL_STATE(463)] = 5334,
+  [SMALL_STATE(464)] = 5341,
+  [SMALL_STATE(465)] = 5345,
+  [SMALL_STATE(466)] = 5349,
+  [SMALL_STATE(467)] = 5353,
+  [SMALL_STATE(468)] = 5357,
+  [SMALL_STATE(469)] = 5361,
+  [SMALL_STATE(470)] = 5365,
+  [SMALL_STATE(471)] = 5369,
+  [SMALL_STATE(472)] = 5373,
+  [SMALL_STATE(473)] = 5377,
+  [SMALL_STATE(474)] = 5381,
+  [SMALL_STATE(475)] = 5385,
+  [SMALL_STATE(476)] = 5389,
+  [SMALL_STATE(477)] = 5393,
+  [SMALL_STATE(478)] = 5397,
+  [SMALL_STATE(479)] = 5401,
+  [SMALL_STATE(480)] = 5405,
+  [SMALL_STATE(481)] = 5409,
+  [SMALL_STATE(482)] = 5413,
+  [SMALL_STATE(483)] = 5417,
+  [SMALL_STATE(484)] = 5421,
+  [SMALL_STATE(485)] = 5425,
+  [SMALL_STATE(486)] = 5429,
+  [SMALL_STATE(487)] = 5433,
+  [SMALL_STATE(488)] = 5437,
+  [SMALL_STATE(489)] = 5441,
+  [SMALL_STATE(490)] = 5445,
+  [SMALL_STATE(491)] = 5449,
+  [SMALL_STATE(492)] = 5453,
+  [SMALL_STATE(493)] = 5457,
+  [SMALL_STATE(494)] = 5461,
+  [SMALL_STATE(495)] = 5465,
+  [SMALL_STATE(496)] = 5469,
+  [SMALL_STATE(497)] = 5473,
+  [SMALL_STATE(498)] = 5477,
+  [SMALL_STATE(499)] = 5481,
+  [SMALL_STATE(500)] = 5485,
+  [SMALL_STATE(501)] = 5489,
+  [SMALL_STATE(502)] = 5493,
+  [SMALL_STATE(503)] = 5497,
+  [SMALL_STATE(504)] = 5501,
+  [SMALL_STATE(505)] = 5505,
+  [SMALL_STATE(506)] = 5509,
+  [SMALL_STATE(507)] = 5513,
+  [SMALL_STATE(508)] = 5517,
+  [SMALL_STATE(509)] = 5521,
+  [SMALL_STATE(510)] = 5525,
+  [SMALL_STATE(511)] = 5529,
+  [SMALL_STATE(512)] = 5533,
+  [SMALL_STATE(513)] = 5537,
+  [SMALL_STATE(514)] = 5541,
+  [SMALL_STATE(515)] = 5545,
+  [SMALL_STATE(516)] = 5549,
+  [SMALL_STATE(517)] = 5553,
+  [SMALL_STATE(518)] = 5557,
+  [SMALL_STATE(519)] = 5561,
+  [SMALL_STATE(520)] = 5565,
+  [SMALL_STATE(521)] = 5569,
+  [SMALL_STATE(522)] = 5573,
+  [SMALL_STATE(523)] = 5577,
+  [SMALL_STATE(524)] = 5581,
+  [SMALL_STATE(525)] = 5585,
+  [SMALL_STATE(526)] = 5589,
+  [SMALL_STATE(527)] = 5593,
+  [SMALL_STATE(528)] = 5597,
+  [SMALL_STATE(529)] = 5601,
+  [SMALL_STATE(530)] = 5605,
+  [SMALL_STATE(531)] = 5609,
+  [SMALL_STATE(532)] = 5613,
+  [SMALL_STATE(533)] = 5617,
+  [SMALL_STATE(534)] = 5621,
+  [SMALL_STATE(535)] = 5625,
+  [SMALL_STATE(536)] = 5629,
+  [SMALL_STATE(537)] = 5633,
+  [SMALL_STATE(538)] = 5637,
+  [SMALL_STATE(539)] = 5641,
+  [SMALL_STATE(540)] = 5645,
+  [SMALL_STATE(541)] = 5649,
+  [SMALL_STATE(542)] = 5653,
+  [SMALL_STATE(543)] = 5657,
+  [SMALL_STATE(544)] = 5661,
+  [SMALL_STATE(545)] = 5665,
+  [SMALL_STATE(546)] = 5669,
+  [SMALL_STATE(547)] = 5673,
+  [SMALL_STATE(548)] = 5677,
+  [SMALL_STATE(549)] = 5681,
+  [SMALL_STATE(550)] = 5685,
+  [SMALL_STATE(551)] = 5689,
+  [SMALL_STATE(552)] = 5693,
+  [SMALL_STATE(553)] = 5697,
+  [SMALL_STATE(554)] = 5701,
+  [SMALL_STATE(555)] = 5705,
+  [SMALL_STATE(556)] = 5709,
+  [SMALL_STATE(557)] = 5713,
+  [SMALL_STATE(558)] = 5717,
+  [SMALL_STATE(559)] = 5721,
+  [SMALL_STATE(560)] = 5725,
+  [SMALL_STATE(561)] = 5729,
+  [SMALL_STATE(562)] = 5733,
+  [SMALL_STATE(563)] = 5737,
+  [SMALL_STATE(564)] = 5741,
+  [SMALL_STATE(565)] = 5745,
 };
 
 static const TSParseActionEntry ts_parse_actions[] = {
   [0] = {.entry = {.count = 0, .reusable = false}},
   [1] = {.entry = {.count = 1, .reusable = false}}, RECOVER(),
   [3] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_file, 0),
-  [5] = {.entry = {.count = 1, .reusable = false}}, SHIFT(182),
-  [7] = {.entry = {.count = 1, .reusable = false}}, SHIFT(92),
-  [9] = {.entry = {.count = 1, .reusable = false}}, SHIFT(78),
-  [11] = {.entry = {.count = 1, .reusable = false}}, SHIFT(64),
+  [5] = {.entry = {.count = 1, .reusable = false}}, SHIFT(214),
+  [7] = {.entry = {.count = 1, .reusable = false}}, SHIFT(76),
+  [9] = {.entry = {.count = 1, .reusable = false}}, SHIFT(65),
+  [11] = {.entry = {.count = 1, .reusable = false}}, SHIFT(66),
   [13] = {.entry = {.count = 1, .reusable = false}}, SHIFT(59),
-  [15] = {.entry = {.count = 1, .reusable = false}}, SHIFT(389),
-  [17] = {.entry = {.count = 1, .reusable = false}}, SHIFT(265),
-  [19] = {.entry = {.count = 1, .reusable = false}}, SHIFT(60),
-  [21] = {.entry = {.count = 1, .reusable = false}}, SHIFT(61),
-  [23] = {.entry = {.count = 1, .reusable = false}}, SHIFT(328),
-  [25] = {.entry = {.count = 1, .reusable = false}}, SHIFT(266),
+  [15] = {.entry = {.count = 1, .reusable = false}}, SHIFT(314),
+  [17] = {.entry = {.count = 1, .reusable = false}}, SHIFT(309),
+  [19] = {.entry = {.count = 1, .reusable = false}}, SHIFT(61),
+  [21] = {.entry = {.count = 1, .reusable = false}}, SHIFT(60),
+  [23] = {.entry = {.count = 1, .reusable = false}}, SHIFT(333),
+  [25] = {.entry = {.count = 1, .reusable = false}}, SHIFT(295),
   [27] = {.entry = {.count = 1, .reusable = false}}, SHIFT(35),
-  [29] = {.entry = {.count = 1, .reusable = false}}, SHIFT(31),
-  [31] = {.entry = {.count = 1, .reusable = false}}, SHIFT(111),
-  [33] = {.entry = {.count = 1, .reusable = false}}, SHIFT(117),
+  [29] = {.entry = {.count = 1, .reusable = false}}, SHIFT(33),
+  [31] = {.entry = {.count = 1, .reusable = false}}, SHIFT(133),
+  [33] = {.entry = {.count = 1, .reusable = false}}, SHIFT(132),
   [35] = {.entry = {.count = 1, .reusable = false}}, SHIFT(27),
-  [37] = {.entry = {.count = 1, .reusable = false}}, SHIFT(118),
-  [39] = {.entry = {.count = 1, .reusable = false}}, SHIFT(169),
-  [41] = {.entry = {.count = 1, .reusable = false}}, SHIFT(120),
-  [43] = {.entry = {.count = 1, .reusable = false}}, SHIFT(456),
-  [45] = {.entry = {.count = 1, .reusable = false}}, SHIFT(133),
-  [47] = {.entry = {.count = 1, .reusable = false}}, SHIFT(134),
-  [49] = {.entry = {.count = 1, .reusable = false}}, SHIFT(89),
-  [51] = {.entry = {.count = 1, .reusable = false}}, SHIFT(135),
-  [53] = {.entry = {.count = 1, .reusable = false}}, SHIFT(186),
-  [55] = {.entry = {.count = 1, .reusable = false}}, SHIFT(155),
-  [57] = {.entry = {.count = 1, .reusable = false}}, SHIFT(71),
-  [59] = {.entry = {.count = 1, .reusable = false}}, SHIFT(62),
-  [61] = {.entry = {.count = 1, .reusable = false}}, SHIFT(137),
-  [63] = {.entry = {.count = 1, .reusable = false}}, SHIFT(140),
-  [65] = {.entry = {.count = 1, .reusable = false}}, SHIFT(381),
-  [67] = {.entry = {.count = 1, .reusable = false}}, SHIFT(146),
-  [69] = {.entry = {.count = 1, .reusable = false}}, SHIFT(74),
-  [71] = {.entry = {.count = 1, .reusable = false}}, SHIFT(461),
-  [73] = {.entry = {.count = 1, .reusable = false}}, SHIFT(458),
-  [75] = {.entry = {.count = 1, .reusable = false}}, SHIFT(449),
-  [77] = {.entry = {.count = 1, .reusable = false}}, SHIFT(463),
+  [37] = {.entry = {.count = 1, .reusable = false}}, SHIFT(126),
+  [39] = {.entry = {.count = 1, .reusable = false}}, SHIFT(189),
+  [41] = {.entry = {.count = 1, .reusable = false}}, SHIFT(125),
+  [43] = {.entry = {.count = 1, .reusable = false}}, SHIFT(449),
+  [45] = {.entry = {.count = 1, .reusable = false}}, SHIFT(124),
+  [47] = {.entry = {.count = 1, .reusable = false}}, SHIFT(119),
+  [49] = {.entry = {.count = 1, .reusable = false}}, SHIFT(99),
+  [51] = {.entry = {.count = 1, .reusable = false}}, SHIFT(114),
+  [53] = {.entry = {.count = 1, .reusable = false}}, SHIFT(198),
+  [55] = {.entry = {.count = 1, .reusable = false}}, SHIFT(101),
+  [57] = {.entry = {.count = 1, .reusable = false}}, SHIFT(94),
+  [59] = {.entry = {.count = 1, .reusable = false}}, SHIFT(70),
+  [61] = {.entry = {.count = 1, .reusable = false}}, SHIFT(105),
+  [63] = {.entry = {.count = 1, .reusable = false}}, SHIFT(104),
+  [65] = {.entry = {.count = 1, .reusable = false}}, SHIFT(429),
+  [67] = {.entry = {.count = 1, .reusable = false}}, SHIFT(143),
+  [69] = {.entry = {.count = 1, .reusable = false}}, SHIFT(82),
+  [71] = {.entry = {.count = 1, .reusable = false}}, SHIFT(455),
+  [73] = {.entry = {.count = 1, .reusable = false}}, SHIFT(453),
+  [75] = {.entry = {.count = 1, .reusable = false}}, SHIFT(451),
+  [77] = {.entry = {.count = 1, .reusable = false}}, SHIFT(450),
   [79] = {.entry = {.count = 1, .reusable = false}}, SHIFT(36),
   [81] = {.entry = {.count = 1, .reusable = false}}, SHIFT(34),
-  [83] = {.entry = {.count = 1, .reusable = false}}, SHIFT(86),
-  [85] = {.entry = {.count = 1, .reusable = false}}, SHIFT(147),
-  [87] = {.entry = {.count = 1, .reusable = false}}, SHIFT(65),
-  [89] = {.entry = {.count = 1, .reusable = false}}, SHIFT(66),
-  [91] = {.entry = {.count = 1, .reusable = false}}, SHIFT(67),
-  [93] = {.entry = {.count = 1, .reusable = false}}, SHIFT(88),
-  [95] = {.entry = {.count = 1, .reusable = false}}, SHIFT(142),
-  [97] = {.entry = {.count = 1, .reusable = false}}, SHIFT(141),
-  [99] = {.entry = {.count = 1, .reusable = false}}, SHIFT(139),
-  [101] = {.entry = {.count = 1, .reusable = false}}, SHIFT(388),
-  [103] = {.entry = {.count = 1, .reusable = false}}, SHIFT(274),
+  [83] = {.entry = {.count = 1, .reusable = false}}, SHIFT(89),
+  [85] = {.entry = {.count = 1, .reusable = false}}, SHIFT(116),
+  [87] = {.entry = {.count = 1, .reusable = false}}, SHIFT(63),
+  [89] = {.entry = {.count = 1, .reusable = false}}, SHIFT(67),
+  [91] = {.entry = {.count = 1, .reusable = false}}, SHIFT(64),
+  [93] = {.entry = {.count = 1, .reusable = false}}, SHIFT(122),
+  [95] = {.entry = {.count = 1, .reusable = false}}, SHIFT(159),
+  [97] = {.entry = {.count = 1, .reusable = false}}, SHIFT(158),
+  [99] = {.entry = {.count = 1, .reusable = false}}, SHIFT(136),
+  [101] = {.entry = {.count = 1, .reusable = false}}, SHIFT(311),
+  [103] = {.entry = {.count = 1, .reusable = false}}, SHIFT(260),
   [105] = {.entry = {.count = 1, .reusable = false}}, SHIFT(26),
-  [107] = {.entry = {.count = 1, .reusable = false}}, SHIFT(136),
-  [109] = {.entry = {.count = 1, .reusable = false}}, SHIFT(158),
-  [111] = {.entry = {.count = 1, .reusable = false}}, SHIFT(85),
-  [113] = {.entry = {.count = 1, .reusable = false}}, SHIFT(160),
-  [115] = {.entry = {.count = 1, .reusable = false}}, SHIFT(149),
-  [117] = {.entry = {.count = 1, .reusable = false}}, SHIFT(170),
-  [119] = {.entry = {.count = 1, .reusable = false}}, SHIFT(172),
-  [121] = {.entry = {.count = 1, .reusable = false}}, SHIFT(115),
-  [123] = {.entry = {.count = 1, .reusable = false}}, SHIFT(114),
-  [125] = {.entry = {.count = 1, .reusable = false}}, SHIFT(112),
-  [127] = {.entry = {.count = 1, .reusable = false}}, SHIFT(173),
-  [129] = {.entry = {.count = 1, .reusable = false}}, SHIFT(110),
-  [131] = {.entry = {.count = 1, .reusable = false}}, SHIFT(176),
-  [133] = {.entry = {.count = 1, .reusable = false}}, SHIFT(107),
-  [135] = {.entry = {.count = 1, .reusable = false}}, SHIFT(102),
-  [137] = {.entry = {.count = 1, .reusable = false}}, SHIFT(100),
+  [107] = {.entry = {.count = 1, .reusable = false}}, SHIFT(127),
+  [109] = {.entry = {.count = 1, .reusable = false}}, SHIFT(221),
+  [111] = {.entry = {.count = 1, .reusable = false}}, SHIFT(87),
+  [113] = {.entry = {.count = 1, .reusable = false}}, SHIFT(222),
+  [115] = {.entry = {.count = 1, .reusable = false}}, SHIFT(230),
+  [117] = {.entry = {.count = 1, .reusable = false}}, SHIFT(242),
+  [119] = {.entry = {.count = 1, .reusable = false}}, SHIFT(245),
+  [121] = {.entry = {.count = 1, .reusable = false}}, SHIFT(160),
+  [123] = {.entry = {.count = 1, .reusable = false}}, SHIFT(154),
+  [125] = {.entry = {.count = 1, .reusable = false}}, SHIFT(152),
+  [127] = {.entry = {.count = 1, .reusable = false}}, SHIFT(248),
+  [129] = {.entry = {.count = 1, .reusable = false}}, SHIFT(149),
+  [131] = {.entry = {.count = 1, .reusable = false}}, SHIFT(249),
+  [133] = {.entry = {.count = 1, .reusable = false}}, SHIFT(147),
+  [135] = {.entry = {.count = 1, .reusable = false}}, SHIFT(142),
+  [137] = {.entry = {.count = 1, .reusable = false}}, SHIFT(140),
   [139] = {.entry = {.count = 1, .reusable = false}}, SHIFT(13),
   [141] = {.entry = {.count = 1, .reusable = false}}, SHIFT(12),
   [143] = {.entry = {.count = 1, .reusable = false}}, SHIFT(11),
-  [145] = {.entry = {.count = 1, .reusable = false}}, SHIFT(30),
-  [147] = {.entry = {.count = 1, .reusable = false}}, SHIFT(196),
-  [149] = {.entry = {.count = 1, .reusable = false}}, SHIFT(457),
-  [151] = {.entry = {.count = 1, .reusable = false}}, SHIFT(453),
-  [153] = {.entry = {.count = 1, .reusable = false}}, SHIFT(451),
-  [155] = {.entry = {.count = 1, .reusable = false}}, SHIFT(450),
-  [157] = {.entry = {.count = 1, .reusable = false}}, SHIFT(491),
-  [159] = {.entry = {.count = 1, .reusable = false}}, SHIFT(79),
-  [161] = {.entry = {.count = 1, .reusable = false}}, SHIFT(69),
-  [163] = {.entry = {.count = 1, .reusable = false}}, SHIFT(94),
-  [165] = {.entry = {.count = 1, .reusable = false}}, SHIFT(82),
-  [167] = {.entry = {.count = 1, .reusable = false}}, SHIFT(181),
-  [169] = {.entry = {.count = 1, .reusable = false}}, SHIFT(487),
+  [145] = {.entry = {.count = 1, .reusable = false}}, SHIFT(29),
+  [147] = {.entry = {.count = 1, .reusable = false}}, SHIFT(250),
+  [149] = {.entry = {.count = 1, .reusable = false}}, SHIFT(462),
+  [151] = {.entry = {.count = 1, .reusable = false}}, SHIFT(463),
+  [153] = {.entry = {.count = 1, .reusable = false}}, SHIFT(457),
+  [155] = {.entry = {.count = 1, .reusable = false}}, SHIFT(456),
+  [157] = {.entry = {.count = 1, .reusable = false}}, SHIFT(482),
+  [159] = {.entry = {.count = 1, .reusable = false}}, SHIFT(86),
+  [161] = {.entry = {.count = 1, .reusable = false}}, SHIFT(71),
+  [163] = {.entry = {.count = 1, .reusable = false}}, SHIFT(128),
+  [165] = {.entry = {.count = 1, .reusable = false}}, SHIFT(88),
+  [167] = {.entry = {.count = 1, .reusable = false}}, SHIFT(203),
+  [169] = {.entry = {.count = 1, .reusable = false}}, SHIFT(484),
   [171] = {.entry = {.count = 1, .reusable = false}}, SHIFT(3),
-  [173] = {.entry = {.count = 1, .reusable = false}}, SHIFT(288),
+  [173] = {.entry = {.count = 1, .reusable = false}}, SHIFT(285),
   [175] = {.entry = {.count = 1, .reusable = true}}, REDUCE(aux_sym_file_repeat1, 2),
-  [177] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(182),
-  [180] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(92),
-  [183] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(78),
-  [186] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(64),
+  [177] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(214),
+  [180] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(76),
+  [183] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(65),
+  [186] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(66),
   [189] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(59),
-  [192] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(389),
-  [195] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(265),
-  [198] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(60),
-  [201] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(61),
-  [204] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(328),
-  [207] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(266),
+  [192] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(314),
+  [195] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(309),
+  [198] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(61),
+  [201] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(60),
+  [204] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(333),
+  [207] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(295),
   [210] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(35),
-  [213] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(31),
-  [216] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(111),
-  [219] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(117),
+  [213] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(33),
+  [216] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(133),
+  [219] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(132),
   [222] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(27),
-  [225] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(118),
-  [228] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(169),
-  [231] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(120),
-  [234] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(456),
-  [237] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(133),
-  [240] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(134),
-  [243] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(89),
-  [246] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(135),
-  [249] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(186),
-  [252] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(155),
-  [255] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(71),
-  [258] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(62),
-  [261] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(137),
-  [264] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(140),
-  [267] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(381),
-  [270] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(146),
-  [273] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(74),
-  [276] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(461),
-  [279] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(458),
-  [282] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(449),
-  [285] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(463),
+  [225] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(126),
+  [228] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(189),
+  [231] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(125),
+  [234] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(449),
+  [237] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(124),
+  [240] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(119),
+  [243] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(99),
+  [246] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(114),
+  [249] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(198),
+  [252] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(101),
+  [255] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(94),
+  [258] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(70),
+  [261] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(105),
+  [264] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(104),
+  [267] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(429),
+  [270] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(143),
+  [273] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(82),
+  [276] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(455),
+  [279] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(453),
+  [282] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(451),
+  [285] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(450),
   [288] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(36),
   [291] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(34),
-  [294] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(86),
-  [297] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(147),
-  [300] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(65),
-  [303] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(66),
-  [306] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(67),
-  [309] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(88),
-  [312] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(142),
-  [315] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(141),
-  [318] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(139),
-  [321] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(388),
-  [324] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(274),
+  [294] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(89),
+  [297] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(116),
+  [300] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(63),
+  [303] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(67),
+  [306] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(64),
+  [309] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(122),
+  [312] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(159),
+  [315] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(158),
+  [318] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(136),
+  [321] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(311),
+  [324] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(260),
   [327] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(26),
-  [330] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(136),
-  [333] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(158),
-  [336] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(85),
-  [339] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(160),
-  [342] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(149),
-  [345] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(170),
-  [348] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(172),
-  [351] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(115),
-  [354] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(114),
-  [357] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(112),
-  [360] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(173),
-  [363] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(110),
-  [366] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(176),
-  [369] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(107),
-  [372] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(102),
-  [375] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(100),
+  [330] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(127),
+  [333] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(221),
+  [336] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(87),
+  [339] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(222),
+  [342] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(230),
+  [345] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(242),
+  [348] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(245),
+  [351] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(160),
+  [354] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(154),
+  [357] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(152),
+  [360] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(248),
+  [363] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(149),
+  [366] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(249),
+  [369] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(147),
+  [372] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(142),
+  [375] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(140),
   [378] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(13),
   [381] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(12),
   [384] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(11),
-  [387] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(30),
-  [390] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(196),
-  [393] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(457),
-  [396] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(453),
-  [399] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(451),
-  [402] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(450),
-  [405] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(491),
-  [408] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(79),
-  [411] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(69),
-  [414] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(94),
-  [417] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(82),
-  [420] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(181),
-  [423] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(487),
+  [387] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(29),
+  [390] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(250),
+  [393] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(462),
+  [396] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(463),
+  [399] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(457),
+  [402] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(456),
+  [405] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(482),
+  [408] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(86),
+  [411] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(71),
+  [414] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(128),
+  [417] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(88),
+  [420] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(203),
+  [423] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(484),
   [426] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(2),
-  [429] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(288),
+  [429] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2), SHIFT_REPEAT(285),
   [432] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_file, 1),
   [434] = {.entry = {.count = 1, .reusable = false}}, SHIFT(2),
-  [436] = {.entry = {.count = 1, .reusable = true}}, SHIFT(182),
-  [438] = {.entry = {.count = 1, .reusable = true}}, SHIFT(92),
-  [440] = {.entry = {.count = 1, .reusable = true}}, SHIFT(78),
-  [442] = {.entry = {.count = 1, .reusable = true}}, SHIFT(64),
+  [436] = {.entry = {.count = 1, .reusable = true}}, SHIFT(214),
+  [438] = {.entry = {.count = 1, .reusable = true}}, SHIFT(76),
+  [440] = {.entry = {.count = 1, .reusable = true}}, SHIFT(65),
+  [442] = {.entry = {.count = 1, .reusable = true}}, SHIFT(66),
   [444] = {.entry = {.count = 1, .reusable = true}}, SHIFT(59),
-  [446] = {.entry = {.count = 1, .reusable = true}}, SHIFT(389),
-  [448] = {.entry = {.count = 1, .reusable = true}}, SHIFT(265),
-  [450] = {.entry = {.count = 1, .reusable = true}}, SHIFT(60),
-  [452] = {.entry = {.count = 1, .reusable = true}}, SHIFT(61),
-  [454] = {.entry = {.count = 1, .reusable = true}}, SHIFT(328),
-  [456] = {.entry = {.count = 1, .reusable = true}}, SHIFT(266),
+  [446] = {.entry = {.count = 1, .reusable = true}}, SHIFT(314),
+  [448] = {.entry = {.count = 1, .reusable = true}}, SHIFT(309),
+  [450] = {.entry = {.count = 1, .reusable = true}}, SHIFT(61),
+  [452] = {.entry = {.count = 1, .reusable = true}}, SHIFT(60),
+  [454] = {.entry = {.count = 1, .reusable = true}}, SHIFT(333),
+  [456] = {.entry = {.count = 1, .reusable = true}}, SHIFT(295),
   [458] = {.entry = {.count = 1, .reusable = true}}, SHIFT(35),
-  [460] = {.entry = {.count = 1, .reusable = true}}, SHIFT(31),
-  [462] = {.entry = {.count = 1, .reusable = true}}, SHIFT(111),
-  [464] = {.entry = {.count = 1, .reusable = true}}, SHIFT(117),
+  [460] = {.entry = {.count = 1, .reusable = true}}, SHIFT(33),
+  [462] = {.entry = {.count = 1, .reusable = true}}, SHIFT(133),
+  [464] = {.entry = {.count = 1, .reusable = true}}, SHIFT(132),
   [466] = {.entry = {.count = 1, .reusable = true}}, SHIFT(27),
-  [468] = {.entry = {.count = 1, .reusable = true}}, SHIFT(118),
-  [470] = {.entry = {.count = 1, .reusable = true}}, SHIFT(169),
-  [472] = {.entry = {.count = 1, .reusable = true}}, SHIFT(120),
-  [474] = {.entry = {.count = 1, .reusable = true}}, SHIFT(456),
-  [476] = {.entry = {.count = 1, .reusable = true}}, SHIFT(133),
-  [478] = {.entry = {.count = 1, .reusable = true}}, SHIFT(134),
-  [480] = {.entry = {.count = 1, .reusable = true}}, SHIFT(89),
-  [482] = {.entry = {.count = 1, .reusable = true}}, SHIFT(135),
-  [484] = {.entry = {.count = 1, .reusable = true}}, SHIFT(186),
-  [486] = {.entry = {.count = 1, .reusable = true}}, SHIFT(155),
-  [488] = {.entry = {.count = 1, .reusable = true}}, SHIFT(71),
-  [490] = {.entry = {.count = 1, .reusable = true}}, SHIFT(62),
-  [492] = {.entry = {.count = 1, .reusable = true}}, SHIFT(137),
-  [494] = {.entry = {.count = 1, .reusable = true}}, SHIFT(140),
-  [496] = {.entry = {.count = 1, .reusable = true}}, SHIFT(381),
-  [498] = {.entry = {.count = 1, .reusable = true}}, SHIFT(146),
-  [500] = {.entry = {.count = 1, .reusable = true}}, SHIFT(74),
-  [502] = {.entry = {.count = 1, .reusable = true}}, SHIFT(461),
-  [504] = {.entry = {.count = 1, .reusable = true}}, SHIFT(458),
+  [468] = {.entry = {.count = 1, .reusable = true}}, SHIFT(126),
+  [470] = {.entry = {.count = 1, .reusable = true}}, SHIFT(189),
+  [472] = {.entry = {.count = 1, .reusable = true}}, SHIFT(125),
+  [474] = {.entry = {.count = 1, .reusable = true}}, SHIFT(449),
+  [476] = {.entry = {.count = 1, .reusable = true}}, SHIFT(124),
+  [478] = {.entry = {.count = 1, .reusable = true}}, SHIFT(119),
+  [480] = {.entry = {.count = 1, .reusable = true}}, SHIFT(99),
+  [482] = {.entry = {.count = 1, .reusable = true}}, SHIFT(114),
+  [484] = {.entry = {.count = 1, .reusable = true}}, SHIFT(198),
+  [486] = {.entry = {.count = 1, .reusable = true}}, SHIFT(101),
+  [488] = {.entry = {.count = 1, .reusable = true}}, SHIFT(94),
+  [490] = {.entry = {.count = 1, .reusable = true}}, SHIFT(70),
+  [492] = {.entry = {.count = 1, .reusable = true}}, SHIFT(105),
+  [494] = {.entry = {.count = 1, .reusable = true}}, SHIFT(104),
+  [496] = {.entry = {.count = 1, .reusable = true}}, SHIFT(429),
+  [498] = {.entry = {.count = 1, .reusable = true}}, SHIFT(143),
+  [500] = {.entry = {.count = 1, .reusable = true}}, SHIFT(82),
+  [502] = {.entry = {.count = 1, .reusable = true}}, SHIFT(455),
+  [504] = {.entry = {.count = 1, .reusable = true}}, SHIFT(453),
   [506] = {.entry = {.count = 1, .reusable = true}}, SHIFT(36),
   [508] = {.entry = {.count = 1, .reusable = true}}, SHIFT(34),
-  [510] = {.entry = {.count = 1, .reusable = true}}, SHIFT(86),
-  [512] = {.entry = {.count = 1, .reusable = true}}, SHIFT(147),
-  [514] = {.entry = {.count = 1, .reusable = true}}, SHIFT(65),
-  [516] = {.entry = {.count = 1, .reusable = true}}, SHIFT(66),
-  [518] = {.entry = {.count = 1, .reusable = true}}, SHIFT(67),
-  [520] = {.entry = {.count = 1, .reusable = true}}, SHIFT(88),
-  [522] = {.entry = {.count = 1, .reusable = true}}, SHIFT(142),
-  [524] = {.entry = {.count = 1, .reusable = true}}, SHIFT(141),
-  [526] = {.entry = {.count = 1, .reusable = true}}, SHIFT(139),
-  [528] = {.entry = {.count = 1, .reusable = true}}, SHIFT(388),
-  [530] = {.entry = {.count = 1, .reusable = true}}, SHIFT(274),
+  [510] = {.entry = {.count = 1, .reusable = true}}, SHIFT(89),
+  [512] = {.entry = {.count = 1, .reusable = true}}, SHIFT(116),
+  [514] = {.entry = {.count = 1, .reusable = true}}, SHIFT(63),
+  [516] = {.entry = {.count = 1, .reusable = true}}, SHIFT(67),
+  [518] = {.entry = {.count = 1, .reusable = true}}, SHIFT(64),
+  [520] = {.entry = {.count = 1, .reusable = true}}, SHIFT(122),
+  [522] = {.entry = {.count = 1, .reusable = true}}, SHIFT(159),
+  [524] = {.entry = {.count = 1, .reusable = true}}, SHIFT(158),
+  [526] = {.entry = {.count = 1, .reusable = true}}, SHIFT(136),
+  [528] = {.entry = {.count = 1, .reusable = true}}, SHIFT(311),
+  [530] = {.entry = {.count = 1, .reusable = true}}, SHIFT(260),
   [532] = {.entry = {.count = 1, .reusable = true}}, SHIFT(26),
-  [534] = {.entry = {.count = 1, .reusable = true}}, SHIFT(136),
-  [536] = {.entry = {.count = 1, .reusable = true}}, SHIFT(158),
-  [538] = {.entry = {.count = 1, .reusable = true}}, SHIFT(85),
-  [540] = {.entry = {.count = 1, .reusable = true}}, SHIFT(160),
-  [542] = {.entry = {.count = 1, .reusable = true}}, SHIFT(149),
-  [544] = {.entry = {.count = 1, .reusable = true}}, SHIFT(170),
-  [546] = {.entry = {.count = 1, .reusable = true}}, SHIFT(172),
-  [548] = {.entry = {.count = 1, .reusable = true}}, SHIFT(115),
-  [550] = {.entry = {.count = 1, .reusable = true}}, SHIFT(114),
-  [552] = {.entry = {.count = 1, .reusable = true}}, SHIFT(112),
-  [554] = {.entry = {.count = 1, .reusable = true}}, SHIFT(173),
-  [556] = {.entry = {.count = 1, .reusable = true}}, SHIFT(110),
-  [558] = {.entry = {.count = 1, .reusable = true}}, SHIFT(176),
-  [560] = {.entry = {.count = 1, .reusable = true}}, SHIFT(107),
-  [562] = {.entry = {.count = 1, .reusable = true}}, SHIFT(102),
-  [564] = {.entry = {.count = 1, .reusable = true}}, SHIFT(100),
+  [534] = {.entry = {.count = 1, .reusable = true}}, SHIFT(127),
+  [536] = {.entry = {.count = 1, .reusable = true}}, SHIFT(221),
+  [538] = {.entry = {.count = 1, .reusable = true}}, SHIFT(87),
+  [540] = {.entry = {.count = 1, .reusable = true}}, SHIFT(222),
+  [542] = {.entry = {.count = 1, .reusable = true}}, SHIFT(230),
+  [544] = {.entry = {.count = 1, .reusable = true}}, SHIFT(242),
+  [546] = {.entry = {.count = 1, .reusable = true}}, SHIFT(245),
+  [548] = {.entry = {.count = 1, .reusable = true}}, SHIFT(160),
+  [550] = {.entry = {.count = 1, .reusable = true}}, SHIFT(154),
+  [552] = {.entry = {.count = 1, .reusable = true}}, SHIFT(152),
+  [554] = {.entry = {.count = 1, .reusable = true}}, SHIFT(248),
+  [556] = {.entry = {.count = 1, .reusable = true}}, SHIFT(149),
+  [558] = {.entry = {.count = 1, .reusable = true}}, SHIFT(249),
+  [560] = {.entry = {.count = 1, .reusable = true}}, SHIFT(147),
+  [562] = {.entry = {.count = 1, .reusable = true}}, SHIFT(142),
+  [564] = {.entry = {.count = 1, .reusable = true}}, SHIFT(140),
   [566] = {.entry = {.count = 1, .reusable = true}}, SHIFT(13),
   [568] = {.entry = {.count = 1, .reusable = true}}, SHIFT(12),
   [570] = {.entry = {.count = 1, .reusable = true}}, SHIFT(11),
-  [572] = {.entry = {.count = 1, .reusable = true}}, SHIFT(30),
-  [574] = {.entry = {.count = 1, .reusable = true}}, SHIFT(453),
-  [576] = {.entry = {.count = 1, .reusable = true}}, SHIFT(451),
-  [578] = {.entry = {.count = 1, .reusable = true}}, SHIFT(450),
-  [580] = {.entry = {.count = 1, .reusable = true}}, SHIFT(491),
-  [582] = {.entry = {.count = 1, .reusable = true}}, SHIFT(79),
-  [584] = {.entry = {.count = 1, .reusable = true}}, SHIFT(69),
-  [586] = {.entry = {.count = 1, .reusable = true}}, SHIFT(94),
-  [588] = {.entry = {.count = 1, .reusable = true}}, SHIFT(82),
-  [590] = {.entry = {.count = 1, .reusable = true}}, SHIFT(181),
-  [592] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__string, 3, .production_id = 9),
-  [594] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__string, 3, .production_id = 9),
-  [596] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__string, 1),
-  [598] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__string, 1),
+  [572] = {.entry = {.count = 1, .reusable = true}}, SHIFT(29),
+  [574] = {.entry = {.count = 1, .reusable = true}}, SHIFT(463),
+  [576] = {.entry = {.count = 1, .reusable = true}}, SHIFT(457),
+  [578] = {.entry = {.count = 1, .reusable = true}}, SHIFT(456),
+  [580] = {.entry = {.count = 1, .reusable = true}}, SHIFT(482),
+  [582] = {.entry = {.count = 1, .reusable = true}}, SHIFT(86),
+  [584] = {.entry = {.count = 1, .reusable = true}}, SHIFT(71),
+  [586] = {.entry = {.count = 1, .reusable = true}}, SHIFT(128),
+  [588] = {.entry = {.count = 1, .reusable = true}}, SHIFT(88),
+  [590] = {.entry = {.count = 1, .reusable = true}}, SHIFT(203),
+  [592] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__string, 1),
+  [594] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__string, 1),
+  [596] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__string, 3, .production_id = 9),
+  [598] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__string, 3, .production_id = 9),
   [600] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_pattern, 1, .production_id = 3),
   [602] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_pattern, 1, .production_id = 3),
-  [604] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2),
-  [606] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__end, 2),
-  [608] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__end, 2),
+  [604] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__end, 2),
+  [606] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__end, 2),
+  [608] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym_file_repeat1, 2),
   [610] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__end, 3),
   [612] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__end, 3),
-  [614] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_symbol, 1, .production_id = 3),
-  [616] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_symbol, 1, .production_id = 3),
-  [618] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__regex, 1, .production_id = 1),
-  [620] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__regex, 1, .production_id = 1),
+  [614] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__regex, 1, .production_id = 1),
+  [616] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__regex, 1, .production_id = 1),
+  [618] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_symbol, 1, .production_id = 3),
+  [620] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_symbol, 1, .production_id = 3),
   [622] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__regex, 3, .production_id = 10),
   [624] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__regex, 3, .production_id = 10),
   [626] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__regex, 3, .production_id = 9),
   [628] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__regex, 3, .production_id = 9),
-  [630] = {.entry = {.count = 1, .reusable = false}}, SHIFT(33),
-  [632] = {.entry = {.count = 1, .reusable = false}}, SHIFT(467),
-  [634] = {.entry = {.count = 1, .reusable = false}}, SHIFT(468),
-  [636] = {.entry = {.count = 1, .reusable = false}}, SHIFT(469),
-  [638] = {.entry = {.count = 1, .reusable = false}}, SHIFT(17),
-  [640] = {.entry = {.count = 1, .reusable = true}}, SHIFT(161),
-  [642] = {.entry = {.count = 1, .reusable = true}}, SHIFT(33),
-  [644] = {.entry = {.count = 1, .reusable = true}}, SHIFT(56),
-  [646] = {.entry = {.count = 1, .reusable = true}}, SHIFT(58),
-  [648] = {.entry = {.count = 1, .reusable = true}}, SHIFT(404),
-  [650] = {.entry = {.count = 1, .reusable = true}}, SHIFT(401),
-  [652] = {.entry = {.count = 1, .reusable = true}}, SHIFT(299),
-  [654] = {.entry = {.count = 1, .reusable = true}}, SHIFT(252),
-  [656] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_composeobject, 1),
-  [658] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_object, 1),
-  [660] = {.entry = {.count = 1, .reusable = true}}, SHIFT(191),
-  [662] = {.entry = {.count = 1, .reusable = false}}, SHIFT(51),
-  [664] = {.entry = {.count = 1, .reusable = false}}, SHIFT(295),
-  [666] = {.entry = {.count = 1, .reusable = false}}, SHIFT(217),
-  [668] = {.entry = {.count = 1, .reusable = false}}, SHIFT(554),
-  [670] = {.entry = {.count = 1, .reusable = false}}, SHIFT(555),
-  [672] = {.entry = {.count = 1, .reusable = false}}, SHIFT(556),
-  [674] = {.entry = {.count = 1, .reusable = false}}, SHIFT(272),
-  [676] = {.entry = {.count = 1, .reusable = false}}, SHIFT(55),
-  [678] = {.entry = {.count = 1, .reusable = false}}, SHIFT(226),
-  [680] = {.entry = {.count = 1, .reusable = false}}, SHIFT(52),
-  [682] = {.entry = {.count = 1, .reusable = false}}, SHIFT(286),
-  [684] = {.entry = {.count = 1, .reusable = false}}, SHIFT(53),
-  [686] = {.entry = {.count = 1, .reusable = false}}, SHIFT(283),
-  [688] = {.entry = {.count = 2, .reusable = true}}, REDUCE(aux_sym__attributes_repeat1, 2), SHIFT_REPEAT(175),
-  [691] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__attributes_repeat1, 2),
-  [693] = {.entry = {.count = 1, .reusable = true}}, SHIFT(202),
-  [695] = {.entry = {.count = 1, .reusable = true}}, SHIFT(399),
-  [697] = {.entry = {.count = 1, .reusable = true}}, SHIFT(175),
-  [699] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__attributes, 1),
-  [701] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__attributes, 2),
-  [703] = {.entry = {.count = 1, .reusable = false}}, SHIFT(212),
-  [705] = {.entry = {.count = 1, .reusable = false}}, SHIFT(280),
-  [707] = {.entry = {.count = 1, .reusable = true}}, REDUCE(aux_sym__attributes_repeat1, 2),
-  [709] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_attribute, 1),
-  [711] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_attribute, 1),
-  [713] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_foreground, 1),
-  [715] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_color, 1),
-  [717] = {.entry = {.count = 1, .reusable = false}}, SHIFT(93),
-  [719] = {.entry = {.count = 1, .reusable = false}}, SHIFT(369),
-  [721] = {.entry = {.count = 1, .reusable = false}}, SHIFT(474),
-  [723] = {.entry = {.count = 1, .reusable = false}}, SHIFT(471),
-  [725] = {.entry = {.count = 1, .reusable = false}}, SHIFT(478),
-  [727] = {.entry = {.count = 1, .reusable = false}}, SHIFT(235),
-  [729] = {.entry = {.count = 1, .reusable = false}}, SHIFT(300),
-  [731] = {.entry = {.count = 1, .reusable = false}}, SHIFT(116),
-  [733] = {.entry = {.count = 1, .reusable = false}}, SHIFT(354),
-  [735] = {.entry = {.count = 1, .reusable = false}}, SHIFT(531),
-  [737] = {.entry = {.count = 1, .reusable = false}}, SHIFT(532),
-  [739] = {.entry = {.count = 1, .reusable = false}}, SHIFT(533),
-  [741] = {.entry = {.count = 1, .reusable = false}}, SHIFT(507),
-  [743] = {.entry = {.count = 1, .reusable = false}}, SHIFT(346),
-  [745] = {.entry = {.count = 1, .reusable = false}}, SHIFT(121),
-  [747] = {.entry = {.count = 1, .reusable = false}}, SHIFT(391),
-  [749] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2), SHIFT_REPEAT(470),
-  [752] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2), SHIFT_REPEAT(63),
-  [755] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2),
-  [757] = {.entry = {.count = 1, .reusable = false}}, SHIFT(99),
-  [759] = {.entry = {.count = 1, .reusable = false}}, SHIFT(405),
-  [761] = {.entry = {.count = 1, .reusable = false}}, SHIFT(409),
-  [763] = {.entry = {.count = 1, .reusable = false}}, SHIFT(412),
-  [765] = {.entry = {.count = 1, .reusable = false}}, SHIFT(470),
-  [767] = {.entry = {.count = 1, .reusable = false}}, SHIFT(63),
-  [769] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_key, 1),
-  [771] = {.entry = {.count = 1, .reusable = false}}, SHIFT(376),
-  [773] = {.entry = {.count = 1, .reusable = false}}, SHIFT(421),
-  [775] = {.entry = {.count = 1, .reusable = false}}, SHIFT(557),
-  [777] = {.entry = {.count = 1, .reusable = false}}, SHIFT(558),
-  [779] = {.entry = {.count = 1, .reusable = false}}, SHIFT(559),
-  [781] = {.entry = {.count = 1, .reusable = false}}, SHIFT(270),
-  [783] = {.entry = {.count = 1, .reusable = false}}, SHIFT(321),
-  [785] = {.entry = {.count = 1, .reusable = false}}, SHIFT(365),
-  [787] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 3),
-  [789] = {.entry = {.count = 1, .reusable = false}}, SHIFT(132),
-  [791] = {.entry = {.count = 1, .reusable = false}}, SHIFT(538),
-  [793] = {.entry = {.count = 1, .reusable = false}}, SHIFT(539),
-  [795] = {.entry = {.count = 1, .reusable = false}}, SHIFT(540),
-  [797] = {.entry = {.count = 1, .reusable = false}}, SHIFT(199),
-  [799] = {.entry = {.count = 1, .reusable = false}}, SHIFT(101),
-  [801] = {.entry = {.count = 1, .reusable = false}}, SHIFT(402),
-  [803] = {.entry = {.count = 1, .reusable = false}}, SHIFT(534),
-  [805] = {.entry = {.count = 1, .reusable = false}}, SHIFT(97),
-  [807] = {.entry = {.count = 1, .reusable = false}}, SHIFT(349),
-  [809] = {.entry = {.count = 1, .reusable = false}}, SHIFT(168),
-  [811] = {.entry = {.count = 1, .reusable = false}}, SHIFT(39),
-  [813] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options2, 1),
-  [815] = {.entry = {.count = 1, .reusable = false}}, SHIFT(371),
-  [817] = {.entry = {.count = 1, .reusable = false}}, SHIFT(333),
-  [819] = {.entry = {.count = 1, .reusable = false}}, SHIFT(324),
-  [821] = {.entry = {.count = 1, .reusable = false}}, SHIFT(429),
-  [823] = {.entry = {.count = 1, .reusable = false}}, SHIFT(95),
-  [825] = {.entry = {.count = 1, .reusable = false}}, SHIFT(68),
-  [827] = {.entry = {.count = 1, .reusable = false}}, SHIFT(545),
-  [829] = {.entry = {.count = 1, .reusable = false}}, SHIFT(546),
-  [831] = {.entry = {.count = 1, .reusable = false}}, SHIFT(547),
-  [833] = {.entry = {.count = 1, .reusable = false}}, SHIFT(166),
-  [835] = {.entry = {.count = 1, .reusable = false}}, SHIFT(560),
-  [837] = {.entry = {.count = 1, .reusable = false}}, SHIFT(561),
-  [839] = {.entry = {.count = 1, .reusable = false}}, SHIFT(562),
-  [841] = {.entry = {.count = 1, .reusable = false}}, SHIFT(348),
-  [843] = {.entry = {.count = 1, .reusable = false}}, SHIFT(98),
-  [845] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2), SHIFT_REPEAT(534),
-  [848] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2), SHIFT_REPEAT(98),
-  [851] = {.entry = {.count = 1, .reusable = false}}, SHIFT(563),
-  [853] = {.entry = {.count = 1, .reusable = false}}, SHIFT(564),
-  [855] = {.entry = {.count = 1, .reusable = false}}, SHIFT(565),
-  [857] = {.entry = {.count = 1, .reusable = false}}, SHIFT(268),
-  [859] = {.entry = {.count = 1, .reusable = false}}, SHIFT(424),
-  [861] = {.entry = {.count = 1, .reusable = false}}, SHIFT(548),
-  [863] = {.entry = {.count = 1, .reusable = false}}, SHIFT(549),
-  [865] = {.entry = {.count = 1, .reusable = false}}, SHIFT(550),
-  [867] = {.entry = {.count = 1, .reusable = false}}, SHIFT(422),
-  [869] = {.entry = {.count = 1, .reusable = false}}, SHIFT(383),
-  [871] = {.entry = {.count = 1, .reusable = false}}, SHIFT(426),
-  [873] = {.entry = {.count = 1, .reusable = false}}, SHIFT(425),
-  [875] = {.entry = {.count = 1, .reusable = false}}, SHIFT(551),
-  [877] = {.entry = {.count = 1, .reusable = false}}, SHIFT(552),
-  [879] = {.entry = {.count = 1, .reusable = false}}, SHIFT(553),
-  [881] = {.entry = {.count = 1, .reusable = false}}, SHIFT(164),
-  [883] = {.entry = {.count = 1, .reusable = false}}, SHIFT(151),
-  [885] = {.entry = {.count = 1, .reusable = false}}, SHIFT(542),
-  [887] = {.entry = {.count = 1, .reusable = false}}, SHIFT(543),
-  [889] = {.entry = {.count = 1, .reusable = false}}, SHIFT(544),
-  [891] = {.entry = {.count = 1, .reusable = false}}, SHIFT(7),
-  [893] = {.entry = {.count = 1, .reusable = false}}, SHIFT(23),
-  [895] = {.entry = {.count = 1, .reusable = false}}, SHIFT(162),
-  [897] = {.entry = {.count = 1, .reusable = false}}, SHIFT(535),
-  [899] = {.entry = {.count = 1, .reusable = false}}, SHIFT(536),
-  [901] = {.entry = {.count = 1, .reusable = false}}, SHIFT(537),
-  [903] = {.entry = {.count = 1, .reusable = false}}, SHIFT(130),
-  [905] = {.entry = {.count = 1, .reusable = false}}, SHIFT(205),
-  [907] = {.entry = {.count = 1, .reusable = false}}, SHIFT(105),
-  [909] = {.entry = {.count = 1, .reusable = false}}, SHIFT(10),
-  [911] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_group_name, 1, .production_id = 3),
-  [913] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_name, 1, .production_id = 3),
-  [915] = {.entry = {.count = 1, .reusable = true}}, SHIFT(96),
-  [917] = {.entry = {.count = 1, .reusable = true}}, SHIFT(436),
-  [919] = {.entry = {.count = 1, .reusable = true}}, SHIFT(148),
-  [921] = {.entry = {.count = 1, .reusable = true}}, SHIFT(87),
-  [923] = {.entry = {.count = 1, .reusable = false}}, SHIFT(308),
-  [925] = {.entry = {.count = 1, .reusable = false}}, SHIFT(19),
-  [927] = {.entry = {.count = 1, .reusable = false}}, SHIFT(108),
-  [929] = {.entry = {.count = 1, .reusable = true}}, SHIFT(32),
-  [931] = {.entry = {.count = 1, .reusable = false}}, SHIFT(122),
-  [933] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__group, 2),
-  [935] = {.entry = {.count = 1, .reusable = false}}, SHIFT(385),
-  [937] = {.entry = {.count = 1, .reusable = true}}, SHIFT(475),
-  [939] = {.entry = {.count = 1, .reusable = true}}, SHIFT(38),
-  [941] = {.entry = {.count = 1, .reusable = true}}, SHIFT(296),
-  [943] = {.entry = {.count = 1, .reusable = false}}, SHIFT(138),
-  [945] = {.entry = {.count = 1, .reusable = false}}, SHIFT(104),
-  [947] = {.entry = {.count = 1, .reusable = true}}, SHIFT(203),
-  [949] = {.entry = {.count = 1, .reusable = false}}, SHIFT(91),
-  [951] = {.entry = {.count = 1, .reusable = false}}, SHIFT(128),
-  [953] = {.entry = {.count = 1, .reusable = false}}, SHIFT(407),
-  [955] = {.entry = {.count = 1, .reusable = false}}, SHIFT(390),
-  [957] = {.entry = {.count = 1, .reusable = false}}, SHIFT(420),
-  [959] = {.entry = {.count = 1, .reusable = false}}, SHIFT(466),
-  [961] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 5, .production_id = 15),
-  [963] = {.entry = {.count = 1, .reusable = false}}, SHIFT(541),
-  [965] = {.entry = {.count = 1, .reusable = false}}, SHIFT(197),
-  [967] = {.entry = {.count = 1, .reusable = false}}, SHIFT(150),
-  [969] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__strings, 1, .production_id = 3),
-  [971] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2), SHIFT_REPEAT(541),
-  [974] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2), SHIFT_REPEAT(189),
-  [977] = {.entry = {.count = 1, .reusable = false}}, SHIFT(124),
-  [979] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__mailboxes, 1),
-  [981] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_description, 1, .production_id = 3),
-  [983] = {.entry = {.count = 1, .reusable = true}}, SHIFT(472),
-  [985] = {.entry = {.count = 1, .reusable = true}}, SHIFT(81),
-  [987] = {.entry = {.count = 1, .reusable = false}}, SHIFT(189),
-  [989] = {.entry = {.count = 1, .reusable = false}}, SHIFT(123),
-  [991] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__header_fields, 1),
-  [993] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_color, 1),
-  [995] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 6, .production_id = 19),
-  [997] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 6, .production_id = 17),
-  [999] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 2, .production_id = 8), SHIFT_REPEAT(466),
-  [1002] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 2, .production_id = 8),
-  [1004] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 5, .production_id = 18),
-  [1006] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 5),
-  [1008] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 4, .production_id = 16),
-  [1010] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 4, .production_id = 12),
-  [1012] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 4),
-  [1014] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_named_mailboxes_directive_repeat1, 2), SHIFT_REPEAT(103),
-  [1017] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym_named_mailboxes_directive_repeat1, 2),
-  [1019] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__mime_types_repeat1, 2), SHIFT_REPEAT(482),
-  [1022] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__mime_types_repeat1, 2),
-  [1024] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__addresses_repeat1, 2), SHIFT_REPEAT(113),
-  [1027] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__addresses_repeat1, 2),
-  [1029] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__options_repeat1, 2), SHIFT_REPEAT(488),
-  [1032] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options_repeat1, 2),
-  [1034] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__options2_repeat1, 2), SHIFT_REPEAT(386),
-  [1037] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options2_repeat1, 2),
-  [1039] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 3, .production_id = 7),
-  [1041] = {.entry = {.count = 1, .reusable = false}}, SHIFT(488),
-  [1043] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options, 1),
-  [1045] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 3),
-  [1047] = {.entry = {.count = 1, .reusable = false}}, SHIFT(386),
-  [1049] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options2, 3),
-  [1051] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__header_fields_repeat1, 2), SHIFT_REPEAT(123),
-  [1054] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__header_fields_repeat1, 2),
-  [1056] = {.entry = {.count = 1, .reusable = false}}, SHIFT(103),
-  [1058] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_named_mailboxes_directive, 4),
-  [1060] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__mailboxes_repeat1, 2), SHIFT_REPEAT(124),
-  [1063] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__mailboxes_repeat1, 2),
-  [1065] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__strings_repeat1, 2, .production_id = 8), SHIFT_REPEAT(150),
-  [1068] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__strings_repeat1, 2, .production_id = 8),
-  [1070] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__headers_repeat1, 2), SHIFT_REPEAT(127),
-  [1073] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__headers_repeat1, 2),
-  [1075] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__functions_repeat1, 2), SHIFT_REPEAT(473),
-  [1078] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__functions_repeat1, 2),
-  [1080] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_background, 1),
-  [1082] = {.entry = {.count = 1, .reusable = false}}, SHIFT(157),
-  [1084] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__regexes, 1, .production_id = 3),
-  [1086] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mime, 1),
-  [1088] = {.entry = {.count = 1, .reusable = false}}, SHIFT(486),
-  [1090] = {.entry = {.count = 1, .reusable = false}}, SHIFT(455),
-  [1092] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__mimes, 1),
-  [1094] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__maps_repeat1, 2), SHIFT_REPEAT(37),
-  [1097] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__maps_repeat1, 2),
-  [1099] = {.entry = {.count = 1, .reusable = false}}, SHIFT(482),
-  [1101] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__mime_types, 2),
-  [1103] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__mimes_repeat1, 2), SHIFT_REPEAT(455),
-  [1106] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__mimes_repeat1, 2),
-  [1108] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__regexes_repeat1, 2, .production_id = 8), SHIFT_REPEAT(157),
-  [1111] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__regexes_repeat1, 2, .production_id = 8),
-  [1113] = {.entry = {.count = 1, .reusable = false}}, SHIFT(113),
-  [1115] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__addresses, 2),
-  [1117] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options, 2),
-  [1119] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options2, 2),
-  [1121] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__header_fields, 2),
-  [1123] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__addresses, 1),
-  [1125] = {.entry = {.count = 1, .reusable = false}}, SHIFT(473),
-  [1127] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__functions, 2),
-  [1129] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__strings, 2, .production_id = 8),
-  [1131] = {.entry = {.count = 1, .reusable = false}}, SHIFT(37),
-  [1133] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__maps, 1),
-  [1135] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__maps, 2),
-  [1137] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_alias, 1, .production_id = 3),
-  [1139] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__functions, 1),
-  [1141] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__regexes, 2, .production_id = 8),
-  [1143] = {.entry = {.count = 1, .reusable = false}}, SHIFT(127),
-  [1145] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__headers, 2),
-  [1147] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__mailboxes, 2),
-  [1149] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_named_mailboxes_directive, 3),
-  [1151] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__headers, 1),
-  [1153] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__mimes, 2),
-  [1155] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_charset, 1, .production_id = 3),
-  [1157] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__mime_types, 1),
-  [1159] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mime, 3, .production_id = 11),
-  [1161] = {.entry = {.count = 1, .reusable = true}}, SHIFT(355),
-  [1163] = {.entry = {.count = 1, .reusable = true}}, SHIFT(236),
-  [1165] = {.entry = {.count = 1, .reusable = true}}, SHIFT(327),
-  [1167] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mailbox, 1, .production_id = 3),
-  [1169] = {.entry = {.count = 1, .reusable = true}}, SHIFT(446),
-  [1171] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_header_field, 1, .production_id = 3),
-  [1173] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_header, 1, .production_id = 3),
-  [1175] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 6, .production_id = 17),
-  [1177] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 6),
-  [1179] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 5, .production_id = 15),
-  [1181] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 5),
-  [1183] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 4, .production_id = 12),
-  [1185] = {.entry = {.count = 1, .reusable = true}}, SHIFT(316),
-  [1187] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 4),
-  [1189] = {.entry = {.count = 1, .reusable = true}}, SHIFT(431),
-  [1191] = {.entry = {.count = 1, .reusable = false}}, SHIFT(40),
-  [1193] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__space, 1),
-  [1195] = {.entry = {.count = 1, .reusable = false}}, SHIFT(298),
-  [1197] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym_named_mailboxes_directive_repeat1, 3),
-  [1199] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_address, 1, .production_id = 3),
-  [1201] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options2_repeat1, 3),
-  [1203] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_quadoption, 1),
-  [1205] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__space_repeat1, 2),
-  [1207] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__space_repeat1, 2), SHIFT_REPEAT(298),
-  [1210] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_map, 1),
-  [1212] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__strings_repeat1, 2, .production_id = 2),
-  [1214] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__regexes_repeat1, 2, .production_id = 2),
-  [1216] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_timeout_hook_directive, 2, .production_id = 4),
-  [1218] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ungroup_directive, 2, .production_id = 2),
-  [1220] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_folder_hook_directive, 3, .production_id = 6),
-  [1222] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__rx_addr, 2, .production_id = 2),
-  [1224] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__rx_addr, 2),
+  [630] = {.entry = {.count = 1, .reusable = false}}, SHIFT(32),
+  [632] = {.entry = {.count = 1, .reusable = false}}, SHIFT(487),
+  [634] = {.entry = {.count = 1, .reusable = false}}, SHIFT(489),
+  [636] = {.entry = {.count = 1, .reusable = false}}, SHIFT(490),
+  [638] = {.entry = {.count = 1, .reusable = false}}, SHIFT(16),
+  [640] = {.entry = {.count = 1, .reusable = true}}, SHIFT(131),
+  [642] = {.entry = {.count = 1, .reusable = true}}, SHIFT(32),
+  [644] = {.entry = {.count = 1, .reusable = true}}, SHIFT(49),
+  [646] = {.entry = {.count = 1, .reusable = true}}, SHIFT(57),
+  [648] = {.entry = {.count = 1, .reusable = true}}, SHIFT(440),
+  [650] = {.entry = {.count = 1, .reusable = true}}, SHIFT(439),
+  [652] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_composeobject, 1),
+  [654] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_object, 1),
+  [656] = {.entry = {.count = 1, .reusable = true}}, SHIFT(255),
+  [658] = {.entry = {.count = 1, .reusable = true}}, SHIFT(217),
+  [660] = {.entry = {.count = 1, .reusable = true}}, SHIFT(171),
+  [662] = {.entry = {.count = 2, .reusable = true}}, REDUCE(aux_sym__attributes_repeat1, 2), SHIFT_REPEAT(97),
+  [665] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__attributes_repeat1, 2),
+  [667] = {.entry = {.count = 1, .reusable = true}}, SHIFT(404),
+  [669] = {.entry = {.count = 1, .reusable = true}}, SHIFT(97),
+  [671] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__attributes, 1),
+  [673] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__attributes, 2),
+  [675] = {.entry = {.count = 1, .reusable = true}}, SHIFT(78),
+  [677] = {.entry = {.count = 1, .reusable = false}}, SHIFT(55),
+  [679] = {.entry = {.count = 1, .reusable = false}}, SHIFT(264),
+  [681] = {.entry = {.count = 1, .reusable = false}}, SHIFT(261),
+  [683] = {.entry = {.count = 1, .reusable = false}}, SHIFT(554),
+  [685] = {.entry = {.count = 1, .reusable = false}}, SHIFT(555),
+  [687] = {.entry = {.count = 1, .reusable = false}}, SHIFT(556),
+  [689] = {.entry = {.count = 1, .reusable = false}}, SHIFT(298),
+  [691] = {.entry = {.count = 1, .reusable = true}}, REDUCE(aux_sym__attributes_repeat1, 2),
+  [693] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_attribute, 1),
+  [695] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_attribute, 1),
+  [697] = {.entry = {.count = 1, .reusable = false}}, SHIFT(56),
+  [699] = {.entry = {.count = 1, .reusable = false}}, SHIFT(263),
+  [701] = {.entry = {.count = 1, .reusable = false}}, SHIFT(54),
+  [703] = {.entry = {.count = 1, .reusable = false}}, SHIFT(215),
+  [705] = {.entry = {.count = 1, .reusable = false}}, SHIFT(58),
+  [707] = {.entry = {.count = 1, .reusable = false}}, SHIFT(241),
+  [709] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_foreground, 1),
+  [711] = {.entry = {.count = 1, .reusable = false}}, SHIFT(268),
+  [713] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_color, 1),
+  [715] = {.entry = {.count = 1, .reusable = false}}, SHIFT(231),
+  [717] = {.entry = {.count = 1, .reusable = false}}, SHIFT(118),
+  [719] = {.entry = {.count = 1, .reusable = false}}, SHIFT(355),
+  [721] = {.entry = {.count = 1, .reusable = false}}, SHIFT(493),
+  [723] = {.entry = {.count = 1, .reusable = false}}, SHIFT(501),
+  [725] = {.entry = {.count = 1, .reusable = false}}, SHIFT(509),
+  [727] = {.entry = {.count = 1, .reusable = false}}, SHIFT(296),
+  [729] = {.entry = {.count = 1, .reusable = false}}, SHIFT(381),
+  [731] = {.entry = {.count = 1, .reusable = false}}, SHIFT(121),
+  [733] = {.entry = {.count = 1, .reusable = false}}, SHIFT(531),
+  [735] = {.entry = {.count = 1, .reusable = false}}, SHIFT(532),
+  [737] = {.entry = {.count = 1, .reusable = false}}, SHIFT(533),
+  [739] = {.entry = {.count = 1, .reusable = false}}, SHIFT(479),
+  [741] = {.entry = {.count = 1, .reusable = false}}, SHIFT(117),
+  [743] = {.entry = {.count = 1, .reusable = false}}, SHIFT(375),
+  [745] = {.entry = {.count = 1, .reusable = false}}, SHIFT(491),
+  [747] = {.entry = {.count = 1, .reusable = false}}, SHIFT(69),
+  [749] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_key, 1),
+  [751] = {.entry = {.count = 1, .reusable = false}}, SHIFT(360),
+  [753] = {.entry = {.count = 1, .reusable = false}}, SHIFT(363),
+  [755] = {.entry = {.count = 1, .reusable = false}}, SHIFT(144),
+  [757] = {.entry = {.count = 1, .reusable = false}}, SHIFT(334),
+  [759] = {.entry = {.count = 1, .reusable = false}}, SHIFT(534),
+  [761] = {.entry = {.count = 1, .reusable = false}}, SHIFT(92),
+  [763] = {.entry = {.count = 1, .reusable = false}}, SHIFT(145),
+  [765] = {.entry = {.count = 1, .reusable = false}}, SHIFT(362),
+  [767] = {.entry = {.count = 1, .reusable = false}}, SHIFT(106),
+  [769] = {.entry = {.count = 1, .reusable = false}}, SHIFT(51),
+  [771] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options2, 1),
+  [773] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2), SHIFT_REPEAT(491),
+  [776] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2), SHIFT_REPEAT(69),
+  [779] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2),
+  [781] = {.entry = {.count = 1, .reusable = false}}, SHIFT(417),
+  [783] = {.entry = {.count = 1, .reusable = false}}, SHIFT(426),
+  [785] = {.entry = {.count = 1, .reusable = false}}, SHIFT(548),
+  [787] = {.entry = {.count = 1, .reusable = false}}, SHIFT(549),
+  [789] = {.entry = {.count = 1, .reusable = false}}, SHIFT(550),
+  [791] = {.entry = {.count = 1, .reusable = false}}, SHIFT(393),
+  [793] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_color_directive, 5),
+  [795] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_color_directive, 4),
+  [797] = {.entry = {.count = 1, .reusable = false}}, SHIFT(115),
+  [799] = {.entry = {.count = 1, .reusable = false}}, SHIFT(538),
+  [801] = {.entry = {.count = 1, .reusable = false}}, SHIFT(539),
+  [803] = {.entry = {.count = 1, .reusable = false}}, SHIFT(540),
+  [805] = {.entry = {.count = 1, .reusable = false}}, SHIFT(283),
+  [807] = {.entry = {.count = 1, .reusable = false}}, SHIFT(399),
+  [809] = {.entry = {.count = 1, .reusable = false}}, SHIFT(102),
+  [811] = {.entry = {.count = 1, .reusable = false}}, SHIFT(62),
+  [813] = {.entry = {.count = 1, .reusable = false}}, SHIFT(320),
+  [815] = {.entry = {.count = 1, .reusable = false}}, SHIFT(557),
+  [817] = {.entry = {.count = 1, .reusable = false}}, SHIFT(558),
+  [819] = {.entry = {.count = 1, .reusable = false}}, SHIFT(559),
+  [821] = {.entry = {.count = 1, .reusable = false}}, SHIFT(301),
+  [823] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_color, 1),
+  [825] = {.entry = {.count = 1, .reusable = false}}, SHIFT(347),
+  [827] = {.entry = {.count = 1, .reusable = false}}, SHIFT(340),
+  [829] = {.entry = {.count = 1, .reusable = false}}, SHIFT(374),
+  [831] = {.entry = {.count = 1, .reusable = false}}, SHIFT(372),
+  [833] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_background, 1),
+  [835] = {.entry = {.count = 1, .reusable = false}}, SHIFT(405),
+  [837] = {.entry = {.count = 1, .reusable = false}}, SHIFT(424),
+  [839] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2), SHIFT_REPEAT(534),
+  [842] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2), SHIFT_REPEAT(90),
+  [845] = {.entry = {.count = 1, .reusable = false}}, SHIFT(90),
+  [847] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 3),
+  [849] = {.entry = {.count = 1, .reusable = false}}, SHIFT(20),
+  [851] = {.entry = {.count = 1, .reusable = true}}, SHIFT(95),
+  [853] = {.entry = {.count = 1, .reusable = true}}, SHIFT(395),
+  [855] = {.entry = {.count = 1, .reusable = true}}, SHIFT(141),
+  [857] = {.entry = {.count = 1, .reusable = true}}, SHIFT(81),
+  [859] = {.entry = {.count = 1, .reusable = false}}, SHIFT(560),
+  [861] = {.entry = {.count = 1, .reusable = false}}, SHIFT(561),
+  [863] = {.entry = {.count = 1, .reusable = false}}, SHIFT(562),
+  [865] = {.entry = {.count = 1, .reusable = false}}, SHIFT(344),
+  [867] = {.entry = {.count = 1, .reusable = true}}, SHIFT(478),
+  [869] = {.entry = {.count = 1, .reusable = true}}, SHIFT(52),
+  [871] = {.entry = {.count = 1, .reusable = true}}, SHIFT(265),
+  [873] = {.entry = {.count = 1, .reusable = false}}, SHIFT(406),
+  [875] = {.entry = {.count = 1, .reusable = false}}, SHIFT(166),
+  [877] = {.entry = {.count = 1, .reusable = false}}, SHIFT(542),
+  [879] = {.entry = {.count = 1, .reusable = false}}, SHIFT(543),
+  [881] = {.entry = {.count = 1, .reusable = false}}, SHIFT(544),
+  [883] = {.entry = {.count = 1, .reusable = false}}, SHIFT(22),
+  [885] = {.entry = {.count = 1, .reusable = false}}, SHIFT(545),
+  [887] = {.entry = {.count = 1, .reusable = false}}, SHIFT(546),
+  [889] = {.entry = {.count = 1, .reusable = false}}, SHIFT(547),
+  [891] = {.entry = {.count = 1, .reusable = false}}, SHIFT(187),
+  [893] = {.entry = {.count = 1, .reusable = false}}, SHIFT(551),
+  [895] = {.entry = {.count = 1, .reusable = false}}, SHIFT(552),
+  [897] = {.entry = {.count = 1, .reusable = false}}, SHIFT(553),
+  [899] = {.entry = {.count = 1, .reusable = false}}, SHIFT(182),
+  [901] = {.entry = {.count = 1, .reusable = true}}, SHIFT(31),
+  [903] = {.entry = {.count = 1, .reusable = false}}, SHIFT(563),
+  [905] = {.entry = {.count = 1, .reusable = false}}, SHIFT(564),
+  [907] = {.entry = {.count = 1, .reusable = false}}, SHIFT(565),
+  [909] = {.entry = {.count = 1, .reusable = false}}, SHIFT(304),
+  [911] = {.entry = {.count = 1, .reusable = false}}, SHIFT(425),
+  [913] = {.entry = {.count = 1, .reusable = false}}, SHIFT(418),
+  [915] = {.entry = {.count = 1, .reusable = true}}, SHIFT(279),
+  [917] = {.entry = {.count = 1, .reusable = false}}, SHIFT(186),
+  [919] = {.entry = {.count = 1, .reusable = false}}, SHIFT(535),
+  [921] = {.entry = {.count = 1, .reusable = false}}, SHIFT(536),
+  [923] = {.entry = {.count = 1, .reusable = false}}, SHIFT(537),
+  [925] = {.entry = {.count = 1, .reusable = false}}, SHIFT(271),
+  [927] = {.entry = {.count = 1, .reusable = false}}, SHIFT(471),
+  [929] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 5, .production_id = 15),
+  [931] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__strings_repeat1, 2, .production_id = 8), SHIFT_REPEAT(190),
+  [934] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__strings_repeat1, 2, .production_id = 8),
+  [936] = {.entry = {.count = 1, .reusable = false}}, SHIFT(190),
+  [938] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__strings, 1, .production_id = 3),
+  [940] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__regexes_repeat1, 2, .production_id = 8), SHIFT_REPEAT(236),
+  [943] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__regexes_repeat1, 2, .production_id = 8),
+  [945] = {.entry = {.count = 1, .reusable = false}}, SHIFT(100),
+  [947] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__addresses, 2),
+  [949] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_name, 1, .production_id = 3),
+  [951] = {.entry = {.count = 1, .reusable = false}}, SHIFT(483),
+  [953] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__functions, 1),
+  [955] = {.entry = {.count = 1, .reusable = false}}, SHIFT(110),
+  [957] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__mailboxes, 1),
+  [959] = {.entry = {.count = 1, .reusable = false}}, SHIFT(492),
+  [961] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options, 2),
+  [963] = {.entry = {.count = 1, .reusable = false}}, SHIFT(386),
+  [965] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options2, 2),
+  [967] = {.entry = {.count = 1, .reusable = false}}, SHIFT(109),
+  [969] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__header_fields, 2),
+  [971] = {.entry = {.count = 1, .reusable = false}}, SHIFT(134),
+  [973] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_named_mailboxes_directive, 3),
+  [975] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__header_fields, 1),
+  [977] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__mailboxes, 2),
+  [979] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_group_name, 1, .production_id = 3),
+  [981] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__group, 2),
+  [983] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__strings, 2, .production_id = 8),
+  [985] = {.entry = {.count = 1, .reusable = false}}, SHIFT(113),
+  [987] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__headers, 2),
+  [989] = {.entry = {.count = 1, .reusable = false}}, SHIFT(236),
+  [991] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__regexes, 1, .production_id = 3),
+  [993] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2), SHIFT_REPEAT(541),
+  [996] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_key_repeat1, 2), SHIFT_REPEAT(193),
+  [999] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__mimes_repeat1, 2), SHIFT_REPEAT(458),
+  [1002] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__mimes_repeat1, 2),
+  [1004] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__headers, 1),
+  [1006] = {.entry = {.count = 1, .reusable = false}}, SHIFT(488),
+  [1008] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__mime_types, 2),
+  [1010] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__maps_repeat1, 2), SHIFT_REPEAT(37),
+  [1013] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__maps_repeat1, 2),
+  [1015] = {.entry = {.count = 1, .reusable = false}}, SHIFT(541),
+  [1017] = {.entry = {.count = 1, .reusable = false}}, SHIFT(193),
+  [1019] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__functions, 2),
+  [1021] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__functions_repeat1, 2), SHIFT_REPEAT(483),
+  [1024] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__functions_repeat1, 2),
+  [1026] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mime, 1),
+  [1028] = {.entry = {.count = 1, .reusable = false}}, SHIFT(476),
+  [1030] = {.entry = {.count = 1, .reusable = false}}, SHIFT(458),
+  [1032] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__mimes, 1),
+  [1034] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__headers_repeat1, 2), SHIFT_REPEAT(113),
+  [1037] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__headers_repeat1, 2),
+  [1039] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__mailboxes_repeat1, 2), SHIFT_REPEAT(110),
+  [1042] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__mailboxes_repeat1, 2),
+  [1044] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_named_mailboxes_directive, 4),
+  [1046] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__header_fields_repeat1, 2), SHIFT_REPEAT(109),
+  [1049] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__header_fields_repeat1, 2),
+  [1051] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options2, 3),
+  [1053] = {.entry = {.count = 1, .reusable = false}}, SHIFT(37),
+  [1055] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__maps, 2),
+  [1057] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 3),
+  [1059] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__mime_types, 1),
+  [1061] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 3, .production_id = 7),
+  [1063] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__mimes, 2),
+  [1065] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options, 1),
+  [1067] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 6, .production_id = 19),
+  [1069] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 6, .production_id = 17),
+  [1071] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 2, .production_id = 8), SHIFT_REPEAT(471),
+  [1074] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 2, .production_id = 8),
+  [1076] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__options2_repeat1, 2), SHIFT_REPEAT(386),
+  [1079] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options2_repeat1, 2),
+  [1081] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 5, .production_id = 18),
+  [1083] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 5),
+  [1085] = {.entry = {.count = 1, .reusable = false}}, SHIFT(199),
+  [1087] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__maps, 1),
+  [1089] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__options_repeat1, 2), SHIFT_REPEAT(492),
+  [1092] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options_repeat1, 2),
+  [1094] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__regexes, 2, .production_id = 8),
+  [1096] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 4, .production_id = 16),
+  [1098] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 4, .production_id = 12),
+  [1100] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__options3, 4),
+  [1102] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__addresses_repeat1, 2), SHIFT_REPEAT(100),
+  [1105] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__addresses_repeat1, 2),
+  [1107] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym_named_mailboxes_directive_repeat1, 2), SHIFT_REPEAT(134),
+  [1110] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym_named_mailboxes_directive_repeat1, 2),
+  [1112] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__addresses, 1),
+  [1114] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__mime_types_repeat1, 2), SHIFT_REPEAT(488),
+  [1117] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__mime_types_repeat1, 2),
+  [1119] = {.entry = {.count = 1, .reusable = true}}, SHIFT(507),
+  [1121] = {.entry = {.count = 1, .reusable = true}}, SHIFT(68),
+  [1123] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_address, 1, .production_id = 3),
+  [1125] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options2_repeat1, 3),
+  [1127] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__space_repeat1, 2),
+  [1129] = {.entry = {.count = 2, .reusable = false}}, REDUCE(aux_sym__space_repeat1, 2), SHIFT_REPEAT(254),
+  [1132] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_map, 1),
+  [1134] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym_named_mailboxes_directive_repeat1, 3),
+  [1136] = {.entry = {.count = 1, .reusable = true}}, SHIFT(431),
+  [1138] = {.entry = {.count = 1, .reusable = false}}, SHIFT(47),
+  [1140] = {.entry = {.count = 1, .reusable = true}}, SHIFT(397),
+  [1142] = {.entry = {.count = 1, .reusable = true}}, SHIFT(206),
+  [1144] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 4),
+  [1146] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 4, .production_id = 12),
+  [1148] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 5),
+  [1150] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_quadoption, 1),
+  [1152] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 5, .production_id = 15),
+  [1154] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 6),
+  [1156] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__options3_repeat1, 6, .production_id = 17),
+  [1158] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mime, 3, .production_id = 11),
+  [1160] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__strings_repeat1, 2, .production_id = 2),
+  [1162] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_charset, 1, .production_id = 3),
+  [1164] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__space, 1),
+  [1166] = {.entry = {.count = 1, .reusable = false}}, SHIFT(254),
+  [1168] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_alias, 1, .production_id = 3),
+  [1170] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_header, 1, .production_id = 3),
+  [1172] = {.entry = {.count = 1, .reusable = true}}, SHIFT(335),
+  [1174] = {.entry = {.count = 1, .reusable = true}}, SHIFT(411),
+  [1176] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_header_field, 1, .production_id = 3),
+  [1178] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_description, 1, .production_id = 3),
+  [1180] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mailbox, 1, .production_id = 3),
+  [1182] = {.entry = {.count = 1, .reusable = false}}, REDUCE(aux_sym__regexes_repeat1, 2, .production_id = 2),
+  [1184] = {.entry = {.count = 1, .reusable = true}}, SHIFT(351),
+  [1186] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_attachments_directive, 3),
+  [1188] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__rx_addr, 2, .production_id = 2),
+  [1190] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym__rx_addr, 2),
+  [1192] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ifdef_directive, 3),
+  [1194] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unignore_directive, 2, .production_id = 2),
+  [1196] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mbox_hook_directive, 3, .production_id = 6),
+  [1198] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_message_hook_directive, 3, .production_id = 4),
+  [1200] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ifndef_directive, 3),
+  [1202] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unmono_directive, 3),
+  [1204] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_open_hook_directive, 3, .production_id = 6),
+  [1206] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_shell_command, 1, .production_id = 3),
+  [1208] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_close_hook_directive, 3, .production_id = 6),
+  [1210] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_append_hook_directive, 3, .production_id = 6),
+  [1212] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_reply_hook_directive, 3, .production_id = 4),
+  [1214] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_send_hook_directive, 3, .production_id = 4),
+  [1216] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_send2_hook_directive, 3, .production_id = 4),
+  [1218] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_spam_directive, 3, .production_id = 2),
+  [1220] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_format, 1, .production_id = 3),
+  [1222] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_subjectrx_directive, 3, .production_id = 2),
+  [1224] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_replacement, 1, .production_id = 3),
   [1226] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_group_directive, 3, .production_id = 7),
-  [1228] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ungroup_directive, 3),
-  [1230] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ungroup_directive, 3, .production_id = 7),
-  [1232] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ifdef_directive, 3),
-  [1234] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ifndef_directive, 3),
-  [1236] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_lists_directive, 3, .production_id = 7),
-  [1238] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unlists_directive, 3),
-  [1240] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unlists_directive, 3, .production_id = 7),
-  [1242] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_subscribe_directive, 3, .production_id = 7),
-  [1244] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unsubscribe_directive, 3),
-  [1246] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unsubscribe_directive, 3, .production_id = 7),
-  [1248] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unmacro_directive, 3),
-  [1250] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unauto_view_directive, 2),
-  [1252] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_auto_view_directive, 2),
-  [1254] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mbox_hook_directive, 3, .production_id = 6),
-  [1256] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_message_hook_directive, 3, .production_id = 4),
-  [1258] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_alternates_directive, 3, .production_id = 7),
-  [1260] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unmono_directive, 3),
-  [1262] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_open_hook_directive, 3, .production_id = 6),
-  [1264] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_shell_command, 1, .production_id = 3),
-  [1266] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_close_hook_directive, 3, .production_id = 6),
-  [1268] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_append_hook_directive, 3, .production_id = 6),
-  [1270] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_reply_hook_directive, 3, .production_id = 4),
-  [1272] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_send_hook_directive, 3, .production_id = 4),
-  [1274] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_send2_hook_directive, 3, .production_id = 4),
-  [1276] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_spam_directive, 3, .production_id = 2),
-  [1278] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_format, 1, .production_id = 3),
-  [1280] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_subjectrx_directive, 3, .production_id = 2),
-  [1282] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_replacement, 1, .production_id = 3),
-  [1284] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_alias_directive, 3, .production_id = 4),
-  [1286] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unattachments_directive, 2),
-  [1288] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalternates_directive, 3),
-  [1290] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_setenv_directive, 3),
-  [1292] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_score_directive, 3),
-  [1294] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalternates_directive, 3, .production_id = 7),
-  [1296] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_attachments_directive, 2),
-  [1298] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalternative_order_directive, 2),
-  [1300] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_alias_directive, 4, .production_id = 4),
-  [1302] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_alternative_order_directive, 2),
-  [1304] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_account_hook_directive, 3, .production_id = 6),
-  [1306] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_group_name, 1, .production_id = 3),
-  [1308] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_attachments_directive, 4),
-  [1310] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__group, 2),
-  [1312] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ignore_directive, 2, .production_id = 2),
-  [1314] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unattachments_directive, 4),
-  [1316] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unignore_directive, 2),
-  [1318] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_bind_directive, 4),
-  [1320] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalternates_directive, 2, .production_id = 2),
-  [1322] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalternates_directive, 2),
-  [1324] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_source_directive, 2, .production_id = 5),
-  [1326] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unscore_directive, 2),
-  [1328] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_alternates_directive, 2, .production_id = 2),
-  [1330] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_index_format_hook_directive, 4, .production_id = 12),
-  [1332] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_folder_hook_directive, 4, .production_id = 13),
-  [1334] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_sidebar_unpin_directive, 2),
-  [1336] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_sidebar_pin_directive, 2),
-  [1338] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_macro_directive, 4),
-  [1340] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_sequence, 1, .production_id = 3),
-  [1342] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unsetenv_directive, 2),
-  [1344] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_finish_directive, 1),
-  [1346] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mbox_hook_directive, 4, .production_id = 14),
-  [1348] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mono_directive, 4, .production_id = 12),
-  [1350] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_toggle_directive, 2),
+  [1228] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalias_directive, 2),
+  [1230] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ungroup_directive, 3),
+  [1232] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_exec_directive, 2),
+  [1234] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_lists_directive, 3, .production_id = 7),
+  [1236] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_setenv_directive, 3),
+  [1238] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_score_directive, 3),
+  [1240] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unlists_directive, 3),
+  [1242] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mailboxes_directive, 2),
+  [1244] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_alias_directive, 4, .production_id = 4),
+  [1246] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unlists_directive, 3, .production_id = 7),
+  [1248] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_subscribe_directive, 3, .production_id = 7),
+  [1250] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unsubscribe_directive, 3),
+  [1252] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unsubscribe_directive, 3, .production_id = 7),
+  [1254] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_alternates_directive, 2, .production_id = 2),
+  [1256] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unmacro_directive, 3),
+  [1258] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalternative_order_directive, 2),
+  [1260] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_folder_hook_directive, 3, .production_id = 6),
+  [1262] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_attachments_directive, 4),
+  [1264] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalternates_directive, 2),
+  [1266] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unattachments_directive, 4),
+  [1268] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_save_hook_directive, 3, .production_id = 4),
+  [1270] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_fcc_hook_directive, 3, .production_id = 4),
+  [1272] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_bind_directive, 4),
+  [1274] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unmailboxes_directive, 2),
+  [1276] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_fcc_save_hook_directive, 3),
+  [1278] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mailto_allow_directive, 2),
+  [1280] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unmailto_allow_directive, 2),
+  [1282] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_echo_directive, 2),
+  [1284] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_group_name, 1, .production_id = 3),
+  [1286] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym__group, 2),
+  [1288] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalternates_directive, 2, .production_id = 2),
+  [1290] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_index_format_hook_directive, 4, .production_id = 12),
+  [1292] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_keyid, 1, .production_id = 3),
+  [1294] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_crypt_hook_directive, 3, .production_id = 6),
+  [1296] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_folder_hook_directive, 4, .production_id = 13),
+  [1298] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_uncolor_directive, 3),
+  [1300] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_alternative_order_directive, 2),
+  [1302] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unignore_directive, 2),
+  [1304] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_attachments_directive, 2),
+  [1306] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_macro_directive, 4),
+  [1308] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_sequence, 1, .production_id = 3),
+  [1310] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_message, 1, .production_id = 3),
+  [1312] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unattachments_directive, 2),
+  [1314] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_iconv_hook_directive, 3, .production_id = 4),
+  [1316] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_charset_hook_directive, 3, .production_id = 4),
+  [1318] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mbox_hook_directive, 4, .production_id = 14),
+  [1320] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mono_directive, 4, .production_id = 12),
+  [1322] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unbind_directive, 3),
+  [1324] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_cd_directive, 2),
+  [1326] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_directory, 1, .production_id = 3),
+  [1328] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_group_directive, 2, .production_id = 2),
+  [1330] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unattachments_directive, 3),
+  [1332] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ignore_directive, 2, .production_id = 2),
+  [1334] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ungroup_directive, 2),
+  [1336] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mime_lookup_directive, 2),
+  [1338] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unmime_lookup_directive, 2),
+  [1340] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalternates_directive, 3, .production_id = 7),
+  [1342] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalternates_directive, 3),
+  [1344] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_alternates_directive, 3, .production_id = 7),
+  [1346] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ungroup_directive, 2, .production_id = 2),
+  [1348] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_my_hdr_directive, 2, .production_id = 2),
+  [1350] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unmy_hdr_directive, 2),
   [1352] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalias_directive, 3),
-  [1354] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unhdr_order_directive, 2),
-  [1356] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_fcc_hook_directive, 3, .production_id = 4),
-  [1358] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_reset_directive, 2),
-  [1360] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unset_directive, 2),
-  [1362] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_set_directive, 2),
-  [1364] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_fcc_save_hook_directive, 3),
-  [1366] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_set_directive, 2, .production_id = 2),
-  [1368] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unignore_directive, 2, .production_id = 2),
-  [1370] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mailboxes_directive, 2),
-  [1372] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unhook_directive, 2),
-  [1374] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unalias_directive, 2),
-  [1376] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_color_directive, 5),
-  [1378] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_hook_type, 1),
-  [1380] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unmailboxes_directive, 2),
-  [1382] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_attachments_directive, 3),
-  [1384] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_color_directive, 5, .production_id = 15),
-  [1386] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_index_format_hook_directive, 5, .production_id = 15),
-  [1388] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mailto_allow_directive, 2),
-  [1390] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_shutdown_hook_directive, 2, .production_id = 4),
-  [1392] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_keyid, 1, .production_id = 3),
-  [1394] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unmailto_allow_directive, 2),
-  [1396] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_startup_hook_directive, 2, .production_id = 4),
-  [1398] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_crypt_hook_directive, 3, .production_id = 6),
-  [1400] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unsubscribe_from_directive, 2),
-  [1402] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_uri, 1, .production_id = 3),
-  [1404] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_subscribe_to_directive, 2),
-  [1406] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_color_directive, 6),
-  [1408] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_color_directive, 6, .production_id = 17),
-  [1410] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_uncolor_directive, 3),
-  [1412] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unsubjectrx_directive, 2, .production_id = 2),
-  [1414] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_exec_directive, 2),
-  [1416] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unsubjectrx_directive, 2),
-  [1418] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_nospam_directive, 2, .production_id = 2),
-  [1420] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_nospam_directive, 2),
-  [1422] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_push_directive, 2, .production_id = 2),
-  [1424] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unmy_hdr_directive, 2),
-  [1426] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_my_hdr_directive, 2, .production_id = 2),
-  [1428] = {.entry = {.count = 1, .reusable = true}}, SHIFT(42),
-  [1430] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_echo_directive, 2),
-  [1432] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_message, 1, .production_id = 3),
-  [1434] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_cd_directive, 2),
-  [1436] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_group_directive, 2, .production_id = 2),
-  [1438] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ungroup_directive, 2),
-  [1440] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_directory, 1, .production_id = 3),
-  [1442] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_save_hook_directive, 3, .production_id = 4),
-  [1444] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_hdr_order_directive, 2),
-  [1446] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_iconv_hook_directive, 3, .production_id = 4),
-  [1448] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_charset_hook_directive, 3, .production_id = 4),
-  [1450] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unbind_directive, 3),
-  [1452] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unattachments_directive, 3),
-  [1454] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unmime_lookup_directive, 2),
-  [1456] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_mime_lookup_directive, 2),
-  [1458] = {.entry = {.count = 1, .reusable = true}}, SHIFT(99),
-  [1460] = {.entry = {.count = 1, .reusable = true}}, SHIFT(476),
-  [1462] = {.entry = {.count = 1, .reusable = true}}, SHIFT(477),
-  [1464] = {.entry = {.count = 1, .reusable = true}}, SHIFT(225),
-  [1466] = {.entry = {.count = 1, .reusable = true}}, SHIFT(262),
-  [1468] = {.entry = {.count = 1, .reusable = true}}, SHIFT(254),
-  [1470] = {.entry = {.count = 1, .reusable = true}}, SHIFT(93),
-  [1472] = {.entry = {.count = 1, .reusable = false}}, SHIFT(480),
-  [1474] = {.entry = {.count = 1, .reusable = true}}, SHIFT(20),
-  [1476] = {.entry = {.count = 1, .reusable = true}}, SHIFT(24),
-  [1478] = {.entry = {.count = 1, .reusable = true}}, SHIFT(367),
-  [1480] = {.entry = {.count = 1, .reusable = true}}, SHIFT(287),
-  [1482] = {.entry = {.count = 1, .reusable = true}}, SHIFT(481),
-  [1484] = {.entry = {.count = 1, .reusable = true}}, SHIFT(501),
-  [1486] = {.entry = {.count = 1, .reusable = true}}, SHIFT(483),
-  [1488] = {.entry = {.count = 1, .reusable = true}}, SHIFT(489),
-  [1490] = {.entry = {.count = 1, .reusable = true}}, SHIFT(493),
-  [1492] = {.entry = {.count = 1, .reusable = true}}, SHIFT(245),
-  [1494] = {.entry = {.count = 1, .reusable = true}}, SHIFT(302),
-  [1496] = {.entry = {.count = 1, .reusable = true}}, SHIFT(509),
-  [1498] = {.entry = {.count = 1, .reusable = true}}, SHIFT(291),
-  [1500] = {.entry = {.count = 1, .reusable = true}}, SHIFT(351),
-  [1502] = {.entry = {.count = 1, .reusable = true}}, SHIFT(492),
-  [1504] = {.entry = {.count = 1, .reusable = true}}, SHIFT(352),
-  [1506] = {.entry = {.count = 1, .reusable = true}}, SHIFT(21),
-  [1508] = {.entry = {.count = 1, .reusable = true}}, SHIFT(16),
-  [1510] = {.entry = {.count = 1, .reusable = true}}, SHIFT(292),
-  [1512] = {.entry = {.count = 1, .reusable = true}}, SHIFT(366),
-  [1514] = {.entry = {.count = 1, .reusable = true}}, SHIFT(264),
-  [1516] = {.entry = {.count = 1, .reusable = true}}, SHIFT(294),
-  [1518] = {.entry = {.count = 1, .reusable = true}}, SHIFT(75),
-  [1520] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_disposition, 1, .production_id = 3),
-  [1522] = {.entry = {.count = 1, .reusable = true}}, SHIFT(380),
-  [1524] = {.entry = {.count = 1, .reusable = true}}, SHIFT(307),
-  [1526] = {.entry = {.count = 1, .reusable = true}}, SHIFT(306),
-  [1528] = {.entry = {.count = 1, .reusable = true}}, SHIFT(485),
-  [1530] = {.entry = {.count = 1, .reusable = true}}, SHIFT(180),
-  [1532] = {.entry = {.count = 1, .reusable = true}}, SHIFT(201),
-  [1534] = {.entry = {.count = 1, .reusable = true}}, SHIFT(200),
-  [1536] = {.entry = {.count = 1, .reusable = true}}, SHIFT(188),
-  [1538] = {.entry = {.count = 1, .reusable = true}}, SHIFT(263),
-  [1540] = {.entry = {.count = 1, .reusable = true}}, SHIFT(25),
-  [1542] = {.entry = {.count = 1, .reusable = true}}, SHIFT(156),
-  [1544] = {.entry = {.count = 1, .reusable = true}}, SHIFT(374),
-  [1546] = {.entry = {.count = 1, .reusable = true}},  ACCEPT_INPUT(),
-  [1548] = {.entry = {.count = 1, .reusable = true}}, SHIFT(174),
-  [1550] = {.entry = {.count = 1, .reusable = true}}, SHIFT(271),
-  [1552] = {.entry = {.count = 1, .reusable = true}}, SHIFT(269),
-  [1554] = {.entry = {.count = 1, .reusable = true}}, SHIFT(347),
-  [1556] = {.entry = {.count = 1, .reusable = true}}, SHIFT(267),
-  [1558] = {.entry = {.count = 1, .reusable = true}}, SHIFT(494),
-  [1560] = {.entry = {.count = 1, .reusable = true}}, SHIFT(495),
-  [1562] = {.entry = {.count = 1, .reusable = true}}, SHIFT(496),
-  [1564] = {.entry = {.count = 1, .reusable = true}}, SHIFT(497),
-  [1566] = {.entry = {.count = 1, .reusable = true}}, SHIFT(498),
-  [1568] = {.entry = {.count = 1, .reusable = true}}, SHIFT(499),
-  [1570] = {.entry = {.count = 1, .reusable = true}}, SHIFT(500),
-  [1572] = {.entry = {.count = 1, .reusable = true}}, SHIFT(502),
-  [1574] = {.entry = {.count = 1, .reusable = true}}, SHIFT(503),
-  [1576] = {.entry = {.count = 1, .reusable = true}}, SHIFT(504),
-  [1578] = {.entry = {.count = 1, .reusable = true}}, SHIFT(505),
-  [1580] = {.entry = {.count = 1, .reusable = true}}, SHIFT(506),
-  [1582] = {.entry = {.count = 1, .reusable = true}}, SHIFT(464),
-  [1584] = {.entry = {.count = 1, .reusable = true}}, SHIFT(508),
-  [1586] = {.entry = {.count = 1, .reusable = true}}, SHIFT(510),
-  [1588] = {.entry = {.count = 1, .reusable = true}}, SHIFT(511),
-  [1590] = {.entry = {.count = 1, .reusable = true}}, SHIFT(512),
-  [1592] = {.entry = {.count = 1, .reusable = true}}, SHIFT(513),
-  [1594] = {.entry = {.count = 1, .reusable = true}}, SHIFT(514),
-  [1596] = {.entry = {.count = 1, .reusable = true}}, SHIFT(465),
-  [1598] = {.entry = {.count = 1, .reusable = true}}, SHIFT(516),
-  [1600] = {.entry = {.count = 1, .reusable = true}}, SHIFT(517),
-  [1602] = {.entry = {.count = 1, .reusable = true}}, SHIFT(518),
-  [1604] = {.entry = {.count = 1, .reusable = true}}, SHIFT(519),
-  [1606] = {.entry = {.count = 1, .reusable = true}}, SHIFT(520),
-  [1608] = {.entry = {.count = 1, .reusable = true}}, SHIFT(521),
-  [1610] = {.entry = {.count = 1, .reusable = true}}, SHIFT(522),
-  [1612] = {.entry = {.count = 1, .reusable = true}}, SHIFT(523),
-  [1614] = {.entry = {.count = 1, .reusable = true}}, SHIFT(524),
-  [1616] = {.entry = {.count = 1, .reusable = true}}, SHIFT(525),
-  [1618] = {.entry = {.count = 1, .reusable = true}}, SHIFT(526),
-  [1620] = {.entry = {.count = 1, .reusable = true}}, SHIFT(527),
-  [1622] = {.entry = {.count = 1, .reusable = true}}, SHIFT(528),
-  [1624] = {.entry = {.count = 1, .reusable = true}}, SHIFT(529),
-  [1626] = {.entry = {.count = 1, .reusable = true}}, SHIFT(530),
+  [1354] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_color_directive, 5, .production_id = 15),
+  [1356] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_index_format_hook_directive, 5, .production_id = 15),
+  [1358] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_auto_view_directive, 2),
+  [1360] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_alias_directive, 3, .production_id = 4),
+  [1362] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unauto_view_directive, 2),
+  [1364] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_hdr_order_directive, 2),
+  [1366] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_account_hook_directive, 3, .production_id = 6),
+  [1368] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_push_directive, 2, .production_id = 2),
+  [1370] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unhdr_order_directive, 2),
+  [1372] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_nospam_directive, 2),
+  [1374] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_color_directive, 6),
+  [1376] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_color_directive, 6, .production_id = 17),
+  [1378] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_nospam_directive, 2, .production_id = 2),
+  [1380] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_source_directive, 2, .production_id = 5),
+  [1382] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unscore_directive, 2),
+  [1384] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unsubjectrx_directive, 2),
+  [1386] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_sidebar_unpin_directive, 2),
+  [1388] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_sidebar_pin_directive, 2),
+  [1390] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unsetenv_directive, 2),
+  [1392] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_finish_directive, 1),
+  [1394] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unsubjectrx_directive, 2, .production_id = 2),
+  [1396] = {.entry = {.count = 1, .reusable = true}}, SHIFT(50),
+  [1398] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_toggle_directive, 2),
+  [1400] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_reset_directive, 2),
+  [1402] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unset_directive, 2),
+  [1404] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_set_directive, 2),
+  [1406] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_set_directive, 2, .production_id = 2),
+  [1408] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_ungroup_directive, 3, .production_id = 7),
+  [1410] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_subscribe_to_directive, 2),
+  [1412] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unhook_directive, 2),
+  [1414] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_hook_type, 1),
+  [1416] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_shutdown_hook_directive, 2, .production_id = 4),
+  [1418] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_startup_hook_directive, 2, .production_id = 4),
+  [1420] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_uri, 1, .production_id = 3),
+  [1422] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_timeout_hook_directive, 2, .production_id = 4),
+  [1424] = {.entry = {.count = 1, .reusable = false}}, REDUCE(sym_unsubscribe_from_directive, 2),
+  [1426] = {.entry = {.count = 1, .reusable = true}}, SHIFT(168),
+  [1428] = {.entry = {.count = 1, .reusable = true}}, SHIFT(118),
+  [1430] = {.entry = {.count = 1, .reusable = true}}, SHIFT(145),
+  [1432] = {.entry = {.count = 1, .reusable = false}}, SHIFT(467),
+  [1434] = {.entry = {.count = 1, .reusable = true}}, SHIFT(19),
+  [1436] = {.entry = {.count = 1, .reusable = true}}, SHIFT(216),
+  [1438] = {.entry = {.count = 1, .reusable = true}}, SHIFT(486),
+  [1440] = {.entry = {.count = 1, .reusable = true}}, SHIFT(515),
+  [1442] = {.entry = {.count = 1, .reusable = true}}, SHIFT(220),
+  [1444] = {.entry = {.count = 1, .reusable = true}}, SHIFT(24),
+  [1446] = {.entry = {.count = 1, .reusable = true}}, SHIFT(379),
+  [1448] = {.entry = {.count = 1, .reusable = true}}, SHIFT(339),
+  [1450] = {.entry = {.count = 1, .reusable = true}}, SHIFT(21),
+  [1452] = {.entry = {.count = 1, .reusable = true}}, SHIFT(17),
+  [1454] = {.entry = {.count = 1, .reusable = true}}, SHIFT(259),
+  [1456] = {.entry = {.count = 1, .reusable = true}}, SHIFT(93),
+  [1458] = {.entry = {.count = 1, .reusable = true}}, SHIFT(306),
+  [1460] = {.entry = {.count = 1, .reusable = true}}, SHIFT(307),
+  [1462] = {.entry = {.count = 1, .reusable = true}}, SHIFT(274),
+  [1464] = {.entry = {.count = 1, .reusable = true}}, SHIFT(359),
+  [1466] = {.entry = {.count = 1, .reusable = true}}, SHIFT(253),
+  [1468] = {.entry = {.count = 1, .reusable = true}}, REDUCE(sym_disposition, 1, .production_id = 3),
+  [1470] = {.entry = {.count = 1, .reusable = true}}, SHIFT(428),
+  [1472] = {.entry = {.count = 1, .reusable = true}}, SHIFT(281),
+  [1474] = {.entry = {.count = 1, .reusable = true}},  ACCEPT_INPUT(),
+  [1476] = {.entry = {.count = 1, .reusable = true}}, SHIFT(338),
+  [1478] = {.entry = {.count = 1, .reusable = true}}, SHIFT(468),
+  [1480] = {.entry = {.count = 1, .reusable = true}}, SHIFT(252),
+  [1482] = {.entry = {.count = 1, .reusable = true}}, SHIFT(469),
+  [1484] = {.entry = {.count = 1, .reusable = true}}, SHIFT(470),
+  [1486] = {.entry = {.count = 1, .reusable = true}}, SHIFT(472),
+  [1488] = {.entry = {.count = 1, .reusable = true}}, SHIFT(258),
+  [1490] = {.entry = {.count = 1, .reusable = true}}, SHIFT(473),
+  [1492] = {.entry = {.count = 1, .reusable = true}}, SHIFT(481),
+  [1494] = {.entry = {.count = 1, .reusable = true}}, SHIFT(103),
+  [1496] = {.entry = {.count = 1, .reusable = true}}, SHIFT(280),
+  [1498] = {.entry = {.count = 1, .reusable = true}}, SHIFT(282),
+  [1500] = {.entry = {.count = 1, .reusable = true}}, SHIFT(474),
+  [1502] = {.entry = {.count = 1, .reusable = true}}, SHIFT(292),
+  [1504] = {.entry = {.count = 1, .reusable = true}}, SHIFT(294),
+  [1506] = {.entry = {.count = 1, .reusable = true}}, SHIFT(175),
+  [1508] = {.entry = {.count = 1, .reusable = true}}, SHIFT(25),
+  [1510] = {.entry = {.count = 1, .reusable = true}}, SHIFT(475),
+  [1512] = {.entry = {.count = 1, .reusable = true}}, SHIFT(183),
+  [1514] = {.entry = {.count = 1, .reusable = true}}, SHIFT(380),
+  [1516] = {.entry = {.count = 1, .reusable = true}}, SHIFT(181),
+  [1518] = {.entry = {.count = 1, .reusable = true}}, SHIFT(299),
+  [1520] = {.entry = {.count = 1, .reusable = true}}, SHIFT(303),
+  [1522] = {.entry = {.count = 1, .reusable = true}}, SHIFT(342),
+  [1524] = {.entry = {.count = 1, .reusable = true}}, SHIFT(305),
+  [1526] = {.entry = {.count = 1, .reusable = true}}, SHIFT(494),
+  [1528] = {.entry = {.count = 1, .reusable = true}}, SHIFT(495),
+  [1530] = {.entry = {.count = 1, .reusable = true}}, SHIFT(496),
+  [1532] = {.entry = {.count = 1, .reusable = true}}, SHIFT(497),
+  [1534] = {.entry = {.count = 1, .reusable = true}}, SHIFT(498),
+  [1536] = {.entry = {.count = 1, .reusable = true}}, SHIFT(499),
+  [1538] = {.entry = {.count = 1, .reusable = true}}, SHIFT(500),
+  [1540] = {.entry = {.count = 1, .reusable = true}}, SHIFT(502),
+  [1542] = {.entry = {.count = 1, .reusable = true}}, SHIFT(503),
+  [1544] = {.entry = {.count = 1, .reusable = true}}, SHIFT(504),
+  [1546] = {.entry = {.count = 1, .reusable = true}}, SHIFT(505),
+  [1548] = {.entry = {.count = 1, .reusable = true}}, SHIFT(506),
+  [1550] = {.entry = {.count = 1, .reusable = true}}, SHIFT(464),
+  [1552] = {.entry = {.count = 1, .reusable = true}}, SHIFT(508),
+  [1554] = {.entry = {.count = 1, .reusable = true}}, SHIFT(510),
+  [1556] = {.entry = {.count = 1, .reusable = true}}, SHIFT(511),
+  [1558] = {.entry = {.count = 1, .reusable = true}}, SHIFT(512),
+  [1560] = {.entry = {.count = 1, .reusable = true}}, SHIFT(513),
+  [1562] = {.entry = {.count = 1, .reusable = true}}, SHIFT(514),
+  [1564] = {.entry = {.count = 1, .reusable = true}}, SHIFT(465),
+  [1566] = {.entry = {.count = 1, .reusable = true}}, SHIFT(516),
+  [1568] = {.entry = {.count = 1, .reusable = true}}, SHIFT(517),
+  [1570] = {.entry = {.count = 1, .reusable = true}}, SHIFT(518),
+  [1572] = {.entry = {.count = 1, .reusable = true}}, SHIFT(519),
+  [1574] = {.entry = {.count = 1, .reusable = true}}, SHIFT(520),
+  [1576] = {.entry = {.count = 1, .reusable = true}}, SHIFT(521),
+  [1578] = {.entry = {.count = 1, .reusable = true}}, SHIFT(522),
+  [1580] = {.entry = {.count = 1, .reusable = true}}, SHIFT(523),
+  [1582] = {.entry = {.count = 1, .reusable = true}}, SHIFT(524),
+  [1584] = {.entry = {.count = 1, .reusable = true}}, SHIFT(525),
+  [1586] = {.entry = {.count = 1, .reusable = true}}, SHIFT(526),
+  [1588] = {.entry = {.count = 1, .reusable = true}}, SHIFT(527),
+  [1590] = {.entry = {.count = 1, .reusable = true}}, SHIFT(528),
+  [1592] = {.entry = {.count = 1, .reusable = true}}, SHIFT(529),
+  [1594] = {.entry = {.count = 1, .reusable = true}}, SHIFT(530),
 };
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 #ifdef TREE_SITTER_HIDE_SYMBOLS
 #define TS_PUBLIC
```

