# Comparing `tmp/JsonPreprocessor-0.4.0.tar.gz` & `tmp/JsonPreprocessor-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsonPreprocessor-0.4.0.tar", last modified: Tue Apr  9 15:45:15 2024, max compression
+gzip compressed data, was "JsonPreprocessor-0.5.0.tar", last modified: Thu Apr 11 15:45:51 2024, max compression
```

## Comparing `JsonPreprocessor-0.4.0.tar` & `JsonPreprocessor-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:45:15.403865 JsonPreprocessor-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:45:15.399865 JsonPreprocessor-0.4.0/JsonPreprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)    65457 2024-04-09 15:42:59.000000 JsonPreprocessor-0.4.0/JsonPreprocessor/CJsonPreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)   323895 2024-04-09 15:45:15.000000 JsonPreprocessor-0.4.0/JsonPreprocessor/JsonPreprocessor.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-09 15:42:59.000000 JsonPreprocessor-0.4.0/JsonPreprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-09 15:42:59.000000 JsonPreprocessor-0.4.0/JsonPreprocessor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:45:15.399865 JsonPreprocessor-0.4.0/JsonPreprocessor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-09 15:45:15.000000 JsonPreprocessor-0.4.0/JsonPreprocessor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 15:45:15.000000 JsonPreprocessor-0.4.0/JsonPreprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:45:15.000000 JsonPreprocessor-0.4.0/JsonPreprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 15:45:15.000000 JsonPreprocessor-0.4.0/JsonPreprocessor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-09 15:42:59.000000 JsonPreprocessor-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-09 15:45:15.399865 JsonPreprocessor-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-09 15:42:59.000000 JsonPreprocessor-0.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:45:15.403865 JsonPreprocessor-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-09 15:42:59.000000 JsonPreprocessor-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:51.780022 JsonPreprocessor-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:51.780022 JsonPreprocessor-0.5.0/JsonPreprocessor/
+-rw-r--r--   0 runner    (1001) docker     (127)    62065 2024-04-11 15:43:58.000000 JsonPreprocessor-0.5.0/JsonPreprocessor/CJsonPreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)   324420 2024-04-11 15:45:51.000000 JsonPreprocessor-0.5.0/JsonPreprocessor/JsonPreprocessor.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-11 15:43:58.000000 JsonPreprocessor-0.5.0/JsonPreprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-11 15:43:58.000000 JsonPreprocessor-0.5.0/JsonPreprocessor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:51.780022 JsonPreprocessor-0.5.0/JsonPreprocessor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-11 15:45:51.000000 JsonPreprocessor-0.5.0/JsonPreprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-11 15:45:51.000000 JsonPreprocessor-0.5.0/JsonPreprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:45:51.000000 JsonPreprocessor-0.5.0/JsonPreprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 15:45:51.000000 JsonPreprocessor-0.5.0/JsonPreprocessor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-11 15:43:58.000000 JsonPreprocessor-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-11 15:45:51.780022 JsonPreprocessor-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-11 15:43:58.000000 JsonPreprocessor-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:45:51.784021 JsonPreprocessor-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-11 15:43:58.000000 JsonPreprocessor-0.5.0/setup.py
```

### Comparing `JsonPreprocessor-0.4.0/JsonPreprocessor/CJsonPreprocessor.py` & `JsonPreprocessor-0.5.0/JsonPreprocessor/CJsonPreprocessor.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     AVOIDDATATYPE    = "JPavoidDataType_"
     COLONS           = "__handleColonsInLine__"
     DUPLICATEDKEY_00 = "__handleDuplicatedKey__00"
     DUPLICATEDKEY_01 = "__handleDuplicatedKey__"
     STRINGCONVERT    = "__ConvertParameterToString__"
     LISTINDEX        = "__IndexOfList__"
     SLICEINDEX       = "__SlicingIndex__"
