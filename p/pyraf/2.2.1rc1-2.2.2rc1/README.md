# Comparing `tmp/pyraf-2.2.1rc1.tar.gz` & `tmp/pyraf-2.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyraf-2.2.1rc1.tar", last modified: Mon Mar 21 09:01:34 2022, max compression
+gzip compressed data, was "pyraf-2.2.2rc1.tar", last modified: Thu Apr 11 08:36:34 2024, max compression
```

## Comparing `pyraf-2.2.1rc1.tar` & `pyraf-2.2.2rc1.tar`

### file list

```diff
@@ -1,160 +1,161 @@
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.156629 pyraf-2.2.1rc1/
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.144629 pyraf-2.2.1rc1/.github/
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.148629 pyraf-2.2.1rc1/.github/workflows/
--rw-r--r--   0 oles      (1000) oles      (1000)     3194 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/.github/workflows/citest.yml
--rw-r--r--   0 oles      (1000) oles      (1000)      497 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/.gitignore
--rw-r--r--   0 oles      (1000) oles      (1000)      172 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/.readthedocs.yaml
--rw-r--r--   0 oles      (1000) oles      (1000)     2837 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 oles      (1000) oles      (1000)     1464 2022-02-01 08:33:37.000000 pyraf-2.2.1rc1/LICENSE.txt
--rw-r--r--   0 oles      (1000) oles      (1000)      215 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/MANIFEST.in
--rw-r--r--   0 oles      (1000) oles      (1000)     4151 2022-03-21 09:01:34.156629 pyraf-2.2.1rc1/PKG-INFO
--rw-r--r--   0 oles      (1000) oles      (1000)     3231 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/README.rst
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.148629 pyraf-2.2.1rc1/docs/
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.148629 pyraf-2.2.1rc1/docs/_static/
--rw-r--r--   0 oles      (1000) oles      (1000)      158 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/docs/_static/brand.css
--rw-r--r--   0 oles      (1000) oles      (1000)     6262 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/docs/_static/pyraflogo.png
--rw-r--r--   0 oles      (1000) oles      (1000)      651 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/docs/conf.py
--rw-r--r--   0 oles      (1000) oles      (1000)    14379 2022-02-01 08:33:37.000000 pyraf-2.2.1rc1/docs/ecl.html
--rw-r--r--   0 oles      (1000) oles      (1000)    58798 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/docs/epar.png
--rw-r--r--   0 oles      (1000) oles      (1000)    42582 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/docs/index.rst
--rw-r--r--   0 oles      (1000) oles      (1000)     3084 2022-02-01 08:33:37.000000 pyraf-2.2.1rc1/docs/ipython_notes.txt
--rw-r--r--   0 oles      (1000) oles      (1000)    22972 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/docs/prow.png
--rw-r--r--   0 oles      (1000) oles      (1000)    42582 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/docs/pyraf_tutorial.rst
--rw-r--r--   0 oles      (1000) oles      (1000)    23530 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/docs/teal_guide.rst
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.152629 pyraf-2.2.1rc1/pyraf/
--rw-r--r--   0 oles      (1000) oles      (1000)    30277 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/GkiMpl.py
--rw-r--r--   0 oles      (1000) oles      (1000)     9077 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/MplCanvasAdapter.py
--rw-r--r--   0 oles      (1000) oles      (1000)    10536 2022-03-18 15:45:27.000000 pyraf-2.2.1rc1/pyraf/Ptkplot.py
--rw-r--r--   0 oles      (1000) oles      (1000)     2241 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/__init__.py
--rw-r--r--   0 oles      (1000) oles      (1000)     5660 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/__main__.py
--rw-r--r--   0 oles      (1000) oles      (1000)     9142 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/aqutil.py
--rw-r--r--   0 oles      (1000) oles      (1000)      362 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/blankcursor.xbm
--rw-r--r--   0 oles      (1000) oles      (1000)     1995 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/cgeneric.py
--rw-r--r--   0 oles      (1000) oles      (1000)    85635 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/cl2py.py
--rw-r--r--   0 oles      (1000) oles      (1000)     2235 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/clast.py
--rw-r--r--   0 oles      (1000) oles      (1000)     6763 2022-03-16 07:42:12.000000 pyraf-2.2.1rc1/pyraf/clcache.py
--rw-r--r--   0 oles      (1000) oles      (1000)     3415 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/cllinecache.py
--rw-r--r--   0 oles      (1000) oles      (1000)    17000 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/clparse.py
--rw-r--r--   0 oles      (1000) oles      (1000)    34205 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/clscan.py
--rw-r--r--   0 oles      (1000) oles      (1000)     6818 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/cltoken.py
--rw-r--r--   0 oles      (1000) oles      (1000)      295 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/epar.optionDB
--rw-r--r--   0 oles      (1000) oles      (1000)    14550 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/epar.py
--rw-r--r--   0 oles      (1000) oles      (1000)     5774 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/filecache.py
--rw-r--r--   0 oles      (1000) oles      (1000)      620 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/fill_clcache.py
--rw-r--r--   0 oles      (1000) oles      (1000)    14727 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/fontdata.py
--rw-r--r--   0 oles      (1000) oles      (1000)    21933 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/generic.py
--rw-r--r--   0 oles      (1000) oles      (1000)    50976 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/gki.py
--rw-r--r--   0 oles      (1000) oles      (1000)     2594 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/gkicmd.py
--rw-r--r--   0 oles      (1000) oles      (1000)     9241 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/gkigcur.py
--rw-r--r--   0 oles      (1000) oles      (1000)     3820 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/gkiiraf.py
--rw-r--r--   0 oles      (1000) oles      (1000)    34788 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/gkitkbase.py
--rw-r--r--   0 oles      (1000) oles      (1000)    14583 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/gkitkplot.py
--rw-r--r--   0 oles      (1000) oles      (1000)     4122 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/graphcap.py
--rw-r--r--   0 oles      (1000) oles      (1000)     7922 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/gwm.py
--rw-r--r--   0 oles      (1000) oles      (1000)    16197 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/ipython_api.py
--rw-r--r--   0 oles      (1000) oles      (1000)      968 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/ipythonrc-pyraf
--rw-r--r--   0 oles      (1000) oles      (1000)      400 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/iraf.py
--rw-r--r--   0 oles      (1000) oles      (1000)    13911 2022-03-18 07:27:17.000000 pyraf-2.2.1rc1/pyraf/irafcompleter.py
--rw-r--r--   0 oles      (1000) oles      (1000)    10193 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/irafdisplay.py
--rw-r--r--   0 oles      (1000) oles      (1000)    16012 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/irafecl.py
--rw-r--r--   0 oles      (1000) oles      (1000)    40099 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/irafexecute.py
--rw-r--r--   0 oles      (1000) oles      (1000)   120866 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/iraffunctions.py
--rw-r--r--   0 oles      (1000) oles      (1000)    13651 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/irafgwcs.py
--rw-r--r--   0 oles      (1000) oles      (1000)    14802 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/irafhelp.py
--rw-r--r--   0 oles      (1000) oles      (1000)     2858 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/irafimcur.py
--rw-r--r--   0 oles      (1000) oles      (1000)     6099 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/irafimport.py
--rw-r--r--   0 oles      (1000) oles      (1000)     1396 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/irafinst.py
--rw-r--r--   0 oles      (1000) oles      (1000)     1971 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/irafnames.py
--rw-r--r--   0 oles      (1000) oles      (1000)    59646 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/irafpar.py
--rw-r--r--   0 oles      (1000) oles      (1000)    76010 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/iraftask.py
--rw-r--r--   0 oles      (1000) oles      (1000)     2514 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/irafukey.py
--rw-r--r--   0 oles      (1000) oles      (1000)     8164 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/msgiobuffer.py
--rw-r--r--   0 oles      (1000) oles      (1000)     9125 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/msgiowidget.py
--rw-r--r--   0 oles      (1000) oles      (1000)     3731 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/newWindowHack.py
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.152629 pyraf-2.2.1rc1/pyraf/noiraf/
--rw-r--r--   0 oles      (1000) oles      (1000)     1716 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/noiraf/cl.par
--rw-r--r--   0 oles      (1000) oles      (1000)      210 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/noiraf/clpackage.cl
--rw-r--r--   0 oles      (1000) oles      (1000)      848 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/noiraf/login.cl
--rw-r--r--   0 oles      (1000) oles      (1000)     1038 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/noiraf/system.cl
--rw-r--r--   0 oles      (1000) oles      (1000)      117 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/noiraf/system.par
--rw-r--r--   0 oles      (1000) oles      (1000)     1341 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/pseteparoption.py
--rw-r--r--   0 oles      (1000) oles      (1000)    19042 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/pycmdline.py
--rw-r--r--   0 oles      (1000) oles      (1000)      958 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/pyrafTk.py
--rw-r--r--   0 oles      (1000) oles      (1000)     1071 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/pyrafglobals.py
--rw-r--r--   0 oles      (1000) oles      (1000)     6791 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/pyraflogo_rgb_web.gif
--rw-r--r--   0 oles      (1000) oles      (1000)     7888 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/splash.py
--rw-r--r--   0 oles      (1000) oles      (1000)     6131 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/sqliteshelve.py
--rw-r--r--   0 oles      (1000) oles      (1000)    12917 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/sscanfmodule.c
--rw-r--r--   0 oles      (1000) oles      (1000)    33325 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/subproc.py
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.152629 pyraf-2.2.1rc1/pyraf/tests/
--rw-r--r--   0 oles      (1000) oles      (1000)        0 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/tests/__init__.py
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.152629 pyraf-2.2.1rc1/pyraf/tests/data/
--rw-r--r--   0 oles      (1000) oles      (1000)    23267 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/tests/data/psdump_prow_250.ps
--rw-r--r--   0 oles      (1000) oles      (1000)    25541 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/tests/data/psdump_prow_256.ps
--rw-r--r--   0 oles      (1000) oles      (1000)    29147 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/tests/data/psdump_prow_256_250.ps
--rw-r--r--   0 oles      (1000) oles      (1000)    32746 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/tests/data/psdump_prow_256_250_200.ps
--rw-r--r--   0 oles      (1000) oles      (1000)   132480 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/tests/data/pset_msstat_input.fits
--rw-r--r--   0 oles      (1000) oles      (1000)    18499 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/tests/data/psi_land_prow_250.ps
--rw-r--r--   0 oles      (1000) oles      (1000)    18758 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/tests/data/psi_land_prow_256.ps
--rw-r--r--   0 oles      (1000) oles      (1000)    22450 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/tests/data/psi_land_prow_256_250.ps
--rw-r--r--   0 oles      (1000) oles      (1000)    26135 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/tests/data/psi_land_prow_256_250_200.ps
--rw-r--r--   0 oles      (1000) oles      (1000)     2060 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/tests/test_basic.py
--rw-r--r--   0 oles      (1000) oles      (1000)     1144 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/tests/test_clcache.py
--rw-r--r--   0 oles      (1000) oles      (1000)    12528 2022-03-18 14:34:54.000000 pyraf-2.2.1rc1/pyraf/tests/test_cli.py
--rw-r--r--   0 oles      (1000) oles      (1000)     8027 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tests/test_core_nongraphics.py
--rw-r--r--   0 oles      (1000) oles      (1000)    12357 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tests/test_graphics.py
--rw-r--r--   0 oles      (1000) oles      (1000)     4906 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tests/test_invocation.py
--rw-r--r--   0 oles      (1000) oles      (1000)     2184 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tests/test_plot.py
--rw-r--r--   0 oles      (1000) oles      (1000)     1673 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tests/test_tasks.py
--rw-r--r--   0 oles      (1000) oles      (1000)    11065 2022-03-21 08:13:11.000000 pyraf-2.2.1rc1/pyraf/tests/test_using_tasks.py
--rw-r--r--   0 oles      (1000) oles      (1000)      537 2022-02-18 14:23:37.000000 pyraf-2.2.1rc1/pyraf/tests/utils.py
--rw-r--r--   0 oles      (1000) oles      (1000)     3086 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/textattrib.py
--rw-r--r--   0 oles      (1000) oles      (1000)     6048 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/tkplottext.py
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.152629 pyraf-2.2.1rc1/pyraf/tools/
--rw-r--r--   0 oles      (1000) oles      (1000)        0 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/__init__.py
--rw-r--r--   0 oles      (1000) oles      (1000)     3219 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/alert.py
--rw-r--r--   0 oles      (1000) oles      (1000)    60413 2022-03-18 07:25:44.000000 pyraf-2.2.1rc1/pyraf/tools/basicpar.py
--rw-r--r--   0 oles      (1000) oles      (1000)     6821 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/capable.py
--rw-r--r--   0 oles      (1000) oles      (1000)    60399 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/cfgpars.py
--rw-r--r--   0 oles      (1000) oles      (1000)     2345 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/compmixin.py
--rw-r--r--   0 oles      (1000) oles      (1000)     1906 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/dialog.py
--rw-r--r--   0 oles      (1000) oles      (1000)    70629 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/editpar.py
--rw-r--r--   0 oles      (1000) oles      (1000)    37396 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/eparoption.py
--rw-r--r--   0 oles      (1000) oles      (1000)    15745 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/filedlg.py
--rw-r--r--   0 oles      (1000) oles      (1000)    14054 2022-03-18 07:25:44.000000 pyraf-2.2.1rc1/pyraf/tools/irafglobals.py
--rw-r--r--   0 oles      (1000) oles      (1000)    19301 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/irafutils.py
--rw-r--r--   0 oles      (1000) oles      (1000)     3494 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/listdlg.py
--rw-r--r--   0 oles      (1000) oles      (1000)     8465 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/minmatch.py
--rw-r--r--   0 oles      (1000) oles      (1000)     2643 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/taskpars.py
--rw-r--r--   0 oles      (1000) oles      (1000)    51260 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/teal.py
--rw-r--r--   0 oles      (1000) oles      (1000)     2793 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/teal_bttn.py
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.156629 pyraf-2.2.1rc1/pyraf/tools/tests/
--rw-r--r--   0 oles      (1000) oles      (1000)        0 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/tests/__init__.py
--rw-r--r--   0 oles      (1000) oles      (1000)    14030 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/tests/cfgobj_output.ref
--rw-r--r--   0 oles      (1000) oles      (1000)     4254 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/tests/rt_sample.cfg
--rw-r--r--   0 oles      (1000) oles      (1000)     7252 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/tests/rt_sample.cfgspc
--rw-r--r--   0 oles      (1000) oles      (1000)     1765 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/tests/test_cfgobj.py
--rw-r--r--   0 oles      (1000) oles      (1000)     4279 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/tests/test_compmixin.py
--rw-r--r--   0 oles      (1000) oles      (1000)      974 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/tests/test_irafutils.py
--rw-r--r--   0 oles      (1000) oles      (1000)     1980 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/tests/test_minmatch.py
--rw-r--r--   0 oles      (1000) oles      (1000)     2371 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/tkrotext.py
--rw-r--r--   0 oles      (1000) oles      (1000)     5566 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/tools/vtor_checks.py
--rw-r--r--   0 oles      (1000) oles      (1000)    45984 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/tpar.py
--rw-r--r--   0 oles      (1000) oles      (1000)    10255 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/urwfiledlg.py
--rwxr-xr-x   0 oles      (1000) oles      (1000)     9233 2022-03-10 07:33:57.000000 pyraf-2.2.1rc1/pyraf/urwutil.py
--rw-r--r--   0 oles      (1000) oles      (1000)      145 2022-03-21 09:01:34.000000 pyraf-2.2.1rc1/pyraf/version.py
--rw-r--r--   0 oles      (1000) oles      (1000)    22438 2022-03-15 10:57:45.000000 pyraf-2.2.1rc1/pyraf/wutil.py
--rw-r--r--   0 oles      (1000) oles      (1000)    12804 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/pyraf/xutil.c
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.152629 pyraf-2.2.1rc1/pyraf.egg-info/
--rw-r--r--   0 oles      (1000) oles      (1000)     4151 2022-03-21 09:01:34.000000 pyraf-2.2.1rc1/pyraf.egg-info/PKG-INFO
--rw-r--r--   0 oles      (1000) oles      (1000)     3290 2022-03-21 09:01:34.000000 pyraf-2.2.1rc1/pyraf.egg-info/SOURCES.txt
--rw-r--r--   0 oles      (1000) oles      (1000)        1 2022-03-21 09:01:34.000000 pyraf-2.2.1rc1/pyraf.egg-info/dependency_links.txt
--rw-r--r--   0 oles      (1000) oles      (1000)       38 2022-03-21 09:01:34.000000 pyraf-2.2.1rc1/pyraf.egg-info/entry_points.txt
--rw-r--r--   0 oles      (1000) oles      (1000)        1 2022-03-21 09:01:34.000000 pyraf-2.2.1rc1/pyraf.egg-info/not-zip-safe
--rw-r--r--   0 oles      (1000) oles      (1000)       84 2022-03-21 09:01:34.000000 pyraf-2.2.1rc1/pyraf.egg-info/requires.txt
--rw-r--r--   0 oles      (1000) oles      (1000)       48 2022-03-21 09:01:34.000000 pyraf-2.2.1rc1/pyraf.egg-info/top_level.txt
--rw-r--r--   0 oles      (1000) oles      (1000)     1549 2022-03-21 09:01:34.156629 pyraf-2.2.1rc1/setup.cfg
--rwxr-xr-x   0 oles      (1000) oles      (1000)      662 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/setup.py
-drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2022-03-21 09:01:34.156629 pyraf-2.2.1rc1/tools/
--rw-r--r--   0 oles      (1000) oles      (1000)     6770 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/tools/compileallcl.py
--rw-r--r--   0 oles      (1000) oles      (1000)     1748 2022-02-16 07:10:36.000000 pyraf-2.2.1rc1/tools/loadall.py
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.465686 pyraf-2.2.2rc1/
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.449687 pyraf-2.2.2rc1/.github/
+-rw-r--r--   0 oles      (1000) oles      (1000)      529 2024-04-11 08:10:46.000000 pyraf-2.2.2rc1/.github/dependabot.yml
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.449687 pyraf-2.2.2rc1/.github/workflows/
+-rw-r--r--   0 oles      (1000) oles      (1000)     3188 2024-04-11 08:10:46.000000 pyraf-2.2.2rc1/.github/workflows/citest.yml
+-rw-r--r--   0 oles      (1000) oles      (1000)      497 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/.gitignore
+-rw-r--r--   0 oles      (1000) oles      (1000)      216 2024-02-12 07:35:26.000000 pyraf-2.2.2rc1/.readthedocs.yaml
+-rw-r--r--   0 oles      (1000) oles      (1000)     2837 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 oles      (1000) oles      (1000)     1464 2022-02-01 08:33:37.000000 pyraf-2.2.2rc1/LICENSE.txt
+-rw-r--r--   0 oles      (1000) oles      (1000)      215 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/MANIFEST.in
+-rw-r--r--   0 oles      (1000) oles      (1000)     4191 2024-04-11 08:36:34.465686 pyraf-2.2.2rc1/PKG-INFO
+-rw-r--r--   0 oles      (1000) oles      (1000)     3231 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/README.rst
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.453687 pyraf-2.2.2rc1/docs/
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.453687 pyraf-2.2.2rc1/docs/_static/
+-rw-r--r--   0 oles      (1000) oles      (1000)      158 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/docs/_static/brand.css
+-rw-r--r--   0 oles      (1000) oles      (1000)     6262 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/docs/_static/pyraflogo.png
+-rw-r--r--   0 oles      (1000) oles      (1000)      651 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/docs/conf.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    14379 2022-02-01 08:33:37.000000 pyraf-2.2.2rc1/docs/ecl.html
+-rw-r--r--   0 oles      (1000) oles      (1000)    58798 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/docs/epar.png
+-rw-r--r--   0 oles      (1000) oles      (1000)    42582 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/docs/index.rst
+-rw-r--r--   0 oles      (1000) oles      (1000)     3084 2022-02-01 08:33:37.000000 pyraf-2.2.2rc1/docs/ipython_notes.txt
+-rw-r--r--   0 oles      (1000) oles      (1000)    22972 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/docs/prow.png
+-rw-r--r--   0 oles      (1000) oles      (1000)    42582 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/docs/pyraf_tutorial.rst
+-rw-r--r--   0 oles      (1000) oles      (1000)    23530 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/docs/teal_guide.rst
+-rw-r--r--   0 oles      (1000) oles      (1000)     1229 2024-04-11 08:10:46.000000 pyraf-2.2.2rc1/pyproject.toml
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.457687 pyraf-2.2.2rc1/pyraf/
+-rw-r--r--   0 oles      (1000) oles      (1000)    30277 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/GkiMpl.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     9205 2024-02-12 07:35:26.000000 pyraf-2.2.2rc1/pyraf/MplCanvasAdapter.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    10536 2022-03-18 15:45:27.000000 pyraf-2.2.2rc1/pyraf/Ptkplot.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     2241 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/__init__.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     5660 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/__main__.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     6940 2024-04-11 08:10:46.000000 pyraf-2.2.2rc1/pyraf/aqutil.py
+-rw-r--r--   0 oles      (1000) oles      (1000)      362 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/blankcursor.xbm
+-rw-r--r--   0 oles      (1000) oles      (1000)     1995 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/cgeneric.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    85635 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/cl2py.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     2235 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/clast.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     6809 2024-02-12 07:35:26.000000 pyraf-2.2.2rc1/pyraf/clcache.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     3415 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/cllinecache.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    17000 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/clparse.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    34205 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/clscan.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     6818 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/cltoken.py
+-rw-r--r--   0 oles      (1000) oles      (1000)      295 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/epar.optionDB
+-rw-r--r--   0 oles      (1000) oles      (1000)    14550 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/epar.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     5774 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/filecache.py
+-rw-r--r--   0 oles      (1000) oles      (1000)      620 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/fill_clcache.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    14727 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/fontdata.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    21933 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/generic.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    50976 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/gki.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     2594 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/gkicmd.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     9241 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/gkigcur.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     3820 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/gkiiraf.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    34788 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/gkitkbase.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    14583 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/gkitkplot.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     4122 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/graphcap.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     7922 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/gwm.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    16197 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/ipython_api.py
+-rw-r--r--   0 oles      (1000) oles      (1000)      968 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/ipythonrc-pyraf
+-rw-r--r--   0 oles      (1000) oles      (1000)      400 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/iraf.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    13911 2022-03-18 07:27:17.000000 pyraf-2.2.2rc1/pyraf/irafcompleter.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    10193 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/irafdisplay.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    16012 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/irafecl.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    40099 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/irafexecute.py
+-rw-r--r--   0 oles      (1000) oles      (1000)   120689 2024-04-11 08:10:46.000000 pyraf-2.2.2rc1/pyraf/iraffunctions.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    13651 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/irafgwcs.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    14802 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/irafhelp.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     2858 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/irafimcur.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     6099 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/irafimport.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     1396 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/irafinst.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     1971 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/irafnames.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    59646 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/irafpar.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    76010 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/iraftask.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     2514 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/irafukey.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     8164 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/msgiobuffer.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     9125 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/msgiowidget.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     3731 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/newWindowHack.py
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.457687 pyraf-2.2.2rc1/pyraf/noiraf/
+-rw-r--r--   0 oles      (1000) oles      (1000)     1716 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/noiraf/cl.par
+-rw-r--r--   0 oles      (1000) oles      (1000)      210 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/noiraf/clpackage.cl
+-rw-r--r--   0 oles      (1000) oles      (1000)      848 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/noiraf/login.cl
+-rw-r--r--   0 oles      (1000) oles      (1000)     1038 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/noiraf/system.cl
+-rw-r--r--   0 oles      (1000) oles      (1000)      117 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/noiraf/system.par
+-rw-r--r--   0 oles      (1000) oles      (1000)     1341 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/pseteparoption.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    19042 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/pycmdline.py
+-rw-r--r--   0 oles      (1000) oles      (1000)      958 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/pyrafTk.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     1071 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/pyrafglobals.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     6791 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/pyraflogo_rgb_web.gif
+-rw-r--r--   0 oles      (1000) oles      (1000)     5709 2024-04-11 08:10:46.000000 pyraf-2.2.2rc1/pyraf/scanf.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     7888 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/splash.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     6205 2024-02-12 07:35:26.000000 pyraf-2.2.2rc1/pyraf/sqliteshelve.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    33325 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/subproc.py
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.461686 pyraf-2.2.2rc1/pyraf/tests/
+-rw-r--r--   0 oles      (1000) oles      (1000)        0 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/tests/__init__.py
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.461686 pyraf-2.2.2rc1/pyraf/tests/data/
+-rw-r--r--   0 oles      (1000) oles      (1000)    23267 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/tests/data/psdump_prow_250.ps
+-rw-r--r--   0 oles      (1000) oles      (1000)    25541 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/tests/data/psdump_prow_256.ps
+-rw-r--r--   0 oles      (1000) oles      (1000)    29147 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/tests/data/psdump_prow_256_250.ps
+-rw-r--r--   0 oles      (1000) oles      (1000)    32746 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/tests/data/psdump_prow_256_250_200.ps
+-rw-r--r--   0 oles      (1000) oles      (1000)   132480 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/tests/data/pset_msstat_input.fits
+-rw-r--r--   0 oles      (1000) oles      (1000)    18499 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/tests/data/psi_land_prow_250.ps
+-rw-r--r--   0 oles      (1000) oles      (1000)    18758 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/tests/data/psi_land_prow_256.ps
+-rw-r--r--   0 oles      (1000) oles      (1000)    22450 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/tests/data/psi_land_prow_256_250.ps
+-rw-r--r--   0 oles      (1000) oles      (1000)    26135 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/tests/data/psi_land_prow_256_250_200.ps
+-rw-r--r--   0 oles      (1000) oles      (1000)     2060 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/tests/test_basic.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     1144 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/pyraf/tests/test_clcache.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    12463 2024-04-11 08:10:46.000000 pyraf-2.2.2rc1/pyraf/tests/test_cli.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     8027 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tests/test_core_nongraphics.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    12441 2024-02-12 07:35:26.000000 pyraf-2.2.2rc1/pyraf/tests/test_graphics.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     4906 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tests/test_invocation.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     2184 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tests/test_plot.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     1673 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tests/test_tasks.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    11065 2022-03-21 08:13:11.000000 pyraf-2.2.2rc1/pyraf/tests/test_using_tasks.py
+-rw-r--r--   0 oles      (1000) oles      (1000)      439 2024-02-12 07:35:26.000000 pyraf-2.2.2rc1/pyraf/tests/utils.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     3086 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/textattrib.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     6048 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/tkplottext.py
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.461686 pyraf-2.2.2rc1/pyraf/tools/
+-rw-r--r--   0 oles      (1000) oles      (1000)        0 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/__init__.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     3219 2024-03-07 07:36:42.000000 pyraf-2.2.2rc1/pyraf/tools/alert.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    60413 2022-03-18 07:25:44.000000 pyraf-2.2.2rc1/pyraf/tools/basicpar.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     6821 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/capable.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    60399 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/cfgpars.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     2345 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/compmixin.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     1906 2024-03-07 07:36:42.000000 pyraf-2.2.2rc1/pyraf/tools/dialog.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    70659 2024-03-07 07:36:42.000000 pyraf-2.2.2rc1/pyraf/tools/editpar.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    37396 2024-03-07 07:36:42.000000 pyraf-2.2.2rc1/pyraf/tools/eparoption.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    15745 2024-03-07 07:36:42.000000 pyraf-2.2.2rc1/pyraf/tools/filedlg.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    14054 2022-03-18 07:25:44.000000 pyraf-2.2.2rc1/pyraf/tools/irafglobals.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    19301 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/irafutils.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     3494 2024-03-07 07:36:42.000000 pyraf-2.2.2rc1/pyraf/tools/listdlg.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     8465 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/minmatch.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     2643 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/taskpars.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    51260 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/teal.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     2793 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/teal_bttn.py
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.461686 pyraf-2.2.2rc1/pyraf/tools/tests/
+-rw-r--r--   0 oles      (1000) oles      (1000)        0 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/tests/__init__.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    14030 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/tests/cfgobj_output.ref
+-rw-r--r--   0 oles      (1000) oles      (1000)     4254 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/tests/rt_sample.cfg
+-rw-r--r--   0 oles      (1000) oles      (1000)     7252 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/tests/rt_sample.cfgspc
+-rw-r--r--   0 oles      (1000) oles      (1000)     1765 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/tests/test_cfgobj.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     4279 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/tests/test_compmixin.py
+-rw-r--r--   0 oles      (1000) oles      (1000)      974 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/tests/test_irafutils.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     1980 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/tests/test_minmatch.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     2371 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/tkrotext.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     5566 2022-03-15 10:57:45.000000 pyraf-2.2.2rc1/pyraf/tools/vtor_checks.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    45984 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/tpar.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    10255 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/urwfiledlg.py
+-rwxr-xr-x   0 oles      (1000) oles      (1000)     9233 2022-03-10 07:33:57.000000 pyraf-2.2.2rc1/pyraf/urwutil.py
+-rw-r--r--   0 oles      (1000) oles      (1000)      414 2024-04-11 08:36:34.000000 pyraf-2.2.2rc1/pyraf/version.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    22438 2024-04-11 08:09:31.000000 pyraf-2.2.2rc1/pyraf/wutil.py
+-rw-r--r--   0 oles      (1000) oles      (1000)    12804 2024-04-11 08:09:31.000000 pyraf-2.2.2rc1/pyraf/xutil.c
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.461686 pyraf-2.2.2rc1/pyraf.egg-info/
+-rw-r--r--   0 oles      (1000) oles      (1000)     4191 2024-04-11 08:36:34.000000 pyraf-2.2.2rc1/pyraf.egg-info/PKG-INFO
+-rw-r--r--   0 oles      (1000) oles      (1000)     3284 2024-04-11 08:36:34.000000 pyraf-2.2.2rc1/pyraf.egg-info/SOURCES.txt
+-rw-r--r--   0 oles      (1000) oles      (1000)        1 2024-04-11 08:36:34.000000 pyraf-2.2.2rc1/pyraf.egg-info/dependency_links.txt
+-rw-r--r--   0 oles      (1000) oles      (1000)       37 2024-04-11 08:36:34.000000 pyraf-2.2.2rc1/pyraf.egg-info/entry_points.txt
+-rw-r--r--   0 oles      (1000) oles      (1000)      120 2024-04-11 08:36:34.000000 pyraf-2.2.2rc1/pyraf.egg-info/requires.txt
+-rw-r--r--   0 oles      (1000) oles      (1000)        6 2024-04-11 08:36:34.000000 pyraf-2.2.2rc1/pyraf.egg-info/top_level.txt
+-rw-r--r--   0 oles      (1000) oles      (1000)       38 2024-04-11 08:36:34.465686 pyraf-2.2.2rc1/setup.cfg
+-rwxr-xr-x   0 oles      (1000) oles      (1000)      611 2024-04-11 08:10:46.000000 pyraf-2.2.2rc1/setup.py
+drwxr-xr-x   0 oles      (1000) oles      (1000)        0 2024-04-11 08:36:34.461686 pyraf-2.2.2rc1/tools/
+-rw-r--r--   0 oles      (1000) oles      (1000)     6770 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/tools/compileallcl.py
+-rw-r--r--   0 oles      (1000) oles      (1000)     1748 2022-02-16 07:10:36.000000 pyraf-2.2.2rc1/tools/loadall.py
```

### Comparing `pyraf-2.2.1rc1/.github/workflows/citest.yml` & `pyraf-2.2.2rc1/.github/workflows/citest.yml`

 * *Files 13% similar despite different names*

```diff
@@ -12,38 +12,38 @@
       iraf:  ${{ matrix.iraf }}
       TERM: dumb
       PYRAF_NO_DISPLAY: no
 
     strategy:
       matrix:
         include:
-          - name: Ubuntu 20.04 (Python-3.8.2), native
-            os: ubuntu-20.04
+          - name: Ubuntu 22.04 (Python-3.10), native
+            os: ubuntu-22.04
             method: native
             iraf: /usr/lib/iraf/
             upload_coverage: yes
 
-          - name: Ubuntu 20.04 (Python-3.8.2), native, without IRAF
-            os: ubuntu-20.04
+          - name: Ubuntu 22.04 (Python-3.10), native, without IRAF
+            os: ubuntu-22.04
             method: native
 
-          - name: Ubuntu 18.04 (Python-3.7), pip
-            os: ubuntu-18.04
+          - name: Ubuntu 20.04 (Python-3.8.2), pip
+            os: ubuntu-20.04
             method: pip
             iraf: /usr/lib/iraf/
 
-          - name: macOS 10.15, pip
-            os: macos-10.15
+          - name: macOS 13, pip
+            os: macos-13
             method: pip
             iraf: /Users/runner/work/iraf/
 
     steps:
       - name: Checkout repository
         if: matrix.method == 'native'
-        uses: actions/checkout@v2
+        uses: actions/checkout@v4
 
       - name: Setup dependencies
         if: startsWith(matrix.os, 'ubuntu') && matrix.method == 'native'
         run: |
           sudo apt-get update
           if [ "$iraf" ]; then
               sudo apt-get install --no-install-recommends iraf iraf-noao iraf-dev
