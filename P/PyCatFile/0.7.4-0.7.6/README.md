# Comparing `tmp/PyCatFile-0.7.4.tar.gz` & `tmp/PyCatFile-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCatFile-0.7.4.tar", last modified: Mon Apr  1 23:44:26 2024, max compression
+gzip compressed data, was "PyCatFile-0.7.6.tar", last modified: Thu Apr 11 01:29:34 2024, max compression
```

## Comparing `PyCatFile-0.7.4.tar` & `PyCatFile-0.7.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:44:26.191751 PyCatFile-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-01 23:44:17.000000 PyCatFile-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-01 23:44:26.191751 PyCatFile-0.7.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:44:26.191751 PyCatFile-0.7.4/PyCatFile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-01 23:44:26.000000 PyCatFile-0.7.4/PyCatFile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-01 23:44:26.000000 PyCatFile-0.7.4/PyCatFile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 23:44:26.000000 PyCatFile-0.7.4/PyCatFile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 23:44:26.000000 PyCatFile-0.7.4/PyCatFile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 23:44:26.000000 PyCatFile-0.7.4/PyCatFile.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 23:44:17.000000 PyCatFile-0.7.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     6992 2024-04-01 23:44:17.000000 PyCatFile-0.7.4/catfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-01 23:44:17.000000 PyCatFile-0.7.4/neocatfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   329914 2024-04-01 23:44:17.000000 PyCatFile-0.7.4/pycatfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 23:44:26.191751 PyCatFile-0.7.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5450 2024-04-01 23:44:17.000000 PyCatFile-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:29:34.890832 PyCatFile-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-11 01:29:24.000000 PyCatFile-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-11 01:29:34.890832 PyCatFile-0.7.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:29:34.890832 PyCatFile-0.7.6/PyCatFile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-11 01:29:34.000000 PyCatFile-0.7.6/PyCatFile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 01:29:34.000000 PyCatFile-0.7.6/PyCatFile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:29:34.000000 PyCatFile-0.7.6/PyCatFile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 01:29:34.000000 PyCatFile-0.7.6/PyCatFile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:29:34.000000 PyCatFile-0.7.6/PyCatFile.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 01:29:24.000000 PyCatFile-0.7.6/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7356 2024-04-11 01:29:24.000000 PyCatFile-0.7.6/catfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4969 2024-04-11 01:29:24.000000 PyCatFile-0.7.6/neocatfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   332511 2024-04-11 01:29:24.000000 PyCatFile-0.7.6/pycatfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-11 01:29:34.890832 PyCatFile-0.7.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5451 2024-04-11 01:29:24.000000 PyCatFile-0.7.6/setup.py
```

### Comparing `PyCatFile-0.7.4/LICENSE` & `PyCatFile-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCatFile-0.7.4/PKG-INFO` & `PyCatFile-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.7.4
+Version: 0.7.6
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `PyCatFile-0.7.4/PyCatFile.egg-info/PKG-INFO` & `PyCatFile-0.7.6/PyCatFile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCatFile
-Version: 0.7.4
+Version: 0.7.6
 Summary: A tar like file format name catfile after unix cat command (concatenate files) .
 Home-page: https://github.com/GameMaker2k/PyCatFile
 Download-URL: https://github.com/GameMaker2k/PyCatFile/archive/master.tar.gz
 Author: Kazuki Przyborowski
 Author-email: kazuki.przyborowski@gmail.com
 Maintainer: Kazuki Przyborowski
 Maintainer-email: kazuki.przyborowski@gmail.com
```

### Comparing `PyCatFile-0.7.4/catfile.py` & `PyCatFile-0.7.6/catfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: catfile.py - Last Update: 4/1/2024 Ver. 0.7.4 RC 1 - Author: cooldude2k $
+    $FileInfo: catfile.py - Last Update: 4/10/2024 Ver. 0.7.6 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import argparse, pycatfile, binascii;
 
 rarfile_support = pycatfile.rarfile_support;
 
@@ -28,28 +28,31 @@
 __file_format_lower__ = pycatfile.__file_format_lower__;
 __file_format_magic__ = pycatfile.__file_format_magic__;
 __file_format_len__ = pycatfile.__file_format_len__;
 __file_format_hex__ = pycatfile.__file_format_hex__;
 __file_format_delimiter__ = pycatfile.__file_format_delimiter__;
 __file_format_list__ = pycatfile.__file_format_list__;
 __use_new_style__ = pycatfile.__use_new_style__;
+__use_advanced_list__ = pycatfile.__use_advanced_list__;
+__use_alt_inode__ = pycatfile.__use_alt_inode__;
 __project_url__ = pycatfile.__project_url__;
 __version_info__ = pycatfile.__version_info__;
 __version_date_info__ = pycatfile.__version_date_info__;
 __version_date__ = pycatfile.__version_date__;
 __version_date_plusrc__ = pycatfile.__version_date_plusrc__;
 __version__ = pycatfile.__version__;
 
 argparser = argparse.ArgumentParser(description="Manipulate concatenated files.", conflict_handler="resolve", add_help=True);
 argparser.add_argument("-V", "--version", action="version", version=__program_name__ + " " + __version__);
 argparser.add_argument("-i", "-f", "--input", help="Specify the file(s) to concatenate or the concatenated file to extract.", required=True);
 argparser.add_argument("-d", "-v", "--verbose", action="store_true", help="Enable verbose mode to display various debugging information.");
 argparser.add_argument("-c", "--create", action="store_true", help="Perform concatenation operation only.");
 argparser.add_argument("-I", "-validate", "--validate", action="store_true", help="Validate CatFile checksums");
 argparser.add_argument("-C", "-checksum", "--checksum", default="crc32", help="Specify the type of checksum to use. Default is crc32.");
+argparser.add_argument("-S", "-skipchecksum", "--skipchecksum", action="store_true", help="Skip checksum check of files.");
 argparser.add_argument("-e", "-x", "--extract", action="store_true", help="Perform extraction operation only.");
 argparser.add_argument("-F", "-format", "--format", default=__file_format_list__[0], help="Specify the format to use");
 argparser.add_argument("-D", "-delimiter", "--delimiter", default=__file_format_list__[5], help="Specify the format to use");
 argparser.add_argument("-m", "-formatver", "--formatver", default=__file_format_list__[6], help="Specify the format version");
 argparser.add_argument("-l", "-t", "--list", action="store_true", help="List files included in the concatenated file.");
 argparser.add_argument("-p", "-preserve", "--preserve", action="store_false", help="Preserve permissions and time of files");
 argparser.add_argument("-R", "-repack", "--repack", action="store_true", help="Re-concatenate files, fixing checksum errors if any.");
