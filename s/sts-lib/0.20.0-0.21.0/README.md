# Comparing `tmp/sts-lib-0.20.0.tar.gz` & `tmp/sts-lib-0.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts-lib-0.20.0.tar", last modified: Mon Apr  8 14:18:41 2024, max compression
+gzip compressed data, was "sts-lib-0.21.0.tar", last modified: Thu Apr 11 14:38:24 2024, max compression
```

## Comparing `sts-lib-0.20.0.tar` & `sts-lib-0.21.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 14:18:41.877618 sts-lib-0.20.0/
--rw-rw-rw-   0        0        0    11358 2020-07-10 16:04:12.000000 sts-lib-0.20.0/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-08 13:49:48.000000 sts-lib-0.20.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5160 2024-04-08 14:18:41.877618 sts-lib-0.20.0/PKG-INFO
--rw-rw-rw-   0        0        0     3818 2020-07-12 06:28:09.000000 sts-lib-0.20.0/README.md
--rw-rw-rw-   0        0        0     1673 2024-04-08 14:18:41.877618 sts-lib-0.20.0/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-08 13:49:48.000000 sts-lib-0.20.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:18:41.837582 sts-lib-0.20.0/sts/
--rw-rw-rw-   0        0        0    36670 2024-04-08 14:09:27.000000 sts-lib-0.20.0/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-08 13:49:45.000000 sts-lib-0.20.0/sts/__main__.py
--rw-rw-rw-   0        0        0     7463 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:18:41.827304 sts-lib-0.20.0/sts/data/
-drwxrwxrwx   0        0        0        0 2024-04-08 14:18:41.847343 sts-lib-0.20.0/sts/data/config/
--rw-rw-rw-   0        0        0      653 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      369 2020-08-12 18:29:24.000000 sts-lib-0.20.0/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      275 2020-07-12 06:22:39.000000 sts-lib-0.20.0/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      323 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      289 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      201 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      287 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      369 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      197 2020-07-12 06:22:39.000000 sts-lib-0.20.0/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      211 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      201 2020-07-16 15:29:01.000000 sts-lib-0.20.0/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      195 2020-07-12 06:22:39.000000 sts-lib-0.20.0/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      367 2020-07-12 06:22:39.000000 sts-lib-0.20.0/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      413 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      273 2020-07-12 06:22:39.000000 sts-lib-0.20.0/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-04-08 14:18:41.867627 sts-lib-0.20.0/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2020-07-10 16:04:12.000000 sts-lib-0.20.0/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2020-07-10 16:04:12.000000 sts-lib-0.20.0/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-04-08 13:53:21.000000 sts-lib-0.20.0/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2020-07-10 16:04:12.000000 sts-lib-0.20.0/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2020-07-12 14:58:22.000000 sts-lib-0.20.0/sts/data/dictionary/TWVariantsRevPhrases.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 14:18:41.867627 sts-lib-0.20.0/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-04-08 13:56:57.000000 sts-lib-0.20.0/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2020-07-10 16:04:12.000000 sts-lib-0.20.0/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-04-08 14:18:41.877618 sts-lib-0.20.0/sts_lib.egg-info/
--rw-rw-rw-   0        0        0     5160 2024-04-08 14:18:41.000000 sts-lib-0.20.0/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1298 2024-04-08 14:18:41.000000 sts-lib-0.20.0/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 14:18:41.000000 sts-lib-0.20.0/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-08 14:18:41.000000 sts-lib-0.20.0/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      170 2024-04-08 14:18:41.000000 sts-lib-0.20.0/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-08 14:18:41.000000 sts-lib-0.20.0/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 14:38:24.797400 sts-lib-0.21.0/
+-rw-rw-rw-   0        0        0    11358 2020-07-10 16:04:12.000000 sts-lib-0.21.0/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-08 13:49:48.000000 sts-lib-0.21.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6931 2024-04-11 14:38:24.797400 sts-lib-0.21.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5589 2024-04-11 14:01:20.000000 sts-lib-0.21.0/README.md
+-rw-rw-rw-   0        0        0     1687 2024-04-11 14:38:24.798409 sts-lib-0.21.0/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-08 13:49:48.000000 sts-lib-0.21.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:38:24.754804 sts-lib-0.21.0/sts/
+-rw-rw-rw-   0        0        0    39647 2024-04-11 14:13:54.000000 sts-lib-0.21.0/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-08 13:49:45.000000 sts-lib-0.21.0/sts/__main__.py
+-rw-rw-rw-   0        0        0     7721 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:38:24.757107 sts-lib-0.21.0/sts/data/
+drwxrwxrwx   0        0        0        0 2024-04-11 14:38:24.771104 sts-lib-0.21.0/sts/data/config/
+-rw-rw-rw-   0        0        0      653 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      369 2020-08-12 18:29:24.000000 sts-lib-0.21.0/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      275 2020-07-12 06:22:39.000000 sts-lib-0.21.0/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      323 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      289 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      201 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      287 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      369 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      197 2020-07-12 06:22:39.000000 sts-lib-0.21.0/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      211 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      201 2020-07-16 15:29:01.000000 sts-lib-0.21.0/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      195 2020-07-12 06:22:39.000000 sts-lib-0.21.0/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      367 2020-07-12 06:22:39.000000 sts-lib-0.21.0/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      413 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      273 2020-07-12 06:22:39.000000 sts-lib-0.21.0/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-04-11 14:38:24.785604 sts-lib-0.21.0/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2020-07-10 16:04:12.000000 sts-lib-0.21.0/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2020-07-10 16:04:12.000000 sts-lib-0.21.0/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-04-11 14:14:43.000000 sts-lib-0.21.0/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2020-07-10 16:04:12.000000 sts-lib-0.21.0/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2020-07-12 14:58:22.000000 sts-lib-0.21.0/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    14030 2024-04-11 14:14:24.000000 sts-lib-0.21.0/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-04-11 14:38:24.789408 sts-lib-0.21.0/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-04-11 14:26:09.000000 sts-lib-0.21.0/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2020-07-10 16:04:12.000000 sts-lib-0.21.0/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 14:38:24.795401 sts-lib-0.21.0/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0     6931 2024-04-11 14:38:24.000000 sts-lib-0.21.0/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-04-11 14:38:24.000000 sts-lib-0.21.0/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 14:38:24.000000 sts-lib-0.21.0/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-11 14:38:24.000000 sts-lib-0.21.0/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      170 2024-04-11 14:38:24.000000 sts-lib-0.21.0/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-11 14:38:24.000000 sts-lib-0.21.0/sts_lib.egg-info/top_level.txt
```

### Comparing `sts-lib-0.20.0/LICENSE` & `sts-lib-0.21.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/PKG-INFO` & `sts-lib-0.21.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.20.0
+Version: 0.21.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -53,50 +53,84 @@
 
     pip install -U sts-lib
 
 ### Command Line
 
 * `sts --help` 或 `sts COMMAND --help` 檢視可用指令的詳細說明文檔。
 