@@ -90,10 +90,10 @@
       - name: Run tests (installed package)
         if: matrix.method == 'pip'
         run: |
           python3 -m pytest -s --pyargs pyraf
 
       - name: "Upload coverage to Codecov"
         if: matrix.upload_coverage == 'yes'
-        uses: codecov/codecov-action@v1
+        uses: codecov/codecov-action@v4
         with:
           fail_ci_if_error: false
```

### Comparing `pyraf-2.2.1rc1/CODE_OF_CONDUCT.md` & `pyraf-2.2.2rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/LICENSE.txt` & `pyraf-2.2.2rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/PKG-INFO` & `pyraf-2.2.2rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pyraf
-Version: 2.2.1rc1
+Version: 2.2.2rc1
 Summary: Pythonic interface to IRAF that can be used in place of the existing IRAF CL
-Home-page: https://iraf-community.github.io/pyraf.html
 Author: Rick White, Perry Greenfield, Chris Sontag, Ole Streicher
 License: BSD 3-Clause
-Keywords: astronomy,astrophysics,utility
-Platform: any
+Keywords: astronomy,astrophysics,utility,iraf
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: configobj
+Requires-Dist: numpy
+Requires-Dist: pyobjc; sys_platform == "darwin"
 Provides-Extra: docs
+Requires-Dist: astropy-sphinx-theme; extra == "docs"
+Requires-Dist: numpydoc; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
 Provides-Extra: test
