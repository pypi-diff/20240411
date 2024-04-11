# Comparing `tmp/rdf_doctor-1.1.0b1-py3-none-any.whl.zip` & `tmp/rdf_doctor-1.1.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 59032 bytes, number of entries: 12
--rw-r--r--  2.0 unx       24 b- defN 24-Mar-21 05:25 doctor/__init__.py
--rw-r--r--  2.0 unx     1650 b- defN 24-Mar-05 05:49 doctor/consts.py
--rw-r--r--  2.0 unx    77463 b- defN 24-Mar-21 05:43 doctor/doctor.py
+Zip file size: 59789 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       25 b- defN 24-Apr-11 00:44 doctor/__init__.py
+-rw-r--r--  2.0 unx     1754 b- defN 24-Mar-29 08:43 doctor/consts.py
+-rw-r--r--  2.0 unx    80752 b- defN 24-Apr-11 00:43 doctor/doctor.py
 -rw-r--r--  2.0 unx   134314 b- defN 24-Mar-12 04:38 doctor/reference/prefixes.tsv
 -rw-r--r--  2.0 unx       90 b- defN 24-Mar-06 07:08 doctor/reference/refine-class-uris.tsv
 -rw-r--r--  2.0 unx      577 b- defN 24-Mar-06 07:13 doctor/reference/refine-prefix-uris.tsv
--rw-r--r--  2.0 unx     1061 b- defN 24-Mar-21 06:56 rdf_doctor-1.1.0b1.dist-info/LICENSE
--rw-r--r--  2.0 unx    10268 b- defN 24-Mar-21 06:56 rdf_doctor-1.1.0b1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-21 06:56 rdf_doctor-1.1.0b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Mar-21 06:56 rdf_doctor-1.1.0b1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Mar-21 06:56 rdf_doctor-1.1.0b1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1007 b- defN 24-Mar-21 06:56 rdf_doctor-1.1.0b1.dist-info/RECORD
-12 files, 226605 bytes uncompressed, 57328 bytes compressed:  74.7%
+-rw-r--r--  2.0 unx     1061 b- defN 24-Apr-11 01:18 rdf_doctor-1.1.0rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10690 b- defN 24-Apr-11 01:18 rdf_doctor-1.1.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 01:18 rdf_doctor-1.1.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-Apr-11 01:18 rdf_doctor-1.1.0rc1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-11 01:18 rdf_doctor-1.1.0rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1013 b- defN 24-Apr-11 01:18 rdf_doctor-1.1.0rc1.dist-info/RECORD
+12 files, 230427 bytes uncompressed, 58073 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-1.1.0b1.dist-info/LICENSE
+Filename: rdf_doctor-1.1.0rc1.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-1.1.0b1.dist-info/METADATA
+Filename: rdf_doctor-1.1.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-1.1.0b1.dist-info/WHEEL
+Filename: rdf_doctor-1.1.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-1.1.0b1.dist-info/entry_points.txt
+Filename: rdf_doctor-1.1.0rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.0b1.dist-info/top_level.txt
+Filename: rdf_doctor-1.1.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.0b1.dist-info/RECORD
+Filename: rdf_doctor-1.1.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.0b1"
+__version__ = "1.1.0rc1"
```

## doctor/consts.py

```diff
@@ -49,7 +49,10 @@
 
 # Errata
 REFINE_CLASS_URIS_FILE_PATH = "reference/refine-class-uris.tsv"
 REFINE_PREFIX_URIS_FILE_PATH = "reference/refine-prefix-uris.tsv"
 
 # Help link URL
 HELP_LINK_URL = "https://github.com/dbcls/rdf-doctor#output-description"
+
+# Default value for disk usage limit, including temporary directories
+TMP_DISK_USAGE_LIMIT_DEFAULT = 95
```

## doctor/doctor.py

```diff
@@ -9,24 +9,25 @@
 import csv
 import codecs
 import time
 import datetime
 from concurrent.futures import ThreadPoolExecutor
 import multiprocessing
 import queue