@@ -65,15 +68,17 @@
 fname = getargs.format;
 fnamelower = fname.lower();
 fnamemagic = fname;
 fnamelen = len(fname);
 fnamehex = binascii.hexlify(fname.encode("UTF-8")).decode("UTF-8");
 fnamever = getargs.formatver;
 fnamesty = __use_new_style__;
-fnamelist = [fname, fnamemagic, fnamelower, fnamelen, fnamehex, getargs.delimiter, fnamever, fnamesty];
+fnamelst = __use_advanced_list__;
+fnameino = __use_alt_inode__;
+fnamelist = [fname, fnamemagic, fnamelower, fnamelen, fnamehex, getargs.delimiter, fnamever, fnamesty, fnamelst, fnameino];
 
 # Determine actions based on user input
 should_create = getargs.create and not getargs.extract and not getargs.list;
 should_extract = getargs.extract and not getargs.create and not getargs.list;
 should_list = getargs.list and not getargs.create and not getargs.extract;
 should_repack = getargs.create and getargs.repack;
 should_validate = getargs.validate;
@@ -86,28 +91,28 @@
   pycatfile.PackArchiveFileFromZipFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
  elif rarfile_support and getargs.convertrar:
   pycatfile.PackArchiveFileFromRarFile(getargs.input, getargs.output, getargs.compression, getargs.level, getargs.checksum, [], fnamelist, getargs.verbose, False);
  else:
   pycatfile.PackArchiveFile(getargs.input, getargs.output, getargs.text, getargs.compression, getargs.level, False, getargs.checksum, [], fnamelist, getargs.verbose, False);
 
 elif should_repack:
- pycatfile.RePackArchiveFile(getargs.input, getargs.output, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, False, [], fnamelist, getargs.verbose, False);
+ pycatfile.RePackArchiveFile(getargs.input, getargs.output, getargs.compression, getargs.level, False, 0, 0, getargs.checksum, getargs.skipchecksum, [], fnamelist, getargs.verbose, False);
 
 elif should_extract:
- pycatfile.UnPackArchiveFile(getargs.input, getargs.output, False, 0, 0, False, fnamelist, getargs.verbose, getargs.preserve, getargs.preserve, False);
+ pycatfile.UnPackArchiveFile(getargs.input, getargs.output, False, 0, 0, getargs.skipchecksum, fnamelist, getargs.verbose, getargs.preserve, getargs.preserve, False);
 
 elif should_list:
  if getargs.converttar:
   pycatfile.TarFileListFiles(getargs.input, getargs.verbose, False);
  elif getargs.convertzip:
   pycatfile.ZipFileListFiles(getargs.input, getargs.verbose, False);
  elif rarfile_support and getargs.convertrar:
   pycatfile.RarFileListFiles(getargs.input, getargs.verbose, False);
  else:
-  pycatfile.ArchiveFileListFiles(getargs.input, 0, 0, False, fnamelist, getargs.verbose, False);
+  pycatfile.ArchiveFileListFiles(getargs.input, 0, 0, getargs.skipchecksum, fnamelist, getargs.verbose, False);
 
 elif should_validate:
  fvalid = pycatfile.ArchiveFileValidate(getargs.input, fnamelist, getargs.verbose, False);
  if(fvalid):
-  pycatfile.VerbosePrintOut("File is valid: " + str(getargs.input));
+  pycatfile.VerbosePrintOut("File is valid: \n" + str(getargs.input));
  else:
-  pycatfile.VerbosePrintOut("File is invalid: " + str(getargs.input));
+  pycatfile.VerbosePrintOut("File is invalid: \n" + str(getargs.input));
```

### Comparing `PyCatFile-0.7.4/neocatfile.py` & `PyCatFile-0.7.6/neocatfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: neocatfile.py - Last Update: 4/1/2024 Ver. 0.7.4 RC 1 - Author: cooldude2k $
+    $FileInfo: neocatfile.py - Last Update: 4/10/2024 Ver. 0.7.6 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 import argparse
 import pycatfile
 
 # Compatibility layer for Python 2 and 3 input
