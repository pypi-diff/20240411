# Comparing `tmp/tree_sitter_earthfile-0.2.1-cp38-abi3-win_amd64.whl.zip` & `tmp/tree_sitter_earthfile-0.2.2-cp38-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 105721 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 15:22 tree_sitter_earthfile/__init__.py
--rw-rw-rw-  2.0 fat       27 b- defN 24-Apr-02 15:22 tree_sitter_earthfile/__init__.pyi
--rw-rw-rw-  2.0 fat   526848 b- defN 24-Apr-02 15:25 tree_sitter_earthfile/_binding.pyd
--rw-rw-rw-  2.0 fat      642 b- defN 24-Apr-02 15:22 tree_sitter_earthfile/binding.c
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-02 15:22 tree_sitter_earthfile/py.typed
--rw-rw-rw-  2.0 fat     2096 b- defN 24-Apr-02 15:22 tree_sitter_earthfile/queries/highlights.scm
--rw-rw-rw-  2.0 fat      271 b- defN 24-Apr-02 15:22 tree_sitter_earthfile/queries/injections.scm
--rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-02 15:25 tree_sitter_earthfile-0.2.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      987 b- defN 24-Apr-02 15:25 tree_sitter_earthfile-0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-02 15:25 tree_sitter_earthfile-0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       31 b- defN 24-Apr-02 15:24 tree_sitter_earthfile-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1098 b- defN 24-Apr-02 15:25 tree_sitter_earthfile-0.2.1.dist-info/RECORD
-12 files, 533264 bytes uncompressed, 103829 bytes compressed:  80.5%
+Zip file size: 105603 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-11 06:11 tree_sitter_earthfile/__init__.py
+-rw-rw-rw-  2.0 fat       27 b- defN 24-Apr-11 06:11 tree_sitter_earthfile/__init__.pyi
+-rw-rw-rw-  2.0 fat   526848 b- defN 24-Apr-11 06:13 tree_sitter_earthfile/_binding.pyd
+-rw-rw-rw-  2.0 fat      642 b- defN 24-Apr-11 06:11 tree_sitter_earthfile/binding.c
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 06:11 tree_sitter_earthfile/py.typed
+-rw-rw-rw-  2.0 fat     1397 b- defN 24-Apr-11 06:11 tree_sitter_earthfile/queries/highlights.scm
+-rw-rw-rw-  2.0 fat      271 b- defN 24-Apr-11 06:11 tree_sitter_earthfile/queries/injections.scm
+-rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-11 06:13 tree_sitter_earthfile-0.2.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      987 b- defN 24-Apr-11 06:13 tree_sitter_earthfile-0.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-11 06:13 tree_sitter_earthfile-0.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       31 b- defN 24-Apr-11 06:13 tree_sitter_earthfile-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1098 b- defN 24-Apr-11 06:13 tree_sitter_earthfile-0.2.2.dist-info/RECORD
+12 files, 532565 bytes uncompressed, 103711 bytes compressed:  80.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tree_sitter_earthfile/queries/highlights.scm
 Comment: 
 
 Filename: tree_sitter_earthfile/queries/injections.scm
 Comment: 
 
-Filename: tree_sitter_earthfile-0.2.1.dist-info/LICENSE
+Filename: tree_sitter_earthfile-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: tree_sitter_earthfile-0.2.1.dist-info/METADATA
+Filename: tree_sitter_earthfile-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: tree_sitter_earthfile-0.2.1.dist-info/WHEEL
+Filename: tree_sitter_earthfile-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: tree_sitter_earthfile-0.2.1.dist-info/top_level.txt
+Filename: tree_sitter_earthfile-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tree_sitter_earthfile-0.2.1.dist-info/RECORD
+Filename: tree_sitter_earthfile-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tree_sitter_earthfile/queries/highlights.scm

```diff
@@ -1,46 +1,52 @@
 (string_array "," @punctuation.delimiter)
 (string_array ["[" "]"] @punctuation.bracket)
 
-(arg_command "ARG" @keyword)
-(build_command "BUILD" @keyword)
-(cache_command "CACHE" @keyword)
-(cmd_command "CMD" @keyword)
-(copy_command "COPY" @keyword)
-(do_command "DO" @keyword)
-(entrypoint_command "ENTRYPOINT" @keyword)
-(env_command "ENV" @keyword)
-(expose_command "EXPOSE" @keyword)
-(from_command "FROM" @keyword)
-(from_dockerfile_command "FROM DOCKERFILE" @keyword)
-(function_command "FUNCTION" @keyword)
-(git_clone_command "GIT CLONE" @keyword)
-(host_command "HOST" @keyword)
-(import_command "IMPORT" @keyword)
-(label_command "LABEL" @keyword)
-(let_command "LET" @keyword)
-(project_command "PROJECT" @keyword)
-(run_command "RUN" @keyword)
-(save_artifact_command ["SAVE ARTIFACT" "AS LOCAL"] @keyword)
-(save_image_command "SAVE IMAGE" @keyword)
-(set_command "SET" @keyword)
-(user_command "USER" @keyword)
-(version_command "VERSION" @keyword)
-(volume_command "VOLUME" @keyword)
-(with_docker_command "WITH DOCKER" @keyword)
-(workdir_command "WORKDIR" @keyword)
+[
+    "ARG"
+    "AS LOCAL"
+    "BUILD"
+    "CACHE"
+    "CMD"
+    "COPY"
+    "DO"
+    "ENTRYPOINT"
+    "ENV"
+    "EXPOSE"
+    "FROM DOCKERFILE"
+    "FROM"
+    "FUNCTION"
+    "GIT CLONE"
+    "HOST"
+    "IMPORT"
+    "LABEL"
+    "LET"
+    "PROJECT"
+    "RUN"
+    "SAVE ARTIFACT"
+    "SAVE IMAGE"
+    "SET"
+    "USER"
+    "VERSION"
+    "VOLUME"
+    "WORKDIR"
+] @keyword
 
 (for_command ["FOR" "IN" "END"] @keyword.control.repeat)
+
 (if_command ["IF" "END"] @keyword.control.conditional)
 (elif_block ["ELSE IF"] @keyword.control.conditional)
 (else_block ["ELSE"] @keyword.control.conditional)
+
 (import_command ["IMPORT" "AS"] @keyword.control.import)
+
 (try_command ["TRY" "FINALLY" "END"] @keyword.control.exception)
-(wait_command ["WAIT" "END"] @keyword.control)
 
+(wait_command ["WAIT" "END"] @keyword.control)
+(with_docker_command ["WITH DOCKER" "END"] @keyword.control)
 
 [
     (comment)
     (line_continuation_comment)
 ] @comment
 
 (line_continuation) @operator
@@ -54,21 +60,15 @@
 (target (identifier) @function)
 
 [
     (double_quoted_string)
     (single_quoted_string)
 ] @string
 (unquoted_string) @string.special
-(escape_sequence) @string.escape
+(escape_sequence) @constant.character.escape
 
 (variable) @variable
 (expansion ["$" "{" "}" "(" ")"] @punctuation.special)
 (build_arg) @variable
 (options (_) @variable.parameter)
 
-(options (_ "=" @operator))
-(build_arg "=" @operator)
-(arg_command "=" @operator)
-(env_command "=" @operator)
-(label "=" @operator)
-(set_command "=" @operator)
-(let_command "=" @operator)
+"=" @operator
```

