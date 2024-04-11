# Comparing `tmp/TEflow-0.2.7.tar.gz` & `tmp/TEflow-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/NewFolder/mySoftWare/OneDrive/GitHub/TEflow/dist/tmpw1pz2usp/TEflow-0.2.7.tar", last modified: Sun Mar 10 14:44:29 2024, max compression
+gzip compressed data, was "TEflow-0.2.8.tar", last modified: Thu Apr 11 12:07:21 2024, max compression
```

## Comparing `TEflow-0.2.7.tar` & `TEflow-0.2.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0 joule01   (1000) joule01   (1000)        0 2024-03-10 14:44:29.000000 TEflow-0.2.7/
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)    11541 2023-09-21 09:19:59.000000 TEflow-0.2.7/LICENSE
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)     2304 2024-03-10 14:44:29.000000 TEflow-0.2.7/PKG-INFO
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)       80 2023-12-08 07:53:28.000000 TEflow-0.2.7/pyproject.toml
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)     1661 2024-02-16 07:21:15.000000 TEflow-0.2.7/README.md
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)     1212 2024-03-10 14:44:29.000000 TEflow-0.2.7/setup.cfg
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)       38 2023-12-08 07:53:28.000000 TEflow-0.2.7/setup.py
-drwxrwxrwx   0 joule01   (1000) joule01   (1000)        0 2024-03-10 14:44:28.000000 TEflow-0.2.7/src/
-drwxrwxrwx   0 joule01   (1000) joule01   (1000)        0 2024-03-10 14:44:29.000000 TEflow-0.2.7/src/teflow/
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)    52590 2024-03-10 14:43:34.000000 TEflow-0.2.7/src/teflow/bandlib.py
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)    20259 2024-02-16 07:21:15.000000 TEflow-0.2.7/src/teflow/engout.py
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)    42496 2024-03-10 14:43:34.000000 TEflow-0.2.7/src/teflow/interface.py
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)    56109 2024-02-28 13:38:28.000000 TEflow-0.2.7/src/teflow/kappa.py
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)    25954 2024-02-28 13:38:28.000000 TEflow-0.2.7/src/teflow/loader.py
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)    15053 2024-02-28 13:38:28.000000 TEflow-0.2.7/src/teflow/mathext.py
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)    20555 2024-03-07 18:10:57.000000 TEflow-0.2.7/src/teflow/utils.py
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)     6840 2024-02-16 07:21:15.000000 TEflow-0.2.7/src/teflow/ztdev.py
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)      622 2024-03-10 14:43:34.000000 TEflow-0.2.7/src/teflow/_version.py
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)      634 2024-02-16 07:21:15.000000 TEflow-0.2.7/src/teflow/__init__.py
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)      675 2024-02-16 07:21:15.000000 TEflow-0.2.7/src/teflow/__main__.py
-drwxrwxrwx   0 joule01   (1000) joule01   (1000)        0 2024-03-10 14:44:28.000000 TEflow-0.2.7/src/TEflow.egg-info/
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)        1 2024-03-10 14:44:28.000000 TEflow-0.2.7/src/TEflow.egg-info/dependency_links.txt
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)      402 2024-03-10 14:44:28.000000 TEflow-0.2.7/src/TEflow.egg-info/entry_points.txt
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)     2304 2024-03-10 14:44:28.000000 TEflow-0.2.7/src/TEflow.egg-info/PKG-INFO
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)       12 2024-03-10 14:44:28.000000 TEflow-0.2.7/src/TEflow.egg-info/requires.txt
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)      562 2024-03-10 14:44:28.000000 TEflow-0.2.7/src/TEflow.egg-info/SOURCES.txt
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)        7 2024-03-10 14:44:28.000000 TEflow-0.2.7/src/TEflow.egg-info/top_level.txt
-drwxrwxrwx   0 joule01   (1000) joule01   (1000)        0 2024-03-10 14:44:29.000000 TEflow-0.2.7/tests/
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)      737 2024-02-28 13:38:28.000000 TEflow-0.2.7/tests/test_Compound.py
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)     1115 2024-02-25 12:38:37.000000 TEflow-0.2.7/tests/test_TEdata.py
--rwxrwxrwx   0 joule01   (1000) joule01   (1000)     1078 2024-02-16 07:21:15.000000 TEflow-0.2.7/tests/test_vinterp.py
+drwxrwxrwx   0 joule02   (1000) joule02   (1000)        0 2024-04-11 12:07:21.659048 TEflow-0.2.8/
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)    11541 2023-09-21 09:19:59.000000 TEflow-0.2.8/LICENSE
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)     2326 2024-04-11 12:07:21.657054 TEflow-0.2.8/PKG-INFO
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)     1661 2024-02-16 07:21:15.000000 TEflow-0.2.8/README.md
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)       80 2023-12-08 07:53:28.000000 TEflow-0.2.8/pyproject.toml
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)     1212 2024-04-11 12:07:21.662056 TEflow-0.2.8/setup.cfg
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)       38 2023-12-08 07:53:28.000000 TEflow-0.2.8/setup.py
+drwxrwxrwx   0 joule02   (1000) joule02   (1000)        0 2024-04-11 12:07:21.396783 TEflow-0.2.8/src/
+drwxrwxrwx   0 joule02   (1000) joule02   (1000)        0 2024-04-11 12:07:21.652054 TEflow-0.2.8/src/TEflow.egg-info/
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)     2326 2024-04-11 12:07:21.000000 TEflow-0.2.8/src/TEflow.egg-info/PKG-INFO
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)      562 2024-04-11 12:07:21.000000 TEflow-0.2.8/src/TEflow.egg-info/SOURCES.txt
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)        1 2024-04-11 12:07:21.000000 TEflow-0.2.8/src/TEflow.egg-info/dependency_links.txt
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)      401 2024-04-11 12:07:21.000000 TEflow-0.2.8/src/TEflow.egg-info/entry_points.txt
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)       12 2024-04-11 12:07:21.000000 TEflow-0.2.8/src/TEflow.egg-info/requires.txt
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)        7 2024-04-11 12:07:21.000000 TEflow-0.2.8/src/TEflow.egg-info/top_level.txt
+drwxrwxrwx   0 joule02   (1000) joule02   (1000)        0 2024-04-11 12:07:21.614511 TEflow-0.2.8/src/teflow/
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)      634 2024-02-16 07:21:15.000000 TEflow-0.2.8/src/teflow/__init__.py
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)      675 2024-02-16 07:21:15.000000 TEflow-0.2.8/src/teflow/__main__.py
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)      622 2024-04-11 12:00:01.000000 TEflow-0.2.8/src/teflow/_version.py
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)    52590 2024-04-11 11:58:58.000000 TEflow-0.2.8/src/teflow/bandlib.py
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)    20293 2024-04-11 12:00:01.000000 TEflow-0.2.8/src/teflow/engout.py
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)    42414 2024-04-11 12:04:22.000000 TEflow-0.2.8/src/teflow/interface.py
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)    56109 2024-02-28 13:38:28.000000 TEflow-0.2.8/src/teflow/kappa.py
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)    25954 2024-02-28 13:38:28.000000 TEflow-0.2.8/src/teflow/loader.py
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)    15053 2024-04-11 11:58:58.000000 TEflow-0.2.8/src/teflow/mathext.py
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)    20555 2024-04-11 11:58:58.000000 TEflow-0.2.8/src/teflow/utils.py
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)     6840 2024-02-16 07:21:15.000000 TEflow-0.2.8/src/teflow/ztdev.py
+drwxrwxrwx   0 joule02   (1000) joule02   (1000)        0 2024-04-11 12:07:21.639052 TEflow-0.2.8/tests/
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)      737 2024-02-28 13:38:28.000000 TEflow-0.2.8/tests/test_Compound.py
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)     1115 2024-02-25 12:38:37.000000 TEflow-0.2.8/tests/test_TEdata.py
+-rwxrwxrwx   0 joule02   (1000) joule02   (1000)     1078 2024-04-11 11:58:58.000000 TEflow-0.2.8/tests/test_vinterp.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `TEflow-0.2.7/LICENSE` & `TEflow-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/PKG-INFO` & `TEflow-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: TEflow
-Version: 0.2.7
+Version: 0.2.8
 Summary: A python3 package for thermoelectric output performance calculations
 Home-page: https://github.com/JianboHIT/TEflow
 Author: Jianbo ZHU
 License: Apache-2.0 license
 Keywords: thermoelectricity,simulation
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 # TEflow (under-developed)
 A python3 package for streamlining thermoelectric workflow from materials to devices
 
 ## Features
 - Model carrier transport
   - Single parabolic band (SPB) model
@@ -43,9 +44,7 @@
 #### References
 
 [^1]: Kim, H. S., Liu, W., Chen, G., Chu, C. W., & Ren, Z. (2015). Relationship between thermoelectric figure of merit and energy conversion efficiency. 
 _Proceedings of the National Academy of Sciences_, 112(27), 8205-8210. DOI: [10.1073/pnas.1510231112](https://doi.org/10.1073/pnas.1510231112)
 
 [^2]: Snyder, G. J., & Snyder, A. H. (2017). Figure of merit ZT of a thermoelectric device defined from materials properties. 
 _Energy & Environmental Science_, 10(11), 2280-2283. DOI: [10.1039/C7EE02007D](https://doi.org/10.1039/C7EE02007D)
-
-
```