```

### Comparing `PyCatFile-0.7.4/pycatfile.py` & `PyCatFile-0.7.6/pycatfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2018-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2018-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2018-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: pycatfile.py - Last Update: 4/1/2024 Ver. 0.7.4 RC 1 - Author: cooldude2k $
+    $FileInfo: pycatfile.py - Last Update: 4/10/2024 Ver. 0.7.6 RC 1 - Author: cooldude2k $
 '''
 
 from __future__ import absolute_import, division, print_function, unicode_literals;
 import io, os, re, sys, time, stat, zlib, base64, shutil, socket, hashlib, datetime, logging, binascii, tempfile, zipfile, platform;
 from ftplib import FTP, FTP_TLS;
 if(sys.version[0]=="2"):
  from urlparse import urlparse, urlunparse;
@@ -155,22 +155,24 @@
 __file_format_lower__ = __file_format_name__.lower();
 __file_format_magic__ = __file_format_name__;
 __file_format_len__ = len(__file_format_magic__);
 __file_format_hex__ = binascii.hexlify(__file_format_magic__.encode("UTF-8")).decode("UTF-8");
 __file_format_delimiter__ = "\x00";
 __file_format_ver__ = "001";
 __use_new_style__ = True;
-__file_format_list__ = [__file_format_name__, __file_format_magic__, __file_format_lower__, __file_format_len__, __file_format_hex__, __file_format_delimiter__, __file_format_ver__, __use_new_style__];
+__use_advanced_list__ = True;
+__use_alt_inode__ = False;
+__file_format_list__ = [__file_format_name__, __file_format_magic__, __file_format_lower__, __file_format_len__, __file_format_hex__, __file_format_delimiter__, __file_format_ver__, __use_new_style__, __use_advanced_list__, __use_alt_inode__];
 __project__ = __program_name__;
 __project_url__ = "https://github.com/GameMaker2k/PyCatFile";
-__version_info__ = (0, 7, 4, "RC 1", 1);
-__version_date_info__ = (2024, 4, 1, "RC 1", 1);
+__version_info__ = (0, 7, 6, "RC 1", 1);
+__version_date_info__ = (2024, 4, 10, "RC 1", 1);
 __version_date__ = str(__version_date_info__[0]) + "." + str(__version_date_info__[1]).zfill(2) + "." + str(__version_date_info__[2]).zfill(2);
 __revision__ = __version_info__[3];
-__revision_id__ = "$Id: 330c6ce992c910537524a1f38d1f5cfc7f1b5bbd $";
+__revision_id__ = "$Id: 9f413e59b208687ef02639cef9ddfc34278a2f0e $";
 if(__version_info__[4] is not None):
  __version_date_plusrc__ = __version_date__ + "-" + str(__version_date_info__[4]);
 if(__version_info__[4] is None):
  __version_date_plusrc__ = __version_date__;
 if(__version_info__[3] is not None):
  __version__ = str(__version_info__[0]) + "." + str(__version_info__[1]) + "." + str(__version_info__[2]) + " " + str(__version_info__[3]);
 if(__version_info__[3] is None):
@@ -569,36 +571,42 @@
   HeaderOut.append(ReadTillNullByte(fp, delimiter));
   rocount = rocount + 1;
  return HeaderOut;
 
 def ReadFileHeaderDataBySize(fp, delimiter=__file_format_delimiter__):
  headerpresize = ReadTillNullByte(fp, delimiter);
  headersize = int(headerpresize, 16);
+ if(headersize<=0):
+  return [];
  headercontent = str(fp.read(headersize).decode('UTF-8')).split(delimiter);
  fp.seek(1, 1);
  rocount = 0;
  roend = int(len(headercontent));
  HeaderOut = [headerpresize];
  while(rocount<roend):
   HeaderOut.append(headercontent[rocount]);
   rocount = rocount + 1;
  return HeaderOut;
 
 def ReadFileHeaderDataWoSize(fp, delimiter=__file_format_delimiter__):
  preheaderdata = ReadFileHeaderData(fp, 2, delimiter);
  headersize = int(preheaderdata[0], 16);
  headernumfields = int(preheaderdata[1], 16);
+ if(headersize<=0 or headernumfields<=0):
+  return [];
  headerdata = ReadFileHeaderData(fp, headernumfields, delimiter);
  HeaderOut = preheaderdata + headerdata;
  return HeaderOut;
 
 def ReadFileHeaderDataBySizeWithContent(fp, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
  delimiter = formatspecs[5];
  fheaderstart = fp.tell();
  HeaderOut = ReadFileHeaderDataBySize(fp, delimiter);
+ if(len(HeaderOut)==0):
+  return False;
  if(re.findall("^[.|/]", HeaderOut[3])):
   fname = HeaderOut[3];
  else:
   fname = "./"+HeaderOut[3];
  fchecksumtype = HeaderOut[-3].lower();
  fcs = HeaderOut[-2].lower();
  fccs = HeaderOut[-1].lower();
@@ -626,14 +634,16 @@
 def ReadFileHeaderDataBySizeWithContentToArray(fp, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
  delimiter = formatspecs[5];
  fheaderstart = fp.tell();
  if(formatspecs[7]):
   HeaderOut = ReadFileHeaderDataBySize(fp, delimiter);
  else:
   HeaderOut = ReadFileHeaderDataWoSize(fp, delimiter);
+ if(len(HeaderOut)==0):
+  return False;
  fheadsize = int(HeaderOut[0], 16);
  fnumfields = int(HeaderOut[1], 16);
  ftype = int(HeaderOut[2], 16);
  if(re.findall("^[.|/]", HeaderOut[3])):
   fname = HeaderOut[3];
  else:
   fname = "./"+HeaderOut[3];
@@ -697,14 +707,16 @@
 def ReadFileHeaderDataBySizeWithContentToList(fp, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
  delimiter = formatspecs[5];
  fheaderstart = fp.tell();
  if(formatspecs[7]):
   HeaderOut = ReadFileHeaderDataBySize(fp, delimiter);
  else:
   HeaderOut = ReadFileHeaderDataWoSize(fp, delimiter);
+ if(len(HeaderOut)==0):
+  return False;
  fheadsize = int(HeaderOut[0], 16);
  fnumfields = int(HeaderOut[1], 16);
  ftype = int(HeaderOut[2], 16);
  if(re.findall("^[.|/]", HeaderOut[3])):
   fname = HeaderOut[3];
  else:
   fname = "./"+HeaderOut[3];
@@ -763,30 +775,43 @@
  fp.seek(1, 1);
  fcontentend = fp.tell() - 1;
  catlist = [ftype, fname, flinkname, fsize, fatime, fmtime, fctime, fbtime, fmode, fwinattributes, fuid, funame, fgid, fgname, fid, finode, flinkcount, fdev_minor, fdev_major, frdev_minor, frdev_major, extrafieldslist, fchecksumtype, fcontents];
  return catlist;
 
 def ReadFileDataBySizeWithContent(fp, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
  delimiter = formatspecs[5];
+ curloc = fp.tell();
+ if(curloc>0):
+  fp.seek(0, 0);
  catheader = ReadFileHeaderData(fp, 4, delimiter);
+ if(curloc>0):
+  fp.seek(curloc, 0);
  headercheck = ValidateHeaderChecksum(catheader[:-1], catheader[2], catheader[3], formatspecs);
  if(not headercheck and not skipchecksum):
   VerbosePrintOut("File Header Checksum Error with file at offset " + str(0));
   return False;
  fnumfiles = int(catheader[1], 16);
  countnum = 0;
  flist = [];
  while(countnum < fnumfiles):
-  flist.append(ReadFileHeaderDataBySizeWithContent(fp, listonly, skipchecksum, formatspecs));
+  HeaderOut = ReadFileHeaderDataBySizeWithContent(fp, listonly, skipchecksum, formatspecs)
+  if(len(HeaderOut)==0):
+   break;
+  flist.append(HeaderOut);
   countnum = countnum + 1;
  return flist;
 
 def ReadFileDataBySizeWithContentToArray(fp, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
  delimiter = formatspecs[5];
+ curloc = fp.tell();
+ if(curloc>0):
+  fp.seek(0, 0);
  catheader = ReadFileHeaderData(fp, 4, delimiter);
+ if(curloc>0):
+  fp.seek(curloc, 0);
  headercheck = ValidateHeaderChecksum(catheader[:-1], catheader[2], catheader[3], formatspecs);
  if(not headercheck and not skipchecksum):
   VerbosePrintOut("File Header Checksum Error with file at offset " + str(0));
   return False;
  catstring = catheader[0];
  catversion = re.findall(r"([\d]+)$", catstring);
  catversions = re.search(r'(.*?)(\d+)$', catstring).groups();
@@ -802,14 +827,16 @@
  elif(seekend<0 and abs(seekend)<=fnumfiles and abs(seekend)>=seekstart):
   seekend = fnumfiles - abs(seekend);
  if(seekstart>0):
   il = 0;
   while(il < seekstart):
    prefhstart = fp.tell();
    preheaderdata = ReadFileHeaderDataBySize(fp, formatspecs[5]);
+   if(len(preheaderdata)==0):
+    break;
    prefsize = int(preheaderdata[5], 16);
    prenewfcs = GetHeaderChecksum(preheaderdata[:-2], preheaderdata[-3].lower(), True, formatspecs);
    prefcs = preheaderdata[-2];
    if(prefcs!=prenewfcs and not skipchecksum):
     VerbosePrintOut("File Header Checksum Error with file " + prefname + " at offset " + str(prefhstart));
     return False;
     valid_archive = False;
@@ -828,15 +855,18 @@
      return False;
    fp.seek(1, 1);
    il = il + 1;
  realidnum = 0;
  countnum = seekstart;
  while(countnum < seekend):
   catlist['ffilelist'].update({realidnum: {'fid': realidnum, 'fidalt': realidnum}});
-  catlist['ffilelist'][realidnum].update(ReadFileHeaderDataBySizeWithContentToArray(fp, listonly, skipchecksum, formatspecs));
+  HeaderOut = ReadFileHeaderDataBySizeWithContentToArray(fp, listonly, skipchecksum, formatspecs);
+  if(len(HeaderOut)):
+   break;
+  catlist['ffilelist'][realidnum].update(HeaderOut);
   countnum = countnum + 1;
   realidnum = realidnum + 1;
  return catlist;
 
 def ReadFileDataBySizeWithContentToArrayIndex(infile, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
  if(isinstance(infile, dict)):
   listcatfiles = infile;
@@ -891,15 +921,20 @@
    catarray['filetypes']['devices']['filetoid'].update(filetoidarray);
    catarray['filetypes']['devices']['idtofile'].update(idtofilearray);
   lcfi = lcfi + 1;
  return catarray;
 
 def ReadFileDataBySizeWithContentToList(fp, seekstart=0, seekend=0, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
  delimiter = formatspecs[5];
+ curloc = fp.tell();
+ if(curloc>0):
+  fp.seek(0, 0);
  catheader = ReadFileHeaderData(fp, 4, delimiter);
+ if(curloc>0):
+  fp.seek(curloc, 0);
  headercheck = ValidateHeaderChecksum(catheader[:-1], catheader[2], catheader[3], formatspecs);
  if(not headercheck and not skipchecksum):
   VerbosePrintOut("File Header Checksum Error with file at offset " + str(0));
   return False;
  catstring = catheader[0];
  catversion = re.findall(r"([\d]+)$", catstring);
  catversions = re.search(r'(.*?)(\d+)$', catstring).groups();
@@ -915,14 +950,16 @@
  elif(seekend<0 and abs(seekend)<=fnumfiles and abs(seekend)>=seekstart):
   seekend = fnumfiles - abs(seekend);
  if(seekstart>0):
   il = 0;
   while(il < seekstart):
    prefhstart = fp.tell();
    preheaderdata = ReadFileHeaderDataBySize(fp, formatspecs[5]);
+   if(len(preheaderdata)==0):
+    break;
    prefsize = int(preheaderdata[5], 16);
    prenewfcs = GetHeaderChecksum(preheaderdata[:-2], preheaderdata[-3].lower(), True, formatspecs);
    prefcs = preheaderdata[-2];
    if(prefcs!=prenewfcs and not skipchecksum):
     VerbosePrintOut("File Header Checksum Error with file " + prefname + " at offset " + str(prefhstart));
     return False;
     valid_archive = False;
@@ -940,15 +977,18 @@
      VerbosePrintOut("File Content Checksum Error with file " + prefname + " at offset " + str(prefcontentstart));
      return False;
    fp.seek(1, 1);
    il = il + 1;
  realidnum = 0;
  countnum = seekstart;
  while(countnum < seekend):
-  catlist.append(ReadFileHeaderDataBySizeWithContentToList(fp, listonly, skipchecksum, formatspecs));
+  HeaderOut = ReadFileHeaderDataBySizeWithContentToList(fp, listonly, skipchecksum, formatspecs);
+  if(len(HeaderOut)):
+   break;
+  catlist.append(HeaderOut);
   countnum = countnum + 1;
   realidnum = realidnum + 1;
  return catlist;
 
 def ReadInFileBySizeWithContentToArray(infile, listonly=False, skipchecksum=False, formatspecs=__file_format_list__):
  delimiter = formatspecs[5];
  if(hasattr(infile, "read") or hasattr(infile, "write")):
@@ -1185,15 +1225,16 @@
  except io.UnsupportedOperation:
   pass;
  except AttributeError:
   pass;
  return fp;
 
 def AppendFilesWithContent(infiles, fp, dirlistfromtxt=False, filevalues=[], extradata=[], followlink=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False):
- advancedlist = True;
+ advancedlist = formatspecs[8];
+ altinode = formatspecs[9];
  if(verbose):
   logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
  if(infiles=="-"):
   for line in sys.stdin:
    infilelist.append(line.strip());
   infilelist = list(filter(None, infilelist));
  elif(infiles!="-" and dirlistfromtxt and os.path.exists(infiles) and (os.path.isfile(infiles) or infiles=="/dev/null" or infiles=="NUL")):
@@ -1216,17 +1257,17 @@
   return False;
  curinode = 0;
  curfid = 0;
  inodelist = [];
  inodetofile = {};
  filetoinode = {};
  inodetocatinode = {};
- fnumfiles = int(len(GetDirList));
+ numfiles = int(len(GetDirList));
+ fnumfiles = format(numfiles, 'x').lower();
  AppendFileHeader(fp, fnumfiles, checksumtype, formatspecs);
- fnumfiles = format(fnumfiles, 'x').lower();
  for curfname in GetDirList:
   catfhstart = fp.tell();
   if(re.findall("^[.|/]", curfname)):
    fname = curfname;
   else:
    fname = "./"+curfname;
   if(verbose):
@@ -1264,20 +1305,26 @@
   flinkname = "";
   fcurfid = format(int(curfid), 'x').lower();
   if(not followlink and finode!=0):
    if(ftype!=1):
     if(finode in inodelist):
      ftype = 1;
      flinkname = inodetofile[finode];
-     fcurinode = format(int(inodetocatinode[finode]), 'x').lower();
+     if(altinode):
+      fcurinode = format(int(finode), 'x').lower();
+     else:
+      fcurinode = format(int(inodetocatinode[finode]), 'x').lower();
     if(finode not in inodelist):
      inodelist.append(finode);
      inodetofile.update({finode: fname});
      inodetocatinode.update({finode: curinode});
-     fcurinode = format(int(curinode), 'x').lower();
+     if(altinode):
+      fcurinode = format(int(finode), 'x').lower();
+     else:
+      fcurinode = format(int(curinode), 'x').lower();
      curinode = curinode + 1;
   else:
    fcurinode = format(int(curinode), 'x').lower();
    curinode = curinode + 1;
   curfid = curfid + 1;
   if(ftype==2):
    flinkname = os.readlink(fname);
@@ -1357,33 +1404,34 @@
      chunk = fpc.read(chunk_size);
      if(not chunk):
       break;
      fcontents += chunk;
   ftypehex = format(ftype, 'x').lower();
   catoutlist = [ftypehex, fname, flinkname, fsize, fatime, fmtime, fctime, fbtime, fmode, fwinattributes, fuid, funame, fgid, fgname, fcurfid, fcurinode, flinkcount, fdev_minor, fdev_major, frdev_minor, frdev_major];
   fp = AppendFileHeaderWithContent(fp, catoutlist, extradata, fcontents, checksumtype, formatspecs);
+ if(numfiles>0):
+  catfp.write(AppendNullBytes([0, 0], formatspecs[5]).encode("UTF-8"));
  fp.seek(0, 0);
  return fp;
 
 def AppendListsWithContent(inlist, fp, dirlistfromtxt=False, filevalues=[], extradata=[], followlink=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False):
- advancedlist = True;
  if(verbose):
   logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging.DEBUG);
  GetDirList = inlist;
  if(not GetDirList):
   return False;
  curinode = 0;
  curfid = 0;
  inodelist = [];
  inodetofile = {};
  filetoinode = {};
  inodetocatinode = {};
- fnumfiles = int(len(GetDirList));
+ numfiles = int(len(GetDirList));
+ fnumfiles = format(numfiles, 'x').lower();
  AppendFileHeader(fp, fnumfiles, checksumtype, formatspecs);
- fnumfiles = format(fnumfiles, 'x').lower();
  for curfname in GetDirList:
   ftype = format(curfname[0], 'x').lower();
   if(re.findall("^[.|/]", curfname[1])):
    fname = curfname[1];
   else:
    fname = "./"+curfname[1];
   fbasedir = os.path.dirname(fname);
@@ -1407,14 +1455,16 @@
   frdev_minor = format(curfname[19], 'x').lower();
   frdev_major = format(curfname[20], 'x').lower();
   extradata = curfname[21];
   fchecksumtype = curfname[22];
   fcontents = curfname[23];
   catoutlist = [ftype, fname, flinkname, fsize, fatime, fmtime, fctime, fbtime, fmode, fwinattributes, fuid, funame, fgid, fgname, fid, finode, flinkcount, fdev_minor, fdev_major, frdev_minor, frdev_major];
   fp = AppendFileHeaderWithContent(fp, catoutlist, extradata, fcontents, checksumtype, formatspecs);
+ if(numfiles>0):
+  catfp.write(AppendNullBytes([0, 0], formatspecs[5]).encode("UTF-8"));
  fp.seek(0, 0);
  return fp;
 
 def AppendInFileWithContent(infile, fp, dirlistfromtxt=False, filevalues=[], extradata=[], followlink=False, checksumtype="crc32", formatspecs=__file_format_list__, verbose=False):
  inlist = ReadInFileBySizeWithContentToList(infile, 0, 0, False, False, formatspecs);
  return AppendListsWithContent(inlist, fp, dirlistfromtxt, filevalues, extradata, followlink, checksumtype, formatspecs, verbose);
 
@@ -2191,15 +2241,16 @@
  checklistout = hash_list;
  if(checkfor in checklistout):
   return True;
  else:
   return False;
 
 def PackArchiveFile(infiles, outfile, dirlistfromtxt=False, compression="auto", compressionlevel=None, followlink=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False, returnfp=False):
- advancedlist = True;
+ advancedlist = formatspecs[8];
+ altinode = formatspecs[9];
  if(outfile!="-" and not hasattr(outfile, "read") and not hasattr(outfile, "write")):
   outfile = RemoveWindowsPath(outfile);
  checksumtype = checksumtype.lower();
  if(not CheckSumSupport(checksumtype, hashlib_guaranteed)):
   checksumtype="crc32";
  if(checksumtype=="none"):
   checksumtype = "";
@@ -2252,14 +2303,15 @@
   return False;
  curinode = 0;
  curfid = 0;
  inodelist = [];
  inodetofile = {};
  filetoinode = {};
  inodetocatinode = {};
+ numfiles = int(len(GetDirList));
  fnumfiles = format(int(len(GetDirList)), 'x').lower();
  fnumfilesa = AppendNullBytes([fnumfiles, checksumtype], formatspecs[5]);
  if(checksumtype=="none" or checksumtype==""):
   catfileheadercshex = format(0, 'x').lower();
  elif(checksumtype=="crc16" or checksumtype=="crc16_ansi" or checksumtype=="crc16_ibm"):
   catfileheadercshex = format(crc16(str(fileheader + fnumfilesa).encode('UTF-8')) & 0xffff, '04x').lower();
  elif(checksumtype=="crc16_ccitt"):
@@ -2328,20 +2380,26 @@
   flinkname = "";
   fcurfid = format(int(curfid), 'x').lower();
   if(not followlink and finode!=0):
    if(ftype!=1):
     if(finode in inodelist):
      ftype = 1;
      flinkname = inodetofile[finode];
-     fcurinode = format(int(inodetocatinode[finode]), 'x').lower();
+     if(altinode):
+      fcurinode = format(int(finode), 'x').lower();
+     else:
+      fcurinode = format(int(inodetocatinode[finode]), 'x').lower();
     if(finode not in inodelist):
      inodelist.append(finode);
      inodetofile.update({finode: fname});
      inodetocatinode.update({finode: curinode});
-     fcurinode = format(int(curinode), 'x').lower();
+     if(altinode):
+      fcurinode = format(int(finode), 'x').lower();
+     else:
+      fcurinode = format(int(curinode), 'x').lower();
      curinode = curinode + 1;
   else:
    fcurinode = format(int(curinode), 'x').lower();
    curinode = curinode + 1;
   curfid = curfid + 1;
   if(ftype==2):
    flinkname = os.readlink(fname);
@@ -2501,14 +2559,16 @@
   try:
    catfp.flush();
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
   except AttributeError:
    pass;
+ if(numfiles>0):
+  catfp.write(AppendNullBytes([0, 0], formatspecs[5]).encode("UTF-8"));
  if(outfile=="-" or hasattr(outfile, "read") or hasattr(outfile, "write")):
   catfp = CompressArchiveFile(catfp, compression, formatspecs);
   try:
    catfp.flush();
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
@@ -2609,14 +2669,15 @@
  try:
   if(hasattr(infile, "read") or hasattr(infile, "write")):
    tarfp = tarfile.open(fileobj=infile, mode="r");
   else:
    tarfp = tarfile.open(infile, "r");
  except FileNotFoundError:
   return False;
+ numfiles = int(len(tarfp.getmembers()));
  fnumfiles = format(int(len(tarfp.getmembers())), 'x').lower();
  fnumfilesa = AppendNullBytes([fnumfiles, checksumtype], formatspecs[5]);
  if(checksumtype=="none" or checksumtype==""):
   catfileheadercshex = format(0, 'x').lower();
  elif(checksumtype=="crc16" or checksumtype=="crc16_ansi" or checksumtype=="crc16_ibm"):
   catfileheadercshex = format(crc16(str(fileheader + fnumfilesa).encode('UTF-8')) & 0xffff, '04x').lower();
  elif(checksumtype=="crc16_ccitt"):
@@ -2803,14 +2864,16 @@
   try:
    catfp.flush();
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
   except AttributeError:
    pass;
+ if(numfiles>0):
+  catfp.write(AppendNullBytes([0, 0], formatspecs[5]).encode("UTF-8"));
  if(outfile=="-" or hasattr(outfile, "read") or hasattr(outfile, "write")):
   catfp = CompressArchiveFile(catfp, compression, formatspecs);
   try:
    catfp.flush();
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
@@ -2898,14 +2961,15 @@
  try:
   zipfp = zipfile.ZipFile(infile, "r", allowZip64=True);
  except FileNotFoundError:
   return False;
  ziptest = zipfp.testzip();
  if(ziptest):
   VerbosePrintOut("Bad file found!");
+ numfiles = int(len(zipfp.infolist()));
  fnumfiles = format(int(len(zipfp.infolist())), 'x').lower();
  fnumfilesa = AppendNullBytes([fnumfiles, checksumtype], formatspecs[5]);
  if(checksumtype=="none" or checksumtype==""):
   catfileheadercshex = format(0, 'x').lower();
  elif(checksumtype=="crc16" or checksumtype=="crc16_ansi" or checksumtype=="crc16_ibm"):
   catfileheadercshex = format(crc16(str(fileheader + fnumfilesa).encode('UTF-8')) & 0xffff, '04x').lower();
  elif(checksumtype=="crc16_ccitt"):
@@ -3112,14 +3176,16 @@
   try:
    catfp.flush();
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
   except AttributeError:
    pass;
+ if(numfiles>0):
+  catfp.write(AppendNullBytes([0, 0], formatspecs[5]).encode("UTF-8"));
  if(outfile=="-" or hasattr(outfile, "read") or hasattr(outfile, "write")):
   catfp = CompressArchiveFile(catfp, compression, formatspecs);
   try:
    catfp.flush();
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
@@ -3191,14 +3257,15 @@
    return False;
   if(not rarfile.is_rarfile(infile) and not rarfile.is_rarfile_sfx(infile)):
    return False;
   rarfp = rarfile.RarFile(infile, "r");
   rartest = rarfp.testrar();
   if(rartest):
    VerbosePrintOut("Bad file found!");
+  numfiles = int(len(rarfp.infolist()));
   fnumfiles = format(int(len(rarfp.infolist())), 'x').lower();
   fnumfilesa = AppendNullBytes([fnumfiles, checksumtype], formatspecs[5]);
   if(checksumtype=="none" or checksumtype==""):
    catfileheadercshex = format(0, 'x').lower();
   elif(checksumtype=="crc16" or checksumtype=="crc16_ansi" or checksumtype=="crc16_ibm"):
    catfileheadercshex = format(crc16(str(fileheader + fnumfilesa).encode('UTF-8')) & 0xffff, '04x').lower();
   elif(checksumtype=="crc16_ccitt"):
@@ -3439,14 +3506,16 @@
    try:
     catfp.flush()
     os.fsync(catfp.fileno())
    except io.UnsupportedOperation:
     pass
    except AttributeError:
     pass
+  if(numfiles>0):
+   catfp.write(AppendNullBytes([0, 0], formatspecs[5]).encode("UTF-8"));
   if(outfile=="-" or hasattr(outfile, "read") or hasattr(outfile, "write")):
    catfp = CompressArchiveFile(catfp, compression, formatspecs)
    try:
     catfp.flush()
     os.fsync(catfp.fileno())
    except io.UnsupportedOperation:
     pass
@@ -3549,15 +3618,20 @@
  '''
  try:
   catfp.seek(0, 0);
  except OSError:
   return False;
  except ValueError:
   return False;
