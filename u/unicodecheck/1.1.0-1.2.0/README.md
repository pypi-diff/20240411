# Comparing `tmp/unicodecheck-1.1.0.tar.gz` & `tmp/unicodecheck-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodecheck-1.1.0.tar", last modified: Tue Apr  9 06:48:16 2024, max compression
+gzip compressed data, was "unicodecheck-1.2.0.tar", last modified: Thu Apr 11 15:48:38 2024, max compression
```

## Comparing `unicodecheck-1.1.0.tar` & `unicodecheck-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-09 06:48:16.607034 unicodecheck-1.1.0/
--rw-r--r--   0 shunsuke   (501) staff       (20)     1064 2023-10-24 08:35:07.000000 unicodecheck-1.1.0/LICENSE
--rw-r--r--   0 shunsuke   (501) staff       (20)     2907 2024-04-09 06:48:16.606834 unicodecheck-1.1.0/PKG-INFO
--rw-r--r--   0 shunsuke   (501) staff       (20)     1969 2024-04-09 06:46:52.000000 unicodecheck-1.1.0/README.md
--rw-r--r--   0 shunsuke   (501) staff       (20)     1043 2024-03-20 16:01:49.000000 unicodecheck-1.1.0/pyproject.toml
--rw-r--r--   0 shunsuke   (501) staff       (20)       38 2024-04-09 06:48:16.607083 unicodecheck-1.1.0/setup.cfg
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-09 06:48:16.605335 unicodecheck-1.1.0/unicodecheck/
--rw-r--r--   0 shunsuke   (501) staff       (20)       22 2024-04-09 06:46:52.000000 unicodecheck-1.1.0/unicodecheck/__init__.py
--rw-r--r--   0 shunsuke   (501) staff       (20)       82 2023-11-11 17:10:51.000000 unicodecheck-1.1.0/unicodecheck/__main__.py
--rw-r--r--   0 shunsuke   (501) staff       (20)      704 2024-04-01 09:57:53.000000 unicodecheck-1.1.0/unicodecheck/args.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     8637 2024-04-09 06:46:52.000000 unicodecheck-1.1.0/unicodecheck/cli.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     2388 2024-03-11 14:57:18.000000 unicodecheck-1.1.0/unicodecheck/core.py
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-09 06:48:16.606393 unicodecheck-1.1.0/unicodecheck.egg-info/
--rw-r--r--   0 shunsuke   (501) staff       (20)     2907 2024-04-09 06:48:16.000000 unicodecheck-1.1.0/unicodecheck.egg-info/PKG-INFO
--rw-r--r--   0 shunsuke   (501) staff       (20)      362 2024-04-09 06:48:16.000000 unicodecheck-1.1.0/unicodecheck.egg-info/SOURCES.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)        1 2024-04-09 06:48:16.000000 unicodecheck-1.1.0/unicodecheck.egg-info/dependency_links.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       55 2024-04-09 06:48:16.000000 unicodecheck-1.1.0/unicodecheck.egg-info/entry_points.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       58 2024-04-09 06:48:16.000000 unicodecheck-1.1.0/unicodecheck.egg-info/requires.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       13 2024-04-09 06:48:16.000000 unicodecheck-1.1.0/unicodecheck.egg-info/top_level.txt
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-11 15:48:38.455134 unicodecheck-1.2.0/
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1064 2023-10-24 08:35:07.000000 unicodecheck-1.2.0/LICENSE
+-rw-r--r--   0 shunsuke   (501) staff       (20)     3004 2024-04-11 15:48:38.454905 unicodecheck-1.2.0/PKG-INFO
+-rw-r--r--   0 shunsuke   (501) staff       (20)     2066 2024-04-09 06:48:33.000000 unicodecheck-1.2.0/README.md
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1043 2024-03-20 16:01:49.000000 unicodecheck-1.2.0/pyproject.toml
+-rw-r--r--   0 shunsuke   (501) staff       (20)       38 2024-04-11 15:48:38.455183 unicodecheck-1.2.0/setup.cfg
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-11 15:48:38.453384 unicodecheck-1.2.0/unicodecheck/
+-rw-r--r--   0 shunsuke   (501) staff       (20)       22 2024-04-09 06:48:33.000000 unicodecheck-1.2.0/unicodecheck/__init__.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)       82 2023-11-11 17:10:51.000000 unicodecheck-1.2.0/unicodecheck/__main__.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)      704 2024-04-01 09:57:53.000000 unicodecheck-1.2.0/unicodecheck/args.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     9228 2024-04-09 06:48:33.000000 unicodecheck-1.2.0/unicodecheck/cli.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     2388 2024-03-11 14:57:18.000000 unicodecheck-1.2.0/unicodecheck/core.py
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-11 15:48:38.454407 unicodecheck-1.2.0/unicodecheck.egg-info/
+-rw-r--r--   0 shunsuke   (501) staff       (20)     3004 2024-04-11 15:48:38.000000 unicodecheck-1.2.0/unicodecheck.egg-info/PKG-INFO
+-rw-r--r--   0 shunsuke   (501) staff       (20)      362 2024-04-11 15:48:38.000000 unicodecheck-1.2.0/unicodecheck.egg-info/SOURCES.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)        1 2024-04-11 15:48:38.000000 unicodecheck-1.2.0/unicodecheck.egg-info/dependency_links.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       55 2024-04-11 15:48:38.000000 unicodecheck-1.2.0/unicodecheck.egg-info/entry_points.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       58 2024-04-11 15:48:38.000000 unicodecheck-1.2.0/unicodecheck.egg-info/requires.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       13 2024-04-11 15:48:38.000000 unicodecheck-1.2.0/unicodecheck.egg-info/top_level.txt
```

### Comparing `unicodecheck-1.1.0/LICENSE` & `unicodecheck-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.1.0/PKG-INFO` & `unicodecheck-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodecheck
-Version: 1.1.0
+Version: 1.2.0
 Summary: Check if Unicode text files are Unicode-normalized
 Maintainer-email: curegit <contact@curegit.jp>
 License: MIT
 Project-URL: homepage, https://github.com/curegit/unicodecheck
 Project-URL: repository, https://github.com/curegit/unicodecheck.git
 Keywords: Unicode,character encoding
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -67,15 +67,16 @@
                         target Unicode normalization (default: NFC)
   -d, --diff            show diffs between the original and normalized (default: False)
   -u [NUMBER], -U [NUMBER], --unified [NUMBER]
                         show unified diffs with NUMBER lines of context [NUMBER=3] (default: False)
   -r, --recursive       follow the directory tree rooted in each PATH argument (default: False)
   -i, --include-hidden  include hidden files and directories (default: False)
   -b PATTERN [PATTERN ...], --blacklist PATTERN [PATTERN ...]