+    STRINGVALUE      = "__StringValueMake-up__"
 
 class CPythonJSONDecoder(json.JSONDecoder):
     """
 Extends the JSON syntax by the Python keywords ``True``, ``False`` and ``None``.
 
 **Arguments:**
 
@@ -192,14 +193,35 @@
         self.dUpdatedParams = {}
         self.lNestedParams = []
         self.lDotInParamName = []
         self.bDuplicatedKeys = True
         self.jsonCheck = {}
         self.JPGlobals = {}
 
+    def __getFailedJsonDoc(self, jsonDecodeError=None, areaBeforePosition=50, areaAfterPosition=20, oneLine=True):
+        failedJsonDoc = None
+        if jsonDecodeError is None:
+            return failedJsonDoc
+        try:
+            jsonDoc = jsonDecodeError.doc
+        except:
+            # 'jsonDecodeError' seems not to be a JSON exception object ('doc' not available)
+            return failedJsonDoc
+        jsonDocSize     = len(jsonDoc)
+        positionOfError = jsonDecodeError.pos
+        if areaBeforePosition > positionOfError:
+            areaBeforePosition = positionOfError
+        if areaAfterPosition > (jsonDocSize - positionOfError):
+            areaAfterPosition = jsonDocSize - positionOfError
+        failedJsonDoc = jsonDoc[positionOfError-areaBeforePosition:positionOfError+areaAfterPosition]
+        failedJsonDoc = f"... {failedJsonDoc} ..."
+        if oneLine is True:
+            failedJsonDoc = failedJsonDoc.replace("\n", r"\n")
+        return failedJsonDoc
+
     def __reset(self) -> None:
         """
 Reset initial variables which are set in constructor method after master JSON file is loaded.
         """
         self.jsonPath = ''
         self.lImportedFiles = []
         self.recursive_level = 0
@@ -679,15 +701,14 @@
 
 * ``oJsonOut``
 
   / *Type*: dict /
 
   Output JSON object as dictionary with all variables resolved.
         """
-
         def __jsonUpdated(k, v, oJson, bNested, keyNested = '', bDuplicatedHandle=False, recursive = False):
             if keyNested != '':
                 if not bDuplicatedHandle and keyNested in oJson.keys():
                     del oJson[keyNested]
                 rootKey = re.sub(r'\[.*\]', "", k, re.UNICODE)
                 if re.search(r'^[0-9]+.*$', rootKey, re.UNICODE):
                     oJson[f"{rootKey}"] = {}
@@ -884,124 +905,14 @@
             if re.match(r"^.+\['" + k + r"'\]$", parentParams, re.UNICODE):
                 parentParams = re.sub("\['" + k + "'\]", "", parentParams)
             if not recursive:
                 parentParams = ''
         del tmpJson
         return oJson, bNested
 