-License-File: LICENSE.txt
+Requires-Dist: astropy; extra == "test"
+Requires-Dist: pytest; extra == "test"
 
 =====
 PyRAF
 =====
 
 |Release| |CI Status| |Coverage Status| |Documentation|
 
@@ -106,9 +108,7 @@
 .. _PyPI: https://pypi.org/project/pyraf
 
 .. _IRAF: https://iraf-community.github.io
 
 .. _iraf-community: https://iraf-community.github.io
 
 .. _Ubuntu: https://www.ubuntu.com/
-
-
```

### Comparing `pyraf-2.2.1rc1/README.rst` & `pyraf-2.2.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/docs/_static/pyraflogo.png` & `pyraf-2.2.2rc1/docs/_static/pyraflogo.png`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/docs/conf.py` & `pyraf-2.2.2rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/docs/ecl.html` & `pyraf-2.2.2rc1/docs/ecl.html`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/docs/epar.png` & `pyraf-2.2.2rc1/docs/epar.png`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/docs/index.rst` & `pyraf-2.2.2rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/docs/ipython_notes.txt` & `pyraf-2.2.2rc1/docs/ipython_notes.txt`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/docs/prow.png` & `pyraf-2.2.2rc1/docs/prow.png`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/docs/pyraf_tutorial.rst` & `pyraf-2.2.2rc1/docs/pyraf_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/docs/teal_guide.rst` & `pyraf-2.2.2rc1/docs/teal_guide.rst`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/GkiMpl.py` & `pyraf-2.2.2rc1/pyraf/GkiMpl.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/MplCanvasAdapter.py` & `pyraf-2.2.2rc1/pyraf/MplCanvasAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import matplotlib
 matplotlib.use('TkAgg')  # set backend
 import matplotlib.backends.backend_tkagg as tkagg
