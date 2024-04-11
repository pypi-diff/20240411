# Comparing `tmp/ntsbuildtools-4.0.8rc0.tar.gz` & `tmp/ntsbuildtools-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntsbuildtools-4.0.8rc0.tar", last modified: Wed Oct  4 19:25:34 2023, max compression
+gzip compressed data, was "ntsbuildtools-4.0.9.tar", last modified: Thu Oct  5 21:05:37 2023, max compression
```

## Comparing `ntsbuildtools-4.0.8rc0.tar` & `ntsbuildtools-4.0.9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.484576 ntsbuildtools-4.0.8rc0/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       24 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/MANIFEST.in
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     9479 2023-10-04 19:25:34.484576 ntsbuildtools-4.0.8rc0/PKG-INFO
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      102 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/README.md
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.472576 ntsbuildtools-4.0.8rc0/docs/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     1003 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/docs/README.md
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     2535 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/docs/changelog.md
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     5424 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/docs/jenkins-cicd.md
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.473576 ntsbuildtools-4.0.8rc0/docs/software-design/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      978 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/docs/software-design/_overview.md
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)    12738 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/docs/software-design/ansible-results.md
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)    12663 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/docs/software-design/cli-framework.md
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     5277 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/docs/software-design/development.md
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      199 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/docs/software-design/refactorings.md
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     7654 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/docs/user-guide.md
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       38 2023-10-04 19:25:34.484576 ntsbuildtools-4.0.8rc0/setup.cfg
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     1629 2023-10-04 19:25:33.000000 ntsbuildtools-4.0.8rc0/setup.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.468576 ntsbuildtools-4.0.8rc0/src/
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.474576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      179 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/__init__.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.476576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       98 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/__init__.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)    11181 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/inventory.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.476576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/playbook/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)        0 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/playbook/__init__.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     4960 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/playbook/results.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.477576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/return_values/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)        0 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/return_values/__init__.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     2679 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/return_values/default.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     2227 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/return_values/factory.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      373 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/return_values/junos_config.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.478576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/cli/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      351 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/cli/__init__.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     3532 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/cli/framework.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     8173 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/cli/tree.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     1450 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/exceptions.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       72 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/io.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      774 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/main.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.478576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/markdown/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)        0 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/markdown/__init__.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     6879 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/markdown/comments.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.479576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      145 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/__init__.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.479576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/example/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       22 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/example/__init__.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      404 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/example/hello_world.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.479576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/infer/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       62 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/infer/__init__.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.480576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/infer/ansible/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       22 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/infer/ansible/__init__.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     1146 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/infer/ansible/playbook_limit.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.480576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/parse/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      114 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/parse/__init__.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.481576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/parse/ansible/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       22 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/parse/ansible/__init__.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     2575 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/parse/ansible/json.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.481576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       37 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/__init__.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.482576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/bitbucket/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       51 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/bitbucket/__init__.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     3321 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/bitbucket/build_status.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     5724 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/bitbucket/pr_comment.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     2423 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/bitbucket/pull_request.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.482576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/github/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       21 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/github/__init__.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     4932 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/github/pr_comment.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.483576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/teams/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       30 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/teams/__init__.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     6370 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/teams/card.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.483576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/teams/
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)        0 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/teams/__init__.py
--rwxrwxr-x   0 jenkins   (1888) jenkins   (1888)     7234 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/teams/card_template.py
--rwxrwxr-x   0 jenkins   (1888) jenkins   (1888)    10317 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/teams/cards.py
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      261 2023-09-26 16:07:31.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools/util.py
-drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-04 19:25:34.475576 ntsbuildtools-4.0.8rc0/src/ntsbuildtools.egg-info/
--rw-r--r--   0 jenkins   (1888) jenkins   (1888)     9479 2023-10-04 19:25:34.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     2305 2023-10-04 19:25:34.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)        1 2023-10-04 19:25:34.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       56 2023-10-04 19:25:34.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       81 2023-10-04 19:25:34.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       14 2023-10-04 19:25:34.000000 ntsbuildtools-4.0.8rc0/src/ntsbuildtools.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.328804 ntsbuildtools-4.0.9/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       24 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/MANIFEST.in
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     9476 2023-10-05 21:05:37.327804 ntsbuildtools-4.0.9/PKG-INFO
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      102 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/README.md
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.316804 ntsbuildtools-4.0.9/docs/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     1003 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/docs/README.md
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     2533 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/docs/changelog.md
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     5424 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/docs/jenkins-cicd.md
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.317804 ntsbuildtools-4.0.9/docs/software-design/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      978 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/docs/software-design/_overview.md
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)    12738 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/docs/software-design/ansible-results.md
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)    12663 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/docs/software-design/cli-framework.md
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     5277 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/docs/software-design/development.md
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      199 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/docs/software-design/refactorings.md
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     7654 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/docs/user-guide.md
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       38 2023-10-05 21:05:37.328804 ntsbuildtools-4.0.9/setup.cfg
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     1626 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/setup.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.312804 ntsbuildtools-4.0.9/src/
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.318804 ntsbuildtools-4.0.9/src/ntsbuildtools/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      179 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/__init__.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.320804 ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       98 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/__init__.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)    11181 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/inventory.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.320804 ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/playbook/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/playbook/__init__.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     4960 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/playbook/results.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.321804 ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/return_values/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/return_values/__init__.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     2679 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/return_values/default.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     2227 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/return_values/factory.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      373 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/return_values/junos_config.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.322804 ntsbuildtools-4.0.9/src/ntsbuildtools/cli/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      351 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/cli/__init__.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     3532 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/cli/framework.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     8173 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/cli/tree.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     1450 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/exceptions.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       72 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/io.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      774 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/main.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.322804 ntsbuildtools-4.0.9/src/ntsbuildtools/markdown/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/markdown/__init__.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     6879 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/markdown/comments.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.322804 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      145 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/__init__.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.323804 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/example/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       22 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/example/__init__.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      404 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/example/hello_world.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.323804 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/infer/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       62 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/infer/__init__.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.323804 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/infer/ansible/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       22 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/infer/ansible/__init__.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     1146 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/infer/ansible/playbook_limit.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.324804 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/parse/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      114 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/parse/__init__.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.324804 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/parse/ansible/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       22 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/parse/ansible/__init__.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     2575 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/parse/ansible/json.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.324804 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       37 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/__init__.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.325804 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/bitbucket/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       51 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/bitbucket/__init__.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     3321 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/bitbucket/build_status.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     5724 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/bitbucket/pr_comment.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     2423 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/bitbucket/pull_request.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.326804 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/github/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       21 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/github/__init__.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     4932 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/github/pr_comment.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.326804 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/teams/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       30 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/teams/__init__.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     6370 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/teams/card.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.327804 ntsbuildtools-4.0.9/src/ntsbuildtools/teams/
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/teams/__init__.py
+-rwxrwxr-x   0 jenkins   (1888) jenkins   (1888)     7234 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/teams/card_template.py
+-rwxrwxr-x   0 jenkins   (1888) jenkins   (1888)    10317 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/teams/cards.py
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)      261 2023-10-05 20:58:16.000000 ntsbuildtools-4.0.9/src/ntsbuildtools/util.py
+drwxrwxr-x   0 jenkins   (1888) jenkins   (1888)        0 2023-10-05 21:05:37.319804 ntsbuildtools-4.0.9/src/ntsbuildtools.egg-info/
+-rw-r--r--   0 jenkins   (1888) jenkins   (1888)     9476 2023-10-05 21:05:37.000000 ntsbuildtools-4.0.9/src/ntsbuildtools.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)     2305 2023-10-05 21:05:37.000000 ntsbuildtools-4.0.9/src/ntsbuildtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)        1 2023-10-05 21:05:37.000000 ntsbuildtools-4.0.9/src/ntsbuildtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       56 2023-10-05 21:05:37.000000 ntsbuildtools-4.0.9/src/ntsbuildtools.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       81 2023-10-05 21:05:37.000000 ntsbuildtools-4.0.9/src/ntsbuildtools.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (1888) jenkins   (1888)       14 2023-10-05 21:05:37.000000 ntsbuildtools-4.0.9/src/ntsbuildtools.egg-info/top_level.txt
```

### Comparing `ntsbuildtools-4.0.8rc0/PKG-INFO` & `ntsbuildtools-4.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntsbuildtools
-Version: 4.0.8rc0
+Version: 4.0.9
 Summary: CLI toolset that supports CICD processes.
 Home-page: https://git.uoregon.edu/projects/ISN/repos/buildtools/browse
 Author: Network & Telecom Svcs (University of Oregon)
 Author-email: rleonar7@uoregon.edu
 License: MIT
 Description: BuildTools is a collection of scripts that support the University of Oregon's Network and Telecom Services team (NTS) 
         continuous integration and deployment solutions. E.g. this solution is used in Jenkinsfile pipelines.