-    def __checkAndUpdateKeyValue(self, sInputStr: str, nestedKey = False) -> str:
-        """
-This function checks and makes up all nested parameters in JSON configuration files.
-
-**Arguments:**
-
-* ``sInputStr*``
-
-  / *Condition*: required / *Type*: str /
-
-  Key or value which is parsed from JSON configuration file.
-
-**Returns:**
-   The string after nested parameters are made up.
-
-   Ex:
-
-      Nested param ${abc}['xyz'] -> "${abc}['xyz']"
-
-      Nested param "${abc}['xyz']" -> "${abc}['xyz']__ConvertParameterToString__"
-        """
-        def __recursiveNestedHandling(sInputStr: str, lNestedParam: list) -> str:
-            """
-This method handles nested parameters are called recursively in a string value.
-            """
-            tmpList = []
-            for item in lNestedParam:
-                item = re.sub(r'([$()\[\]])', r'\\\1', item)
-                pattern = rf"(\${{\s*[^{re.escape(self.specialCharacters)}]*" + item + \
-                            rf"[^{re.escape(self.specialCharacters)}]*\s*}}(\[\s*.+\s*\])*)"
-                if re.search(pattern, sInputStr, re.UNICODE):
-                    sInputStr = re.sub("(" + pattern + ")", "\\1" + CNameMangling.STRINGCONVERT.value, sInputStr, re.UNICODE)
-                tmpResults = re.findall("(" + pattern + CNameMangling.STRINGCONVERT.value + ")", sInputStr, re.UNICODE)
-                for result in tmpResults:
-                    tmpList.append(result[0])
-            if tmpList != []:
-                sInputStr = __recursiveNestedHandling(sInputStr, tmpList)
-
-            return sInputStr
-
-        variablePattern = rf"[^{re.escape(self.specialCharacters)}]+"
-        indexPattern = r"\[[\s\-\+\d]*\]|\[.*:.*\]"
-        dictPattern = r"\[+\s*'.+'\s*\]+|\[+\s*\d+\s*\]+|\[+\s*\${\s*" + variablePattern + r"\s*}.*\]+|" + indexPattern
-        nestedPattern = r"\${\s*" + variablePattern + r"(\.*\${\s*" + variablePattern + r"\s*})*" + r"\s*}(" + dictPattern + r")*"
-        valueStrPattern = r"[\"|\']\s*[0-9A-Za-z_\-\s*]+[\"|\']"
-        valueNumberPattern = r"[0-9\.]+"
-
-        if "${" in sInputStr:
-            if re.match(r"^\s*" + nestedPattern + r"[\s,\]}]*$", sInputStr, re.UNICODE):
-                iCheck = sInputStr.count("]") - sInputStr.count("[")
-                if iCheck > 0:
-                    tmpItems = sInputStr.split("]")
-                    index = len(tmpItems) - iCheck
-                    sParam = "]".join(tmpItems[:index])
-                    dReplacements = {"$":"\$", "[":"\[", "]":"\]", "-":"\-", "+":"\+"}
-                    paramPattern = self.__multipleReplace(sParam, dReplacements)
-                    sInputStr = re.sub("(" + paramPattern + ")", "\"\\1\"", sInputStr, re.UNICODE)
-                else:
-                    sInputStr = re.sub("(" + nestedPattern + ")", "\"\\1\"", sInputStr, re.UNICODE)
-                nestedParam = re.sub(r"^\s*\"(.+)\".*$", "\\1", sInputStr)
-                self.lNestedParams.append(nestedParam)
-            elif re.match(r"^\s*\"\s*" + nestedPattern + r"\"[\s,\]}]*$", sInputStr, re.UNICODE):
-                nestedParam = re.sub(r"^\s*\"(.+)\".*$", "\\1", sInputStr)
-                self.lNestedParams.append(nestedParam)
-                sInputStr = sInputStr.replace(nestedParam, nestedParam + CNameMangling.STRINGCONVERT.value)
-            elif ((re.match(r"[\s{\[]*\".+\"\s*", sInputStr) and sInputStr.count("\"")==2) \
-                or (re.match(r"^\s*\${.+}[,\s]*$", sInputStr) and sInputStr.count("{")==sInputStr.count("}") \
-                    and not re.search(r"(?<!^)(?<!\.)[^\.]\${", sInputStr.strip()) and not nestedKey)) \
-                and re.search("(" + nestedPattern + ")", sInputStr, re.UNICODE):
-                if sInputStr.strip()[-1] == ",":
-                    sInputStr = sInputStr.strip()[:-2] + CNameMangling.STRINGCONVERT.value + "\","
-                else:
-                    sInputStr = sInputStr.strip()[:-1] + CNameMangling.STRINGCONVERT.value + "\""
-            elif "," in sInputStr.strip()[:-1]:
-                listPattern = r"^\s*(\"*" + nestedPattern + r"\"*\s*,+\s*|" + valueStrPattern + r"\s*,+\s*|" + valueNumberPattern + r"\s*,+\s*)+" + \
-                            r"(\"*" + nestedPattern + r"\"*\s*,*\s*|" + valueStrPattern + r"\s*,*\s*|" + valueNumberPattern + r"[\s,]*)*[\]}\s]*$"
-                lNestedParam = re.findall("(" + nestedPattern + ")", sInputStr, re.UNICODE)
-                for nestedParam in lNestedParam:
-                    self.lNestedParams.append(nestedParam[0])
-                if re.match(listPattern, sInputStr):
-                    items = sInputStr.split(",")
-                    newInputStr = ''
-                    for item in items:
-                        tmpItem = item
-                        if "${" in item:
-                            if not re.match(r"^[\s\"]*" + nestedPattern + r"[\"\]}\s]*$", item, re.UNICODE):
-                                self.__reset()
-                                raise Exception(f"Invalid parameter format: {item}")
-                            elif re.match(r"^\s*\".*" + nestedPattern + r".*\"\s*$", item, re.UNICODE):
-                                item = re.sub("(" + nestedPattern + ")", "\\1" + CNameMangling.STRINGCONVERT.value, item)
-                                tmpList = []
-                                for subItem in re.findall("(" + nestedPattern + CNameMangling.STRINGCONVERT.value + ")", item, re.UNICODE):
-                                    tmpList.append(subItem[0])
-                                item = __recursiveNestedHandling(item, tmpList)
-                            elif re.match(r"^\s*" + nestedPattern + r"[\s\]}]*$", item, re.UNICODE):
-                                item = re.sub("(" + nestedPattern + ")", "\"\\1\"", item, re.UNICODE)
-                                nestedParam = re.sub(r"^\s*\"(.+)\".*$", "\\1", item)
-                                self.lNestedParams.append(nestedParam)
-                        newInputStr = newInputStr + item if tmpItem==items[len(items)-1] else newInputStr + item + ","
-                    sInputStr = newInputStr
-            elif nestedKey and re.match(r"^\s*\${[^\(\)\!@#%\^\&\-\+\/\\\=`~\?]+[}\[\]]+\s*$", sInputStr):
-                sInputStr = re.sub(r"^\s*(\${[^\(\)\!@#%\^\&\-\+\/\\\=`~\?]+[}\[\]]+)\s*$", "\"\\1\"", sInputStr)
-            elif not re.match(r"^\s*\".+\"[,\s]*$", sInputStr):
-                if not re.match(r"^.+,\s*$", sInputStr):
-                    sInputStr = re.sub(r"^\s*(.+)\s*$", "\"\\1\"", sInputStr)
-                else:
-                    sInputStr = re.sub(r"^\s*(.+)\s*,\s*$", "\"\\1\",", sInputStr)
-        sOutput = sInputStr
-        return sOutput
-
     def __checkDotInParamName(self, oJson : dict):
         """
 This is recrusive funtion collects all parameters which contain "." in the name.
 
 **Arguments:**
 
 * ``oJson``
@@ -1175,26 +1086,14 @@
 
 * ``oJson``
 
   / *Type*: dict /
 
   Preprocessed JSON file(s) as Python dictionary
         """