+from matplotlib.backend_bases import ResizeEvent
 from .Ptkplot import hideTkCursor
 from .Ptkplot import FullWindowCursor
 import tkinter
 from .wutil import moveCursorTo, WUTIL_USING_X
 
 
 class MplCanvasAdapter(tkagg.FigureCanvasTkAgg):
@@ -86,15 +87,16 @@
         self._tkcanvas.delete(self._tkphoto)
         self._tkphoto = tkinter.PhotoImage(master=self._tkcanvas,
                                            width=int(width),
                                            height=int(height))
         self._tkcanvas.create_image(int(width / 2),
                                     int(height / 2),
                                     image=self._tkphoto)
-        self.resize_event()
+        self.callbacks.process('resize_event', ResizeEvent('resize_event', self))
+        self.draw_idle()
 
     def flush(self):
 
         self.__doIdleRedraw = 0
 
     # draw could be defined to catch events before passing through
```

### Comparing `pyraf-2.2.1rc1/pyraf/Ptkplot.py` & `pyraf-2.2.2rc1/pyraf/Ptkplot.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/__init__.py` & `pyraf-2.2.2rc1/pyraf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/__main__.py` & `pyraf-2.2.2rc1/pyraf/__main__.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/cgeneric.py` & `pyraf-2.2.2rc1/pyraf/cgeneric.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/cl2py.py` & `pyraf-2.2.2rc1/pyraf/cl2py.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/clast.py` & `pyraf-2.2.2rc1/pyraf/clast.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/clcache.py` & `pyraf-2.2.2rc1/pyraf/clcache.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
 # be found in the cache (since the file contents, not the
 # name, determine the shelve key) while staying up-to-date
 # with changes of the CL file contents when the script is
 # being developed.
 
 
 def _currentVersion():
-    return "4e" if pyrafglobals._use_ecl else "4c"
+    v = "4e" if pyrafglobals._use_ecl else "4c"
+    return v + str(sqliteshelve.pickle_protocol)
 
 
 class _FileContentsCache(filecache.FileCacheDict):
 
     def __init__(self):
         # create file dictionary with md5 digest as value
         filecache.FileCacheDict.__init__(self, filecache.MD5Cache)