+import shutil
 from unidecode import unidecode
 from collections import defaultdict
 from pathlib import Path
 import tempfile
 import uuid
 from doctor.consts import VERSION_FILE, TARGET_CLASS_ALL, EXTENSION_NT, EXTENSION_TTL, \
                             EXTENSION_RDF, EXTENSION_XML, EXTENSION_OWL, EXTENSION_GZ, EXTENSION_ZIP, EXTENSION_TAR_GZ, \
                             PREFIXES_FILE_PATH, REFINE_CLASS_URIS_FILE_PATH, REFINE_PREFIX_URIS_FILE_PATH, HELP_LINK_URL, \
                             FILE_TYPE_TTL, FILE_TYPE_NT, FILE_TYPE_RDF_XML, FILE_TYPE_TTL_GZ, FILE_TYPE_NT_GZ, FILE_TYPE_RDF_XML_GZ, \
-                            FILE_TYPE_TTL_ZIP, FILE_TYPE_NT_ZIP, FILE_TYPE_RDF_XML_ZIP, FILE_TYPE_ALL, FILE_TYPE_DICT
+                            FILE_TYPE_TTL_ZIP, FILE_TYPE_NT_ZIP, FILE_TYPE_RDF_XML_ZIP, FILE_TYPE_ALL, FILE_TYPE_DICT, TMP_DISK_USAGE_LIMIT_DEFAULT
 
 from shexer.shaper import Shaper
 from shexer.consts import NT, TURTLE, RDF_XML, GZ, ZIP, MIXED_INSTANCES
 
 is_displaying_spinner = False
 in_progress_rdflib_query = False
 
@@ -36,32 +37,32 @@
 
     error_msg = validate_command_line_args_other(args)
     if error_msg is not None:
         print(error_msg)
         return
 
     # Generate temporary directory for compressed file decompression
-    with tempfile.TemporaryDirectory() as temp_dir:
+    with tempfile.TemporaryDirectory(dir=args.tmp_dir) as temp_dir:
 
         input_file_2d_list = []
         # If the option is specified to separate results for each input file
         if args.each:
             if args.output is None:
                 print("The --each option should be used with the --output option.")
                 return
 
             # Get an array containing each file to be processed
             # Acquire as a two-dimensional array for compatibility with subsequent processing
-            input_file_2d_list, exists_file_types, error_msg = get_input_files_each(args.input, temp_dir)
+            input_file_2d_list, exists_file_types, error_msg = get_input_files_each(args.input, temp_dir, args.tmp_dir_disk_usage_limit)
             if error_msg is not None:
                 print(error_msg)
                 return
         else:
             # Retrieve input files in dictionary format by type
-            input_file_2d_list, exists_file_types, error_msg = get_input_files_by_type(args.input, temp_dir)
+            input_file_2d_list, exists_file_types, error_msg = get_input_files_by_type(args.input, temp_dir, args.tmp_dir_disk_usage_limit)
             if error_msg is not None:
                 print(error_msg)
                 return
 
         if args.type:
             if args.type == "all":
                 target_file_types = exists_file_types
@@ -131,28 +132,31 @@
 
                             with open(args.output + "/" + output_file_name + compression_exetention + ".shex", "w", encoding="utf-8") as f:
                                 f.write("".join(result_output[0]))
 
                     if args.verbose:
                         print_overwrite(get_dt_now() + " -- Done!")
 
-                elif type(result_output) in [ValueError, IndexError, Exception]:
+                elif type(result_output) in [ValueError, IndexError, MemoryError, Exception]:
                     # Error case
                     raise result_output
 
                 else:
                     # Else case does not occur.
                     raise Exception("An exception error has occurred. Not the expected processing result.")
 
         except ValueError as e:
             print(e)
 
         except IndexError as e:
             print(e)
 
+        except MemoryError as e:
+            print(e)
+
         except KeyboardInterrupt:
             print ("Keyboard interrupt occurred.")
 
         except Exception as e:
             print(e)
 
         finally:
@@ -238,14 +242,26 @@
                         metavar="URL")
 
     # Separate results by file when multiple files are specified (-e、--each)
     parser.add_argument("-e","--each",
                         action="store_true",
                         help="separate results by file when multiple files are specified")
 