-        def __handleListElements(sInput : str) -> str:
-            items = re.split("\s*,\s*", sInput)
-            j=0
-            newItem = ""
-            for item in items:
-                j+=1
-                if j<len(items):
-                    newItem = newItem + self.__checkAndUpdateKeyValue(item) + ","
-                else:
-                    newItem = newItem + self.__checkAndUpdateKeyValue(item)
-            return newItem
-        
         def __handleDuplicatedKey(dInput : dict) -> dict:
             listKeys = list(dInput.keys())
             dictValues = {}
             for key in listKeys:
                 if CNameMangling.DUPLICATEDKEY_01.value in key:
                     origKey = re.sub(CNameMangling.DUPLICATEDKEY_01.value + "\d+\s*$", "", key)
                     dictValues[origKey] = copy.deepcopy(dInput[origKey])
@@ -1231,14 +1130,36 @@
                     self.__checkNestedParam(k, bKey=True)
                 if isinstance(v, list):
                     for item in v:
                         if isinstance(item, str) and "${" in item:
                             self.__checkNestedParam(item)
                 elif isinstance(v, dict):
                     __checkKeynameFormat(v)
+        
+        def __handleLastElement(sInput : str) -> str:
+            '''
+This function handle a last element of a list or dictionary
+            '''
+            param = re.search(r'(' + nestedPattern + r')', sInput)
+            if param is not None and re.match(r'^[\s\[\]{}]*$', sInput.replace(param[0], '')):
+                sParam = param[0]
+                if sParam.count('[')<sParam.count(']'):
+                    while re.search(r'\[[^\]]+\]', sParam):
+                        sParam = re.sub(r'\[[^\]]+\]', '', sParam)
+                    while re.search(r'\${[^}]+}', sParam):
+                        sParam = re.sub(r'\${[^}]+}', '', sParam)
+                    index = len(sParam)
+                    sParam = param[0]
+                    sParam = sParam[:-index]
+                dReplacements = {"$":"\$", "[":"\[", "]":"\]", ".":"\.", "-":"\-", "+":"\+"}
+                tmpPattern = self.__multipleReplace(sParam, dReplacements)
+                sInput = re.sub(r'(' + tmpPattern + r')', '"\\1"', sInput)
+            else:
+                sInput = '"' + sInput.strip() + '"'
+            return sInput
 
         jFile = CString.NormalizePath(jFile, sReferencePathAbs=os.path.dirname(os.path.abspath(sys.argv[0])))
         if  not(os.path.isfile(jFile)):
             self.__reset()
             raise Exception(f"File '{jFile}' is not existing!")
 
         self.lImportedFiles.append(jFile)
