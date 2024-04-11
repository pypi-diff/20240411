# Comparing `tmp/pollination-apps-0.9.0.tar.gz` & `tmp/pollination-apps-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-apps-0.9.0.tar", last modified: Tue Sep  5 21:56:05 2023, max compression
+gzip compressed data, was "pollination-apps-0.9.1.tar", last modified: Sun Sep 17 00:06:31 2023, max compression
```

## Comparing `pollination-apps-0.9.0.tar` & `pollination-apps-0.9.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/.dependabot/
--rw-r--r--   0 runner    (1001) docker     (999)      305 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/.dependabot/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (999)     1147 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (999)     1557 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)     2849 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      287 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)      293 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (999)      279 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (999)      445 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (999)     1070 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     2027 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1032 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (999)      165 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (999)      202 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (999)       80 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/docs/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)      236 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (999)     7136 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (999)      301 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)      170 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps/cli/
--rw-r--r--   0 runner    (1001) docker     (999)     8710 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps/cli/assets/
--rw-r--r--   0 runner    (1001) docker     (999)      703 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/cli/assets/art.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1112 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (999)     3234 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/client.py
--rw-r--r--   0 runner    (1001) docker     (999)     1852 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/config.py
--rw-r--r--   0 runner    (1001) docker     (999)      742 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/env.py
--rw-r--r--   0 runner    (1001) docker     (999)      963 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/login.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps/template/
--rw-r--r--   0 runner    (1001) docker     (999)      313 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps/template/assets/
--rw-r--r--   0 runner    (1001) docker     (999)      403 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/assets/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps/template/assets/hooks/
--rw-r--r--   0 runner    (1001) docker     (999)     1606 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/assets/hooks/post_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)     3583 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-automated.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      966 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-manual.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      268 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)      144 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (999)     4100 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/.pollination/
--rw-r--r--   0 runner    (1001) docker     (999)      113 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/.pollination/config.ini
--rw-r--r--   0 runner    (1001) docker     (999)      133 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (999)      447 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/app.py
--rw-r--r--   0 runner    (1001) docker     (999)      138 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)      293 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/vtk.Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     2027 2023-09-05 21:56:04.000000 pollination-apps-0.9.0/pollination_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1811 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/pollination_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-05 21:56:04.000000 pollination-apps-0.9.0/pollination_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       64 2023-09-05 21:56:04.000000 pollination-apps-0.9.0/pollination_apps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      125 2023-09-05 21:56:04.000000 pollination-apps-0.9.0/pollination_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       17 2023-09-05 21:56:04.000000 pollination-apps-0.9.0/pollination_apps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      124 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)      102 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1053 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 21:56:05.000000 pollination-apps-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (999)       34 2023-09-05 21:54:55.000000 pollination-apps-0.9.0/tests/test_true.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.150795 pollination-apps-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/.dependabot/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/.dependabot/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.142795 pollination-apps-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-09-17 00:06:31.150795 pollination-apps-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/docs/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/pollination_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/pollination_apps/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     8710 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/pollination_apps/cli/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/cli/assets/art.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/pollination_apps/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/pollination_apps/template/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/assets/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/pollination_apps/template/assets/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/assets/hooks/post_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.150795 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-automated.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-manual.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.150795 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.150795 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/.pollination/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/.pollination/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/vtk.Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.146795 pollination-apps-0.9.1/pollination_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-09-17 00:06:31.000000 pollination-apps-0.9.1/pollination_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2023-09-17 00:06:31.000000 pollination-apps-0.9.1/pollination_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-17 00:06:31.000000 pollination-apps-0.9.1/pollination_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-17 00:06:31.000000 pollination-apps-0.9.1/pollination_apps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-09-17 00:06:31.000000 pollination-apps-0.9.1/pollination_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-17 00:06:31.000000 pollination-apps-0.9.1/pollination_apps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-09-17 00:06:31.150795 pollination-apps-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-17 00:06:31.150795 pollination-apps-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-09-17 00:05:17.000000 pollination-apps-0.9.1/tests/test_true.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pollination-apps-0.9.0/.devcontainer/Dockerfile` & `pollination-apps-0.9.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/.devcontainer/devcontainer.json` & `pollination-apps-0.9.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/.github/workflows/ci.yaml` & `pollination-apps-0.9.1/.github/workflows/ci.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         os: [ubuntu-latest]
     runs-on: ${{ matrix.os }}
     steps:
       - uses: actions/checkout@v2
       - name: set up Python
         uses: actions/setup-python@v2
         with:
-          python-version: 3.7
+          python-version: "3.10"
       - name: install python dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements.txt
           pip install -r dev-requirements.txt
       - name: run tests
         run: python -m pytest --cov=pollination_apps tests/
@@ -30,15 +30,15 @@
     needs: test
     if: github.ref == 'refs/heads/master' && github.repository_owner == 'pollination'
     steps:
       - uses: actions/checkout@v2
       - name: set up Python
         uses: actions/setup-python@v2
         with:
-          python-version: 3.7
+          python-version: "3.10"
       - name: set up node # we need node for for semantic release
         uses: actions/setup-node@v2.1.2
         with:
           node-version: 14.2.0
       - name: install python dependencies
         run: |
           python -m pip install --upgrade pip
```

### Comparing `pollination-apps-0.9.0/LICENSE` & `pollination-apps-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/README.md` & `pollination-apps-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/docs/conf.py` & `pollination-apps-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/pollination_apps/cli/__init__.py` & `pollination-apps-0.9.1/pollination_apps/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/pollination_apps/cli/assets/art.txt` & `pollination-apps-0.9.1/pollination_apps/cli/assets/art.txt`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/pollination_apps/cli/context.py` & `pollination-apps-0.9.1/pollination_apps/cli/context.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/pollination_apps/client.py` & `pollination-apps-0.9.1/pollination_apps/client.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/pollination_apps/config.py` & `pollination-apps-0.9.1/pollination_apps/config.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/pollination_apps/env.py` & `pollination-apps-0.9.1/pollination_apps/env.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/pollination_apps/login.py` & `pollination-apps-0.9.1/pollination_apps/login.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/pollination_apps/template/assets/hooks/post_gen_project.py` & `pollination-apps-0.9.1/pollination_apps/template/assets/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-automated.yaml` & `pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-automated.yaml`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-manual.yaml` & `pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-manual.yaml`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/README.md` & `pollination-apps-0.9.1/pollination_apps/template/assets/{{cookiecutter.app_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/pollination_apps.egg-info/SOURCES.txt` & `pollination-apps-0.9.1/pollination_apps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.9.0/setup.py` & `pollination-apps-0.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,13 +20,14 @@
     install_requires=requirements,
     entry_points={
         "console_scripts": ["pollination-apps = pollination_apps.cli:main"]
     },
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
     license="MIT"
 )
```