+ curloc = catfp.tell();
+ if(curloc>0):
+  catfp.seek(0, 0);
  catheader = ReadFileHeaderData(catfp, 4, formatspecs[5]);
+ if(curloc>0):
+  catfp.seek(curloc, 0);
  catstring = catheader[0];
  catversion = re.findall(r"([\d]+)$", catstring);
  fprenumfiles = catheader[1];
  fnumfiles = int(fprenumfiles, 16);
  fprechecksumtype = catheader[2];
  fprechecksum = catheader[3];
  fileheader = AppendNullByte(catstring, formatspecs[5]);
@@ -3598,14 +3672,16 @@
   il = -1;
   while(il < seekto):
    prefhstart = catfp.tell();
    if(formatspecs[7]):
     preheaderdata = ReadFileHeaderDataBySize(catfp, formatspecs[5]);
    else:
     preheaderdata = ReadFileHeaderDataWoSize(catfp, formatspecs[5]);
+   if(len(preheaderdata)==0):
+    break;
    prefheadsize = int(preheaderdata[0], 16);
    prefnumfields = int(preheaderdata[1], 16);
    preftype = int(preheaderdata[2], 16);
    if(re.findall("^[.|/]", preheaderdata[3])):
     prefname = preheaderdata[3];
    else:
     prefname = "./"+preheaderdata[3];