@@ -1256,14 +1177,15 @@
             try:
                 listDummy = shlex.split(line)
             except Exception as error:
                 self.__reset()
                 raise Exception(f"\n{str(error)} in line: '{line}'")
 
             if "${" in line:
+                curLine = line
                 lNestedVar = re.findall(rf"\${{\s*([^{re.escape(self.specialCharacters)}]+)\s*}}", line, re.UNICODE)
                 for nestedVar in lNestedVar:
                     if nestedVar[0].isdigit():
                         self.__reset()
                         raise Exception(f"Invalid parameter format in line: {line.strip()}")
                 tmpList01 = re.findall(r"(\"[^\"]+\")", line)
                 line = re.sub(r"(\"[^\"]+\")", CNameMangling.COLONS.value, line)
@@ -1271,84 +1193,93 @@
                 tmpList02 = re.findall(slicingPattern, line)
                 line = re.sub(slicingPattern, CNameMangling.SLICEINDEX.value, line)
                 indexPattern = r"\[[\s\-\+\d]*\]"
                 if re.search(indexPattern, line):
                     indexList = re.findall(indexPattern, line)
                     line = re.sub("(" + indexPattern + ")", CNameMangling.LISTINDEX.value, line)
                 items = re.split("\s*:\s*", line)
-                newLine = ""
-                i=0
+                iItems = len(items)-1 if items[-1]=='' else len(items) 
+                newLine = ''
+                preItem = ''
+                i=1
                 for item in items:
-                    nestedKey = False
-                    nestedKeyPattern = r"^\s*,\s*\${.+[\]}]\s*$"
-                    if i==0 or re.match(nestedKeyPattern, item):
-                        nestedKey = True
                     if CNameMangling.COLONS.value in item:
                         while CNameMangling.COLONS.value in item:
                             item = item.replace(CNameMangling.COLONS.value, tmpList01.pop(0), 1)
                     elif CNameMangling.LISTINDEX.value in item:
                         while CNameMangling.LISTINDEX.value in item:
                             item = item.replace(CNameMangling.LISTINDEX.value, indexList.pop(0), 1)
                     elif CNameMangling.SLICEINDEX.value in item:
                         while CNameMangling.SLICEINDEX.value in item:
                             item = item.replace(CNameMangling.SLICEINDEX.value, tmpList02.pop(0), 1)
