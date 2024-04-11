# Comparing `tmp/cnl2asp-1.3.0.tar.gz` & `tmp/cnl2asp-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnl2asp-1.3.0.tar", last modified: Wed Apr 10 13:15:18 2024, max compression
+gzip compressed data, was "cnl2asp-1.3.1.tar", last modified: Thu Apr 11 12:26:09 2024, max compression
```

## Comparing `cnl2asp-1.3.0.tar` & `cnl2asp-1.3.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:15:18.180815 cnl2asp-1.3.0/
--rw-r--r--   0 carmine    (501) staff       (20)    11357 2022-05-07 07:05:44.000000 cnl2asp-1.3.0/LICENSE
--rw-r--r--   0 carmine    (501) staff       (20)      654 2024-04-10 13:15:18.180642 cnl2asp-1.3.0/PKG-INFO
--rw-r--r--   0 carmine    (501) staff       (20)    10643 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/README.md
--rw-r--r--   0 carmine    (501) staff       (20)       38 2024-04-10 13:15:18.180856 cnl2asp-1.3.0/setup.cfg
--rw-r--r--   0 carmine    (501) staff       (20)     1039 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/setup.py
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:15:18.172799 cnl2asp-1.3.0/src/
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:15:18.174327 cnl2asp-1.3.0/src/cnl2asp/
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:15:18.176621 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/
--rwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/__init__.py
--rwxr-xr-x   0 carmine    (501) staff       (20)     1517 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_aggregate.py
--rwxr-xr-x   0 carmine    (501) staff       (20)     4505 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_atom.py
--rwxr-xr-x   0 carmine    (501) staff       (20)     1837 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_attribute.py
--rwxr-xr-x   0 carmine    (501) staff       (20)     1594 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_conjunction.py
--rwxr-xr-x   0 carmine    (501) staff       (20)      471 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_element.py
--rw-r--r--   0 carmine    (501) staff       (20)     1053 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_encoding.py
--rwxr-xr-x   0 carmine    (501) staff       (20)     6394 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_operation.py
--rwxr-xr-x   0 carmine    (501) staff       (20)      510 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_program.py
--rwxr-xr-x   0 carmine    (501) staff       (20)     4703 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_rule.py
--rw-r--r--   0 carmine    (501) staff       (20)      414 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_temporal_formula.py
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:15:18.177465 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/solver/
--rw-r--r--   0 carmine    (501) staff       (20)        0 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/solver/__init__.py
--rw-r--r--   0 carmine    (501) staff       (20)     8020 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py
--rw-r--r--   0 carmine    (501) staff       (20)      561 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py
--rw-r--r--   0 carmine    (501) staff       (20)     1638 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py
--rw-r--r--   0 carmine    (501) staff       (20)      609 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py
--rw-r--r--   0 carmine    (501) staff       (20)        0 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/__init__.py
--rw-r--r--   0 carmine    (501) staff       (20)     6878 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/cnl2asp.py
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:15:18.178053 cnl2asp-1.3.0/src/cnl2asp/converter/
--rwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/converter/__init__.py
--rwxr-xr-x   0 carmine    (501) staff       (20)    25041 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/converter/asp_converter.py
--rw-r--r--   0 carmine    (501) staff       (20)     7333 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/converter/cnl2json_converter.py
--rwxr-xr-x   0 carmine    (501) staff       (20)     4916 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/converter/converter_interface.py
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:15:18.178245 cnl2asp-1.3.0/src/cnl2asp/exception/
--rw-r--r--   0 carmine    (501) staff       (20)        0 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/exception/__init__.py
--rw-r--r--   0 carmine    (501) staff       (20)     2369 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/exception/cnl2asp_exceptions.py
--rw-r--r--   0 carmine    (501) staff       (20)    16830 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/grammar.lark
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:15:18.178675 cnl2asp-1.3.0/src/cnl2asp/parser/
--rwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/parser/__init__.py
--rwxr-xr-x   0 carmine    (501) staff       (20)     3199 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/parser/command.py
--rwxr-xr-x   0 carmine    (501) staff       (20)    45312 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/parser/parser.py
--rwxr-xr-x   0 carmine    (501) staff       (20)     7027 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/parser/proposition_builder.py
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:15:18.180107 cnl2asp-1.3.0/src/cnl2asp/specification/
--rw-r--r--   0 carmine    (501) staff       (20)        0 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/__init__.py
--rw-r--r--   0 carmine    (501) staff       (20)     1103 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/aggregate_component.py
--rw-r--r--   0 carmine    (501) staff       (20)     4080 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/attribute_component.py
--rw-r--r--   0 carmine    (501) staff       (20)      741 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/component.py
--rw-r--r--   0 carmine    (501) staff       (20)      540 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/constant_component.py
--rw-r--r--   0 carmine    (501) staff       (20)    13928 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/entity_component.py
--rw-r--r--   0 carmine    (501) staff       (20)     1667 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/name_component.py
--rw-r--r--   0 carmine    (501) staff       (20)     3215 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/operation_component.py
--rw-r--r--   0 carmine    (501) staff       (20)     1122 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/problem.py
--rw-r--r--   0 carmine    (501) staff       (20)    11502 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/proposition.py
--rw-r--r--   0 carmine    (501) staff       (20)     1081 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/relation_component.py
--rw-r--r--   0 carmine    (501) staff       (20)     3963 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/signaturemanager.py
--rw-r--r--   0 carmine    (501) staff       (20)     1288 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/specification/specification.py
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:15:18.180310 cnl2asp-1.3.0/src/cnl2asp/utility/
--rw-r--r--   0 carmine    (501) staff       (20)        0 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/utility/__init__.py
--rw-r--r--   0 carmine    (501) staff       (20)      933 2024-04-10 13:14:36.000000 cnl2asp-1.3.0/src/cnl2asp/utility/utility.py
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-10 13:15:18.180470 cnl2asp-1.3.0/src/cnl2asp.egg-info/
--rw-r--r--   0 carmine    (501) staff       (20)      654 2024-04-10 13:15:18.000000 cnl2asp-1.3.0/src/cnl2asp.egg-info/PKG-INFO
--rw-r--r--   0 carmine    (501) staff       (20)     1993 2024-04-10 13:15:18.000000 cnl2asp-1.3.0/src/cnl2asp.egg-info/SOURCES.txt
--rw-r--r--   0 carmine    (501) staff       (20)        1 2024-04-10 13:15:18.000000 cnl2asp-1.3.0/src/cnl2asp.egg-info/dependency_links.txt
--rw-r--r--   0 carmine    (501) staff       (20)       30 2024-04-10 13:15:18.000000 cnl2asp-1.3.0/src/cnl2asp.egg-info/requires.txt
--rw-r--r--   0 carmine    (501) staff       (20)        8 2024-04-10 13:15:18.000000 cnl2asp-1.3.0/src/cnl2asp.egg-info/top_level.txt
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.678627 cnl2asp-1.3.1/
+-rw-rw-r--   0 simone    (1000) simone    (1000)    11357 2024-04-10 06:53:15.000000 cnl2asp-1.3.1/LICENSE
+-rw-r--r--   0 simone    (1000) simone    (1000)      654 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)    10643 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/README.md
+-rw-rw-r--   0 simone    (1000) simone    (1000)       38 2024-04-11 12:26:09.678627 cnl2asp-1.3.1/setup.cfg
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1039 2024-04-10 13:27:01.000000 cnl2asp-1.3.1/setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.666628 cnl2asp-1.3.1/src/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.666628 cnl2asp-1.3.1/src/cnl2asp/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.670628 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/
+-rwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/__init__.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     1517 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_aggregate.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     4505 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_atom.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     1837 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_attribute.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     1594 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_conjunction.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      471 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_element.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1053 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_encoding.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     6394 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_operation.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      510 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_program.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     4703 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_rule.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      414 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_temporal_formula.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.670628 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     8020 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      561 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1638 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      609 2024-04-10 11:30:37.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     6992 2024-04-10 14:25:04.000000 cnl2asp-1.3.1/src/cnl2asp/cnl2asp.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/src/cnl2asp/converter/
+-rwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/converter/__init__.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)    25041 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/converter/asp_converter.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     7333 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/converter/cnl2json_converter.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     4916 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/converter/converter_interface.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/src/cnl2asp/exception/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/exception/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2369 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/exception/cnl2asp_exceptions.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    16830 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/grammar.lark
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/src/cnl2asp/parser/
+-rwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/parser/__init__.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     3199 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/parser/command.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)    45312 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/parser/parser.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     7027 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/parser/proposition_builder.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/src/cnl2asp/specification/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1103 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/aggregate_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     4080 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/attribute_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      741 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      540 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/constant_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    13928 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/entity_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1667 2024-04-10 11:16:53.000000 cnl2asp-1.3.1/src/cnl2asp/specification/name_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3215 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/operation_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1122 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/problem.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    11502 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/proposition.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1081 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/relation_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3963 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/signaturemanager.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1288 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/specification.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/src/cnl2asp/utility/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/utility/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      933 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/utility/utility.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/src/cnl2asp.egg-info/
+-rw-r--r--   0 simone    (1000) simone    (1000)      654 2024-04-11 12:26:09.000000 cnl2asp-1.3.1/src/cnl2asp.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1993 2024-04-11 12:26:09.000000 cnl2asp-1.3.1/src/cnl2asp.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2024-04-11 12:26:09.000000 cnl2asp-1.3.1/src/cnl2asp.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       30 2024-04-11 12:26:09.000000 cnl2asp-1.3.1/src/cnl2asp.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        8 2024-04-11 12:26:09.000000 cnl2asp-1.3.1/src/cnl2asp.egg-info/top_level.txt
```

### Comparing `cnl2asp-1.3.0/LICENSE` & `cnl2asp-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/PKG-INFO` & `cnl2asp-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnl2asp
-Version: 1.3.0
+Version: 1.3.1
 Summary: A tool for converting a Controlled Natural Language based on English into Answer Set Programming
 Home-page: https://github.com/dodaro/cnl2asp/tree/main
 Author: Carmine Dodaro
 Author-email: carmine.dodaro@unical.it
 Maintainer: Simone Caruso
 Maintainer-email: simone.caruso@edu.unige.it
 License: Apache License