@@ -3799,15 +3875,20 @@
  '''
  try:
   catfp.seek(0, 0);
  except OSError:
   return False;
  except ValueError:
   return False;
+ curloc = catfp.tell();
+ if(curloc>0):
+  catfp.seek(0, 0);
  catheader = ReadFileHeaderData(catfp, 4, formatspecs[5]);
+ if(curloc>0):
+  catfp.seek(curloc, 0);
  catstring = catheader[0];
  catversion = re.findall(r"([\d]+)$", catstring);
  fprenumfiles = catheader[1];
  fnumfiles = int(fprenumfiles, 16);
  fprechecksumtype = catheader[2];
  fprechecksum = catheader[3];
  fileheader = AppendNullByte(catstring, formatspecs[5]);
@@ -3846,14 +3927,16 @@
   il = -1;
   while(il < seekto):
    prefhstart = catfp.tell();
    if(formatspecs[7]):
     preheaderdata = ReadFileHeaderDataBySize(catfp, formatspecs[5]);
    else:
     preheaderdata = ReadFileHeaderDataWoSize(catfp, formatspecs[5]);
+   if(len(preheaderdata)==0):
+    break;
    prefheadsize = int(preheaderdata[0], 16);
    prefnumfields = int(preheaderdata[1], 16);
    preftype = int(preheaderdata[2], 16);
    if(re.findall("^[.|/]", preheaderdata[3])):
     prefname = preheaderdata[3];
    else:
     prefname = "./"+preheaderdata[3];
@@ -4061,15 +4144,20 @@
  '''
  try:
   catfp.seek(0, 0);
  except OSError:
   return False;
  except ValueError:
   return False;