```

### Comparing `ntsbuildtools-4.0.8rc0/docs/README.md` & `ntsbuildtools-4.0.9/docs/README.md`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/docs/changelog.md` & `ntsbuildtools-4.0.9/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 > We started tracking this changelog as of version 3.0.0.
 
-## [4.0.8] - Sept 18, 2023
+## [4.0.9] - Oct 5, 2023
 
 ### Changed
 
 * `buildtools post teams card pull-request` has changed some arguments to optional (instead of 'required').
   * pull_request_author
   * pull_request_title
 * `buildtools parse ansible json` will now display all "failures" before displaying any "diffs"
```

### Comparing `ntsbuildtools-4.0.8rc0/docs/jenkins-cicd.md` & `ntsbuildtools-4.0.9/docs/jenkins-cicd.md`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/docs/software-design/_overview.md` & `ntsbuildtools-4.0.9/docs/software-design/_overview.md`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/docs/software-design/ansible-results.md` & `ntsbuildtools-4.0.9/docs/software-design/ansible-results.md`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/docs/software-design/cli-framework.md` & `ntsbuildtools-4.0.9/docs/software-design/cli-framework.md`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/docs/software-design/development.md` & `ntsbuildtools-4.0.9/docs/software-design/development.md`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/docs/user-guide.md` & `ntsbuildtools-4.0.9/docs/user-guide.md`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/setup.py` & `ntsbuildtools-4.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         return file_pointer.read()
 
 
 setup(
     name="ntsbuildtools",
     package_dir={"": "src"},
     packages=find_packages("src"),
-    version="4.0.8rc0",  # We attempt to follow 'semantic versioning', i.e. https://semver.org/
+    version="4.0.9",  # We attempt to follow 'semantic versioning', i.e. https://semver.org/
     license="MIT",
     description="CLI toolset that supports CICD processes.",
     long_description_content_type="text/markdown",
     long_description=read_project_file("docs/user-guide.md"),
     author="Network & Telecom Svcs (University of Oregon)",
     author_email="rleonar7@uoregon.edu",
     url="https://git.uoregon.edu/projects/ISN/repos/buildtools/browse",
```

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/inventory.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/inventory.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/playbook/results.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/playbook/results.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/return_values/default.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/return_values/default.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/ansible/return_values/factory.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/ansible/return_values/factory.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/cli/framework.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/cli/framework.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/cli/tree.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/cli/tree.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/exceptions.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/exceptions.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/main.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/main.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/markdown/comments.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/markdown/comments.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/infer/ansible/playbook_limit.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/infer/ansible/playbook_limit.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/parse/ansible/json.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/parse/ansible/json.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/bitbucket/build_status.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/bitbucket/build_status.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/bitbucket/pr_comment.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/bitbucket/pr_comment.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/bitbucket/pull_request.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/bitbucket/pull_request.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/github/pr_comment.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/github/pr_comment.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/subcommands/post/teams/card.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/subcommands/post/teams/card.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/teams/card_template.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/teams/card_template.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools/teams/cards.py` & `ntsbuildtools-4.0.9/src/ntsbuildtools/teams/cards.py`

 * *Files identical despite different names*

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools.egg-info/PKG-INFO` & `ntsbuildtools-4.0.9/src/ntsbuildtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntsbuildtools
-Version: 4.0.8rc0
+Version: 4.0.9
 Summary: CLI toolset that supports CICD processes.
 Home-page: https://git.uoregon.edu/projects/ISN/repos/buildtools/browse
 Author: Network & Telecom Svcs (University of Oregon)
 Author-email: rleonar7@uoregon.edu
 License: MIT
 Description: BuildTools is a collection of scripts that support the University of Oregon's Network and Telecom Services team (NTS) 
         continuous integration and deployment solutions. E.g. this solution is used in Jenkinsfile pipelines.
```

### Comparing `ntsbuildtools-4.0.8rc0/src/ntsbuildtools.egg-info/SOURCES.txt` & `ntsbuildtools-4.0.9/src/ntsbuildtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