```

### Comparing `cnl2asp-1.3.0/README.md` & `cnl2asp-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_aggregate.py` & `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_aggregate.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_atom.py` & `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_atom.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_attribute.py` & `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_attribute.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_conjunction.py` & `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_conjunction.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_encoding.py` & `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_encoding.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_operation.py` & `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_operation.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/ASP_elements/asp_rule.py` & `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_rule.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py` & `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py` & `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py` & `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py` & `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/cnl2asp.py` & `cnl2asp-1.3.1/src/cnl2asp/cnl2asp.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 import os
 import tempfile
 import traceback
 from enum import Enum
 from textwrap import indent
 from typing import TextIO
 
-from clingo.ast import parse_files
 from cnl2asp.utility.utility import Utility
 from lark import Lark, UnexpectedCharacters
 from lark.exceptions import VisitError
-from ngo import optimize, Predicate
 
 from cnl2asp.ASP_elements.asp_program import ASPProgram
 from cnl2asp.converter.cnl2json_converter import Cnl2jsonConverter
 from cnl2asp.exception.cnl2asp_exceptions import ParserError
 from cnl2asp.specification.attribute_component import AttributeComponent
 from cnl2asp.specification.entity_component import EntityComponent
 from cnl2asp.converter.asp_converter import ASPConverter