+ curloc = catfp.tell();
+ if(curloc>0):
+  catfp.seek(0, 0);
  catheader = ReadFileHeaderData(catfp, 4, formatspecs[5]);
+ if(curloc>0):
+  catfp.seek(curloc, 0);
  catstring = catheader[0];
  catversion = re.findall(r"([\d]+)$", catstring);
  fprenumfiles = catheader[1];
  fnumfiles = int(fprenumfiles, 16);
  fprechecksumtype = catheader[2];
  fprechecksum = catheader[3];
  il = 0; 
@@ -4096,30 +4184,34 @@
   catfileheadercshex = checksumoutstr.hexdigest().lower();
  else:
   catfileheadercshex = format(0, 'x').lower();
  fileheader = fileheader + AppendNullByte(catfileheadercshex, formatspecs[5]);
  valid_archive = True;
  invalid_archive = False;
  if(verbose):
-  VerbosePrintOut("Checking File Header Checksum of file at offset " + str(0));
   VerbosePrintOut(infile);
+  VerbosePrintOut("Number of Records " + str(fnumfiles));
  if(fprechecksum==catfileheadercshex):
   if(verbose):
-   VerbosePrintOut("File Header Checksum Passed");
+   VerbosePrintOut("File Header Checksum Passed at offset " + str(0));
  else:
   if(verbose):
