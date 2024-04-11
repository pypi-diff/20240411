# Comparing `tmp/d3vis_ipynb-0.1.0.tar.gz` & `tmp/d3vis_ipynb-0.1.1.tar.gz`

## Comparing `d3vis_ipynb-0.1.0.tar` & `d3vis_ipynb-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/D3vis_ipynb.json
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/RELEASE.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/install.json
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/setup.cfg
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/setup.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/_version.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/embedding.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/web.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/widgets.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/package.json
--rw-r--r--   0        0        0    22687 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/static/380.ee013a9b91711778a778.js
--rw-r--r--   0        0        0    23295 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/static/493.d829e8f3d475b29a72ba.js
--rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/static/remoteEntry.c14fe8243d2c28e7d82d.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/static/style.js
--rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    88462 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/d3vis_ipynb/nbextension/index.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/amd-public-path.js
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/package.json
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/webpack.config.js
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/webpack.exports.config.js
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/css/widget.css
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/lib/extension.js
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/lib/index.js
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/lib/labplugin.js
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/lib/web-dev.js
--rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/lib/widgets.js
--rw-r--r--   0        0        0     9326 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/lib/graphs/barplot.js
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/lib/graphs/histogramplot.js
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/lib/graphs/linearhistplot.js
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/lib/graphs/scatterplot.js
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/lib/tools/lasso.js
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/js/lib/wrappers/embedding.wrapper.js
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/.gitignore
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/README.md
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/D3vis_ipynb.json
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/MANIFEST.in
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/RELEASE.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/install.json
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/setup.cfg
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/setup.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/_version.py
+-rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/embedding.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/web.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/widgets.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/package.json
+-rw-r--r--   0        0        0    22687 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/380.bce32fc1670ea497a572.js
+-rw-r--r--   0        0        0    23295 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/493.e98395b66f4058ecc2a8.js
+-rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/remoteEntry.7e42e6f84b582762349a.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/style.js
+-rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    88462 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/nbextension/index.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/amd-public-path.js
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/package.json
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/webpack.config.js
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/webpack.exports.config.js
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/css/widget.css
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/extension.js
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/index.js
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/labplugin.js
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/web-dev.js
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/widgets.js
+-rw-r--r--   0        0        0     9326 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/graphs/barplot.js
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/graphs/histogramplot.js
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/graphs/linearhistplot.js
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/graphs/scatterplot.js
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/tools/lasso.js
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/wrappers/embedding.wrapper.js
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/README.md
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/PKG-INFO
```

### Comparing `d3vis_ipynb-0.1.0/RELEASE.md` & `d3vis_ipynb-0.1.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/setup.cfg` & `d3vis_ipynb-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/d3vis_ipynb/__init__.py` & `d3vis_ipynb-0.1.1/d3vis_ipynb/__init__.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/d3vis_ipynb/embedding.py` & `d3vis_ipynb-0.1.1/d3vis_ipynb/embedding.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/d3vis_ipynb/web.py` & `d3vis_ipynb-0.1.1/d3vis_ipynb/web.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/d3vis_ipynb/widgets.py` & `d3vis_ipynb-0.1.1/d3vis_ipynb/widgets.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/package.json` & `d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9603365384615384%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.7e42e6f84b582762349a.js'}}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -16,15 +16,15 @@
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c14fe8243d2c28e7d82d.js"
+            "load": "static/remoteEntry.7e42e6f84b582762349a.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../d3vis_ipynb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -54,9 +54,9 @@
         "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/static/380.ee013a9b91711778a778.js` & `d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/380.bce32fc1670ea497a572.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -724,11 +724,11 @@
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
         330: e => {
-            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.0","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.1","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/static/493.d829e8f3d475b29a72ba.js` & `d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/493.e98395b66f4058ecc2a8.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -755,11 +755,11 @@
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
         330: e => {
-            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.0","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.1","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js` & `d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/static/remoteEntry.c14fe8243d2c28e7d82d.js` & `d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/remoteEntry.7e42e6f84b582762349a.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, d, u, s, l, f, c, p, h, v, b, g, m, y, w = {
+    var e, r, t, n, a, o, i, d, u, s, l, f, p, c, h, v, b, g, m, y, w = {
             772: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(380).then((() => () => t(380))),
                         "./extension": () => Promise.all([t.e(56), t.e(493)]).then((() => () => t(493)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    o = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                o = t.S[n];
-                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                a = t.S[n];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => o,
-                    init: () => a
+                    get: () => a,
+                    init: () => o
                 })
             }
         },
         S = {};
 
     function E(e) {
         var r = S[e];
@@ -43,48 +43,48 @@
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
         56: "2d1dea0ba8f2782da6dd",
-        380: "ee013a9b91711778a778",
-        493: "d829e8f3d475b29a72ba",
+        380: "bce32fc1670ea497a572",
+        493: "e98395b66f4058ecc2a8",
         693: "c8409ce8329f6703470f"
     } [e] + ".js?v=" + {
         56: "2d1dea0ba8f2782da6dd",
-        380: "ee013a9b91711778a778",
-        493: "d829e8f3d475b29a72ba",
+        380: "bce32fc1670ea497a572",
+        493: "e98395b66f4058ecc2a8",
         693: "c8409ce8329f6703470f"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "d3vis_ipynb:", E.l = (t, n, o, a) => {
+    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "d3vis_ipynb:", E.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, d;
-            if (void 0 !== o)
+            if (void 0 !== a)
                 for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
                     var l = u[s];
-                    if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + o) {
+                    if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + a) {
                         i = l;
                         break
                     }
                 }
-            i || (d = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (d = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
-                    var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
+                    i.onerror = i.onload = null, clearTimeout(p);
+                    var a = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), d && document.head.appendChild(i)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -94,31 +94,31 @@
         })
     }, (() => {
         E.S = {};
         var e = {},
             r = {};
         E.I = (t, n) => {
             n || (n = []);
-            var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
+                if (n.push(a), e[t]) return e[t];
                 E.o(E.S, t) || (E.S[t] = {});
-                var a = E.S[t],
+                var o = E.S[t],
                     i = "d3vis_ipynb",
                     d = (e, r, t, n) => {
-                        var o = a[e] = a[e] || {},
-                            d = o[r];
-                        (!d || !d.loaded && (!n != !d.eager ? n : i > d.from)) && (o[r] = {
+                        var a = o[e] = o[e] || {},
+                            d = a[r];
+                        (!d || !d.loaded && (!n != !d.eager ? n : i > d.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (d("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), d("d3vis_ipynb", "0.1.0", (() => E.e(380).then((() => () => E(380)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), d("d3vis_ipynb", "0.1.1", (() => E.e(380).then((() => () => E(380)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -133,98 +133,98 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
+            var a = e[n],
+                o = (typeof a)[0];
+            if (n >= r.length) return "u" == o;
             var i = r[n],
                 d = (typeof i)[0];
-            if (a != d) return "o" == a && "n" == d || "s" == d || "u" == a;
-            if ("o" != a && "u" != a && o != i) return o < i;
+            if (o != d) return "o" == o && "n" == d || "s" == d || "u" == o;
+            if ("o" != o && "u" != o && a != i) return a < i;
             n++
         }
-    }, o = e => {
+    }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(d = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, d);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(d = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, d);
             return t
         }
         var i = [];
-        for (a = 1; a < e.length; a++) {
-            var d = e[a];
-            i.push(0 === d ? "not(" + u() + ")" : 1 === d ? "(" + u() + " || " + u() + ")" : 2 === d ? i.pop() + " " + i.pop() : o(d))
+        for (o = 1; o < e.length; o++) {
+            var d = e[o];
+            i.push(0 === d ? "not(" + u() + ")" : 1 === d ? "(" + u() + " || " + u() + ")" : 2 === d ? i.pop() + " " + i.pop() : a(d))
         }
         return u();
 
         function u() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                o = n < 0;
-            o && (n = -n - 1);
+                a = n < 0;
+            a && (n = -n - 1);
             for (var i = 0, d = 1, u = !0;; d++, i++) {
                 var s, l, f = d < e.length ? (typeof e[d])[0] : "";
-                if (i >= r.length || "o" == (l = (typeof(s = r[i]))[0])) return !u || ("u" == f ? d > n && !o : "" == f != o);
+                if (i >= r.length || "o" == (l = (typeof(s = r[i]))[0])) return !u || ("u" == f ? d > n && !a : "" == f != a);
                 if ("u" == l) {
                     if (!u || "u" != f) return !1
                 } else if (u)
                     if (f == l)
                         if (d <= n) {
                             if (s != e[d]) return !1
                         } else {
-                            if (o ? s > e[d] : s < e[d]) return !1;
+                            if (a ? s > e[d] : s < e[d]) return !1;
                             s != e[d] && (u = !1)
                         }
                 else if ("s" != f && "n" != f) {
-                    if (o || d <= n) return !1;
+                    if (a || d <= n) return !1;
                     u = !1, d--
                 } else {
-                    if (d <= n || l < f != o) return !1;
+                    if (d <= n || l < f != a) return !1;
                     u = !1
                 } else "s" != f && "n" != f && (u = !1, d--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
-        var o = d(e, t);
-        return a(n, o) || f(u(e, t, o, n)), c(e[t][o])
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
+        var a = d(e, t);
+        return o(n, a) || f(u(e, t, a, n)), p(e[t][a])
     }, l = (e, r, t) => {
-        var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
+        var a = e[r];
+        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
-        var a = E.I(r);
-        return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
-        var a = r && E.o(r, t) && l(r, t, n);
-        return a ? c(a) : o()
+    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, a) {
+        var o = E.I(r);
+        return o && o.then ? o.then(e.bind(e, r, E.S[r], t, n, a)) : e(r, E.S[r], t, n, a)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = c(((e, r, t, n, a) => {
+        var o = r && E.o(r, t) && l(r, t, n);
+        return o ? p(o) : a()
     })), b = {}, g = {
         801: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1
         ]),
@@ -244,51 +244,51 @@
                 y[e] = !0;
                 var n = r => {
                     delete b[e], E.m[e] = t => {
                         throw delete E.c[e], r
                     }
                 };
                 try {
-                    var o = g[e]();
-                    o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
+                    var a = g[e]();
+                    a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         var e = {
             71: 0
         };
         E.f.j = (r, t) => {
             var n = E.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (56 != r) {
-                var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                t.push(n[2] = o);
-                var a = E.p + E.u(r),
+                var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                t.push(n[2] = a);
+                var o = E.p + E.u(r),
                     i = new Error;
-                E.l(a, (t => {
+                E.l(o, (t => {
                     if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var o = t && ("load" === t.type ? "missing" : t.type),
-                            a = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                        var a = t && ("load" === t.type ? "missing" : t.type),
+                            o = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, o, [a, i, d] = t,
+                var n, a, [o, i, d] = t,
                     u = 0;
-                if (a.some((r => 0 !== e[r]))) {
+                if (o.some((r => 0 !== e[r]))) {
                     for (n in i) E.o(i, n) && (E.m[n] = i[n]);
                     d && d(E)
                 }
-                for (r && r(t); u < a.length; u++) o = a[u], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); u < o.length; u++) a = o[u], E.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunkd3vis_ipynb = self.webpackChunkd3vis_ipynb || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
     var P = E(772);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).d3vis_ipynb = P
 })();
```

### Comparing `d3vis_ipynb-0.1.0/d3vis_ipynb/labextension/static/third-party-licenses.json` & `d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/d3vis_ipynb/nbextension/index.js` & `d3vis_ipynb-0.1.1/d3vis_ipynb/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -179,15 +179,15 @@
             55: t => {
                 t.exports = e
             },
             308: e => {
                 e.exports = t
             },
             330: t => {
-                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.0","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.1","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         r = {};
 
     function i(t) {
         var e = r[t];
         if (void 0 !== e) return e.exports;
```

### Comparing `d3vis_ipynb-0.1.0/js/amd-public-path.js` & `d3vis_ipynb-0.1.1/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/js/package.json` & `d3vis_ipynb-0.1.1/js/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -50,9 +50,9 @@
         "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `d3vis_ipynb-0.1.0/js/webpack.config.js` & `d3vis_ipynb-0.1.1/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/js/webpack.exports.config.js` & `d3vis_ipynb-0.1.1/js/webpack.exports.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/js/css/widget.css` & `d3vis_ipynb-0.1.1/js/css/widget.css`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/js/lib/labplugin.js` & `d3vis_ipynb-0.1.1/js/lib/labplugin.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/js/lib/web-dev.js` & `d3vis_ipynb-0.1.1/js/lib/web-dev.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/js/lib/widgets.js` & `d3vis_ipynb-0.1.1/js/lib/widgets.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/js/lib/graphs/barplot.js` & `d3vis_ipynb-0.1.1/js/lib/graphs/barplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/js/lib/graphs/histogramplot.js` & `d3vis_ipynb-0.1.1/js/lib/graphs/histogramplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/js/lib/graphs/linearhistplot.js` & `d3vis_ipynb-0.1.1/js/lib/graphs/linearhistplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/js/lib/graphs/scatterplot.js` & `d3vis_ipynb-0.1.1/js/lib/graphs/scatterplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/js/lib/tools/lasso.js` & `d3vis_ipynb-0.1.1/js/lib/tools/lasso.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/js/lib/wrappers/embedding.wrapper.js` & `d3vis_ipynb-0.1.1/js/lib/wrappers/embedding.wrapper.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/LICENSE.txt` & `d3vis_ipynb-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.0/README.md` & `d3vis_ipynb-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 A Custom Jupyter Widget Library with visualizations created with D3.js.
 
 ## Installation
 
 To install use pip:
 
-    $ pip install d3vis_ipynb
+    $ pip install d3vis-ipynb
 
 For a development installation (requires [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/)),
 
     $ git clone https://github.com/H-IAAC/d3vis_ipynb.git
     $ cd d3vis_ipynb
     $ pip install -e .
     $ jupyter nbextension install --py --symlink --overwrite --sys-prefix d3vis_ipynb
```

### Comparing `d3vis_ipynb-0.1.0/pyproject.toml` & `d3vis_ipynb-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "ipywidgets>=7.7.1",
     "simplejson >=3.19.0",
     "anywidget >= 0.9.6"
 ]
-version = "0.1.0"
+version = "0.1.1"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
```

### Comparing `d3vis_ipynb-0.1.0/PKG-INFO` & `d3vis_ipynb-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: d3vis_ipynb
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Custom Jupyter Widget Library with visualizations created with D3.js.
 Project-URL: Homepage, https://github.com/H-IAAC/d3vis_ipynb
 Author-email: Daniel Adam Miranda <daniel.miranda@eldorado.org.br>
 License: Copyright (c) 2024 Daniel Adam Miranda
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -69,15 +69,15 @@
 
 A Custom Jupyter Widget Library with visualizations created with D3.js.
 
 ## Installation
 
 To install use pip:
 
-    $ pip install d3vis_ipynb
+    $ pip install d3vis-ipynb
 
 For a development installation (requires [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/)),
 
     $ git clone https://github.com/H-IAAC/d3vis_ipynb.git
     $ cd d3vis_ipynb
     $ pip install -e .
     $ jupyter nbextension install --py --symlink --overwrite --sys-prefix d3vis_ipynb
```