@@ -49,14 +47,16 @@
 
 
 class Cnl2asp:
     def __init__(self, cnl_input: TextIO | str, debug: bool = False):
         self._debug = debug
         if isinstance(cnl_input, str):
             self.cnl_input = cnl_input
+            if os.path.isfile(cnl_input):
+                self.cnl_input = open(cnl_input).read()
         else:
             self.cnl_input = cnl_input.read()
 
     def parse_input(self):
         with open(os.path.join(os.path.dirname(__file__), "grammar.lark"), "r") as grammar:
             cnl_parser = Lark(grammar.read(), propagate_positions=True)
             specification: SpecificationComponent = CNLTransformer().transform(cnl_parser.parse(self.cnl_input))
@@ -114,14 +114,16 @@
         except Exception as e:
             print("Error in asp conversion:", str(e))
             if self._debug:
                 traceback.print_exception(e)
             return ''
 
     def optimize(self, asp_encoding: str):
+        from clingo.ast import parse_files
+        from ngo import optimize, Predicate
         prg = []
         with tempfile.NamedTemporaryFile(mode="w") as file:
             file.write(asp_encoding)
             file.seek(0)
             parse_files([file.name], prg.append)
             prg = optimize(prg, [Predicate("node",1)], [Predicate("assigned_to",2)])
             optimized_encoding = ''