### Comparing `TEflow-0.2.7/README.md` & `TEflow-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/setup.cfg` & `TEflow-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/src/teflow/bandlib.py` & `TEflow-0.2.8/src/teflow/bandlib.py`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/src/teflow/engout.py` & `TEflow-0.2.8/src/teflow/engout.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
         Convenient entry to evaluate thermoelectric leg of generator
         '''
         
         T = datas_TCSK[0]
         Tc, Th = T[0], T[1:]
         
         # initialling
-        rst = AttrDict(Tc=Tc, Th=Th)
+        rst = AttrDict(Tc=Tc*np.ones_like(Th), Th=Th)
         logger.debug('Invoke valuate() method of %s', cls.__name__)
         gen = cls(TEdatas=datas_TCSK, Tc=Tc, Th=Th, L=L)
         
         # build device
         prfs = gen.build()
         rst['deltaT'] = prfs.deltaT
         rst['PFeng']  = prfs.PFeng
@@ -503,15 +503,15 @@
         Convenient entry to evaluate thermoelectric p-n pair of generator
         '''
         
         T = datas_p_TCSK[0]
         Tc, Th = T[0], T[1:]
         
         # initialling
-        rst = AttrDict(Tc=Tc, Th=Th)
+        rst = AttrDict(Tc=Tc*np.ones_like(Th), Th=Th)
         logger.debug('Invoke valuate() method of %s', cls.__name__)
         gen = cls(TEdatas_p=datas_p_TCSK, 
                   TEdatas_n=datas_n_TCSK,
                   Tc=Tc, Th=Th, L=L)
         
         # to maximize Yita
         logger.info('>>> To get maximal Yita <<<')