-                    i+=1
-                    newSubItem = ""
-                    if re.search(r"^\s*\[.+\][\s,]*$", item) and item.count('[')==item.count(']'):
-                        item = item.strip()
-                        bLastElement = True
-                        if item.endswith(","):
-                            bLastElement = False
-                        item = re.sub(r"^\[", "", item)
-                        item = re.sub(r"\s*\][\s,]*$", "", item)
-                        newSubItem = __handleListElements(item)
-                        newSubItem = "[" + newSubItem + "]" if bLastElement else "[" + newSubItem + "],"
-                    elif re.search(r"^\s*\[.*\${.+", item):
-                        item = item.strip()
-                        item = re.sub(r"^\[", "", item)
-                        newSubItem = __handleListElements(item)
-                        newSubItem = "[" + newSubItem
-                    elif re.search(r"]\s*,*\s*", item) and item.count('[') < item.count(']') and \
-                        re.match(r"^.+[\]}\"]+\s*\],*\s*$", item):
-                        item = item.rstrip()
-                        bLastElement = True
-                        if item.endswith(","):
-                            bLastElement = False
-                        item = re.sub(r"\s*\][\s,]*$", "", item)
-                        newSubItem = __handleListElements(item)
-                        newSubItem = newSubItem + "]" if bLastElement else newSubItem + "],"
-                    elif re.match(r"^[\s\"]*\${.+[}\]]+[\"\s]*,[\s\"]*\${.+[}\]]+[\"\s]*$", item):
-                        subItems = re.split("\s*,\s*", item)
-                        subItem1 = self.__checkAndUpdateKeyValue(subItems[0], nestedKey)
-                        subItem2 = self.__checkAndUpdateKeyValue(subItems[1], nestedKey=True)
-                        newSubItem = subItem1 + ", " + subItem2
-                    else:
-                        newSubItem = self.__checkAndUpdateKeyValue(item, nestedKey)
-                    if i<len(items):
-                        newLine = newLine + newSubItem + " : "
+                    curItem = item
+                    if "${" in item:
+                        variablePattern = rf"[^{re.escape(self.specialCharacters)}]+"
+                        indexPattern = r"\[[\s\-\+\d]*\]|\[.*:.*\]"
+                        dictPattern = r"\[+\s*'.+'\s*\]+|\[+\s*\d+\s*\]+|\[+\s*\${\s*" + variablePattern + r"\s*}.*\]+|" + indexPattern
+                        nestedPattern = r"\${\s*" + variablePattern + r"(\.*\${\s*" + variablePattern + r"\s*})*" + r"\s*}(" + dictPattern + r")*"
+                        bHandle = False
+                        if '"' in item and item.count('"')%2==0:
+                            tmpList = re.findall(r'"[^"]+"', item)
+                            item = re.sub(r'"[^"]+"', CNameMangling.STRINGVALUE.value, item)
+                        if re.search(r'[\(\)\!@#%\^\&\/\\\=`~\?]+', item):
+                            item = re.sub(r'^\s*(.+)\s*,*', '"\\1"', item)
+                            bHandle = True
+                        if "," in item and not bHandle:
+                            if item.count(',')>1 and not re.match(r'^\[|{.+$', item.strip()):
+                                dReplacements = {"$":"\$", "[":"\[", "]":"\]", ".":"\.", "-":"\-", "+":"\+"}
+                                tmpPattern1 = self.__multipleReplace(preItem, dReplacements)
+                                tmpPattern2 = self.__multipleReplace(curItem, dReplacements)
+                                if re.search(tmpPattern1 + '\s*:\s*' + tmpPattern2, curLine):
+                                    item = re.sub(r'^\s*(.+)\s*', '"\\1"', item)
+                                    bHandle = True
+                            if not bHandle:
+                                subItems = item.split(',')
+                                iSubItems = len(subItems) -1 if subItems[-1]=='' else len(subItems)
+                                newSubItem = ""
+                                j=1
+                                for subItem in subItems:
+                                    if "${" in subItem:
+                                        if iSubItems>1 and j<iSubItems:
+                                            if re.match(r'^\${.+$', subItem.strip()):
+                                                subItem = '"' + subItem.strip() + '"'
+                                            else:
+                                                subItem = re.sub(r'(\${.+$)', '"\\1"', subItem.strip())
+                                        else:
+                                            subItem = __handleLastElement(subItem)   
+                                    if j < iSubItems:
+                                        newSubItem = newSubItem + subItem + ', '
+                                    else:
+                                        newSubItem = newSubItem + subItem + ',' if subItem=='' else newSubItem + subItem
+                                    j+=1
+                                item = newSubItem
+                        else:
+                            if "${" in item and not bHandle:
+                                item = __handleLastElement(item)
+                        while CNameMangling.STRINGVALUE.value in item:
+                            if "${" in tmpList[0]:
+                                sValue = tmpList.pop(0)
+                                sValue = re.sub(r'(' + nestedPattern + r')', '\\1' + CNameMangling.STRINGCONVERT.value, sValue)
+                                item = item.replace(CNameMangling.STRINGVALUE.value, sValue, 1)
+                            else:
+                                item = item.replace(CNameMangling.STRINGVALUE.value, tmpList.pop(0), 1)
+                    if i<iItems:
+                        newLine = newLine + item + " : "
                     else:
-                        newLine = newLine + newSubItem
+                        newLine = newLine + item + " :" if item=='' else newLine + item
+                    preItem = curItem
+                    i+=1
                 for nestedParam in self.lNestedParams:
                     dReplacements = {"$" : "\$", "[" : "\[", "]" : "\]"}
                     tmpNestedParam = self.__multipleReplace(nestedParam, dReplacements)
                     if re.search(r"(\s*\"str\(" + tmpNestedParam + "\)\"\s*:)", newLine.replace(CNameMangling.STRINGCONVERT.value, '')) \
                         or re.search(r"(\s*\"" + tmpNestedParam + r"\"\s*:)", newLine.replace(CNameMangling.STRINGCONVERT.value, '')):
                         self.lNestedParams.remove(nestedParam)
                 if re.search(r"\[\s*\+\s*\d+\s*\]", newLine):
                     newLine = re.sub(r"\[\s*\+\s*(\d+)\s*\]", "[\\1]", newLine)
-                if ":" in newLine:
-                    tmpValue = re.search(r"^.+:\s*([0-9a-zA-Z\${},\[\]\.\_\-\+;/\s]*),*\s*$", newLine) 
-                    if tmpValue is not None:
-                        tmpStr = tmpValue.group(1)
-                        if re.match(r"^[^\[{]+", tmpStr):
-                            tmpStr = tmpStr.strip()[:-1] if tmpStr.strip()[-1] == "," else tmpStr.strip()
-                            if "${" in tmpStr:
-                                dReplacements = {"$":"\$", "[":"\[", "]":"\]", ".":"\.", "-":"\-", "+":"\+"}
-                                tmpPattern = self.__multipleReplace(tmpStr, dReplacements)
-                                newLine = re.sub("(" + tmpPattern + ")", '"\\1"', newLine)
                 sJsonDataUpdated = sJsonDataUpdated + newLine + "\n"
             else:
                 sJsonDataUpdated = sJsonDataUpdated + line + "\n"
         lKeyName = re.findall(r'("[^:"]+")\s*:\s*', sJsonDataUpdated)
         for key in lKeyName:
             keyDecode = bytes(key, 'utf-8').decode('unicode_escape')
             self.__keyNameValidation(keyDecode)
@@ -1365,26 +1296,38 @@
             self.bDuplicatedKeys = False
             try:
                 self.jsonCheck = json.loads(sJsonDataUpdated,
                                 cls=CJSONDecoder,
                                 object_pairs_hook=self.__processImportFiles)
             except Exception as error:
                 self.__reset()
-                raise Exception(f"JSON file: {jFile}\n{error}")
+                failedJsonDoc = self.__getFailedJsonDoc(error)
+                jsonException = "not defined"
+                if failedJsonDoc is None:
+                    jsonException = f"{error}\nIn file: '{jFile}'"
+                else:
+                    jsonException = f"{error}\nNearby: '{failedJsonDoc}'\nIn file: '{jFile}'"
+                raise Exception(jsonException)
             self.bDuplicatedKeys = True
 
         # Load Json object with checking duplicated keys feature is enabled.
         # The duplicated keys feature uses the self.jsonCheck object to check duplicated keys. 
         try:
             oJson = json.loads(sJsonDataUpdated,
                                cls=CJSONDecoder,
                                object_pairs_hook=self.__processImportFiles)
         except Exception as error:
             self.__reset()