```

### Comparing `cnl2asp-1.3.0/src/cnl2asp/converter/asp_converter.py` & `cnl2asp-1.3.1/src/cnl2asp/converter/asp_converter.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/converter/cnl2json_converter.py` & `cnl2asp-1.3.1/src/cnl2asp/converter/cnl2json_converter.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/converter/converter_interface.py` & `cnl2asp-1.3.1/src/cnl2asp/converter/converter_interface.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/exception/cnl2asp_exceptions.py` & `cnl2asp-1.3.1/src/cnl2asp/exception/cnl2asp_exceptions.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/grammar.lark` & `cnl2asp-1.3.1/src/cnl2asp/grammar.lark`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/parser/command.py` & `cnl2asp-1.3.1/src/cnl2asp/parser/command.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/parser/parser.py` & `cnl2asp-1.3.1/src/cnl2asp/parser/parser.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/parser/proposition_builder.py` & `cnl2asp-1.3.1/src/cnl2asp/parser/proposition_builder.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/specification/aggregate_component.py` & `cnl2asp-1.3.1/src/cnl2asp/specification/aggregate_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/specification/attribute_component.py` & `cnl2asp-1.3.1/src/cnl2asp/specification/attribute_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/specification/component.py` & `cnl2asp-1.3.1/src/cnl2asp/specification/component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/specification/constant_component.py` & `cnl2asp-1.3.1/src/cnl2asp/specification/constant_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/specification/entity_component.py` & `cnl2asp-1.3.1/src/cnl2asp/specification/entity_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/specification/name_component.py` & `cnl2asp-1.3.1/src/cnl2asp/specification/name_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/specification/operation_component.py` & `cnl2asp-1.3.1/src/cnl2asp/specification/operation_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/specification/problem.py` & `cnl2asp-1.3.1/src/cnl2asp/specification/problem.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/specification/proposition.py` & `cnl2asp-1.3.1/src/cnl2asp/specification/proposition.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/specification/relation_component.py` & `cnl2asp-1.3.1/src/cnl2asp/specification/relation_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/specification/signaturemanager.py` & `cnl2asp-1.3.1/src/cnl2asp/specification/signaturemanager.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/specification/specification.py` & `cnl2asp-1.3.1/src/cnl2asp/specification/specification.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp/utility/utility.py` & `cnl2asp-1.3.1/src/cnl2asp/utility/utility.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.0/src/cnl2asp.egg-info/PKG-INFO` & `cnl2asp-1.3.1/src/cnl2asp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnl2asp
-Version: 1.3.0
+Version: 1.3.1
 Summary: A tool for converting a Controlled Natural Language based on English into Answer Set Programming
 Home-page: https://github.com/dodaro/cnl2asp/tree/main
 Author: Carmine Dodaro
 Author-email: carmine.dodaro@unical.it
 Maintainer: Simone Caruso
 Maintainer-email: simone.caruso@edu.unige.it
 License: Apache License
```

### Comparing `cnl2asp-1.3.0/src/cnl2asp.egg-info/SOURCES.txt` & `cnl2asp-1.3.1/src/cnl2asp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