-   VerbosePrintOut("File Header Checksum Error with file " + infile + " at offset " + str(0));
-  valid_archive = False;
-  invalid_archive = True;
+   VerbosePrintOut("File Header Checksum Failed at offset " + str(0));
+   valid_archive = False;
+   invalid_archive = True;
+ if(verbose):
+  VerbosePrintOut("");
  while(il<fnumfiles):
   catfhstart = catfp.tell();
   if(formatspecs[7]):
    catheaderdata = ReadFileHeaderDataBySize(catfp, formatspecs[5]);
   else:
    catheaderdata = ReadFileHeaderDataWoSize(catfp, formatspecs[5]);
+  if(len(catheaderdata)==0):
+   break;
   catfheadsize = int(catheaderdata[0], 16);
   catfnumfields = int(catheaderdata[1], 16);
   catftype = int(catheaderdata[2], 16);
   if(re.findall("^[.|/]", catheaderdata[3])):
    catfname = catheaderdata[3];
   else:
    catfname = "./"+catheaderdata[3];
@@ -4176,22 +4268,22 @@
   elif(catfchecksumtype=="crc64" or catfchecksumtype=="crc64_iso"):
    catnewfcs = format(crc64_iso(hout.encode('UTF-8')) & 0xffffffffffffffff, '016x').lower();
   elif(CheckSumSupportAlt(catfchecksumtype, hashlib_guaranteed)):
    checksumoutstr = hashlib.new(catfchecksumtype);
    checksumoutstr.update(hout.encode('UTF-8'));
    catnewfcs = checksumoutstr.hexdigest().lower();
   if(verbose):
-   VerbosePrintOut("Checking File Header Checksum of file at offset " + str(catfhstart));
    VerbosePrintOut(catfname);
+   VerbosePrintOut("Record Number " + str(il) + "; File ID " + str(fid) + "; iNode Number " + str(finode));
   if(catfcs==catnewfcs):
    if(verbose):
-    VerbosePrintOut("File Header Checksum Passed");
+    VerbosePrintOut("File Header Checksum Passed at offset " + str(catfhstart));
   else:
    if(verbose):
-    VerbosePrintOut("File Header Checksum Error with file " + catfname + " at offset " + str(catfhstart));
+    VerbosePrintOut("File Header Checksum Failed at offset " + str(catfhstart));
    valid_archive = False;
    invalid_archive = True;
   catfhend = catfp.tell() - 1;
   catfcontentstart = catfp.tell();
   catfcontents = "";
   pyhascontents = False;
   if(catfsize>0):
@@ -4211,23 +4303,20 @@
    elif(catfchecksumtype=="crc64" or catfchecksumtype=="crc64_iso"):
     catnewfcs = format(crc64_iso(catfcontents) & 0xffffffffffffffff, '016x').lower();
    elif(CheckSumSupportAlt(catfchecksumtype, hashlib_guaranteed)):
     checksumoutstr = hashlib.new(catfchecksumtype);
     checksumoutstr.update(catfcontents);
     catnewfccs = checksumoutstr.hexdigest().lower();
    pyhascontents = True;
-   if(verbose):
-    VerbosePrintOut("Checking File Content Checksum of file at offset " + str(catfcontentstart));
-    VerbosePrintOut(catfname);
    if(catfccs==catnewfccs):
     if(verbose):
-     VerbosePrintOut("File Content Checksum Passed");
+     VerbosePrintOut("File Content Checksum Passed at offset " + str(catfcontentstart));
    else:
     if(verbose):
-     VerbosePrintOut("File Header Checksum Error with file " + catfname + " at offset " + str(catfcontentstart));
+     VerbosePrintOut("File Content Checksum Failed at offset " + str(catfcontentstart));
     valid_archive = False;
     invalid_archive = True;
   if(verbose):
    VerbosePrintOut("");
   catfp.seek(1, 1);
   il = il + 1;
  if(valid_archive):