-* `sts convert [OPTIONs] [file [file ...]]` 執行簡繁轉換：
+* `sts convert [OPTIONs] [file ...]` 執行簡繁轉換：
   * `file` 為一或多個欲轉換的檔案。（省略則讀取標準輸入 STDIN）
   * `-c CONFIG` 指定配置檔，可為內建配置檔名稱或自製 JSON 配置檔的路徑。可用的內建配置檔詳見 [sts/data/config](https://github.com/danny0838/sts-lib/tree/master/sts/data/config) 目錄，可簡寫，例如輸入 `s2t` 代表使用 `sts/data/config/s2t.json`。
   * `-f FORMAT` 指定輸出格式，可用格式如下：
     * `txt`：純文字，適合一般使用。
     * `txtm`：純文字加轉換標示。
     * `html`：加上 HTML 標記的文本，可嵌入至網頁應用程式做互動式校對。
     * `htmlpage`：加入 HTML 樣式的網頁，可直接開啟做互動式校對。
     * `json`：以 JSON 格式表示轉換輸出，可用其他程式進一步解析處理。
   * `--exclude PATTERN` 指定用於忽略簡繁轉換的正規表示式。有指定 `return` 子群組時會取代為子群組的值。
     * 例如 `sts convert -c s2twp --exclude "「.*?」"` 會把 `「程序」正义` 轉換為 `「程序」正義`。
     * 例如 `sts convert -c s2twp --exclude "-{(?P<return>.*?)}-"` 會把 `-{程序}-正义` 轉換為 `程序正義`。
   * `--in-enc ENCODING` 指定輸入編碼。可用編碼參見[這裡](https://docs.python.org/3/library/codecs.html#standard-encodings)。
   * `--out-enc ENCODING` 指定輸出編碼。可用編碼參見[這裡](https://docs.python.org/3/library/codecs.html#standard-encodings)。
-  * `-o OUTPUT` 指定對應輸入檔案轉換結果的輸出路徑。（無對應者輸出至原處）
+  * `-o OUTPUT` 可重覆多次，指定對應輸入檔案轉換結果的輸出路徑。（無對應者輸出至原檔）
   * `--stdout` 將所有轉換結果輸出至標準輸出 STDOUT。
 
 ### Python
 
 ```python
 from sts import StsMaker, StsConverter
 
 # generate a dictionary file from a config and get its path
 dictfile = StsMaker().make('s2t', quiet=True)
 
-# initialize the converter from the dictionary file
-converter = StsConverter(dictfile, options={})
+# initialize a converter from the dictionary file
+converter = StsConverter(dictfile)
 
-# perform conversion for a text
-converter.convert_text('汉字')  # 漢字
+# perform conversion for a string
+converter.convert_text('汉字', format='txt', exclude=None)  # 漢字
 
 # perform conversion for a file (None for stdin/stdout)
-converter.convert_file(input=None, output=None)
+converter.convert_file(input=None, output=None
+                       input_encoding='UTF-8', output_encoding='UTF-8',
+                       format='txt', exclude=None)
 
-# process conversion data generator
-[p for p in converter.convert("汉字")]  # [StsDictConv(key=['汉'], values=['漢']), '字']
+# perform a conversion for a string and process the result data generator
+[p for p in converter.convert("干了吧")]  # [StsDictConv(key=['干', '了'], values=['幹了', '乾了']), '吧']
+```
+
+## Config 配置檔
+
+```javascript
+/**
+ * @typedef {Object} configScheme
+ * @property {string} [name] - name/description of the config
+ * @property {string[]} [requires] - required configs, which are made before
+ *     making from this config, as an absolute path, or a path relative to the
+ *     directory of this config file, or the basename of a built-in config file
+ *     (with or without ".json")
+ * @property {dictScheme[]} dicts - schemes of each dictionary file to generate
+ */
+
+/**
+ * @typedef {Object} dictScheme
+ * @property {string} file - path of the dictionary file to generate. Each as
+ *     an absolute path, or a path relative to the specified output directory
+ *     (or the directory of this config file). Each should be a .tlist
+ *     (compiled trie), .jlist (compiled table), or .list (plain text table).
+ * @property {string} mode - the mode to handle the loaded source files: "load"
+ *     to simply merge the loaded keys and values; "swap" to reverse the
+ *     dictionary (i.e. use the values as keys and the keys as values); "join"
+ *     to build from a chain of dictionaries (in which case src must be an
+ *     array of subarrays of strings)
+ * @property {boolean} [sort] - true to sort the keys of the output dictionary
+ * @property {Array.<(string|string[])>} src - the source files. Each as an
+ *     absolute path, or a path relative to the directory of this config file,
+ *     or the basename of a built-in dictionary file. Each should be a .txt or
+ *     .list dictionary file.
+ */
 ```
 
 ## License 許可協議
 
 本專案以 Apache License 2.0 協議授權使用。
 
 詞典檔原始資料來自同文堂、維基百科、OpenCC 等開源專案，再按本專案之需求編校。
```

### Comparing `sts-lib-0.20.0/setup.cfg` & `sts-lib-0.21.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -66,40 +66,41 @@
 00000410: 0a09 6973 6f72 7420 3e3d 2035 2e35 0d0a  ..isort >= 5.5..
 00000420: 0974 6f78 203e 3d20 342e 300d 0a0d 0a5b  .tox >= 4.0....[
 00000430: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
 00000440: 2e66 696e 645d 0d0a 6578 636c 7564 6520  .find]..exclude 
 00000450: 3d20 7465 7374 730d 0a0d 0a5b 6f70 7469  = tests....[opti
 00000460: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
 00000470: 5d0d 0a73 7473 203d 200d 0a09 6461 7461  ]..sts = ...data
-00000480: 2f63 6f6e 6669 672f 2a2e 6a73 6f6e 0d0a  /config/*.json..
-00000490: 0964 6174 612f 6469 6374 696f 6e61 7279  .data/dictionary
-000004a0: 2f2a 2e74 7874 0d0a 0964 6174 612f 7363  /*.txt...data/sc
-000004b0: 6865 6d65 2f2a 2e74 7874 0d0a 0d0a 5b6f  heme/*.txt....[o
-000004c0: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
-000004d0: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
-000004e0: 7269 7074 7320 3d20 0d0a 0973 7473 203d  ripts = ...sts =
-000004f0: 2073 7473 2e63 6c69 3a6d 6169 6e0d 0a0d   sts.cli:main...
-00000500: 0a5b 666c 616b 6538 5d0d 0a65 7863 6c75  .[flake8]..exclu
-00000510: 6465 203d 2062 7569 6c64 2c20 2e67 6974  de = build, .git
-00000520: 0d0a 6d61 782d 6c69 6e65 2d6c 656e 6774  ..max-line-lengt
-00000530: 6820 3d20 3136 300d 0a65 7874 656e 642d  h = 160..extend-
-00000540: 7365 6c65 6374 203d 200d 0a09 4531 3233  select = ...E123
-00000550: 0d0a 6967 6e6f 7265 203d 200d 0a09 5735  ..ignore = ...W5
-00000560: 3033 0d0a 6967 6e6f 7265 2d6e 616d 6573  03..ignore-names
-00000570: 203d 200d 0a09 7365 7455 700d 0a09 7465   = ...setUp...te
-00000580: 6172 446f 776e 0d0a 0973 6574 5570 436c  arDown...setUpCl
-00000590: 6173 730d 0a09 7465 6172 446f 776e 436c  ass...tearDownCl
-000005a0: 6173 730d 0a09 7365 7455 704d 6f64 756c  ass...setUpModul
-000005b0: 650d 0a09 7465 6172 446f 776e 4d6f 6475  e...tearDownModu
-000005c0: 6c65 0d0a 0961 7379 6e63 5365 7455 700d  le...asyncSetUp.
-000005d0: 0a09 6173 796e 6354 6561 7244 6f77 6e0d  ..asyncTearDown.
-000005e0: 0a09 7365 7455 7054 6573 7444 6174 610d  ..setUpTestData.
-000005f0: 0a09 6661 696c 7572 6545 7863 6570 7469  ..failureExcepti
-00000600: 6f6e 0d0a 096c 6f6e 674d 6573 7361 6765  on...longMessage
-00000610: 0d0a 096d 6178 4469 6666 0d0a 0d0a 5b69  ...maxDiff....[i
-00000620: 736f 7274 5d0d 0a6d 756c 7469 5f6c 696e  sort]..multi_lin
-00000630: 655f 6f75 7470 7574 203d 2033 0d0a 696e  e_output = 3..in
-00000640: 636c 7564 655f 7472 6169 6c69 6e67 5f63  clude_trailing_c
-00000650: 6f6d 6d61 203d 2074 7275 650d 0a0d 0a5b  omma = true....[
-00000660: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000670: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000680: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000480: 2f2a 2e68 746d 6c0d 0a09 6461 7461 2f63  /*.html...data/c
+00000490: 6f6e 6669 672f 2a2e 6a73 6f6e 0d0a 0964  onfig/*.json...d
+000004a0: 6174 612f 6469 6374 696f 6e61 7279 2f2a  ata/dictionary/*
+000004b0: 2e74 7874 0d0a 0964 6174 612f 7363 6865  .txt...data/sche
+000004c0: 6d65 2f2a 2e74 7874 0d0a 0d0a 5b6f 7074  me/*.txt....[opt
+000004d0: 696f 6e73 2e65 6e74 7279 5f70 6f69 6e74  ions.entry_point
+000004e0: 735d 0d0a 636f 6e73 6f6c 655f 7363 7269  s]..console_scri
+000004f0: 7074 7320 3d20 0d0a 0973 7473 203d 2073  pts = ...sts = s
+00000500: 7473 2e63 6c69 3a6d 6169 6e0d 0a0d 0a5b  ts.cli:main....[
+00000510: 666c 616b 6538 5d0d 0a65 7863 6c75 6465  flake8]..exclude
+00000520: 203d 2062 7569 6c64 2c20 2e67 6974 0d0a   = build, .git..
+00000530: 6d61 782d 6c69 6e65 2d6c 656e 6774 6820  max-line-length 
+00000540: 3d20 3136 300d 0a65 7874 656e 642d 7365  = 160..extend-se
+00000550: 6c65 6374 203d 200d 0a09 4531 3233 0d0a  lect = ...E123..
+00000560: 6967 6e6f 7265 203d 200d 0a09 5735 3033  ignore = ...W503
+00000570: 0d0a 6967 6e6f 7265 2d6e 616d 6573 203d  ..ignore-names =
+00000580: 200d 0a09 7365 7455 700d 0a09 7465 6172   ...setUp...tear
+00000590: 446f 776e 0d0a 0973 6574 5570 436c 6173  Down...setUpClas
+000005a0: 730d 0a09 7465 6172 446f 776e 436c 6173  s...tearDownClas
+000005b0: 730d 0a09 7365 7455 704d 6f64 756c 650d  s...setUpModule.
+000005c0: 0a09 7465 6172 446f 776e 4d6f 6475 6c65  ..tearDownModule
+000005d0: 0d0a 0961 7379 6e63 5365 7455 700d 0a09  ...asyncSetUp...
+000005e0: 6173 796e 6354 6561 7244 6f77 6e0d 0a09  asyncTearDown...
+000005f0: 7365 7455 7054 6573 7444 6174 610d 0a09  setUpTestData...
+00000600: 6661 696c 7572 6545 7863 6570 7469 6f6e  failureException
+00000610: 0d0a 096c 6f6e 674d 6573 7361 6765 0d0a  ...longMessage..
+00000620: 096d 6178 4469 6666 0d0a 0d0a 5b69 736f  .maxDiff....[iso
+00000630: 7274 5d0d 0a6d 756c 7469 5f6c 696e 655f  rt]..multi_line_
+00000640: 6f75 7470 7574 203d 2033 0d0a 696e 636c  output = 3..incl
+00000650: 7564 655f 7472 6169 6c69 6e67 5f63 6f6d  ude_trailing_com
+00000660: 6d61 203d 2074 7275 650d 0a0d 0a5b 6567  ma = true....[eg
+00000670: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000680: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000690: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `sts-lib-0.20.0/sts/__init__.py` & `sts-lib-0.21.0/sts/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import math
 import os
 import re
 import sys
 from collections import OrderedDict, namedtuple
 from contextlib import nullcontext
 
-__version__ = '0.20.0'
+__version__ = '0.21.0'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 
 
 def lazyprop(fn):
     """Lazy property decorator
@@ -45,14 +45,46 @@
     @_lazyprop.setter
     def _lazyprop(self, value):
         setattr(self, attr_name, value)
 
     return _lazyprop
 
 
+class StreamList(list):
+    """A wrapper to make an iterable JSON serializable as a list.
+
+    - Must be an instance of list (to make JSON encoder treat as a list).
+    - Must be truthy when non-empty and falsy when empty.
+    """
+    def __init__(self, iterable):
+        self._iterator = iter(iterable)
+        self._head_sent = False
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if self._head_sent:
+            return next(self._iterator)
+        if not hasattr(self, '_head'):
+            self._head = next(self._iterator)
+        self._head_sent = True
+        return self._head
+
+    def __bool__(self):
+        if hasattr(self, '_head'):
+            return True
+        try:
+            self._head = next(self._iterator)
+        except StopIteration:
+            return False
+        else:
+            return True
+
+
 class Unicode():
     """Utilities for Unicode string handling.
     """
     @staticmethod
     def composite_length(text, pos):
         """Get the length of the Unicode composite at pos.
 
@@ -250,23 +282,22 @@
             self.add(key, values, skip_check=skip_check)
         return self
 
     def load(self, *files):
         """Add all key-values pairs from plain-dict file(s).
         """
         for file in files:
-            with open(file, 'r', encoding='UTF-8') as f:
-                for line in f:
+            with open(file, 'r', encoding='UTF-8') as fh:
+                for line in fh:
                     try:
                         key, values, *_ = line.rstrip('\n').split('\t')
                     except ValueError:
                         pass
                     else:
                         self.add(key, values.split(' '))
-                f.close()
         return self
 
     def dump(self, file=None, sort=False):
         """Dump key-values pairs to a plain-dict file.
 
         Args:
             file: path of file to save. Use stdout if None.
@@ -287,18 +318,17 @@
         """Load from a JSON file.
 
         NOTE: The input data format may vary across subclasses.
 
         Returns:
             a new object with the same class.
         """
-        with open(file, 'r', encoding='UTF-8') as f:
+        with open(file, 'r', encoding='UTF-8') as fh:
             stsdict = self.__class__()
-            stsdict._dict = json.load(f)
-            f.close()
+            stsdict._dict = json.load(fh)
         return stsdict
 
     def dumpjson(self, file=None, indent=None, sort=False):
         """Dump key-values pairs to a JSON file.
 
         NOTE: The output data format may vary across subclasses.
 
@@ -308,15 +338,19 @@
             sort: True to sort the output.
         """
         with (
             open(file, 'w', encoding='UTF-8', newline='')
             if file
             else nullcontext(sys.stdout)
         ) as fh:
-            json.dump(self._dict, fh, ensure_ascii=False, indent=indent, sort_keys=sort)
+            json.dump(
+                self._dict, fh, indent=indent, sort_keys=sort,
+                separators=(',', ':') if indent is None else None,
+                ensure_ascii=False, check_circular=False,
+            )
 
     def print(self, sort=False):
         """Print key-values pairs.
 
         Args:
             sort: True to sort the output.
         """
@@ -386,76 +420,100 @@
     def join(self, stsdict):
         """Join another dictionary.
 
         Applying the returned dictionary to a text simulates the effect
         of applying using self and then using stsdict.
 
         This will invoke stsdict.apply_enum and it's recommended that stsdict
-        be Table or Trie class for better performance.
+        be a Table or Trie for better performance.
 
         Returns:
             a new object with the same class.
         """
         dict1 = self._join_postfix(stsdict)
         dict2 = stsdict._join_prefix(self)
         return dict1.update(dict2)
 
     def _join_prefix(self, stsdict):
         """Prefix self with stsdict.
 
-        Convert keys of self using swapped stsdict.
-        (Enumerate all potential matches.)
+        Convert keys of self using the reversed stsdict, enumerating all
+        possible matches.
+
+        Yield a new key-value pair for the first value of an stsdict entry,
+        e.g.:
+
+            table:
+                註冊表 => 登錄檔
+            stsdict:
+                注 => 註 注
+            reversed stsdict:
+                註 => 注
+            table._join_prefix(stsdict):
+                注冊表 => 登錄檔
+                註冊表 => 登錄檔
+
+        Yield a new minor key-value pair for each minor value of an stsdict
+        entry, e.g.:
+
+            table:
+                註冊表 => 登錄檔
+            stsdict:
+                注 => 注 註
+            reversed stsdict:
+                註 => 注
+            table._join_prefix(stsdict):
+                註冊表 => 登錄檔
+                注冊表 => 注冊表 登錄檔
 
         Returns:
             a new object with the same class.
-
-        e.g.
-        table:
-            註冊表 => 登錄檔
-        stsdict:
-            注 => 註 注
-        swapped stsdict:
-            註 => 注
-        table._join_prefix(stsdict):
-            注冊表 => 登錄檔
-            註冊表 => 登錄檔
         """
         dict_ = self.__class__()
         converter = self.__class__()
+        converter_minor = self.__class__()
         for key, values in stsdict.items():
-            converter.add(values[0], [key])
+            for i, value in enumerate(values):
+                if i == 0:
+                    converter.add(value, [key])
+                else:
+                    converter_minor.add(value, [key])
         for key, values in self.items():
             for newkey in converter.apply_enum(key, include_short=True, include_self=True):
                 dict_.add(newkey, values)
+            for newkey in converter_minor.apply_enum(key, include_short=True, include_self=True):
+                if newkey == key:
+                    continue
+                dict_.add(newkey, newkey)
+                dict_.add(newkey, values)
         return dict_
 
     def _join_postfix(self, stsdict):
         """Postfix self with stsdict.
 
-        Convert values of self using stsdict.
-        (Enumerate maximal matches.)
+        Convert values of self using stsdict, enumerating all maximal matches.
+        Plus all conversions of stsdict.
+
+        Example:
+            table:
+                因为 => 因爲
+            stsdict:
+                爲 => 為
+            table._join_postfix(stsdict):
+                因为 => 因為
+                爲 => 為
 
         Returns:
             a new object with the same class.
-
-        e.g.
-        table:
-            因为 => 因爲
-        stsdict:
-            爲 => 為
-        table._join_postfix(stsdict):
-            因为 => 因為
-            爲 => 為
         """
         dict_ = self.__class__()
         for key, values in self.items():
             for value in values:
                 dict_.add(key, stsdict.apply_enum(value))
-        dict_.update(stsdict)
-        return dict_
+        return dict_.update(stsdict)
 
     def _split(self, parts):
         """Split parts into a list of Unicode composites.
 
         With automatic type handling.
         """
         if isinstance(parts, str):
@@ -492,16 +550,17 @@
 
     def apply(self, parts):
         """Convert text using the dictionary.
 
         Args:
             parts: a string or iterable parts to be converted.
 
-        Returns:
-             a generator of parts, which is a string or an StsDictConv.
+        Yields:
+            the next converted part as an StsDictConv, or an unmatched part as
+            a str.
         """
         parts = self._split(parts)
         i = 0
         total = len(parts)
         while i < total:
             match = self.match(parts, i)
             if match is not None:
@@ -510,37 +569,37 @@
             else:
                 yield parts[i]
                 i += 1
 
     def apply_enum(self, parts, include_short=False, include_self=False):
         """Enumerate all possible conversions of text.
 
+        Example:
+            table:
+                钟 => 鐘 鍾
+                药 => 藥 葯
+                用药 => 用藥
+            text:
+                '看钟用药'
+            table.apply_enum(text, include_short=False, include_self=False):
+                ['看鐘用藥', '看鍾用藥']
+            table.apply_enum(text, include_short=True, include_self=False):
+                ['看鐘用藥', '看鐘用葯', '看鍾用藥', '看鍾用葯']
+            table.apply_enum(text, include_short=False, include_self=True):
+                ['看鐘用藥', '看鐘用药', '看鍾用藥', '看鍾用药', '看钟用藥', '看钟用药']
+            table.apply_enum(text, include_short=True, include_self=True):
+                ['看鐘用藥', '看鐘用药', '看鐘用葯', '看鍾用藥', '看鍾用药', '看鍾用葯', '看钟用藥', '看钟用药', '看钟用葯']
+
         Args:
             parts: a string or iterable parts to be converted.
             include_short: include non-maximal-match conversions
             include_self: include source for every match
 
         Returns:
-            list: a list of possible conversions.
-
-        e.g.
-        table:
-            钟 => 鐘 鍾
-            药 => 藥 葯
-            用药 => 用藥
-        text:
-            '看钟用药'
-        table.apply_enum(text, include_short=False, include_self=False):
-            ['看鐘用藥', '看鍾用藥']
-        table.apply_enum(text, include_short=True, include_self=False):
-            ['看鐘用藥', '看鐘用葯', '看鍾用藥', '看鍾用葯']
-        table.apply_enum(text, include_short=False, include_self=True):
-            ['看鐘用藥', '看鐘用药', '看鍾用藥', '看鍾用药', '看钟用藥', '看钟用药']
-        table.apply_enum(text, include_short=True, include_self=True):
-            ['看鐘用藥', '看鐘用药', '看鐘用葯', '看鍾用藥', '看鍾用药', '看鍾用葯', '看钟用藥', '看钟用药', '看钟用葯']
+            a list of possible conversions.
         """
         text = parts
         parts = self._split(parts)
 
         stack = [(parts, 0, 0)]
         substack = []
         results = OrderedDict()
@@ -794,42 +853,61 @@
         if match:
             conv = StsDictConv(parts[pos:match_end], match)
             return StsDictMatch(conv, pos, match_end)
         return None
 
 
 class StsMaker():
-    """A class for making a dictionary.
+    """A class for making dictionary file(s).
     """
-    def make(self, config_name, base_dir=None, output_dir=None, skip_check=False, skip_requires=False, quiet=False):
-        """Make a dictionary according to config.
-
-        Load dictionaries specified in config and generate a new dictionary.
+    def make(self, config_name, base_dir=None, output_dir=None,
+             skip_check=False, skip_requires=False, quiet=False):
+        """Make dictionary file(s) according to a config.
 
         scheme of config (.json):
-        {
-            "name": "...",
-            "requires": [
-                "..."  // a required config (relative to this config file)
-            ],
-            "dicts": [{
-                "file": "...",  // relative to default config directory
-                "type": "...",  // list, jlist, tlist
-                "mode": "...",  // load, swap, join
-                "src": ["...", ...]  // list of .txt or .list files
-            }, ...]
-        }
+            {
+                "name": "...",
+                "requires": [
+                    "..."  // a required config (relative to this config file)
+                ],
+                "dicts": [  // dictionaries to generate
+                    {
+                        "file": "...",  // path of the generated dictionary
+                                        // file, relative to output_dir
+                        "mode": "...",  // mode to handle the loaded sources:
+                                        // load, swap, join
+                        "sort": true,   // truthy to sort the keys of the
+                                        // generated dictionary
+                        "src": ["...", ...]  // list of the source file paths,
+                                             // should be .txt or .list files
+                    },
+                    ...
+                ]
+            }
+
+        Args:
+            config_name: a str for the config file or name
+            base_dir: a str for the base directory to parse the config path
+                from config_name, or None for CWD
+            output_dir: a str for the output directory, or None for
+                the directory of the config file
+            skip_check: truthy to generate every dictionary no matter that it's
+                already up-to-date
+            skip_requires: truthy to skip making from required configs
+            quiet: truthy to skip reporting details
+
+        Returns:
+            a str for the path of the last generated dictionary file
         """
         # locate and load the config file
         config_file = self.get_config_file(config_name, base_dir=base_dir)
         config_dir = os.path.abspath(os.path.dirname(config_file))
 
-        with open(config_file, 'r', encoding='UTF-8') as f:
-            config = json.load(f)
-            f.close()
+        with open(config_file, 'r', encoding='UTF-8') as fh:
+            config = json.load(fh)
 
         # handle required configs
         if not skip_requires:
             for cf in config.get('requires', []):
                 self.make(cf, base_dir=config_dir, output_dir=output_dir, skip_requires=skip_requires, quiet=quiet)
 
         # make the requested dicts
@@ -883,19 +961,19 @@
             return config
 
         relative_config = os.path.join(base_dir, config) if base_dir is not None else config
         if os.path.isfile(relative_config):
             return relative_config
 
         if os.path.basename(config) == config:
-            search_file = os.path.join(self.DEFAULT_CONFIG_DIR, config)
+            search_file = os.path.join(self.default_config_dir, config)
             if os.path.isfile(search_file):
                 return search_file
             if not config.lower().endswith('.json'):
-                search_file = os.path.join(self.DEFAULT_CONFIG_DIR, config + '.json')
+                search_file = os.path.join(self.default_config_dir, config + '.json')
                 if os.path.isfile(search_file):
                     return search_file
 
         return relative_config
 
     def get_stsdict_file(self, stsdict, base_dir=None):
         """Calculate the path of a dictionary file.
@@ -909,15 +987,15 @@
             return stsdict
 
         relative_stsdict = os.path.join(base_dir, stsdict) if base_dir is not None else stsdict
         if os.path.isfile(relative_stsdict):
             return relative_stsdict
 
         if os.path.basename(stsdict) == stsdict:
-            search_file = os.path.join(self.DEFAULT_DICTIONARY_DIR, stsdict)
+            search_file = os.path.join(self.default_dictionary_dir, stsdict)
             if os.path.isfile(search_file):
                 return search_file
 
         return relative_stsdict
 
     def check_update(self, output, filegroups):
         """Check if the output file needs update.
@@ -930,22 +1008,22 @@
                 files = [files]
             for file in files:
                 if os.path.getmtime(file) > os.path.getmtime(output):
                     return True
 
         return False
 
-    DEFAULT_CONFIG_DIR = os.path.join(os.path.dirname(__file__), 'data', 'config')
-    DEFAULT_DICTIONARY_DIR = os.path.join(os.path.dirname(__file__), 'data', 'dictionary')
+    default_config_dir = os.path.join(os.path.dirname(__file__), 'data', 'config')
+    default_dictionary_dir = os.path.join(os.path.dirname(__file__), 'data', 'dictionary')
 
 
 class StsConverter():
     """Convert a text using an stsdict.
     """
-    def __init__(self, stsdict, options=None):
+    def __init__(self, stsdict):
         """Initialize a converter.
 
         Args:
             stsdict: an StsDict or a str, bytes or os.PathLike object for a
                 dictionary file
         """
         if isinstance(stsdict, StsDict):
@@ -954,158 +1032,152 @@
             _, ext = os.path.splitext(stsdict)
             if ext.lower() == '.jlist':
                 self.table = Table().loadjson(stsdict)
             elif ext.lower() == '.tlist':
                 self.table = Trie().loadjson(stsdict)
             else:  # default: list
                 self.table = Table().load(stsdict)
-        self.options = {**self.default_options, **(options or {})}
 
-    def convert(self, text):
-        """Convert a text.
+    def convert(self, text, exclude=None):
+        """Convert a text and yield each part.
 
-        Returns:
-            a generator of converted data.
-        """
-        try:
-            regex = re.compile(self.options['exclude'])
-        except TypeError:
-            conversion = self.table.apply(text)
-        except re.error as ex:
-            raise ValueError(f'regex syntax error for --exclude: {ex}')
-        else:
-            def convert_with_regex(text, regex):
-                index = 0
-                for m in regex.finditer(text):
-                    start, end = m.start(0), m.end(0)
-
-                    t = text[index:start]
-                    if t:
-                        yield from self.table.apply(t)
-
-                    t = text[start:end]
-                    if t:
-                        try:
-                            yield m.group('return')
-                        except IndexError:
-                            yield t
-
-                    index = end
+        Yields:
+            the next converted part as an StsDictConv, or an unmatched part as
+            a str.
+        """
+        if exclude is None:
+            yield from self.table.apply(text)
+            return
+
+        def convert_with_regex(text, regex):
+            index = 0
+            for m in regex.finditer(text):
+                start, end = m.start(0), m.end(0)
 
-                t = text[index:]
+                t = text[index:start]
                 if t:
                     yield from self.table.apply(t)
 
-            conversion = convert_with_regex(text, regex)
-
-        yield from conversion
+                t = text[start:end]
+                if t:
+                    try:
+                        yield m.group('return')
+                    except IndexError:
+                        yield t
+
+                index = end
+
+            t = text[index:]
+            if t:
+                yield from self.table.apply(t)
+
+        yield from convert_with_regex(text, exclude)
+
+    def convert_formatted(self, text, format=None, exclude=None):
+        """Convert a text and yield each formatted part.
+        """
+        conv = self.convert(text, exclude=exclude)
+        format = format if format is not None else 'txt'
+        formatter = getattr(self, f'_convert_formatted_{format}')
+        yield from formatter(conv)
+
+    def _convert_formatted_txt(self, parts):
+        for part in parts:
+            if isinstance(part, str):
+                yield part
+            else:
+                yield part[1][0]
 
-    def convert_text(self, text):
-        """Convert a text.
+    def _convert_formatted_txtm(self, parts, start='{{', end='}}', sep='->', vsep='|'):
+        for part in parts:
+            if isinstance(part, str):
+                yield part
+            else:
+                olds, news = part
+                old = ''.join(olds)
 
-        Returns:
-            converted text content.
-        """
-        def parts_to_text(parts):
-            for part in parts:
-                if isinstance(part, str):
-                    yield part
+                if len(news) == 1 and old == news[0]:
+                    yield f'{start}{old}{end}'
                 else:
-                    yield part[1][0]
+                    new = vsep.join(news)
+                    yield f'{start}{old}{sep}{new}{end}'
 
-        def parts_to_marked_text(parts):
-            for part in parts:
-                if isinstance(part, str):
-                    yield part
-                else:
-                    olds, news = part
-                    old = ''.join(olds)
+    def _convert_formatted_html(self, parts):
+        for part in parts:
+            if isinstance(part, str):
+                yield html.escape(part)
+            else:
+                olds, news = part
+                old = ''.join(olds)
+                content = f'<del hidden>{html.escape(old)}</del>'
+                for i, v in enumerate(news):
+                    hidden = '' if i == 0 else ' hidden'
+                    content += f'<ins{hidden}>{html.escape(v)}</ins>'
+
+                part = f"""<a>{content}</a>"""
+                yield part
+
+    def _convert_formatted_htmlpage(self, parts):
+        with open(self.default_htmlpage_template,
+                  encoding='UTF-8', newline='') as fh:
+            html = fh.read()
+
+        pos = 0
+        for m in self.regex_template.finditer(html):
+            yield html[pos:m.start(0)]
+
+            key = m.group(1)
+            if key == 'CONTENT':
+                yield from self._convert_formatted_html(parts)
+            elif key == 'VERSION':
+                yield __version__
+
+            pos = m.end(0)
+
+        yield html[pos:]
+
+    def _convert_formatted_json(self, parts, indent=None):
+        encoder = json.JSONEncoder(
+            indent=indent,
+            separators=(',', ':') if indent is None else None,
+            ensure_ascii=False, check_circular=False,
+        )
+        yield from encoder.iterencode(StreamList(parts))
 
-                    if len(news) == 1 and old == news[0]:
-                        yield '{{' + old + '}}'
-                    else:
-                        yield '{{' + old + '->' + '|'.join(news) + '}}'
+    def convert_text(self, text, format=None, exclude=None):
+        """Convert a text and return the result.
 
-        def parts_to_html(parts):
-            for part in parts:
-                if isinstance(part, str):
-                    yield html.escape(part)
-                else:
-                    olds, news = part
-                    old = ''.join(olds)
-                    content = f'<del>{html.escape(old)}</del>'
-                    for v in news:
-                        content += f'<ins>{html.escape(v)}</ins>'
-
-                    # classes
-                    classes = ['sts-conv']
-                    if len(news) == 1:
-                        classes.append('single')
-                    else:
-                        classes.append('plural')
-                    if old == news[0]:
-                        classes.append('exact')
-                    if len(olds) == 1:
-                        classes.append('atomic')
-
-                    part = f"""<span class="{' '.join(classes)}">{content}</span>"""
-                    yield part
-
-        conversion = self.convert(text)
-
-        if self.options['format'] == 'htmlpage':
-            return """<!DOCTYPE html>
-<html>
-<head>
-<meta charset="UTF-8">
-<style>
-pre { white-space: pre-wrap; }
-.sts-conv { font-weight: normal; border: thin dotted #AAA; }
-.sts-conv.plural { background: #FFFF99; }
-.sts-conv.exact { background: #DDDDFF; }
-.sts-conv.single { background: #CCFFCC; }
-.sts-conv ins, .sts-conv del { text-decoration: none; }
-.sts-conv del { display: none; }
-.sts-conv ins { display: none; }
-.sts-conv ins:first-of-type { display: inline; }
-</style>
-</head>
-<body>
-<pre contenteditable="true">""" + ''.join(parts_to_html(conversion)) + """</pre>
-</body>
-</html>"""
-        elif self.options['format'] == 'html':
-            return ''.join(parts_to_html(conversion))
-        elif self.options['format'] == 'json':
-            return json.dumps(list(conversion), ensure_ascii=False)
-        elif self.options['format'] == 'txtm':
-            return ''.join(parts_to_marked_text(conversion))
-        else:  # default: format = 'txt'
-            return ''.join(parts_to_text(conversion))
+        Returns:
+            a str of converted parts in the specified format.
+        """
+        conv = self.convert_formatted(text, format=format, exclude=exclude)
+        return ''.join(conv)
 
-    def convert_file(self, input=None, output=None, input_encoding='UTF-8', output_encoding='UTF-8'):
+    def convert_file(self, input=None, output=None,
+                     input_encoding='UTF-8', output_encoding='UTF-8',
+                     format=None, exclude=None):
         """Convert input and write to output.
 
         Args:
             input: a file path or None for stdin.
             output: a file path or None for stdout.
         """
         with (
             open(input, 'r', encoding=input_encoding, newline='')
             if input
             else nullcontext(sys.stdin)
         ) as fh:
             text = fh.read()
 
-        conversion = self.convert_text(text)
+        conv = self.convert_formatted(text, format=format, exclude=exclude)
 
         with (
             open(output, 'w', encoding=output_encoding, newline='')
             if output
             else nullcontext(sys.stdout)
         ) as fh:
-            fh.write(conversion)
+            for part in conv:
+                fh.write(part)
+
+    default_htmlpage_template = os.path.join(os.path.dirname(__file__), 'data', 'htmlpage.tpl.html')
 
-    default_options = {
-        'format': 'txt',
-        'exclude': None,
-    }
+    regex_template = re.compile(r'%(\w+)%')
```

### Comparing `sts-lib-0.20.0/sts/cli.py` & `sts-lib-0.21.0/sts/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 """Command line interface."""
 import argparse
 import os
+import re
 import sys
 
 from . import StsConverter, StsMaker, Table
 from . import __doc__ as _doc
 from . import __version__
 
 
@@ -65,31 +66,38 @@
 def convert(args):
     """Convert a file using the given config.
     """
     inputs = args['file']
     outputs = args['output']
     force_stdout = args['stdout']
     config = args['config']
-    options = {
-        'format': args['format'],
-        'exclude': args['exclude'],
-    }
+    format = args['format']
+    exclude = args['exclude']
     input_encoding = args['in_enc']
     output_encoding = args['out_enc']
 
     stsdict = StsMaker().make(config, quiet=True)
-    converter = StsConverter(stsdict, options)
+    converter = StsConverter(stsdict)
 
     # read STDIN if no input file is specified
     if not len(inputs):
         inputs.append(None)
 
     for i, input in enumerate(inputs):
         output = None if force_stdout else input if i >= len(outputs) else outputs[i]
-        converter.convert_file(input, output, input_encoding, output_encoding)
+        converter.convert_file(input, output, input_encoding, output_encoding,
+                               format=format, exclude=exclude)
+
+
+def regex(text):
+    """Compile a regex str with nice error message."""
+    try:
+        return re.compile(text)
+    except re.error as exc:
+        raise ValueError(f'regex syntax error: {exc}') from None
 
 
 def parse_args(argv=None):
     # Improve program name when executed through python -m
     # NOTE: We don't expect a bad command name such as having a space.
     if os.path.basename(sys.argv[0]) == '__main__.py':
         prog = f'{os.path.basename(sys.executable)} -m sts'
@@ -110,15 +118,15 @@
     parser_convert.add_argument('-c', '--config', default='s2t',
                                 help="""the config to use, either a built-in config name or a path to a custom JSON file
 (built-in configs: s2t|t2s|s2tw|tw2s|s2twp|tw2sp|s2hk|hk2s|t2tw|tw2t|t2hk|hk2t|t2jp|jp2t)
 (default: %(default)s)""")
     parser_convert.add_argument('-f', '--format', default='txt',
                                 choices=['txt', 'txtm', 'html', 'htmlpage', 'json'], metavar='FORMAT',
                                 help="""output format (txt|txtm|html|htmlpage|json) (default: %(default)s)""")
-    parser_convert.add_argument('--exclude',
+    parser_convert.add_argument('--exclude', type=regex,
                                 help="""exclude text matching given regex from conversion, and replace it with the "return" subgroup value if exists""")
     parser_convert.add_argument('--in-enc', default='UTF-8', metavar='ENCODING',
                                 help="""encoding for input (default: %(default)s)""")
     parser_convert.add_argument('--out-enc', default='UTF-8', metavar='ENCODING',
                                 help="""encoding for output (default: %(default)s)""")
     parser_convert.add_argument('-o', '--output', default=[], action='append',
                                 help="""path to output (for the corresponding input) (default: to input)""")
```

### Comparing `sts-lib-0.20.0/sts/data/config/_default.json` & `sts-lib-0.21.0/sts/data/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/dictionary/HKVariants.txt` & `sts-lib-0.21.0/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts-lib-0.21.0/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts-lib-0.21.0/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/dictionary/JPVariants.txt` & `sts-lib-0.21.0/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/dictionary/STCharacters.txt` & `sts-lib-0.21.0/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/dictionary/STPhrases.txt` & `sts-lib-0.21.0/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/dictionary/TSCharacters.txt` & `sts-lib-0.21.0/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/dictionary/TSPhrases.txt` & `sts-lib-0.21.0/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/dictionary/TWPhrasesIT.txt` & `sts-lib-0.21.0/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/dictionary/TWPhrasesName.txt` & `sts-lib-0.21.0/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/dictionary/TWPhrasesOther.txt` & `sts-lib-0.21.0/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts-lib-0.21.0/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/scheme/st_multi.txt` & `sts-lib-0.21.0/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts/data/scheme/variant.txt` & `sts-lib-0.21.0/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts-lib-0.20.0/sts_lib.egg-info/PKG-INFO` & `sts-lib-0.21.0/sts_lib.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.20.0
+Version: 0.21.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -53,50 +53,84 @@
 
     pip install -U sts-lib
 
 ### Command Line
 
 * `sts --help` 或 `sts COMMAND --help` 檢視可用指令的詳細說明文檔。
 
-* `sts convert [OPTIONs] [file [file ...]]` 執行簡繁轉換：
+* `sts convert [OPTIONs] [file ...]` 執行簡繁轉換：
   * `file` 為一或多個欲轉換的檔案。（省略則讀取標準輸入 STDIN）
   * `-c CONFIG` 指定配置檔，可為內建配置檔名稱或自製 JSON 配置檔的路徑。可用的內建配置檔詳見 [sts/data/config](https://github.com/danny0838/sts-lib/tree/master/sts/data/config) 目錄，可簡寫，例如輸入 `s2t` 代表使用 `sts/data/config/s2t.json`。
   * `-f FORMAT` 指定輸出格式，可用格式如下：
     * `txt`：純文字，適合一般使用。
     * `txtm`：純文字加轉換標示。
     * `html`：加上 HTML 標記的文本，可嵌入至網頁應用程式做互動式校對。
     * `htmlpage`：加入 HTML 樣式的網頁，可直接開啟做互動式校對。
     * `json`：以 JSON 格式表示轉換輸出，可用其他程式進一步解析處理。
   * `--exclude PATTERN` 指定用於忽略簡繁轉換的正規表示式。有指定 `return` 子群組時會取代為子群組的值。
     * 例如 `sts convert -c s2twp --exclude "「.*?」"` 會把 `「程序」正义` 轉換為 `「程序」正義`。
     * 例如 `sts convert -c s2twp --exclude "-{(?P<return>.*?)}-"` 會把 `-{程序}-正义` 轉換為 `程序正義`。
   * `--in-enc ENCODING` 指定輸入編碼。可用編碼參見[這裡](https://docs.python.org/3/library/codecs.html#standard-encodings)。
   * `--out-enc ENCODING` 指定輸出編碼。可用編碼參見[這裡](https://docs.python.org/3/library/codecs.html#standard-encodings)。
-  * `-o OUTPUT` 指定對應輸入檔案轉換結果的輸出路徑。（無對應者輸出至原處）
+  * `-o OUTPUT` 可重覆多次，指定對應輸入檔案轉換結果的輸出路徑。（無對應者輸出至原檔）
   * `--stdout` 將所有轉換結果輸出至標準輸出 STDOUT。
 
 ### Python
 
 ```python
 from sts import StsMaker, StsConverter
 
 # generate a dictionary file from a config and get its path
 dictfile = StsMaker().make('s2t', quiet=True)
 
-# initialize the converter from the dictionary file
-converter = StsConverter(dictfile, options={})
+# initialize a converter from the dictionary file
+converter = StsConverter(dictfile)
 
-# perform conversion for a text
-converter.convert_text('汉字')  # 漢字
+# perform conversion for a string
+converter.convert_text('汉字', format='txt', exclude=None)  # 漢字
 
 # perform conversion for a file (None for stdin/stdout)
-converter.convert_file(input=None, output=None)
+converter.convert_file(input=None, output=None
+                       input_encoding='UTF-8', output_encoding='UTF-8',
+                       format='txt', exclude=None)
 
-# process conversion data generator
-[p for p in converter.convert("汉字")]  # [StsDictConv(key=['汉'], values=['漢']), '字']
+# perform a conversion for a string and process the result data generator
+[p for p in converter.convert("干了吧")]  # [StsDictConv(key=['干', '了'], values=['幹了', '乾了']), '吧']
+```
+
+## Config 配置檔
+
+```javascript
+/**
+ * @typedef {Object} configScheme
+ * @property {string} [name] - name/description of the config
+ * @property {string[]} [requires] - required configs, which are made before
+ *     making from this config, as an absolute path, or a path relative to the
+ *     directory of this config file, or the basename of a built-in config file
+ *     (with or without ".json")
+ * @property {dictScheme[]} dicts - schemes of each dictionary file to generate
+ */
+
+/**
+ * @typedef {Object} dictScheme
+ * @property {string} file - path of the dictionary file to generate. Each as
+ *     an absolute path, or a path relative to the specified output directory
+ *     (or the directory of this config file). Each should be a .tlist
+ *     (compiled trie), .jlist (compiled table), or .list (plain text table).
+ * @property {string} mode - the mode to handle the loaded source files: "load"
+ *     to simply merge the loaded keys and values; "swap" to reverse the
+ *     dictionary (i.e. use the values as keys and the keys as values); "join"
+ *     to build from a chain of dictionaries (in which case src must be an
+ *     array of subarrays of strings)
+ * @property {boolean} [sort] - true to sort the keys of the output dictionary
+ * @property {Array.<(string|string[])>} src - the source files. Each as an
+ *     absolute path, or a path relative to the directory of this config file,
+ *     or the basename of a built-in dictionary file. Each should be a .txt or
+ *     .list dictionary file.
+ */
 ```
 
 ## License 許可協議
 
 本專案以 Apache License 2.0 協議授權使用。
 
 詞典檔原始資料來自同文堂、維基百科、OpenCC 等開源專案，再按本專案之需求編校。
```

### Comparing `sts-lib-0.20.0/sts_lib.egg-info/SOURCES.txt` & `sts-lib-0.21.0/sts_lib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 sts/__init__.py
 sts/__main__.py
 sts/cli.py
+sts/data/htmlpage.tpl.html
 sts/data/config/_default.json
 sts/data/config/hk2s.json
 sts/data/config/hk2t.json
 sts/data/config/jp2t.json
 sts/data/config/s2hk.json
 sts/data/config/s2t.json
 sts/data/config/s2tw.json
```