+    # Temporary directory (--tmp-dir [DIRECTORY]、default: Platform-dependent default temporary directory)
+    parser.add_argument("--tmp-dir", type=str,
+                        default=None,
+                        help='Temporary directory where the unzipped contents are placed when processing tar.gz or zip (default: Platform-dependent default temporary directory)',
+                        metavar="DIRECTORY")
+
+    # Temporary directory usage upper limit(--tmp-dir-disk-usage-limit [percentage]、default: 95)
+    parser.add_argument("--tmp-dir-disk-usage-limit", type=int,
+                        default=TMP_DISK_USAGE_LIMIT_DEFAULT,
+                        help='Percentage of disk usage that contains the temporary directory where unzipped contents are placed when processing tar.gz or zip. Interrupt processing when the specified usage percentage is exceeded (1-100 default: 95)',
+                        metavar="PERCENTAGE")
+
     # Prefix URI dictionary file path(--prefix-uri-dict [FILE]、default: reference/refine-prefix-uris.tsv)
     parser.add_argument("--prefix-uri-dict", type=str,
                         default=str(Path(__file__).resolve().parent.joinpath(REFINE_PREFIX_URIS_FILE_PATH)),
                         help='path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the prefix (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-prefix-uris.tsv)',
                         metavar="FILE")
 
     # Class URI dictionary file path(--class-uri-dict [FILE]、default: reference/refine-class-uris.tsv)
@@ -278,15 +294,15 @@
 #     ttl_gz: [["test10.ttl.gz", "test11.ttl.gz", "test12.ttl.gz"], "gz", "turtle"]
 #     nt_gz: [["test13.nt.gz", "test14.nt.gz", "test15.nt.gz"], gz, "nt"],
 #     rdf_xml_gz: [["test16.rdf.gz", "test17.xml.gz", "test18.owl.gz"], gz, "xml"],
 #     ttl_zip: [["test19.ttl.zip", "test20.ttl.zip", "test21.ttl.zip"], zip, "turtle"]
 #     nt_zip: [["test22.nt.zip", "test23.nt.zip", "test24.nt.zip"], zip, "nt"],
 #     rdf_xml_zip: [["test25.rdf.zip", "test26.xml.zip", "test27.owl.zip"], zip, "xml"]
 # }
-def get_input_files_by_type(input_files, temp_dir):
+def get_input_files_by_type(input_files, temp_dir, tmp_dir_disk_usage_limit):
 
     input_file_list_ttl = []            # Turtle(.ttl)
     input_file_list_nt = []             # N-Triples(.nt)
     input_file_list_rdf_xml = []        # RDF/XML(.rdf, .xml, .owl)
     input_file_list_ttl_gz = []         # GZ compressed Turtle(.ttl.gz)
     input_file_list_nt_gz = []          # GZ compressed N-Triples(.nt.gz)
     input_file_list_rdf_xml_gz = []     # GZ compressed RDF/XML(.rdf.gz, .xml.gz, .owl.gz)
@@ -356,14 +372,19 @@
                     input_file_list_nt_gz.append(input_file)
                 elif input_format == RDF_XML:
                     input_file_list_rdf_xml_gz.append(input_file)
                 else:
                     extension = get_extension_before_compression(input_file) + "." + compression_mode
 
                     if extension == EXTENSION_TAR_GZ:
+                        # Check disk usage percentage
+                        if get_disk_usage_percentage(temp_dir) >= tmp_dir_disk_usage_limit:
+                            error_msg = 'The process was canceled because the disk usage exceeded ' + str(tmp_dir_disk_usage_limit) + '%.'
+                            return None, None, error_msg
+
                         extract_path = Path(temp_dir) / Path(input_file + "_" + str(uuid.uuid4())).name
                         # For .tar.gz, expand and process the contents
                         with tarfile.open(input_file, 'r:gz') as tar:
                             tar.extractall(extract_path)
 
                         # Loop by recursively retrieving files in a directory
                         for root, _, files in os.walk(top=extract_path):
@@ -413,14 +434,19 @@
                 elif input_format == NT:
                     input_file_list_nt_zip.append(input_file)
                 elif input_format == RDF_XML:
                     input_file_list_rdf_xml_zip.append(input_file)
                 else:
                     extension = get_extension_before_compression(input_file) + "." + compression_mode
                     if extension == EXTENSION_ZIP:
+                        # Check disk usage percentage
+                        if get_disk_usage_percentage(temp_dir) >= tmp_dir_disk_usage_limit:
+                            error_msg = 'The process was canceled because the disk usage exceeded ' + str(tmp_dir_disk_usage_limit) + '%.'
+                            return None, None, error_msg
+
                         extract_path = Path(temp_dir) / Path(input_file + "_" + str(uuid.uuid4())).name
                         # For .zip, expand and process the contents
                         with ZipFile(input_file,'r') as zip:
                             zip.extractall(extract_path)
 
                         # Loop by recursively retrieving files in a directory
                         for root, _, files in os.walk(top=extract_path):
@@ -529,15 +555,15 @@
 #     ["test7.nt", None, "nt"],
 #     ["test8.nt.gz", "gz", "nt"],
 #     ["test9.rdf", None, "xml"],
 #     ["test10.xml", None, "xml"],
 #     ["test11.owl", None, "xml"],
 #     ["test12.rdf.zip", "zip", "xml"]
 # ]
-def get_input_files_each(input_files, temp_dir):
+def get_input_files_each(input_files, temp_dir, tmp_dir_disk_usage_limit):
 
     input_file_2d_list = []
     exists_file_types = []
 
     for input_file in input_files:
         if Path(input_file).exists() == False:
             error_msg = '"' + input_file + '" does not exist.'
@@ -579,14 +605,19 @@
                 # Case None
                 if compression_mode is None:
                     extension = get_extension(input_file)
                 else:
                     extension = get_extension_before_compression(input_file) + "." + compression_mode
 
                 if extension == EXTENSION_TAR_GZ:
+                    # Check disk usage percentage
+                    if get_disk_usage_percentage(temp_dir) >= tmp_dir_disk_usage_limit:
+                        error_msg = 'The process was canceled because the disk usage exceeded ' + str(tmp_dir_disk_usage_limit) + '%.'
+                        return None, None, error_msg
+
                     extract_path = Path(temp_dir) / Path(input_file + "_" + str(uuid.uuid4())).name
                     # For .tar.gz, expand and process the contents
                     with tarfile.open(input_file, 'r:gz') as tar:
                         tar.extractall(extract_path)
 
                     # Loop by recursively retrieving files in a directory
                     for root, _, files in os.walk(top=extract_path):
@@ -602,14 +633,19 @@
                             elif input_format == RDF_XML:
                                 input_file_2d_list.append([[file_path], compression_mode, RDF_XML])
                             else:
                                 # No processing except for .ttl, .nt, .rdf, .xml, .owl and their compressed
                                 pass
 
                 elif extension == EXTENSION_ZIP:
+                    # Check disk usage percentage
+                    if get_disk_usage_percentage(temp_dir) >= tmp_dir_disk_usage_limit:
+                        error_msg = 'The process was canceled because the disk usage exceeded ' + str(tmp_dir_disk_usage_limit) + '%.'
+                        return None, None, error_msg
+
                     extract_path = Path(temp_dir) / Path(input_file + "_" + str(uuid.uuid4())).name
                     # For .zip, expand and process the contents
                     with ZipFile(input_file,'r') as zip:
                         zip.extractall(extract_path)
 
                     # Loop by recursively retrieving files in a directory
                     for root, _, files in os.walk(top=extract_path):
@@ -742,15 +778,15 @@
 def validate_command_line_args_other(args):
     if args.output is not None:
         # Existence check of file output destination directory
         if Path(args.output).is_file():
             error_msg = "Output directory error: A directory must be specified as the output destination. Files cannot be specified."
             return error_msg
 
-        output_dir = Path(args.output).parent
+        output_dir = Path(args.output)
         if output_dir:
             if Path(output_dir).exists() == False:
                 error_msg = "Output directory error: Output directory does not exist."
                 return error_msg
 
             # Check if the file output destination has write permission
             if os.access(output_dir, os.W_OK) == False:
@@ -805,28 +841,51 @@
                 return error_msg
         else:
             for type in types:
                 if type not in FILE_TYPE_DICT:
                     error_msg = 'Type error: "' + type + '" is an unsupported input file format. "' + FILE_TYPE_TTL + '", "' + FILE_TYPE_NT + '", "' + FILE_TYPE_RDF_XML + '", "' + FILE_TYPE_TTL_GZ + '", "' + FILE_TYPE_NT_GZ + '", "' + FILE_TYPE_RDF_XML_GZ + '", "' + FILE_TYPE_TTL_ZIP + '", "' + FILE_TYPE_NT_ZIP + '" and "' + FILE_TYPE_RDF_XML_ZIP + '" are supported.'
                     return error_msg
 