```

### Comparing `pyraf-2.2.1rc1/pyraf/cllinecache.py` & `pyraf-2.2.2rc1/pyraf/cllinecache.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/clparse.py` & `pyraf-2.2.2rc1/pyraf/clparse.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/clscan.py` & `pyraf-2.2.2rc1/pyraf/clscan.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/cltoken.py` & `pyraf-2.2.2rc1/pyraf/cltoken.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/epar.py` & `pyraf-2.2.2rc1/pyraf/epar.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/filecache.py` & `pyraf-2.2.2rc1/pyraf/filecache.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/fill_clcache.py` & `pyraf-2.2.2rc1/pyraf/fill_clcache.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/fontdata.py` & `pyraf-2.2.2rc1/pyraf/fontdata.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/generic.py` & `pyraf-2.2.2rc1/pyraf/generic.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/gki.py` & `pyraf-2.2.2rc1/pyraf/gki.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/gkicmd.py` & `pyraf-2.2.2rc1/pyraf/gkicmd.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/gkigcur.py` & `pyraf-2.2.2rc1/pyraf/gkigcur.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/gkiiraf.py` & `pyraf-2.2.2rc1/pyraf/gkiiraf.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/gkitkbase.py` & `pyraf-2.2.2rc1/pyraf/gkitkbase.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/gkitkplot.py` & `pyraf-2.2.2rc1/pyraf/gkitkplot.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/graphcap.py` & `pyraf-2.2.2rc1/pyraf/graphcap.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/gwm.py` & `pyraf-2.2.2rc1/pyraf/gwm.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/ipython_api.py` & `pyraf-2.2.2rc1/pyraf/ipython_api.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/ipythonrc-pyraf` & `pyraf-2.2.2rc1/pyraf/ipythonrc-pyraf`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/irafcompleter.py` & `pyraf-2.2.2rc1/pyraf/irafcompleter.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/irafdisplay.py` & `pyraf-2.2.2rc1/pyraf/irafdisplay.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/irafecl.py` & `pyraf-2.2.2rc1/pyraf/irafecl.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/irafexecute.py` & `pyraf-2.2.2rc1/pyraf/irafexecute.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/iraffunctions.py` & `pyraf-2.2.2rc1/pyraf/iraffunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,20 +79,15 @@
 from . import irafinst as _irafinst
 from . import irafpar as _irafpar
 from . import iraftask as _iraftask
 from . import irafexecute as _irafexecute
 from . import cl2py as _cl2py
 from . import gki
 from . import irafecl
-try:
-    from . import sscanf
-except OSError:
-    # basic usage does not actually require sscanf
-    sscanf = None
-    print("Warning: sscanf library not installed on " + sys.platform)
+from . import scanf as sscanf
 
 
 # FP_EPSILON is the smallest number such that: 1.0 + epsilon > 1.0;  Use None
 # in the finfo ctor to make it use the default precision for a Python float.
 FP_EPSILON = _numpy.finfo(None).eps
 
 # -----------------------------------------------------
@@ -176,15 +171,15 @@
 (http://www.google.com/search?q=mkiraf).
 """)
 
         arch = _os.environ.get('IRAFARCH', '')
 
         # stacksize problem on linux
         # https://iraf-community.github.io/iraf-v216/issues/61
-        if arch in ('redhat', 'linux', 'linuxppc', 'suse'):
+        if arch in ('redhat', 'linux', 'linuxppc', 'suse', 'macosx'):
             import resource
             try:
                 hardlimit = resource.getrlimit(resource.RLIMIT_STACK)[1]
                 resource.setrlimit(resource.RLIMIT_STACK, (hardlimit, hardlimit))
             except (ValueError, OSError):
                 pass  # Ignore the error and hope the best...
 
@@ -238,14 +233,16 @@
             fname = _os.path.abspath('login.cl')
         elif access('home$login.cl'):
             fname = 'home$login.cl'
         elif access(_os.path.expanduser('~/.iraf/login.cl')):
             fname = _os.path.expanduser('~/.iraf/login.cl')
         elif access('/etc/iraf/login.cl'):
             fname = '/etc/iraf/login.cl'
+        elif access('hlib$login.cl'):
+            fname = 'hlib$login.cl'
         else:
             fname = None
 
         if fname:
             # define and load user package
             userpkg = IrafTaskFactory('', 'user', '.pkg', fname, 'clpackage',
                                       'bin$')
@@ -1982,23 +1979,20 @@
         line = eval(line, {'iraf': iraf}, theLocals)
         # format also needs to be evaluated
         format = eval(format, theLocals)
     except EOFError:
         _weirdEOF(theLocals, namelist)
         _nscan = 0
         return EOF
-    if sscanf is None:
-        raise RuntimeError("fscanf is not supported on this platform")
-    f = sscanf.sscanf(line, format)
-    n = min(len(f), len(namelist))
+    f = sscanf.scanf(format, line)
     # if list is null, add a null string
     # ugly but should be right most of the time
-    if n == 0 and namelist:
-        f = ['']
-        n = 1
+    if f is None and namelist:
+        f = ('')
+    n = min(len(f), len(namelist))
     if len(kw):
         raise TypeError('unexpected keyword argument: ' +
                         repr(list(kw.keys())))
     n_actual = 0  # this will be the actual number of values converted
     for i in range(n):
         cmd = namelist[i] + ' = ' + repr(f[i])
         try:
```

### Comparing `pyraf-2.2.1rc1/pyraf/irafgwcs.py` & `pyraf-2.2.2rc1/pyraf/irafgwcs.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/irafhelp.py` & `pyraf-2.2.2rc1/pyraf/irafhelp.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/irafimcur.py` & `pyraf-2.2.2rc1/pyraf/irafimcur.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/irafimport.py` & `pyraf-2.2.2rc1/pyraf/irafimport.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/irafinst.py` & `pyraf-2.2.2rc1/pyraf/irafinst.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/irafnames.py` & `pyraf-2.2.2rc1/pyraf/irafnames.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/irafpar.py` & `pyraf-2.2.2rc1/pyraf/irafpar.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/iraftask.py` & `pyraf-2.2.2rc1/pyraf/iraftask.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/irafukey.py` & `pyraf-2.2.2rc1/pyraf/irafukey.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/msgiobuffer.py` & `pyraf-2.2.2rc1/pyraf/msgiobuffer.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/msgiowidget.py` & `pyraf-2.2.2rc1/pyraf/msgiowidget.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/newWindowHack.py` & `pyraf-2.2.2rc1/pyraf/newWindowHack.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/noiraf/cl.par` & `pyraf-2.2.2rc1/pyraf/noiraf/cl.par`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/noiraf/login.cl` & `pyraf-2.2.2rc1/pyraf/noiraf/login.cl`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/noiraf/system.cl` & `pyraf-2.2.2rc1/pyraf/noiraf/system.cl`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/pseteparoption.py` & `pyraf-2.2.2rc1/pyraf/pseteparoption.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/pycmdline.py` & `pyraf-2.2.2rc1/pyraf/pycmdline.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/pyrafTk.py` & `pyraf-2.2.2rc1/pyraf/pyrafTk.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/pyrafglobals.py` & `pyraf-2.2.2rc1/pyraf/pyrafglobals.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/pyraflogo_rgb_web.gif` & `pyraf-2.2.2rc1/pyraf/pyraflogo_rgb_web.gif`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/splash.py` & `pyraf-2.2.2rc1/pyraf/splash.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/sqliteshelve.py` & `pyraf-2.2.2rc1/pyraf/sqliteshelve.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 # SOFTWARE.
 
 import pickle
 import sqlite3
 import os
 
 