@@ -4320,15 +4409,20 @@
  '''
  try:
   catfp.seek(0, 0);
  except OSError:
   return False;
  except ValueError:
   return False;
+ curloc = catfp.tell();
+ if(curloc>0):
+  catfp.seek(0, 0);
  catheader = ReadFileHeaderData(catfp, 4, formatspecs[5]);
+ if(curloc>0):
+  catfp.seek(curloc, 0);
  catstring = catheader[0];
  catversion = re.findall(r"([\d]+)$", catstring);
  fprenumfiles = catheader[1];
  fnumfiles = int(fprenumfiles, 16);
  fprechecksumtype = catheader[2];
  fprechecksum = catheader[3];
  fileheader = AppendNullByte(catstring, formatspecs[5]);
@@ -4371,14 +4465,16 @@
   il = 0;
   while(il < seekstart):
    prefhstart = catfp.tell();
    if(formatspecs[7]):
     preheaderdata = ReadFileHeaderDataBySize(catfp, formatspecs[5]);
    else:
     preheaderdata = ReadFileHeaderDataWoSize(catfp, formatspecs[5]);
+   if(len(preheaderdata)==0):
+    break;
    prefheadsize = int(preheaderdata[0], 16);
    prefnumfields = int(preheaderdata[1], 16);
    if(re.findall("^[.|/]", preheaderdata[3])):
     prefname = preheaderdata[3];
    else:
     prefname = "./"+preheaderdata[3];
    prefsize = int(preheaderdata[5], 16);
@@ -4455,14 +4551,16 @@
  realidnum = 0;
  while(fileidnum<seekend):
   catfhstart = catfp.tell();
   if(formatspecs[7]):
    catheaderdata = ReadFileHeaderDataBySize(catfp, formatspecs[5]);
   else:
    catheaderdata = ReadFileHeaderDataWoSize(catfp, formatspecs[5]);
+  if(len(catheaderdata)==0):
+   break;
   catfheadsize = int(catheaderdata[0], 16);
   catfnumfields = int(catheaderdata[1], 16);
   catftype = int(catheaderdata[2], 16);
   if(re.findall("^[.|/]", catheaderdata[3])):
    catfname = catheaderdata[3];
   else:
    catfname = "./"+catheaderdata[3];
@@ -4599,15 +4697,16 @@
   listcatfiles = ArchiveFileToArray(catfp, seekstart, seekend, listonly, skipchecksum, formatspecs, returnfp);
   return listcatfiles;
 
 def ListDirToArrayAlt(infiles, dirlistfromtxt=False, followlink=False, listonly=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False):
  catver = formatspecs[6];
  fileheaderver = str(int(catver.replace(".", "")));
  fileheader = AppendNullByte(formatspecs[1] + fileheaderver, formatspecs[5]);
- advancedlist = True;
+ advancedlist = formatspecs[8];
+ altinode = formatspecs[9];
  infilelist = [];
  if(infiles=="-"):
   for line in sys.stdin:
    infilelist.append(line.strip());
   infilelist = list(filter(None, infilelist));
  elif(infiles!="-" and dirlistfromtxt and os.path.exists(infiles) and (os.path.isfile(infiles) or infiles=="/dev/null" or infiles=="NUL")):
   if(not os.path.exists(infiles) or not os.path.isfile(infiles)):
@@ -4706,20 +4805,26 @@
   fbasedir = os.path.dirname(fname);
   fcurfid = curfid;
   if(not followlink and finode!=0):
    if(ftype!=1):
     if(finode in inodelist):
      ftype = 1;
      flinkname = inodetofile[finode];
-     fcurinode = inodetocatinode[finode];
+     if(altinode):
+      fcurinode = finode;
+     else:
+      fcurinode = inodetocatinode[finode];
     if(finode not in inodelist):
      inodelist.append(finode);
      inodetofile.update({finode: fname});
      inodetocatinode.update({finode: curinode});
-     fcurinode = curinode;
+     if(altinode):
+      fcurinode = finode;
+     else:
+      fcurinode = curinode;
      curinode = curinode + 1;
   else:
    fcurinode = curinode;
    curinode = curinode + 1;
   curfid = curfid + 1;
   if(ftype==2):
    flinkname = os.readlink(fname);
@@ -5135,15 +5240,14 @@
    fcontents = "";
    pyhascontents = False;
   catlist['ffilelist'].update({fileidnum: {'fid': fileidnum, 'fidalt': fileidnum, 'fheadersize': int(catheaersize, 16), 'fhstart': catfhstart, 'fhend': catfhend, 'ftype': ftype, 'fname': fname, 'fbasedir': fbasedir, 'flinkname': flinkname, 'fsize': fsize, 'fatime': fatime, 'fmtime': fmtime, 'fctime': fctime, 'fbtime': fbtime, 'fmode': fmode, 'fchmode': fchmode, 'ftypemod': ftypemod, 'fwinattributes': fwinattributes, 'fuid': fuid, 'funame': funame, 'fgid': fgid, 'fgname': fgname, 'finode': finode, 'flinkcount': flinkcount, 'fminor': fdev_minor, 'fmajor': fdev_major, 'frminor': frdev_minor, 'frmajor': frdev_major, 'fchecksumtype': checksumtype, 'fnumfields': catfnumfields + 2, 'frawheader': catheaderdata, 'fextrafields': catfextrafields, 'fextrafieldsize': extrasizelen, 'fextralist': extrafieldslist, 'fheaderchecksum': int(catfileheadercshex, 16), 'fcontentchecksum': int(catfilecontentcshex, 16), 'fhascontents': pyhascontents, 'fcontentstart': catfcontentstart, 'fcontentend': catfcontentend, 'fcontents': fcontents} });
   fileidnum = fileidnum + 1;
  return catlist;
 
 def ZipFileToArrayAlt(infiles, listonly=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False):
- advancedlist = True;
  curinode = 0;
  curfid = 0;
  inodelist = [];
  inodetofile = {};
  filetoinode = {};
  inodetocatinode = {};
  fileidnum = 0;
@@ -5401,15 +5505,14 @@
 
 if(not rarfile_support):
  def RarFileToArrayAlt(infiles, listonly=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False):
   return False;
 
 if(rarfile_support):
  def RarFileToArrayAlt(infiles, listonly=False, checksumtype="crc32", extradata=[], formatspecs=__file_format_list__, verbose=False):
-  advancedlist = True;
   curinode = 0;
   curfid = 0;
   inodelist = [];
   inodetofile = {};
   filetoinode = {};
   inodetocatinode = {};
   fileidnum = 0;
@@ -6262,14 +6365,16 @@
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
   except AttributeError:
    pass;
   lcfi = lcfi + 1;
   reallcfi = reallcfi + 1;
+ if(lcfx>0):
+  catfp.write(AppendNullBytes([0, 0], formatspecs[5]).encode("UTF-8"));
  if(outfile=="-" or hasattr(outfile, "read") or hasattr(outfile, "write")):
   catfp = CompressArchiveFile(catfp, compression, formatspecs);
   try:
    catfp.flush();
    os.fsync(catfp.fileno());
   except io.UnsupportedOperation:
    pass;
```

### Comparing `PyCatFile-0.7.4/setup.py` & `PyCatFile-0.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     Revised BSD License for more details.
 
     Copyright 2016-2024 Cool Dude 2k - http://idb.berlios.de/
     Copyright 2016-2024 Game Maker 2k - http://intdb.sourceforge.net/
     Copyright 2016-2024 Kazuki Przyborowski - https://github.com/KazukiPrzyborowski
 
-    $FileInfo: setup.py - Last Update: 4/1/2024 Ver. 0.7.4 RC 1 - Author: cooldude2k $
+    $FileInfo: setup.py - Last Update: 4/10/2024 Ver. 0.7.6 RC 1 - Author: cooldude2k $
 '''
 
 import os, re, sys, pkg_resources;
 from setuptools import setup;
 
 verinfofilename = os.path.realpath("."+os.path.sep+os.path.sep+"pycatfile.py");
 verinfofile = open(verinfofilename, "r");
```