```

### Comparing `TEflow-0.2.7/src/teflow/interface.py` & `TEflow-0.2.8/src/teflow/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,17 +273,17 @@
                 x2 = np.arange(start, stop, step)
                 logger.debug(f'Using np.arange({start}, {stop}, {step})')
             else:
                 logger.debug(f'Current value of range option: {options.range}')
                 raise ValueError('Failed to parse --range option: '
                                  "'START:STEP:END' format is required.")
         else:
-            npoint = options.npoint
-            x2 = np.linspace(x[0], x[-1], num=npoint)
-            logger.debug(f'Using np.linspace({x[0]}, {x[-1]}, num={npoint}) ')
+            npoints = options.npoints
+            x2 = np.linspace(x[0], x[-1], num=npoints)
+            logger.debug(f'Using np.linspace({x[0]}, {x[-1]}, num={npoints}) ')
         
         logger.info('Generate sampling points automatically')
     else:
         logger.info(f'Read sampling points from {outputfile}')
 
     # check method
     _METHODS = {'linear', 'line', 'cubic', 'pchip', 'Akima',
@@ -568,16 +568,14 @@
         else:
             datas_p, datas_n = datas[:4, :], datas[[0, 4, 5, 6], :]
         out = GenPair.valuate(datas_p, datas_n, L=length)
     else:
         out = GenLeg.valuate(datas, L=length)
 
     # deal with results
-    out['Tc'] = 300 * np.ones_like(out['deltaT'])
-    out['Th'] = 300 + out['deltaT']
     props = 'Tc     Th       PFeng  ZTeng  Pout   Yita'
     outdata = np.vstack([out[p] for p in props.split()]).T
 
     # output
     info = f'Engineering performance (L={length}mm, A=100mm^2)'\
            f' - {TIME} {INFO}\n{props}'
     comment = '' if options.bare else info
```

### Comparing `TEflow-0.2.7/src/teflow/kappa.py` & `TEflow-0.2.8/src/teflow/kappa.py`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/src/teflow/loader.py` & `TEflow-0.2.8/src/teflow/loader.py`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/src/teflow/mathext.py` & `TEflow-0.2.8/src/teflow/mathext.py`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/src/teflow/utils.py` & `TEflow-0.2.8/src/teflow/utils.py`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/src/teflow/ztdev.py` & `TEflow-0.2.8/src/teflow/ztdev.py`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/src/teflow/_version.py` & `TEflow-0.2.8/src/teflow/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
-__version__ = '0.2.7'
+__version__ = '0.2.8'
```

### Comparing `TEflow-0.2.7/src/teflow/__init__.py` & `TEflow-0.2.8/src/teflow/__init__.py`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/src/teflow/__main__.py` & `TEflow-0.2.8/src/teflow/__main__.py`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/src/TEflow.egg-info/PKG-INFO` & `TEflow-0.2.8/src/TEflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: TEflow
-Version: 0.2.7
+Version: 0.2.8
 Summary: A python3 package for thermoelectric output performance calculations
 Home-page: https://github.com/JianboHIT/TEflow
 Author: Jianbo ZHU
 License: Apache-2.0 license
 Keywords: thermoelectricity,simulation
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 # TEflow (under-developed)
 A python3 package for streamlining thermoelectric workflow from materials to devices
 
 ## Features
 - Model carrier transport
   - Single parabolic band (SPB) model
@@ -43,9 +44,7 @@
 #### References
 
 [^1]: Kim, H. S., Liu, W., Chen, G., Chu, C. W., & Ren, Z. (2015). Relationship between thermoelectric figure of merit and energy conversion efficiency. 
 _Proceedings of the National Academy of Sciences_, 112(27), 8205-8210. DOI: [10.1073/pnas.1510231112](https://doi.org/10.1073/pnas.1510231112)
 
 [^2]: Snyder, G. J., & Snyder, A. H. (2017). Figure of merit ZT of a thermoelectric device defined from materials properties. 
 _Energy & Environmental Science_, 10(11), 2280-2283. DOI: [10.1039/C7EE02007D](https://doi.org/10.1039/C7EE02007D)
-
-
```

### Comparing `TEflow-0.2.7/src/TEflow.egg-info/SOURCES.txt` & `TEflow-0.2.8/src/TEflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/tests/test_Compound.py` & `TEflow-0.2.8/tests/test_Compound.py`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/tests/test_TEdata.py` & `TEflow-0.2.8/tests/test_TEdata.py`

 * *Files identical despite different names*

### Comparing `TEflow-0.2.7/tests/test_vinterp.py` & `TEflow-0.2.8/tests/test_vinterp.py`

 * *Files identical despite different names*