+pickle_protocol = 4
+"""Protocol version to use for pickling objects"""
+
+
 class Shelf:
     """An SQLite implementation of the Python Shelf interface
 
     """
     def __init__(self, fname, mode):
         """Open or create an existing sqlite3_shelf
 
@@ -71,15 +75,15 @@
 
     def __setitem__(self, key, value):
         """Set an entry for key to value using pickling
 
         """
         if self.readonly:
             raise OSError("Readonly database")
-        pdata = pickle.dumps(value, pickle.HIGHEST_PROTOCOL)
+        pdata = pickle.dumps(value, protocol=pickle_protocol)
         cursor = self.db.cursor()
         try:
             cursor.execute("insert or replace into shelf (key_str, value_str)"
                            " values (:key,:value)",
                            {'key': key, 'value': sqlite3.Binary(pdata)})
             self.db.commit()
         finally:
```

### Comparing `pyraf-2.2.1rc1/pyraf/subproc.py` & `pyraf-2.2.2rc1/pyraf/subproc.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/data/psdump_prow_250.ps` & `pyraf-2.2.2rc1/pyraf/tests/data/psdump_prow_250.ps`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/data/psdump_prow_256.ps` & `pyraf-2.2.2rc1/pyraf/tests/data/psdump_prow_256.ps`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/data/psdump_prow_256_250.ps` & `pyraf-2.2.2rc1/pyraf/tests/data/psdump_prow_256_250.ps`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/data/psdump_prow_256_250_200.ps` & `pyraf-2.2.2rc1/pyraf/tests/data/psdump_prow_256_250_200.ps`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/data/pset_msstat_input.fits` & `pyraf-2.2.2rc1/pyraf/tests/data/pset_msstat_input.fits`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/data/psi_land_prow_250.ps` & `pyraf-2.2.2rc1/pyraf/tests/data/psi_land_prow_250.ps`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/data/psi_land_prow_256.ps` & `pyraf-2.2.2rc1/pyraf/tests/data/psi_land_prow_256.ps`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/data/psi_land_prow_256_250.ps` & `pyraf-2.2.2rc1/pyraf/tests/data/psi_land_prow_256_250.ps`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/data/psi_land_prow_256_250_200.ps` & `pyraf-2.2.2rc1/pyraf/tests/data/psi_land_prow_256_250_200.ps`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/test_basic.py` & `pyraf-2.2.2rc1/pyraf/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/test_clcache.py` & `pyraf-2.2.2rc1/pyraf/tests/test_clcache.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/test_cli.py` & `pyraf-2.2.2rc1/pyraf/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import math
 from contextlib import contextmanager, redirect_stderr
 import pytest
 
 from .utils import HAS_IRAF
 
 from .. import iraf
-from .. import sscanf
+from .. import scanf
 from .. import pyrafglobals
 
 
 @contextmanager
 def use_ecl(flag):
     """Temporary enable/disable usage of ECL"""
     # This is a quite dirty hack that is adjusted to do just enough to
@@ -55,33 +55,28 @@
     with use_ecl(ecl_flag):
         stdout = io.StringIO()
         iraf.clExecute(f'print "i: " ({arg})', StdoutAppend=stdout)
         assert stdout.getvalue().strip() == f'i: {expected}'
 
 
 @pytest.mark.parametrize('arg,fmt,expected', [
-    ("seven 6 4.0 -7", "%s %d %g %d", ['seven', 6, 4.0, -7]), # aliveness
-    ("seven", "%d", []),
-    ("seven", "%c%3c%99c", ['s', 'eve', 'n']),
-    ("0xabc90", "%x", [703632]),
+    ("seven 6 4.0 -7", "%s %d %g %d", ('seven', 6, 4.0, -7)), # aliveness
+    ("seven", "%d", None),
+    ("seven", "%c%3c%99c", ('s', 'eve', 'n')),
+    ("seven", "%[sev]", ('seve', )),
+    ("0xabc90", "%x", (703632, )),
 ])  
-def test_sscanf(arg, fmt, expected):
+def test_scanf(arg, fmt, expected):
     """A basic unit test that sscanf was built/imported correctly and
     can run.
     """
-    l = sscanf.sscanf(arg, fmt)
+    l = scanf.scanf(fmt, arg)
     assert l == expected
 
 
-def test_sscanf_error():
-    # API error
-    with pytest.raises(TypeError):
-        sscanf.sscanf()
-
-
 @pytest.mark.skipif(not HAS_IRAF, reason='Need IRAF to run')
 @pytest.mark.parametrize('arg,expected', [
     ("pw", "user.pwd"),
     ("lang", "clpackage.language"),
     ("st", "plot.stdplot plot.stdgraph user.strings imcoords.starfind"),
     ("std", "plot.stdplot plot.stdgraph"),
     ("stdg", "plot.stdgraph"),
```

### Comparing `pyraf-2.2.1rc1/pyraf/tests/test_core_nongraphics.py` & `pyraf-2.2.2rc1/pyraf/tests/test_core_nongraphics.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/test_graphics.py` & `pyraf-2.2.2rc1/pyraf/tests/test_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 try:
     host_arch = sys.implementation._multiarch.split("-")[0]
 except AttributeError:
     import platform
     host_arch = platform.machine()
 is_i386 = host_arch in ('i386', 'i486', 'i586', 'i686')
+is_macos = sys.platform == 'darwin'
 
 from ..tools import capable
 
 from .utils import HAS_IRAF, DATA_DIR
 
 if HAS_IRAF:
     from pyraf import iraf
@@ -209,30 +210,30 @@
 
 def test_gki_control_codes():
     """ Simple aliveness test for the control2name dict """
     for ctl in gki.GKI_ILLEGAL_LIST:
         assert gki.control2name[ctl] == 'control_unknown'
 
 
-@pytest.mark.skipif(is_i386, reason='diff is not identical on i386')
+@pytest.mark.skipif(is_i386 or is_macos, reason='diff is not identical on i386')
 def test_gki_single_prow():
     """ Test a prow-plot of a single row from dev$pix to .ps """
     iraf.plot(_doprint=0)  # load plot for prow
     # get look at tmp dir before plot/flush
     flistBef = findAllTmpPskFiles()
     # plot
     iraf.prow("dev$pix", row=256, dev=PSDEV)  # plot
     iraf.gflush()
     # get output postscript temp file name
     psOut = getNewTmpPskFile(flistBef, "single_prow")
     # diff
     diffit(EXP2IGNORE, psOut, os.path.join(DATA_DIR, PSDEV + "_prow_256.ps"))
 
 
-@pytest.mark.skipif(is_i386, reason='diff is not identical on i386')
+@pytest.mark.skipif(is_i386 or is_macos, reason='diff is not identical on i386')
 def test_gki_prow_1_append():
     """ Test a prow-plot with 1 append (2 rows total, dev$pix) to .ps """
     iraf.plot(_doprint=0)  # load plot for prow
     # get look at tmp dir before plot/flush
     flistBef = findAllTmpPskFiles()
     # plot
     iraf.prow("dev$pix", row=256, dev=PSDEV)  # plot
@@ -241,15 +242,15 @@
     # get output postscript temp file name
     psOut = getNewTmpPskFile(flistBef, "prow_1_append")
     # diff
     diffit(EXP2IGNORE, psOut, os.path.join(DATA_DIR,
                                            PSDEV + "_prow_256_250.ps"))
 
 
-@pytest.mark.skipif(is_i386, reason='diff is not identical on i386')
+@pytest.mark.skipif(is_i386 or is_macos, reason='diff is not identical on i386')
 def test_gki_prow_2_appends():
     """ Test a prow-plot with 2 appends (3 rows total, dev$pix) to .ps """
     iraf.plot(_doprint=0)  # load plot for prow
     # get look at tmp dir before plot/flush
     flistBef = findAllTmpPskFiles()
     # plot
     iraf.prow("dev$pix", row=256, dev=PSDEV)  # plot
@@ -259,15 +260,15 @@
     # get output postscript temp file name
     psOut = getNewTmpPskFile(flistBef, "prow_2_appends")
     # diff
     diffit(EXP2IGNORE, psOut,
            os.path.join(DATA_DIR, PSDEV + "_prow_256_250_200.ps"))
 
 
-@pytest.mark.skipif(is_i386, reason='diff is not identical on i386')
+@pytest.mark.skipif(is_i386 or is_macos, reason='diff is not identical on i386')
 def test_gki_2_prows_no_append():
     """ Test 2 prow calls with no append (2 dev$pix rows) to 2 .ps's """
     iraf.plot(_doprint=0)  # load plot for prow
     # get look at tmp dir before plot/flush
     flistBef = findAllTmpPskFiles()
     # plot
     iraf.prow("dev$pix", row=256, dev=PSDEV)  # plot
```

### Comparing `pyraf-2.2.1rc1/pyraf/tests/test_invocation.py` & `pyraf-2.2.2rc1/pyraf/tests/test_invocation.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/test_plot.py` & `pyraf-2.2.2rc1/pyraf/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/test_tasks.py` & `pyraf-2.2.2rc1/pyraf/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tests/test_using_tasks.py` & `pyraf-2.2.2rc1/pyraf/tests/test_using_tasks.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/textattrib.py` & `pyraf-2.2.2rc1/pyraf/textattrib.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tkplottext.py` & `pyraf-2.2.2rc1/pyraf/tkplottext.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/alert.py` & `pyraf-2.2.2rc1/pyraf/tools/alert.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/basicpar.py` & `pyraf-2.2.2rc1/pyraf/tools/basicpar.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/capable.py` & `pyraf-2.2.2rc1/pyraf/tools/capable.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/cfgpars.py` & `pyraf-2.2.2rc1/pyraf/tools/cfgpars.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/compmixin.py` & `pyraf-2.2.2rc1/pyraf/tools/compmixin.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/dialog.py` & `pyraf-2.2.2rc1/pyraf/tools/dialog.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/editpar.py` & `pyraf-2.2.2rc1/pyraf/tools/editpar.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         # Now fill in the Canvas Window
         #
 
         # The makeEntries method creates the parameter entry Frame
         self.makeEntries(canvas.entries, self.top.status)
 
         # Force an update of the entry Frame