-                        notify if having PATTERN (default: None)
+                        notify if having PATTERN (case-sensitive) (default: None)
+  -e, --error           return non-zero exit code on detection (default: False)
   -v, --verbose         report non-essential logs (default: False)
 ```
 
 ## Tips
 
 ### Check whether filenames are normalized
```

### Comparing `unicodecheck-1.1.0/README.md` & `unicodecheck-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -40,15 +40,16 @@
                         target Unicode normalization (default: NFC)
   -d, --diff            show diffs between the original and normalized (default: False)
   -u [NUMBER], -U [NUMBER], --unified [NUMBER]
                         show unified diffs with NUMBER lines of context [NUMBER=3] (default: False)
   -r, --recursive       follow the directory tree rooted in each PATH argument (default: False)
   -i, --include-hidden  include hidden files and directories (default: False)
   -b PATTERN [PATTERN ...], --blacklist PATTERN [PATTERN ...]
-                        notify if having PATTERN (default: None)
+                        notify if having PATTERN (case-sensitive) (default: None)
+  -e, --error           return non-zero exit code on detection (default: False)
   -v, --verbose         report non-essential logs (default: False)
 ```
 
 ## Tips
 
 ### Check whether filenames are normalized
```

### Comparing `unicodecheck-1.1.0/pyproject.toml` & `unicodecheck-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.1.0/unicodecheck/args.py` & `unicodecheck-1.2.0/unicodecheck/args.py`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.1.0/unicodecheck/cli.py` & `unicodecheck-1.2.0/unicodecheck/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 from rich.console import Console
 from rich.text import Text
 from .args import nonempty, uint, src, upper
 from .core import is_binary, detect_unicode_enc, is_norm, normalize, diff
 
 
 def main() -> int:
