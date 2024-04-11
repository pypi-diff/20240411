# Comparing `tmp/pyside6_qml_stubgen-0.1.0a1.tar.gz` & `tmp/pyside6_qml_stubgen-0.1.0a2.tar.gz`

## Comparing `pyside6_qml_stubgen-0.1.0a1.tar` & `pyside6_qml_stubgen-0.1.0a2.tar`

### file list

```diff
@@ -1,34 +1,38 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/conftest.py
--rw-r--r--   0        0        0    22552 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/pyside6_qml_stubgen.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/requirements.txt
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/.github/workflows/test.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/__init__.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/test_run.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/README
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/qmldir
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/qmltyperegistrations1-0.cpp
--rw-r--r--   0        0        0    15713 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/types1-0.json
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/types1-0.qmltypes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/qmldir
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/qmltyperegistrations1-100.cpp
--rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/types1-100.json
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/types1-100.qmltypes
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/qmldir
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/types1-100.json
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/types1-100.qmltypes
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/qmldir
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/qmltyperegistrations2-1.cpp
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/types2-1.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/types2-1.qmltypes
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/target/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/target/advanced.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/target/advanced2.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/target/clses.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/target/clses2.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/tests/target/submodule.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/.gitignore
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/LICENCE.md
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/README.md
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/conftest.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/requirements.txt
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/.github/workflows/test.yml
+-rw-r--r--   0        0        0    14646 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/pyside6_qml_stubgen/__init__.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/pyside6_qml_stubgen/__main__.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/pyside6_qml_stubgen/dirty_file_detection.py
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/pyside6_qml_stubgen/pyside_patching.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/pyside6_qml_stubgen/qmlregistrar_types.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/__init__.py
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/test_run.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/README
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/qmldir
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/qmltyperegistrations1-0.cpp
+-rw-r--r--   0        0        0    15603 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/types1-0.json
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/types1-0.qmltypes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced/qmldir
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced/qmltyperegistrations1-100.cpp
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced/types1-100.json
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced/types1-100.qmltypes
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced2/qmldir
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced2/types1-100.json
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced2/types1-100.qmltypes
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/sub/qmldir
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/sub/qmltyperegistrations2-1.cpp
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/sub/types2-1.json
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/reference/target/sub/types2-1.qmltypes
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/target/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/target/advanced.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/target/advanced2.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/target/clses.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/target/clses2.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/tests/target/submodule.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/.gitignore
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/LICENCE.md
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/README.md
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a2/PKG-INFO
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/.github/workflows/test.yml` & `pyside6_qml_stubgen-0.1.0a2/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
           python -m pip install --upgrade pip
           pip install -r requirements.txt
       - name: Check formatting with black
         run: |
           black --check .
       - name: Type check with mypy
         run: |
-          mypy pyside6_qml_stubgen.py tests --exclude tests/target
+          mypy pyside6_qml_stubgen tests --exclude tests/target
       - name: Test with pytest
         run: |
           pytest
       - name: Build wheel
         if: matrix.os == 'ubuntu-latest'
         run: |
           python -m build
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/qmltyperegistrations1-0.cpp` & `pyside6_qml_stubgen-0.1.0a2/tests/reference/target/qmltyperegistrations1-0.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 **
 ** WARNING! All changes made in this file will be lost!
 *****************************************************************************/
 
 #include <QtQml/qqml.h>
 #include <QtQml/qqmlmoduleregistration.h>
 
-#include <tests/target/clses.py>
-#include <tests/target/clses2.py>
+#include <in/clses.py>
+#include <in/clses2.py>
 
 
 #if !defined(QT_STATIC)
 #define Q_QMLTYPE_EXPORT Q_DECL_EXPORT
 #else
 #define Q_QMLTYPE_EXPORT
 #endif
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/types1-0.json` & `pyside6_qml_stubgen-0.1.0a2/tests/reference/target/types1-0.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714287%*

 * *Differences: {'0': "{'inputFile': 'in/clses.py'}",*

 * * '1': "{'inputFile': 'in/clses.py'}",*

 * * '10': "{'inputFile': 'in/clses2.py'}",*

 * * '2': "{'inputFile': 'in/clses2.py'}",*

 * * '3': "{'inputFile': 'in/clses.py'}",*

 * * '4': "{'inputFile': 'in/clses.py'}",*

 * * '5': "{'inputFile': 'in/clses.py'}",*

 * * '6': "{'inputFile': 'in/clses2.py'}",*

 * * '7': "{'inputFile': 'in/clses2.py'}",*

 * * '8': "{'inputFile': 'in/clses.py'}",*

 * * '9': "{'inputFile': 'in/clses.py'}"}*

```diff
@@ -27,15 +27,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/clses.py",
+        "inputFile": "in/clses.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 0,
         "QT_MODULES": [
@@ -62,15 +62,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/clses.py",
+        "inputFile": "in/clses.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 0,
         "QT_MODULES": [
@@ -96,15 +96,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/clses2.py",
+        "inputFile": "in/clses2.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 0,
         "QT_MODULES": [
@@ -131,15 +131,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/clses.py",
+        "inputFile": "in/clses.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [
             "target 1.0"
         ],
         "QML_IMPORT_MAJOR_VERSION": 1,
@@ -249,15 +249,15 @@
                     {
                         "access": "public",
                         "name": "QStandardItemModel"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/clses.py",
+        "inputFile": "in/clses.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 0,
         "QT_MODULES": [
@@ -288,15 +288,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/clses.py",
+        "inputFile": "in/clses.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 0,
         "QT_MODULES": [
@@ -326,15 +326,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/clses2.py",
+        "inputFile": "in/clses2.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [
             "target 1.0"
         ],
         "QML_IMPORT_MAJOR_VERSION": 1,
@@ -395,15 +395,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/clses2.py",
+        "inputFile": "in/clses2.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 0,
         "QT_MODULES": [
@@ -434,15 +434,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/clses.py",
+        "inputFile": "in/clses.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 0,
         "QT_MODULES": [
@@ -477,15 +477,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/clses.py",
+        "inputFile": "in/clses.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 0,
         "QT_MODULES": [
@@ -519,11 +519,11 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/clses2.py",
+        "inputFile": "in/clses2.py",
         "outputRevision": 68
     }
 ]
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/types1-0.qmltypes` & `pyside6_qml_stubgen-0.1.0a2/tests/reference/target/types1-0.qmltypes`

 * *Files 10% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 // This file describes the plugin-supplied types contained in the library.
 // It is used for QML tooling purposes only.
 //
 // This file was auto-generated by qmltyperegistrar.
 
 Module {
     Component {
-        file: "tests/target/clses.py"
+        file: "in/clses.py"
         name: "Anonymous"
         accessSemantics: "reference"
         prototype: "QObject"
     }
     Component {
-        file: "tests/target/clses.py"
+        file: "in/clses.py"
         name: "Named"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target/NamedSomethingDifferent 1.0"]
         exportMetaObjectRevisions: [256]
     }
     Component {
-        file: "tests/target/clses2.py"
+        file: "in/clses2.py"
         name: "Named2"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target/NamedSomethingDifferent2 1.0"]
         exportMetaObjectRevisions: [256]
     }
     Component {
-        file: "tests/target/clses.py"
+        file: "in/clses.py"
         name: "Normal"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target/Normal 1.0"]
         exportMetaObjectRevisions: [256]
     }
     Component {
@@ -56,15 +56,15 @@
         Method {
             name: "_q_emitItemChanged"
             Parameter { name: "topLeft"; type: "QModelIndex" }
             Parameter { name: "bottomRight"; type: "QModelIndex" }
         }
     }
     Component {
-        file: "tests/target/clses.py"
+        file: "in/clses.py"
         name: "SignalsAndProperties"
         accessSemantics: "reference"
         prototype: "QStandardItemModel"
         exports: ["target/SignalsAndProperties 1.0"]
         exportMetaObjectRevisions: [256]
         Enum {
             name: "Flags"
@@ -99,35 +99,35 @@
             Parameter { name: "x"; type: "int" }
             Parameter { name: "y"; type: "QString" }
             Parameter { name: "z"; type: "Normal"; isPointer: true }
         }
         Method { name: "slot2"; type: "Uncreatable"; isPointer: true }
     }
     Component {
-        file: "tests/target/clses.py"
+        file: "in/clses.py"
         name: "Singleton"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target/Singleton 1.0"]
         isCreatable: false
         isSingleton: true
         exportMetaObjectRevisions: [256]
     }
     Component {
-        file: "tests/target/clses2.py"
+        file: "in/clses2.py"
         name: "Singleton2"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target/Singleton2 1.0"]
         isCreatable: false
         isSingleton: true
         exportMetaObjectRevisions: [256]
     }
     Component {
-        file: "tests/target/clses2.py"
+        file: "in/clses2.py"
         name: "Singleton3"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target/Singleton3 1.0"]
         isCreatable: false
         isSingleton: true
         exportMetaObjectRevisions: [256]
@@ -144,33 +144,33 @@
             name: "normChanged"
             Parameter { type: "Named2"; isPointer: true }
             Parameter { type: "int" }
             Parameter { type: "bool" }
         }
     }
     Component {
-        file: "tests/target/clses.py"
+        file: "in/clses.py"
         name: "Uncreatable"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target/Uncreatable 1.0"]
         isCreatable: false
         exportMetaObjectRevisions: [256]
     }
     Component {
-        file: "tests/target/clses.py"
+        file: "in/clses.py"
         name: "UncreatableWithReason"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target/UncreatableWithReason 1.0"]
         isCreatable: false
         exportMetaObjectRevisions: [256]
     }
     Component {
-        file: "tests/target/clses2.py"
+        file: "in/clses2.py"
         name: "UncreatableWithReason2"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target/UncreatableWithReason2 1.0"]
         isCreatable: false
         exportMetaObjectRevisions: [256]
     }
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/qmltyperegistrations1-100.cpp` & `pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced/qmltyperegistrations1-100.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 **
 ** WARNING! All changes made in this file will be lost!
 *****************************************************************************/
 
 #include <QtQml/qqml.h>
 #include <QtQml/qqmlmoduleregistration.h>
 
-#include <tests/target/advanced.py>
+#include <in/advanced.py>
 
 
 #if !defined(QT_STATIC)
 #define Q_QMLTYPE_EXPORT Q_DECL_EXPORT
 #else
 #define Q_QMLTYPE_EXPORT
 #endif
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/types1-100.json` & `pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced/types1-100.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {'0': "{'inputFile': 'in/advanced.py'}",*

 * * '1': "{'inputFile': 'in/advanced.py'}",*

 * * '2': "{'inputFile': 'in/advanced.py'}",*

 * * '3': "{'inputFile': 'in/advanced.py'}",*

 * * '4': "{'inputFile': 'in/advanced.py'}"}*

```diff
@@ -30,15 +30,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/advanced.py",
+        "inputFile": "in/advanced.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 100,
         "QT_MODULES": [
@@ -71,15 +71,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/advanced.py",
+        "inputFile": "in/advanced.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 100,
         "QT_MODULES": [
@@ -100,15 +100,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/advanced.py",
+        "inputFile": "in/advanced.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 100,
         "QT_MODULES": [
@@ -129,15 +129,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/advanced.py",
+        "inputFile": "in/advanced.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 100,
         "QT_MODULES": [
@@ -171,11 +171,11 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/advanced.py",
+        "inputFile": "in/advanced.py",
         "outputRevision": 68
     }
 ]
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced/types1-100.qmltypes` & `pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced/types1-100.qmltypes`

 * *Files 22% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 // This file describes the plugin-supplied types contained in the library.
 // It is used for QML tooling purposes only.
 //
 // This file was auto-generated by qmltyperegistrar.
 
 Module {
     Component {
-        file: "tests/target/advanced.py"
+        file: "in/advanced.py"
         name: "Layout"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target.advanced/Layout 1.0"]
         exportMetaObjectRevisions: [256]
         attachedType: "LayoutAttached"
     }
     Component {
-        file: "tests/target/advanced.py"
+        file: "in/advanced.py"
         name: "LayoutAttached"
         accessSemantics: "reference"
         prototype: "QObject"
         Property { name: "margins"; type: "QMargins"; read: "margins"; index: 1; isReadonly: true }
     }
     Component {
-        file: "tests/target/advanced.py"
+        file: "in/advanced.py"
         name: "LineEditorExtension"
         accessSemantics: "reference"
         prototype: "QObject"
     }
     Component {
-        file: "tests/target/advanced.py"
+        file: "in/advanced.py"
         name: "LineEditor"
         accessSemantics: "reference"
         prototype: "QObject"
         extension: "LineEditorExtension"
         exports: ["target.advanced/LineEditor 1.0"]
         exportMetaObjectRevisions: [256]
     }
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp` & `pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 **
 ** WARNING! All changes made in this file will be lost!
 *****************************************************************************/
 
 #include <QtQml/qqml.h>
 #include <QtQml/qqmlmoduleregistration.h>
 
-#include <tests/target/advanced2.py>
+#include <in/advanced2.py>
 
 
 #if !defined(QT_STATIC)
 #define Q_QMLTYPE_EXPORT Q_DECL_EXPORT
 #else
 #define Q_QMLTYPE_EXPORT
 #endif
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/types1-100.json` & `pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced2/types1-100.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {'0': "{'inputFile': 'in/advanced2.py'}",*

 * * '1': "{'inputFile': 'in/advanced2.py'}",*

 * * '2': "{'inputFile': 'in/advanced2.py'}",*

 * * '3': "{'inputFile': 'in/advanced2.py'}",*

 * * '4': "{'inputFile': 'in/advanced2.py'}"}*

```diff
@@ -30,15 +30,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/advanced2.py",
+        "inputFile": "in/advanced2.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 100,
         "QT_MODULES": [
@@ -71,15 +71,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/advanced2.py",
+        "inputFile": "in/advanced2.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 100,
         "QT_MODULES": [
@@ -100,15 +100,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/advanced2.py",
+        "inputFile": "in/advanced2.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 100,
         "QT_MODULES": [
@@ -129,15 +129,15 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/advanced2.py",
+        "inputFile": "in/advanced2.py",
         "outputRevision": 68
     },
     {
         "PY_MODULES": [],
         "QML_IMPORT_MAJOR_VERSION": 1,
         "QML_IMPORT_MINOR_VERSION": 100,
         "QT_MODULES": [
@@ -171,11 +171,11 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/advanced2.py",
+        "inputFile": "in/advanced2.py",
         "outputRevision": 68
     }
 ]
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/advanced2/types1-100.qmltypes` & `pyside6_qml_stubgen-0.1.0a2/tests/reference/target/advanced2/types1-100.qmltypes`

 * *Files 11% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 // This file describes the plugin-supplied types contained in the library.
 // It is used for QML tooling purposes only.
 //
 // This file was auto-generated by qmltyperegistrar.
 
 Module {
     Component {
-        file: "tests/target/advanced2.py"
+        file: "in/advanced2.py"
         name: "Layout2"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target.advanced2/Layout2 1.0"]
         exportMetaObjectRevisions: [256]
         attachedType: "LayoutAttached2"
     }
     Component {
-        file: "tests/target/advanced2.py"
+        file: "in/advanced2.py"
         name: "LayoutAttached2"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target.advanced2/LayoutAttached2 1.0"]
         exportMetaObjectRevisions: [256]
         Property { name: "margins"; type: "QMargins"; read: "margins"; index: 1; isReadonly: true }
     }
     Component {
-        file: "tests/target/advanced2.py"
+        file: "in/advanced2.py"
         name: "LineEditorExtension2"
         accessSemantics: "reference"
         prototype: "QObject"
     }
     Component {
-        file: "tests/target/advanced2.py"
+        file: "in/advanced2.py"
         name: "LineEditor2"
         accessSemantics: "reference"
         prototype: "QObject"
         extension: "LineEditorExtension2"
         exports: ["target.advanced2/LineEditor2 1.0"]
         exportMetaObjectRevisions: [256]
     }
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/qmltyperegistrations2-1.cpp` & `pyside6_qml_stubgen-0.1.0a2/tests/reference/target/sub/qmltyperegistrations2-1.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 **
 ** WARNING! All changes made in this file will be lost!
 *****************************************************************************/
 
 #include <QtQml/qqml.h>
 #include <QtQml/qqmlmoduleregistration.h>
 
-#include <tests/target/submodule.py>
+#include <in/submodule.py>
 
 
 #if !defined(QT_STATIC)
 #define Q_QMLTYPE_EXPORT Q_DECL_EXPORT
 #else
 #define Q_QMLTYPE_EXPORT
 #endif
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/types2-1.json` & `pyside6_qml_stubgen-0.1.0a2/tests/reference/target/sub/types2-1.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {'0': "{'inputFile': 'in/submodule.py'}"}*

```diff
@@ -35,11 +35,11 @@
                     {
                         "access": "public",
                         "name": "QObject"
                     }
                 ]
             }
         ],
-        "inputFile": "tests/target/submodule.py",
+        "inputFile": "in/submodule.py",
         "outputRevision": 68
     }
 ]
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/reference/target/sub/types2-1.qmltypes` & `pyside6_qml_stubgen-0.1.0a2/tests/reference/target/sub/types2-1.qmltypes`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 // This file describes the plugin-supplied types contained in the library.
 // It is used for QML tooling purposes only.
 //
 // This file was auto-generated by qmltyperegistrar.
 
 Module {
     Component {
-        file: "tests/target/submodule.py"
+        file: "in/submodule.py"
         name: "Obj"
         accessSemantics: "reference"
         prototype: "QObject"
         exports: ["target.sub/Obj 2.0"]
         exportMetaObjectRevisions: [512]
         Property {
             name: "anon"
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/target/advanced.py` & `pyside6_qml_stubgen-0.1.0a2/tests/target/advanced.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/target/advanced2.py` & `pyside6_qml_stubgen-0.1.0a2/tests/target/advanced2.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/target/clses.py` & `pyside6_qml_stubgen-0.1.0a2/tests/target/clses.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a1/tests/target/clses2.py` & `pyside6_qml_stubgen-0.1.0a2/tests/target/clses2.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a1/LICENCE.md` & `pyside6_qml_stubgen-0.1.0a2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a1/README.md` & `pyside6_qml_stubgen-0.1.0a2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,14 @@
 ----------------------
 
 ```bash
 $ pyside6-qml-stubgen --help
 Generate QML stub files (.qmltypes) from Python modules (which use PySide6)
 
 Usage:
-    pyside6-qml-stubgen <in-dir> --out-dir=<out-dir> [--ignore=<path>...] [--metatypes-dir=<dir>] [--qmltyperegistrar-path=<path>]
+    pyside6-qml-stubgen <in-dir>... --out-dir=<out-dir> [--ignore=<path>...] [--metatypes-dir=<dir>] [--qmltyperegistrar-path=<path>]
 
 Options:
     --ignore=<path>                     Ignore all Python files that are children of thispath
     --metatypes-dir=<dir>               Directory of the Qt 6 metatype files for core modules (automatically detected if not provided)
     --qmltyperegistrar-path=<path>      Path of the qmltyperegistrar tool (automatically detected if not provided)
 ```
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/pyproject.toml` & `pyside6_qml_stubgen-0.1.0a2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 [project]
 name = "pyside6-qml-stubgen"
 description = "Generate QML stub files (.qmltypes) from Python modules (which use PySide6)"
-authors = [
-    {name = "Matthew Joyce"},
-]
+authors = [{ name = "Matthew Joyce" }]
 readme = "README.md"
-dependencies = [
-    "PySide6>=6.4",
-    "docopt"
-]
+dependencies = ["PySide6 >= 6.4", "docopt", "pydantic >= 2"]
 requires-python = ">= 3.10"
 keywords = ["qml", "type checking", "pyside6", "qt6"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: X11 Applications :: Qt",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
@@ -27,25 +22,31 @@
 
 [project.urls]
 Homepage = "https://github.com/matsjoyce/pyside6-qml-stubgen"
 Repository = "https://github.com/matsjoyce/pyside6-qml-stubgen.git"
 Issues = "https://github.com/matsjoyce/pyside6-qml-stubgen/issues"
 
 [project.scripts]
-pyside6-qml-stubgen = "pyside6_qml_stubgen:main"
+pyside6-qml-stubgen = "pyside6_qml_stubgen.__main__:main"
 
 [project.optional-dependencies]
-dev = [
-    "pytest",
-    "mypy",
-    "black",
-    "types-docopt",
-    "build",
-    "pytest-cov"
-]
+dev = ["pytest", "mypy", "black", "types-docopt", "build", "pytest-cov"]
 
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
 source = "vcs"
+
+[tool.mypy]
+python_version = "3.10"
+warn_unused_configs = true
+show_error_codes = true
+follow_imports = "silent"
+disallow_untyped_defs = true
+disallow_incomplete_defs = true
+warn_redundant_casts = true
+warn_unused_ignores = true
+warn_unreachable = true
+strict_equality = true
+local_partial_types = true
```

### Comparing `pyside6_qml_stubgen-0.1.0a1/PKG-INFO` & `pyside6_qml_stubgen-0.1.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyside6-qml-stubgen
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Generate QML stub files (.qmltypes) from Python modules (which use PySide6)
 Project-URL: Homepage, https://github.com/matsjoyce/pyside6-qml-stubgen
 Project-URL: Repository, https://github.com/matsjoyce/pyside6-qml-stubgen.git
 Project-URL: Issues, https://github.com/matsjoyce/pyside6-qml-stubgen/issues
 Author: Matthew Joyce
 License-File: LICENCE.md
 Keywords: pyside6,qml,qt6,type checking
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.10
 Requires-Dist: docopt
+Requires-Dist: pydantic>=2
 Requires-Dist: pyside6>=6.4
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
@@ -81,14 +82,14 @@
 ----------------------
 
 ```bash
 $ pyside6-qml-stubgen --help
 Generate QML stub files (.qmltypes) from Python modules (which use PySide6)
 
 Usage:
-    pyside6-qml-stubgen <in-dir> --out-dir=<out-dir> [--ignore=<path>...] [--metatypes-dir=<dir>] [--qmltyperegistrar-path=<path>]
+    pyside6-qml-stubgen <in-dir>... --out-dir=<out-dir> [--ignore=<path>...] [--metatypes-dir=<dir>] [--qmltyperegistrar-path=<path>]
 
 Options:
     --ignore=<path>                     Ignore all Python files that are children of thispath
     --metatypes-dir=<dir>               Directory of the Qt 6 metatype files for core modules (automatically detected if not provided)
     --qmltyperegistrar-path=<path>      Path of the qmltyperegistrar tool (automatically detected if not provided)
 ```
```