-            raise Exception(f"JSON file: {jFile}\n{error}")
+            failedJsonDoc = self.__getFailedJsonDoc(error)
+            jsonException = "not defined"
+            if failedJsonDoc is None:
+                jsonException = f"{error}\nIn file: '{jFile}'"
+            else:
+                jsonException = f"{error}\nNearby: '{failedJsonDoc}'\nIn file: '{jFile}'"
+            raise Exception(jsonException)
         self.__checkDotInParamName(oJson)
         __checkKeynameFormat(oJson)
 
         if masterFile:
             oJson = __handleDuplicatedKey(oJson)
             for k, v in oJson.items():
                 if re.match(r"^[0-9]+.*$", k) or re.match(r"^[\s\"]*\${.+}[\s\"]*$", k) \
```

### Comparing `JsonPreprocessor-0.4.0/JsonPreprocessor/JsonPreprocessor.pdf` & `JsonPreprocessor-0.5.0/JsonPreprocessor/JsonPreprocessor.pdf`

 * *Files 10% similar despite different names*

#### Comparing `JsonPreprocessor-0.4.0/JsonPreprocessor/JsonPreprocessor.pdf` & `JsonPreprocessor-0.5.0/JsonPreprocessor/JsonPreprocessor.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: ''
-CreationDate: 'D:20240409154513Z'
+CreationDate: 'D:20240411154550Z'
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: 'D:20240409154513Z'
+ModDate: 'D:20240411154550Z'
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.22 (TeX Live 2022/dev/Debian) kpathsea version 6.3.4/dev'
 Producer: 'pdfTeX-1.40.22'
 Subject: ''
 Title: ''
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 JsonPreprocessor
-v. 0.4.0
+v. 0.5.0
 Mai Dinh Nam Son
-15.03.2024
+10.04.2024
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -1363,19 +1363,19 @@
 
 Name
 
 JsonPreprocessor
 
 Version
 
-0.4.0
+0.5.0
 
 Date
 
-15.03.2024
+10.04.2024
 
 Description
 
 Preprocessor for json files
 
 Package URL
 
@@ -1478,15 +1478,25 @@
 
 - Optimized regular expression patterns
 - Improved duplicated parameters handling
 - Added mechanism to prevent Python application freeze
 - Removed globals scope out of all exec method executions
 - Optimized errors handling while loading nested parameters
 - Fixed bugs
+0.5.0
+
+04/2024
+
+Extended debugging support. In case of JSON syntax errors, the JsonPreprocessor exception contains an extract of the JSON content nearby the position,
+where the error occurred.
+
+28
+
+CHAPTER 6. HISTORY
 
 JsonPreprocessor.pdf
-Created at 09.04.2024 - 15:45:12
+Created at 11.04.2024 - 15:45:48
 by GenPackageDoc v. 0.41.1
 
-28
+29
```

### Comparing `JsonPreprocessor-0.4.0/JsonPreprocessor/__init__.py` & `JsonPreprocessor-0.5.0/JsonPreprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.4.0/JsonPreprocessor/version.py` & `JsonPreprocessor-0.5.0/JsonPreprocessor/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of JsonPreprocessor
 #
-VERSION      = "0.4.0"
-VERSION_DATE = "15.03.2024"
+VERSION      = "0.5.0"
+VERSION_DATE = "10.04.2024"
```

### Comparing `JsonPreprocessor-0.4.0/JsonPreprocessor.egg-info/PKG-INFO` & `JsonPreprocessor-0.5.0/JsonPreprocessor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonPreprocessor
-Version: 0.4.0
+Version: 0.5.0
 Summary: Preprocessor for json files
 Home-page: https://github.com/test-fullautomation/python-jsonpreprocessor
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JsonPreprocessor-0.4.0/LICENSE` & `JsonPreprocessor-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.4.0/PKG-INFO` & `JsonPreprocessor-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonPreprocessor
-Version: 0.4.0
+Version: 0.5.0
 Summary: Preprocessor for json files
 Home-page: https://github.com/test-fullautomation/python-jsonpreprocessor
 Author: Mai Dinh Nam Son
 Author-email: son.maidinhnam@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JsonPreprocessor-0.4.0/README.rst` & `JsonPreprocessor-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.4.0/setup.py` & `JsonPreprocessor-0.5.0/setup.py`

 * *Files identical despite different names*