-    exit_code = 0
+    ok_code = 0
+    error_code = 1
+    issue_code = 3
+
+    exit_code = ok_code
 
     console = Console()
     error_console = Console(stderr=True)
 
     class SigPipeExit(BaseException):
         exit_code = 128 + 13
 
@@ -75,24 +79,27 @@
         parser.add_argument("paths", metavar="PATH", type=src, nargs="+", help="describe input file or directory (pass '-' to specify stdin)")
         parser.add_argument("-V", "--version", action="version", version=version)
         parser.add_argument("-m", "--mode", type=upper, choices=["NFC", "NFD", "NFKC", "NFKD"], default="NFC", help="target Unicode normalization")
         parser.add_argument("-d", "--diff", action="store_true", help="show diffs between the original and normalized")
         parser.add_argument("-u", "-U", "--unified", metavar="NUMBER", default=False, type=uint, nargs="?", const=3, help="show unified diffs with NUMBER lines of context [NUMBER=3]")
         parser.add_argument("-r", "--recursive", action="store_true", help="follow the directory tree rooted in each PATH argument")
         parser.add_argument("-i", "--include-hidden", action="store_true", help="include hidden files and directories")
-        parser.add_argument("-b", "--blacklist", metavar="PATTERN", type=nonempty, nargs="+", action="extend", help="notify if having PATTERN")
+        parser.add_argument("-b", "--blacklist", metavar="PATTERN", type=nonempty, nargs="+", action="extend", help="notify if having PATTERN (case-sensitive)")
+        parser.add_argument("-e", "--error", action="store_true", help="return non-zero exit code on detection")
         parser.add_argument("-v", "--verbose", action="store_true", help="report non-essential logs")
         args = parser.parse_args()
 
         mode: str = args.mode
         show_diff: bool = args.diff or args.unified is not False
         unified_diff: bool = args.unified is not False
         context_lines: int = 0 if args.unified is None else args.unified
         recursive: bool = args.recursive
         include_hidden: bool = args.include_hidden
+        blacklist: list[str] = [] if args.blacklist is None else list(args.blacklist)
+        error: bool = args.error
         verbose: bool = args.verbose
         paths: list[str | None] = list(args.paths)
 
         # stdin の出現を 1 回にする
         if None in paths:
             paths = [p for p in paths if p is not None]
             paths.append(None)
@@ -116,19 +123,19 @@
                         else:
                             pattern = os.path.join(glob.escape(str(path)), "*")
                         globs = (Path(e) for e in glob.iglob(pattern, recursive=recursive, include_hidden=include_hidden))
                         files = (f for f in globs if f.is_file())
                     # 存在しないパスの場合
                     else:
                         print_error(f"{path}: No such file or directory")
-                        exit_code = 1
+                        exit_code = error_code
                         break
                 except Exception:
                     print_error(f"{p}: Unprocessable path")
-                    exit_code = 1
+                    exit_code = error_code
                     break
             # ファイルごとに処理
             for f in files:
                 file = None
                 try:
                     stream: bytes | BufferedIOBase
                     if f is None:
@@ -148,37 +155,42 @@
                     if isbin:
                         if verbose:
                             print_verbose(f"{fpath}: Skip binary file")
                         continue
                     # ユニコードの符号方式を調べる
                     encoding = detect_unicode_enc(stream)
                     if encoding is None:
-                        if args.verbose:
+                        if verbose:
                             print_verbose(f"{fpath}: Skip non-Unicode file")
                         continue
                     # デコードをテスト
                     try:
                         if isinstance(stream, bytes):
                             text = stream.decode(encoding)
                         else:
                             text = stream.read().decode(encoding)
                     except Exception:
+                        if error and exit_code == ok_code:
+                            exit_code = issue_code
                         print_issue(f"{fpath}: Invalid Unicode (or misunderstanding encoding)")
                         continue
                     # ブラックリスト照合
-                    if args.blacklist is not None:
-                        for pat in args.blacklist:
-                            if text.find(pat) >= 0:
-                                print_issue(f"{fpath}: Having pattern: {pat}")
+                    for pat in blacklist:
+                        if text.find(pat) >= 0:
+                            if error and exit_code == ok_code:
+                                exit_code = issue_code
+                            print_issue(f"{fpath}: Having pattern: {pat}")
                     # 正規形かテスト
                     if is_norm(text, mode):
                         if verbose:
                             print_verbose(f"{fpath}: OK ({mode})")
                         continue
                     # 正規形でない場合
+                    if error and exit_code == ok_code:
+                        exit_code = issue_code
                     print_issue(f"{fpath}: Not normalized in {mode}")
                     if show_diff:
                         normalized = normalize(text, mode)
                         for line in diff(text, normalized, filename=fname, unified=unified_diff, n=context_lines):
                             write(line)
                         print()
                 # 想定しないエラーを強調表示して続行（パーミッションエラーなど）
@@ -188,15 +200,15 @@
                 finally:
                     if file is not None:
                         file.close()
         return exit_code
 
     # SIGPIPE での終了を通知
     except SigPipeExit as e:
-        exit_code = exit_code if exit_code != 0 else e.exit_code
+        exit_code = exit_code if exit_code != ok_code else e.exit_code
         print_cancel("SIGPIPE")
         return exit_code
 
     # SIGINT での終了を短く表示
     except KeyboardInterrupt:
         exit_code = 130
         print_cancel("KeyboardInterrupt")
```

### Comparing `unicodecheck-1.1.0/unicodecheck/core.py` & `unicodecheck-1.2.0/unicodecheck/core.py`

 * *Files identical despite different names*

### Comparing `unicodecheck-1.1.0/unicodecheck.egg-info/PKG-INFO` & `unicodecheck-1.2.0/unicodecheck.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodecheck
-Version: 1.1.0
+Version: 1.2.0
 Summary: Check if Unicode text files are Unicode-normalized
 Maintainer-email: curegit <contact@curegit.jp>
 License: MIT
 Project-URL: homepage, https://github.com/curegit/unicodecheck
 Project-URL: repository, https://github.com/curegit/unicodecheck.git
 Keywords: Unicode,character encoding
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -67,15 +67,16 @@
                         target Unicode normalization (default: NFC)
   -d, --diff            show diffs between the original and normalized (default: False)
   -u [NUMBER], -U [NUMBER], --unified [NUMBER]
                         show unified diffs with NUMBER lines of context [NUMBER=3] (default: False)
   -r, --recursive       follow the directory tree rooted in each PATH argument (default: False)
   -i, --include-hidden  include hidden files and directories (default: False)
   -b PATTERN [PATTERN ...], --blacklist PATTERN [PATTERN ...]
-                        notify if having PATTERN (default: None)
+                        notify if having PATTERN (case-sensitive) (default: None)
+  -e, --error           return non-zero exit code on detection (default: False)
   -v, --verbose         report non-essential logs (default: False)
 ```
 
 ## Tips
 
 ### Check whether filenames are normalized
```