+    # Check temporary directory
+    if args.tmp_dir is not None:
+        # Existence check of file temporary directory destination directory
+        if Path(args.tmp_dir).is_file():
+            error_msg = "Temporary directory error: A directory must be specified as the temporary directory destination. Files cannot be specified."
+            return error_msg
+
+        tmp_dir = Path(args.tmp_dir)
+        if tmp_dir:
+            if Path(tmp_dir).exists() == False:
+                error_msg = "Temporary directory error: Temporary directory does not exist."
+                return error_msg
+
+            # Check if the file temporary directory destination has write permission
+            if os.access(tmp_dir, os.W_OK) == False:
+                error_msg = "Temporary directory error: You don't have write permission on the temporary directory."
+                return error_msg
+
+    # Check temporary directory usage limit
+    if args.tmp_dir_disk_usage_limit < 1 or args.tmp_dir_disk_usage_limit > 100:
+        error_msg = "Temporary directory disk usage limit error: Please specify the upper limit of Disk containing temporary directory usage percentage as a number between 1 and 100."
+        return error_msg
+
     return None
 
 
 # Processing when the report format is "shex"
 def get_shex_result(args, input_file_list, input_format, compression_mode, result_queue):
 
     try:
         widely_used_prefixes_dict = get_widely_used_prefixes_dict(args.prefix_list)
 
         # Get Prefix when input file is turtle format
         if input_format == NT:
             input_prefixes = []
             duplicated_prefixes = []
-            namespaces_dict = default_namespaces()
+            namespaces_dict = get_default_namespaces_dict()
         else:
             if args.verbose:
                 print_overwrite(get_dt_now() + " -- Getting prefixes from input file...")
 
             if input_format == TURTLE:
                 input_prefixes, duplicated_prefixes, duplicated_prefixes_dict = get_input_prefixes_turtle(input_file_list, compression_mode)
             elif input_format == RDF_XML:
@@ -969,19 +1028,22 @@
 
         if len(report_result) != 0:
             shex_final_result.extend(report_result)
 
         result_queue.put([shex_final_result, input_file_list, input_format, compression_mode])
 
     except ValueError as e:
-        result_queue.put(ValueError('An index error has occurred.\n\nValueError message: ' + str(e)))
+        result_queue.put(ValueError('A value error has occurred.\n\nValueError message: ' + str(e)))
 
     except IndexError as e:
         result_queue.put(IndexError('An index error has occurred.\n\nIndexError message: ' + str(e)))
 
+    except MemoryError as e:
+        result_queue.put(MemoryError('A memory error has occurred.\n\nMemoryError message: ' + str(e)))
+
     except Exception as e:
         result_queue.put(Exception('An exception error has occurred.\n\nException message: ' + str(e)))
 
 
 # Call the shex_graph method of shexer's shaper class and output the result
 def get_shaper_result(args, input_file_list, input_format, compression_mode, namespaces_dict):
     # Set parameters when calling the shaper class depending on whether the class is specified as an argument
@@ -1114,29 +1176,14 @@
             if input_class == refine_class_uri[0]:
                 class_comparison_result.append(input_class+"\t"+refine_class_uri[1]+"\n")
                 break
 
     return class_comparison_result, fingerprint_class_dict
 
 
-# Refer to the dictionary of prefix URIs and obtain a list that combines candidate pairs of URI rewrite source and rewrite destination
-def get_prefix_comparison_result(input_prefixes, refine_prefix_uris_file):
-    refine_prefix_uris = get_refine_prefix_uris(refine_prefix_uris_file)
-    prefix_comparison_result = []
-
-    # Perform clustering by fingerprint for the acquired class name
-    for input_prefix in input_prefixes:
-        for refine_prefix_uri in refine_prefix_uris:
-            if input_prefix[1] == refine_prefix_uri[0] and refine_prefix_uri[1] != "":
-                prefix_comparison_result.append(str(input_prefix[0]+"\t"+input_prefix[1]+"\t"+refine_prefix_uri[1]+"\n"))
-                break
-
-    return prefix_comparison_result
-
-
 # Get the output result when there are multiple different strings with the same key for the class
 def get_fingerprint_comparison_result(fingerprint_class_dict):
     fingerprint_comparison_result = []
     # Extract if there are multiple different strings with the same key
     for value in fingerprint_class_dict.values():
         if len(value) >= 2:
             if len(fingerprint_comparison_result) != 0:
@@ -1326,15 +1373,15 @@
     string = unidecode(string)
     words = string.split()
     words = sorted(list(set(words)))
     return " ".join(words)
 
 # A dictionary of namespaces to pass to sheXer
 # This function is used only when the input file is N-Triples.
-def default_namespaces():
+def get_default_namespaces_dict():
     return {
             "http://www.w3.org/2002/07/owl#": "owl",
             "http://www.w3.org/1999/02/22-rdf-syntax-ns#": "rdf",
             "http://www.w3.org/2000/01/rdf-schema#": "rdfs",
             "http://www.w3.org/2001/XMLSchema#": "xsd",
             "http://www.w3.org/XML/1998/namespace": "xml",
             "http://www.w3.org/2004/02/skos/core#": "skos",
@@ -1367,15 +1414,14 @@
         print("The following types of files were found.")
         for key, value in FILE_TYPE_DICT.items():
             if key in exists_file_types:
                 print(value)
 
         while True:
             user_input = input("\n1: Process all\n2: Specify file type\n(1/2):")
-            print(user_input)
             if user_input == "1":
                 is_process_all = True
                 break
             elif user_input == "2":
                 is_process_all = False
                 break
 
@@ -1530,8 +1576,13 @@
             exists_suggest = True
 
     suggest_string += "\n"
 
     if exists_suggest:
         return suggest_string
     else:
-        return ""
+        return ""
+
+# Returns the usage percentage of the specified disk
+def get_disk_usage_percentage(path):
+    disk_usage = shutil.disk_usage(path)
+    return disk_usage.used / disk_usage.total * 100
```

## Comparing `rdf_doctor-1.1.0b1.dist-info/LICENSE` & `rdf_doctor-1.1.0rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-1.1.0b1.dist-info/METADATA` & `rdf_doctor-1.1.0rc1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 1.1.0b1
+Version: 1.1.0rc1
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask (>=2.2.5)
 Requires-Dist: Flask-Cors (>=3.0.9)
 Requires-Dist: rdflib (>=6.3.1)
 Requires-Dist: SPARQLWrapper (>=2.0.0)
 Requires-Dist: wlighter (>=1.0.1)
-Requires-Dist: shexer (>=2.2.2)
+Requires-Dist: shexer (>=2.3.0)
 Requires-Dist: unidecode (>=1.3.6)
 
 # rdf-doctor
 [![Pyversions](https://img.shields.io/pypi/pyversions/rdf-doctor.svg)](https://pypi.python.org/pypi/rdf-doctor)
 
 ## Motivation
 DBCLS has conducted to convert various life science databases to RDF and support it. This development will enable us to provide a high-quality dataset that better links existing RDF datasets stored in the RDF portal site and newly developed RDF.
@@ -60,14 +60,17 @@
   -t TYPE, --type TYPE  specifies the type of the input file ("all" or individually from the following Multiple types can be specified by separating them with a comma. ttl, nt, rdf_xml, ttl_gz, nt_gz, rdf_xml_gz, ttl_zip, nt_zip, rdf_xml_zip)
   -r, --report          add report to results
   -o DIRECTORY, --output DIRECTORY
                         directory to output results (standard output if not specified)
   -c URL [URL ...], --classes URL [URL ...]
                         set the target classes to be inspected to one of: all (defalut) or URL1 URL2...
   -e, --each            separate results by file when multiple files are specified
+  --tmp-dir DIRECTORY   Temporary directory where the unzipped contents are placed when processing tar.gz or zipped directory
+  --tmp-dir-disk-usage-limit PERCENTAGE
+                        Percentage of disk usage that contains the temporary directory where unzipped contents are placed when processing tar.gz or zipped directory. Interrupt processing when the specified usage percentage is exceeded (1-100 default: 95)
   --prefix-uri-dict FILE
                         path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the prefix (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-
                         doctor/blob/main/doctor/reference/refine-prefix-uris.tsv)
   --class-uri-dict FILE
                         path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the class (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-
                         doctor/blob/main/doctor/reference/refine-class-uris.tsv)
   --prefix-list FILE    list of prefixes (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/prefixes.tsv)
```