## Comparing `tree_sitter_earthfile-0.2.1.dist-info/LICENSE` & `tree_sitter_earthfile-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tree_sitter_earthfile-0.2.1.dist-info/METADATA` & `tree_sitter_earthfile-0.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-earthfile
-Version: 0.2.1
+Version: 0.2.2
 Summary: Earthfile grammar for tree-sitter
 License: MIT
 Project-URL: Homepage, https://github.com/tree-sitter/tree-sitter-earthfile
 Keywords: incremental,parsing,tree-sitter,earthfile
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
```

## Comparing `tree_sitter_earthfile-0.2.1.dist-info/RECORD` & `tree_sitter_earthfile-0.2.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 tree_sitter_earthfile/__init__.py,sha256=b49F9QXcBSzekYK6czZvmdtuGwDStmfTwwwbFGkS8H4,92
 tree_sitter_earthfile/__init__.pyi,sha256=8xf7bY1szgDY9HRJ7FJ326So4SFgMiSRfCB4LADkTpU,27
-tree_sitter_earthfile/_binding.pyd,sha256=Cty-_mxYVVQydCTT0pyIjOuLDNRcOJT3hMMGOVk-H7I,526848
+tree_sitter_earthfile/_binding.pyd,sha256=YUa3wuH4d2HyATCeT1z2khfi3u80ldoxoQEuW7oxPU4,526848
 tree_sitter_earthfile/binding.c,sha256=MKxNXwWUTomdXfVWUkzuE2I7Giioe_EcSNnz2Iw-P9Q,642
 tree_sitter_earthfile/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tree_sitter_earthfile/queries/highlights.scm,sha256=FTLCyqk0TDZrGlcgEK0PpNSBr5xU7XBC_8fRetGuv0M,2096
+tree_sitter_earthfile/queries/highlights.scm,sha256=sHHDVqyppK76MTfeSHoaeKUgkEVjJ84jXchDcRWVREE,1397
 tree_sitter_earthfile/queries/injections.scm,sha256=-GVsiRO-9Cz_5wl71HXOXI7zbMv49V8I1sxJXrizujE,271
-tree_sitter_earthfile-0.2.1.dist-info/LICENSE,sha256=_VBuaug4WgiXJ36qNSlMQzxZZmW40iKiVm5SHHBDL3c,1072
-tree_sitter_earthfile-0.2.1.dist-info/METADATA,sha256=PBNkOp6EHHsQZPtqLdefFlkdx4HfLc89S--Owb6BsP0,987
-tree_sitter_earthfile-0.2.1.dist-info/WHEEL,sha256=UyMHzmWA0xVqVPKfTiLs2eN3OWWZUl-kQemNbpIqlKo,100
-tree_sitter_earthfile-0.2.1.dist-info/top_level.txt,sha256=Ddv97tXjIVquwTZTacOwi0oCQaBjxY52xeUX6Riy1vQ,31
-tree_sitter_earthfile-0.2.1.dist-info/RECORD,,
+tree_sitter_earthfile-0.2.2.dist-info/LICENSE,sha256=_VBuaug4WgiXJ36qNSlMQzxZZmW40iKiVm5SHHBDL3c,1072
+tree_sitter_earthfile-0.2.2.dist-info/METADATA,sha256=qVk_SXBXlo3q3Q-GKBp8W-aiGM9ZsJiPEPj5yMvuZws,987
+tree_sitter_earthfile-0.2.2.dist-info/WHEEL,sha256=UyMHzmWA0xVqVPKfTiLs2eN3OWWZUl-kQemNbpIqlKo,100
+tree_sitter_earthfile-0.2.2.dist-info/top_level.txt,sha256=Ddv97tXjIVquwTZTacOwi0oCQaBjxY52xeUX6Riy1vQ,31
+tree_sitter_earthfile-0.2.2.dist-info/RECORD,,
```