-        canvas.entries.update()
+        canvas.entries.update_idletasks()
 
         # Determine the size of the entry Frame
         width = canvas.entries.winfo_width()
         height = canvas.entries.winfo_height()
 
         # Reconfigure the Canvas size based on the Frame.
         if (self.numParams <= MINPARAMS):
@@ -330,28 +330,28 @@
         self.yscrollincrement = 5 # changed Mar2010, had been 50 a long time
         canvas.config(yscrollincrement=self.yscrollincrement)
 
         # Set the actual viewable region for the Canvas
         canvas.config(width=width, height=viewHeight)
 
         # Force an update of the Canvas
-        canvas.update()
+        canvas.update_idletasks()
 
         # Associate deletion of the main window to a Abort
         self.top.protocol("WM_DELETE_WINDOW", self.abort)
 
         # Trigger all widgets one time before starting in case they have
         # values which would run a trigger
         self.checkAllTriggers('init')
 
         # Set focus to first parameter
         self.setViewAtTop()
 
         # Finally show it
-        self.top.update()
+        self.top.update_idletasks()
         self.top.deiconify()
 
         # Enable interactive resizing in height
         self.top.resizable(width=FALSE, height=TRUE)
 
         # Limit maximum window height
         width = self.top.winfo_width()
```

### Comparing `pyraf-2.2.1rc1/pyraf/tools/eparoption.py` & `pyraf-2.2.2rc1/pyraf/tools/eparoption.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/filedlg.py` & `pyraf-2.2.2rc1/pyraf/tools/filedlg.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/irafglobals.py` & `pyraf-2.2.2rc1/pyraf/tools/irafglobals.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/irafutils.py` & `pyraf-2.2.2rc1/pyraf/tools/irafutils.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/listdlg.py` & `pyraf-2.2.2rc1/pyraf/tools/listdlg.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/minmatch.py` & `pyraf-2.2.2rc1/pyraf/tools/minmatch.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/taskpars.py` & `pyraf-2.2.2rc1/pyraf/tools/taskpars.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/teal.py` & `pyraf-2.2.2rc1/pyraf/tools/teal.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/teal_bttn.py` & `pyraf-2.2.2rc1/pyraf/tools/teal_bttn.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/tests/cfgobj_output.ref` & `pyraf-2.2.2rc1/pyraf/tools/tests/cfgobj_output.ref`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/tests/rt_sample.cfg` & `pyraf-2.2.2rc1/pyraf/tools/tests/rt_sample.cfg`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/tests/rt_sample.cfgspc` & `pyraf-2.2.2rc1/pyraf/tools/tests/rt_sample.cfgspc`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/tests/test_cfgobj.py` & `pyraf-2.2.2rc1/pyraf/tools/tests/test_cfgobj.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/tests/test_compmixin.py` & `pyraf-2.2.2rc1/pyraf/tools/tests/test_compmixin.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/tests/test_irafutils.py` & `pyraf-2.2.2rc1/pyraf/tools/tests/test_irafutils.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/tests/test_minmatch.py` & `pyraf-2.2.2rc1/pyraf/tools/tests/test_minmatch.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/tkrotext.py` & `pyraf-2.2.2rc1/pyraf/tools/tkrotext.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tools/vtor_checks.py` & `pyraf-2.2.2rc1/pyraf/tools/vtor_checks.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/tpar.py` & `pyraf-2.2.2rc1/pyraf/tpar.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/urwfiledlg.py` & `pyraf-2.2.2rc1/pyraf/urwfiledlg.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/urwutil.py` & `pyraf-2.2.2rc1/pyraf/urwutil.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/wutil.py` & `pyraf-2.2.2rc1/pyraf/wutil.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf/xutil.c` & `pyraf-2.2.2rc1/pyraf/xutil.c`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/pyraf.egg-info/PKG-INFO` & `pyraf-2.2.2rc1/pyraf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pyraf
-Version: 2.2.1rc1
+Version: 2.2.2rc1
 Summary: Pythonic interface to IRAF that can be used in place of the existing IRAF CL
-Home-page: https://iraf-community.github.io/pyraf.html
 Author: Rick White, Perry Greenfield, Chris Sontag, Ole Streicher
 License: BSD 3-Clause
-Keywords: astronomy,astrophysics,utility
-Platform: any
+Keywords: astronomy,astrophysics,utility,iraf
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: configobj
+Requires-Dist: numpy
+Requires-Dist: pyobjc; sys_platform == "darwin"
 Provides-Extra: docs
+Requires-Dist: astropy-sphinx-theme; extra == "docs"
+Requires-Dist: numpydoc; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
 Provides-Extra: test
-License-File: LICENSE.txt
+Requires-Dist: astropy; extra == "test"
+Requires-Dist: pytest; extra == "test"
 
 =====
 PyRAF
 =====
 
 |Release| |CI Status| |Coverage Status| |Documentation|
 
@@ -106,9 +108,7 @@
 .. _PyPI: https://pypi.org/project/pyraf
 
 .. _IRAF: https://iraf-community.github.io
 
 .. _iraf-community: https://iraf-community.github.io
 
 .. _Ubuntu: https://www.ubuntu.com/
-
-
```

### Comparing `pyraf-2.2.1rc1/pyraf.egg-info/SOURCES.txt` & `pyraf-2.2.2rc1/pyraf.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 .gitignore
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE.txt
 MANIFEST.in
 README.rst
-setup.cfg
+pyproject.toml
 setup.py
+.github/dependabot.yml
 .github/workflows/citest.yml
 docs/conf.py
 docs/ecl.html
 docs/epar.png
 docs/index.rst
 docs/ipython_notes.txt
 docs/prow.png
@@ -67,31 +68,30 @@
 pyraf/msgiowidget.py
 pyraf/newWindowHack.py
 pyraf/pseteparoption.py
 pyraf/pycmdline.py
 pyraf/pyrafTk.py
 pyraf/pyrafglobals.py
 pyraf/pyraflogo_rgb_web.gif
+pyraf/scanf.py
 pyraf/splash.py
 pyraf/sqliteshelve.py
-pyraf/sscanfmodule.c
 pyraf/subproc.py
 pyraf/textattrib.py
 pyraf/tkplottext.py
 pyraf/tpar.py
 pyraf/urwfiledlg.py
 pyraf/urwutil.py
 pyraf/version.py
 pyraf/wutil.py
 pyraf/xutil.c
 pyraf.egg-info/PKG-INFO
 pyraf.egg-info/SOURCES.txt
 pyraf.egg-info/dependency_links.txt
 pyraf.egg-info/entry_points.txt
-pyraf.egg-info/not-zip-safe
 pyraf.egg-info/requires.txt
 pyraf.egg-info/top_level.txt
 pyraf/noiraf/cl.par
 pyraf/noiraf/clpackage.cl
 pyraf/noiraf/login.cl
 pyraf/noiraf/system.cl
 pyraf/noiraf/system.par
```

### Comparing `pyraf-2.2.1rc1/setup.py` & `pyraf-2.2.2rc1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 import os
 import platform
 
 from setuptools import setup, Extension
 
-modules = [Extension('pyraf.sscanf', ['pyraf/sscanfmodule.c'])]
+modules = []
 
 # On a Mac, xutil is not required since the graphics is done directly with Aqua.
 # If one still wants to include it, the parameters
 #     library_dirs="/usr/X11/libs"
 #     include_dirs="/usr/X11/include"
 # need to be added to the Extension
 if platform.system() not in ('Darwin', 'Windows'):
```

### Comparing `pyraf-2.2.1rc1/tools/compileallcl.py` & `pyraf-2.2.2rc1/tools/compileallcl.py`

 * *Files identical despite different names*

### Comparing `pyraf-2.2.1rc1/tools/loadall.py` & `pyraf-2.2.2rc1/tools/loadall.py`

 * *Files identical despite different names*

