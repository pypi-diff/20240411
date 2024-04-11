# Comparing `tmp/documenteer-1.2.1.tar.gz` & `tmp/documenteer-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "documenteer-1.2.1.tar", last modified: Tue Apr  2 17:09:35 2024, max compression
+gzip compressed data, was "documenteer-1.2.2.tar", last modified: Thu Apr 11 19:23:41 2024, max compression
```

## Comparing `documenteer-1.2.1.tar` & `documenteer-1.2.2.tar`

### file list

```diff
@@ -1,314 +1,314 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.975126 documenteer-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-02 17:09:08.000000 documenteer-1.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.931126 documenteer-1.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.931126 documenteer-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/workflows/ci-cron.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 17:09:08.000000 documenteer-1.2.1/.github/workflows/dependencies.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-02 17:09:08.000000 documenteer-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 17:09:08.000000 documenteer-1.2.1/.npmrc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 17:09:08.000000 documenteer-1.2.1/.nvmrc
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-02 17:09:08.000000 documenteer-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 17:09:08.000000 documenteer-1.2.1/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 17:09:08.000000 documenteer-1.2.1/.prettierrc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.931126 documenteer-1.2.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 17:09:08.000000 documenteer-1.2.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-02 17:09:08.000000 documenteer-1.2.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)    38485 2024-04-02 17:09:08.000000 documenteer-1.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-02 17:09:08.000000 documenteer-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 17:09:08.000000 documenteer-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-02 17:09:08.000000 documenteer-1.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-02 17:09:35.975126 documenteer-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-02 17:09:08.000000 documenteer-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.931126 documenteer-1.2.1/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 17:09:08.000000 documenteer-1.2.1/changelog.d/_template.md.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.919126 documenteer-1.2.1/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.931126 documenteer-1.2.1/demo/ipynb-technote/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/ipynb-technote/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/ipynb-technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/ipynb-technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/ipynb-technote/diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/ipynb-technote/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/ipynb-technote/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.931126 documenteer-1.2.1/demo/md-technote/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/md-technote/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/md-technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/md-technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/md-technote/diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/md-technote/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/md-technote/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.935126 documenteer-1.2.1/demo/rst-technote/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/rst-technote/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/rst-technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/rst-technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/rst-technote/diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/rst-technote/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 17:09:08.000000 documenteer-1.2.1/demo/rst-technote/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.935126 documenteer-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (127)    38485 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.935126 documenteer-1.2.1/docs/dev/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.935126 documenteer-1.2.1/docs/dev/api/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/api/documenteer.conf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/api/documenteer.ext.rst
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/api/documenteer.requestsutils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/api/documenteer.sphinxrunner.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/api/documenteer.stackdocs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/html-templates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/theme-assets.rst
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/dev/theme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/documenteer.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.939126 documenteer-1.2.1/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/badges.rst
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/configuration-preset.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/diagrams.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/extend-conf-py.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/including-notebooks.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/markdown-primer.md
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/openapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/organization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.939126 documenteer-1.2.1/docs/guides/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/build-overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/cpp-api-linking.rst
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/package-docs-cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pipelines/stack-docs-cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/pyproject-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/rst-epilog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/tabsets.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/guides/toml-reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.943126 documenteer-1.2.1/docs/sphinx-extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/autocppapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/autodocreset.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/docushare-reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/githubbibcache.rst
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/jira-reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/lsst-pybtex-style.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/lssttasks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/openapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/package-toctree.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/sphinx-extensions/remote-code-block.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.943126 documenteer-1.2.1/docs/technotes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.943126 documenteer-1.2.1/docs/technotes/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/_templates/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/author-metadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/document-status.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/edit-locally.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/edit-on-github.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/how-your-technote-gets-published.rst
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/migrate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-02 17:09:08.000000 documenteer-1.2.1/docs/technotes/start-a-technote.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.943126 documenteer-1.2.1/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-02 17:09:08.000000 documenteer-1.2.1/licenses/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-02 17:09:08.000000 documenteer-1.2.1/licenses/astropy-helpers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-02 17:09:08.000000 documenteer-1.2.1/licenses/sphinx-issue.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13362 2024-04-02 17:09:08.000000 documenteer-1.2.1/licenses/sphinx.txt
--rw-r--r--   0 runner    (1001) docker     (127)   212497 2024-04-02 17:09:15.000000 documenteer-1.2.1/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-02 17:09:08.000000 documenteer-1.2.1/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 17:09:08.000000 documenteer-1.2.1/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-02 17:09:08.000000 documenteer-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 17:09:35.975126 documenteer-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.919126 documenteer-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.919126 documenteer-1.2.1/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.919126 documenteer-1.2.1/src/assets/rubin-technote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.947126 documenteer-1.2.1/src/assets/rubin-technote/styles/
--rw-r--r--   0 runner    (1001) docker     (127)   137996 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/SourceSans3VF-Italic.ttf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   170188 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/SourceSans3VF-Upright.ttf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/_hacks.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/_properties.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.947126 documenteer-1.2.1/src/assets/rubin-technote/styles/components/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/components/_article-header.scss
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/components/_authors.scss
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/components/_index.scss
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/components/_sidebar-section.scss
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/components/_version-info.scss
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/assets/rubin-technote/styles/rubin-technote.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.947126 documenteer-1.2.1/src/documenteer/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.951126 documenteer-1.2.1/src/documenteer/assets/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)   137996 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/731c8feefe13e72a8691.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   170188 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/b8bc3440ba2145e132f5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.951126 documenteer-1.2.1/src/documenteer/assets/rsd-assets/
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/rubin-favicon-transparent-32px.png
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/rubin-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/rubin-pydata-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/rubin-technote.css
--rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/rubin-technote.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.951126 documenteer-1.2.1/src/documenteer/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/scripts/rubin-technote.js
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-02 17:09:17.000000 documenteer-1.2.1/src/documenteer/assets/scripts/rubin-technote.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.955126 documenteer-1.2.1/src/documenteer/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17509 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/_toml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/guide.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/pipelinespkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/conf/technote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.955126 documenteer-1.2.1/src/documenteer/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/autocppapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/autodocreset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/githubbibcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/jira.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lsstdocushare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.955126 documenteer-1.2.1/src/documenteer/ext/lssttasks/
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39797 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/configfieldlists.py
--rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/crossrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/pyapisummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/taskutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/topiclists.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/lssttasks/topics.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/mockcoderefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/packagetoctree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/ext/remotecodeblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/packagemetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/requestsutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.959126 documenteer-1.2.1/src/documenteer/services/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/services/technoteauthor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/services/technotemigration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/sphinxrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.959126 documenteer-1.2.1/src/documenteer/stackdocs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.959126 documenteer-1.2.1/src/documenteer/stackdocs/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1063166 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
--rw-r--r--   0 runner    (1001) docker     (127)   105749 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/data/doxygen.defaults.conf
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/data/mainpage.dox
--rw-r--r--   0 runner    (1001) docker     (127)    23844 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/doxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/packagecli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/stackdocs/stackcli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.963126 documenteer-1.2.1/src/documenteer/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/authordb.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/latex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.923126 documenteer-1.2.1/src/documenteer/storage/localtemplates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.963126 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/localtemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/storage/technotetoml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.923126 documenteer-1.2.1/src/documenteer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.963126 documenteer-1.2.1/src/documenteer/templates/pydata/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/pydata/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.963126 documenteer-1.2.1/src/documenteer/templates/technote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/technote/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.963126 documenteer-1.2.1/src/documenteer/templates/technote/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/technote/components/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/technote/components/sidebar-source.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.963126 documenteer-1.2.1/src/documenteer/templates/technote/sections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/technote/sections/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/technote/sections/header-article.html
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/templates/technote/sections/sidebar-primary.html
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-02 17:09:08.000000 documenteer-1.2.1/src/documenteer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.971126 documenteer-1.2.1/src/documenteer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-02 17:09:35.000000 documenteer-1.2.1/src/documenteer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-02 17:09:35.000000 documenteer-1.2.1/src/documenteer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 17:09:35.000000 documenteer-1.2.1/src/documenteer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 17:09:35.000000 documenteer-1.2.1/src/documenteer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-02 17:09:35.000000 documenteer-1.2.1/src/documenteer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 17:09:35.000000 documenteer-1.2.1/src/documenteer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/afw.doxygen.conf
--rw-r--r--   0 runner    (1001) docker     (127)    82475 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/authordb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   199942 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/doxygen.tag.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.923126 documenteer-1.2.1/tests/data/package_alpha/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_alpha/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.923126 documenteer-1.2.1/tests/data/package_alpha/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_alpha/doc/_static/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/doc/_static/package_alpha/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/doc/doxygen.conf.in
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/doc/manifest.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_alpha/doc/package.alpha/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/doc/package.alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_alpha/doc/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/doc/package_alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_alpha/include/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_alpha/src/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_alpha/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.923126 documenteer-1.2.1/tests/data/package_beta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/data/package_beta/doc/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/data/package_beta/doc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.967126 documenteer-1.2.1/tests/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/autocppapi_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/jira_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/lsstdocushare_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.971126 documenteer-1.2.1/tests/ext/lssttasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/lssttasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/lssttasks/taskutils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/mockcoderefs_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/packagetoctree_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/ext/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/packagemetadata_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.923126 documenteer-1.2.1/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.971126 documenteer-1.2.1/tests/roots/test-autocppapi/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/roots/test-autocppapi/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)   199942 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/roots/test-autocppapi/doxygen.tag.zip
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/roots/test-autocppapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.971126 documenteer-1.2.1/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/services/technotemigration_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:35.971126 documenteer-1.2.1/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/storage/authordb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/storage/technotetoml_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_conf_toml.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_conf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_stackdocs_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_stackdocs_doxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_stackdocs_doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_stackdocs_pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-02 17:09:08.000000 documenteer-1.2.1/tests/test_stackdocs_rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-02 17:09:08.000000 documenteer-1.2.1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-02 17:09:08.000000 documenteer-1.2.1/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.972368 documenteer-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-11 19:23:26.000000 documenteer-1.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.924368 documenteer-1.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.924368 documenteer-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/workflows/ci-cron.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/workflows/dependencies.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-11 19:23:26.000000 documenteer-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 19:23:26.000000 documenteer-1.2.2/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 19:23:26.000000 documenteer-1.2.2/.nvmrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-11 19:23:26.000000 documenteer-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-11 19:23:26.000000 documenteer-1.2.2/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-11 19:23:26.000000 documenteer-1.2.2/.prettierrc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.924368 documenteer-1.2.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-11 19:23:26.000000 documenteer-1.2.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-11 19:23:26.000000 documenteer-1.2.2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39095 2024-04-11 19:23:26.000000 documenteer-1.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-11 19:23:26.000000 documenteer-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-11 19:23:26.000000 documenteer-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-11 19:23:26.000000 documenteer-1.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-11 19:23:41.972368 documenteer-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-11 19:23:26.000000 documenteer-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.924368 documenteer-1.2.2/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-11 19:23:26.000000 documenteer-1.2.2/changelog.d/_template.md.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.916368 documenteer-1.2.2/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.924368 documenteer-1.2.2/demo/ipynb-technote/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/ipynb-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/ipynb-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/ipynb-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/ipynb-technote/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/ipynb-technote/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/ipynb-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.928368 documenteer-1.2.2/demo/md-technote/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/md-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/md-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/md-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/md-technote/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/md-technote/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/md-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.928368 documenteer-1.2.2/demo/rst-technote/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/rst-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/rst-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/rst-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/rst-technote/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/rst-technote/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/rst-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.928368 documenteer-1.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    39095 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.928368 documenteer-1.2.2/docs/dev/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.932368 documenteer-1.2.2/docs/dev/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/api/documenteer.conf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/api/documenteer.ext.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/api/documenteer.requestsutils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/api/documenteer.sphinxrunner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/api/documenteer.stackdocs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/html-templates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/theme-assets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/theme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/documenteer.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.932368 documenteer-1.2.2/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/configuration-preset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/diagrams.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/extend-conf-py.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/including-notebooks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/markdown-primer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/organization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.936368 documenteer-1.2.2/docs/guides/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/build-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/cpp-api-linking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/package-docs-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/stack-docs-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pyproject-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/rst-epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/tabsets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/toml-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.936368 documenteer-1.2.2/docs/sphinx-extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/autocppapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/autodocreset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/docushare-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/githubbibcache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/jira-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/lsst-pybtex-style.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/lssttasks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/package-toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/remote-code-block.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.940368 documenteer-1.2.2/docs/technotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.940368 documenteer-1.2.2/docs/technotes/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/_templates/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/author-metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/document-status.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/edit-locally.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/edit-on-github.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/how-your-technote-gets-published.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/migrate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/start-a-technote.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.940368 documenteer-1.2.2/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-11 19:23:26.000000 documenteer-1.2.2/licenses/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-11 19:23:26.000000 documenteer-1.2.2/licenses/astropy-helpers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-11 19:23:26.000000 documenteer-1.2.2/licenses/sphinx-issue.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13362 2024-04-11 19:23:26.000000 documenteer-1.2.2/licenses/sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   212497 2024-04-11 19:23:34.000000 documenteer-1.2.2/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-11 19:23:26.000000 documenteer-1.2.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 19:23:26.000000 documenteer-1.2.2/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-11 19:23:26.000000 documenteer-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:23:41.972368 documenteer-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.916368 documenteer-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.916368 documenteer-1.2.2/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.916368 documenteer-1.2.2/src/assets/rubin-technote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.940368 documenteer-1.2.2/src/assets/rubin-technote/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)   137996 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/SourceSans3VF-Italic.ttf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   170188 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/SourceSans3VF-Upright.ttf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/_hacks.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/_properties.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.940368 documenteer-1.2.2/src/assets/rubin-technote/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/components/_article-header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/components/_authors.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/components/_index.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/components/_sidebar-section.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/components/_version-info.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/rubin-technote.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.944368 documenteer-1.2.2/src/documenteer/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.948368 documenteer-1.2.2/src/documenteer/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)   137996 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/731c8feefe13e72a8691.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   170188 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/b8bc3440ba2145e132f5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.948368 documenteer-1.2.2/src/documenteer/assets/rsd-assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/rubin-favicon-transparent-32px.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/rubin-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/rubin-pydata-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/rubin-technote.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/rubin-technote.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.948368 documenteer-1.2.2/src/documenteer/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/scripts/rubin-technote.js
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/scripts/rubin-technote.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.948368 documenteer-1.2.2/src/documenteer/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17509 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13853 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/pipelinespkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/technote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.952368 documenteer-1.2.2/src/documenteer/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/autocppapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/autodocreset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/githubbibcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lsstdocushare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.952368 documenteer-1.2.2/src/documenteer/ext/lssttasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39797 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/configfieldlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/crossrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/pyapisummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/taskutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/topiclists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/mockcoderefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/packagetoctree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/remotecodeblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/packagemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/requestsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.952368 documenteer-1.2.2/src/documenteer/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/services/technoteauthor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/services/technotemigration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/sphinxrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.956368 documenteer-1.2.2/src/documenteer/stackdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.956368 documenteer-1.2.2/src/documenteer/stackdocs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1063166 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   105749 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/data/doxygen.defaults.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/data/mainpage.dox
+-rw-r--r--   0 runner    (1001) docker     (127)    23844 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/packagecli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/stackcli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.956368 documenteer-1.2.2/src/documenteer/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/authordb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/latex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.916368 documenteer-1.2.2/src/documenteer/storage/localtemplates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.960368 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/technotetoml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.920368 documenteer-1.2.2/src/documenteer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.960368 documenteer-1.2.2/src/documenteer/templates/pydata/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/pydata/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.960368 documenteer-1.2.2/src/documenteer/templates/technote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/technote/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.960368 documenteer-1.2.2/src/documenteer/templates/technote/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/technote/components/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/technote/components/sidebar-source.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.960368 documenteer-1.2.2/src/documenteer/templates/technote/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/technote/sections/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/technote/sections/header-article.html
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/technote/sections/sidebar-primary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.968368 documenteer-1.2.2/src/documenteer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-11 19:23:41.000000 documenteer-1.2.2/src/documenteer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-11 19:23:41.000000 documenteer-1.2.2/src/documenteer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:23:41.000000 documenteer-1.2.2/src/documenteer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 19:23:41.000000 documenteer-1.2.2/src/documenteer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-11 19:23:41.000000 documenteer-1.2.2/src/documenteer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 19:23:41.000000 documenteer-1.2.2/src/documenteer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/afw.doxygen.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    82475 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/authordb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   199942 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/doxygen.tag.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.920368 documenteer-1.2.2/tests/data/package_alpha/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_alpha/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.920368 documenteer-1.2.2/tests/data/package_alpha/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_alpha/doc/_static/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/doc/_static/package_alpha/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/doc/doxygen.conf.in
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/doc/manifest.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_alpha/doc/package.alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/doc/package.alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_alpha/doc/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/doc/package_alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_alpha/include/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_alpha/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.920368 documenteer-1.2.2/tests/data/package_beta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_beta/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_beta/doc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/autocppapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/jira_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/lsstdocushare_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.968368 documenteer-1.2.2/tests/ext/lssttasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/lssttasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/lssttasks/taskutils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/mockcoderefs_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/packagetoctree_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/packagemetadata_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.920368 documenteer-1.2.2/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.968368 documenteer-1.2.2/tests/roots/test-autocppapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/roots/test-autocppapi/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   199942 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/roots/test-autocppapi/doxygen.tag.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/roots/test-autocppapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.968368 documenteer-1.2.2/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/services/technotemigration_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.968368 documenteer-1.2.2/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/storage/authordb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/storage/technotetoml_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_conf_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_conf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_stackdocs_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_stackdocs_doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_stackdocs_doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_stackdocs_pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_stackdocs_rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-11 19:23:26.000000 documenteer-1.2.2/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-11 19:23:26.000000 documenteer-1.2.2/webpack.config.js
```

### Comparing `documenteer-1.2.1/.github/workflows/ci-cron.yaml` & `documenteer-1.2.2/.github/workflows/ci-cron.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/.github/workflows/ci.yaml` & `documenteer-1.2.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/.github/workflows/dependencies.yaml` & `documenteer-1.2.2/.github/workflows/dependencies.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/.gitignore` & `documenteer-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/.pre-commit-config.yaml` & `documenteer-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/.vscode/tasks.json` & `documenteer-1.2.2/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/CHANGELOG.md` & `documenteer-1.2.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Change Log
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-1.2.2'></a>
+## 1.2.2 (2024-04-11)
+
+### Bug fixes
+
+- Update `jira_uri_template` configuration default to `https://rubinobs.atlassian.net/browse/{issue}`. This will make all :jira:, :jirab:, and :jirap: roles point to the new Jira instance for Rubin Observatory.
+- Drop `jira.lsstcorp.org` from the linkcheck ignore list defaults for `documenteer.config.guide` since that instance is no longer being used.
+- Replace `jira.lsstcorp.org` URLs in documentation to `rubinobs.atlassian.net`.
+
 <a id='changelog-1.2.1'></a>
 ## 1.2.1 (2024-04-02)
 
 ### Bug fixes
 
 - Fix the "Source parser for markdown not registered" error for Markdown-based technotes. With the MyST-NB extension the Markdown parser is automatically registered, so the `documenteer.conf.technote` configuration now resets the `source_suffix` configuration originally created by the Technote package.
 
@@ -336,15 +345,15 @@
 - New Sphinx configuration facilities should prevent recursion issues by more cleanly populating the Python attributes in the configuration module:
 
   - Technote projects now import `documenteer.conf.technote` in their `conf.py` files.
   - Stack projects now import `documenteer.conf.pipelines` in their `conf.py` files.
   - Individual Stack packages now import `documenteer.conf.pipelinespkg` in their `conf.py` files.
 
   The previous configuration sub-package, `documenteer.sphinxconf` is deprecated.
-  [[DM-20866](https://jira.lsstcorp.org/browse/DM-20866)]
+  [[DM-20866](https://rubinobs.atlassian.net/browse/DM-20866)]
 
   Overall, the configurations are compatible with these exceptions:
 
   - ReStructuredText source files are no longer copied into the built site for Pipelines projects (`html_copy_source` is `False`).
     This change reduces the upload site of the pipelines.lsst.io site.
   - Updated the MathJax CDN URL to point to cdnjs.
 
@@ -359,85 +368,85 @@
   It's intended to be used equivalently to the `automodapi` extension.
 
   The built-in Doxygen build considers all Stack packages with a `doc/doxygen.conf.in` file.
   Documenteer creates a Doxygen configuration from the contents of each package's `doxygen.conf.in` file, along with built-in defaults appropriate for pipelines.lsst.io.
   For example, individual packages can add to the `EXCLUDE` tag.
   By default, each package's `include` directory is included in the Doxygen build.
 
-  [[DM-22698](https://jira.lsstcorp.org/browse/DM-22698), [DM-23094](https://jira.lsstcorp.org/browse/DM-23094), [DM-22461](https://jira.lsstcorp.org/browse/DM-22461)]
+  [[DM-22698](https://rubinobs.atlassian.net/browse/DM-22698), [DM-23094](https://rubinobs.atlassian.net/browse/DM-23094), [DM-22461](https://rubinobs.atlassian.net/browse/DM-22461)]
 
 - Improved Sphinx runner (`documenteer.sphinxrunner`).
-  [[DM-26768](https://jira.lsstcorp.org/browse/DM-26768)]
+  [[DM-26768](https://rubinobs.atlassian.net/browse/DM-26768)]
 
 - Added static type checking using [mypy](https://mypy.readthedocs.io/en/stable/).
-  [[DM-22717](https://jira.lsstcorp.org/browse/DM-22717), [DM-26288](https://jira.lsstcorp.org/browse/DM-26288)]
+  [[DM-22717](https://rubinobs.atlassian.net/browse/DM-22717), [DM-26288](https://rubinobs.atlassian.net/browse/DM-26288)]
 
 - Improved packaging, testing, and development environment:
 
   - PEP 518-ify the build process by adding a `pyproject.toml` file.
   - Removed the deprecated pytest-runner plugin.
   - Moved most of the packaging configuration to `setup.cfg`.
   - Adopted black and isort for code formatting.
   - Migrated to `tox` for running tests.
   - Migrated to `pre-commit` for running linters and code formatters.
   - Migrated to GitHub Actions from Travis CI.
 
-  [`DM-22957 <https://jira.lsstcorp.org/browse/DM-22957>`_, `DM-26288 <https://jira.lsstcorp.org/browse/DM-26288>`_]
+  [`DM-22957 <https://rubinobs.atlassian.net/browse/DM-22957>`_, `DM-26288 <https://rubinobs.atlassian.net/browse/DM-26288>`_]
 
 - Documentation improvements:
 
   - Added a new Developer guide and Release procedure guide.
   - Added an installation page.
   - Moved the Python API reference to its own page.
   - Improved the README to list features.
 
 - Added GitHub community health features: contributing, support, and code of conduct files.
 
 ## 0.5.5 (2019-12-09)
 
 - Technote configuration now uses `yaml.safe_load` instead of `yaml.load`.
   See the [pyyaml docs for details](https://github.com/yaml/pyyaml/wiki/PyYAML-yaml.load(input)-Deprecation).
-  [[DM-22537](https://jira.lsstcorp.org/browse/DM-22537)]
+  [[DM-22537](https://rubinobs.atlassian.net/browse/DM-22537)]
 
 ## 0.5.4 (2019-11-03)
 
 - This new version of the technote sphinx theme should fix the edition link in the sidebar for non-main editions.
-  [[DM-20839](https://jira.lsstcorp.org/browse/DM-20839)]
+  [[DM-20839](https://rubinobs.atlassian.net/browse/DM-20839)]
 
 ## 0.5.3 (2019-08-07)
 
 - Enabled the `html_use_index` and `html_domain_indices` configurations for Stack documentation projects to enable automatic index generation.
   The `genindex` contains links to all command-line options and Python objects (Sphinx's domains).
   This also opens us up to a more general content index by way of the [index directive](https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#index-generating-markup).
-  [[DM-20850](https://jira.lsstcorp.org/browse/DM-20850)]
+  [[DM-20850](https://rubinobs.atlassian.net/browse/DM-20850)]
 
 - Fixed compatibility with docutils 0.15.
   Now Sphinx will control which version of docutils is used, which should now be 0.15.
 
 - Also updated the intersphinx URL for Pandas to use https.
 
 ## 0.5.2 (2019-08-01)
 
 - Add [sphinxcontrib.autoprogram](https://sphinxcontrib-autoprogram.readthedocs.io/en/stable/) to enable automated reference documentation of argparse-based command-line scripts.
   This extension is available with the `documenteer[pipelines]` installation extra and enabled by default for LSST Science Pipelines projects.
-  [[DM-20767](https://jira.lsstcorp.org/browse/)]
+  [[DM-20767](https://rubinobs.atlassian.net/browse/)]
 
 - Update the official list of tested and supported Python versions to Python 3.6 and 3.7.
 
 ## 0.5.1 (2019-07-22)
 
 - Pin docutils temporarily to `0.14`.
   The latest release, 0.15, is currently incompatible with the `:jira:` role.
 
 ## 0.5.0 (2019-02-11)
 
 - The stack documentation build now requires that packages be explicitly required by the main documentation project's EUPS table file.
   Before, a package only needed a `doc/manifest.yaml` file and to be currently set up in the EUPS environment to be linked into the documentation build.
   This would lead to packages being included in a documentation build despite not being a part of that stack product.
-  [[DM-17765](https://jira.lsstcorp.org/browse/DM-17765)]
+  [[DM-17765](https://rubinobs.atlassian.net/browse/DM-17765)]
 
 - This release adds the [sphinx-jinja](https://github.com/tardyp/sphinx-jinja) extension for `documenteer[pipelines]` installations.
   This extension makes it possible to dynamically create content with Jinja templating.
 
   The `documenteer.sphinxconfig.stackconf` module sets up a `default` context for the `jinja` directive that includes all module attributes in the Sphinx config module.
 
 - The `documenteer.sphinxconfig.stackconf` module includes several new configuration attributes that are driven by the presence of an `EUPS_TAG` environment variable.
@@ -449,54 +458,54 @@
   - `release`
   - `version`
   - `scipipe_conda_ref`
   - `newinstall_ref`
   - `pipelines_demo_ref`
 
   These variables are accessible from the `jinja` directive's context.
-  [[DM-17065](https://jira.lsstcorp.org/browse/DM-17065)]
+  [[DM-17065](https://rubinobs.atlassian.net/browse/DM-17065)]
 
 - This release also added some new substitutions to the `rst_epilog` of stack-based projects:
 
   - `|eups-tag|` --- the current EUPS tag, based on the `EUPS_TAG` environment variable.
   - `|eups-tag-mono|` --- monospace typeface version of `|eups-tag|`.
   - `|eups-tag-bold|` --- bold typeface version of `|eups-tag|`.
 
   The `|current-release|` substitution is no longer available.
 
 - Fixed some bugs with the display of copyrights in stack-based projects.
 
 - The project's name is also used as the `logotext` at the top of the page for stack-based projects.
   Previously the `logotext` would always be "LSST Science Pipelines."
-  [[DM-17263](https://jira.lsstcorp.org/browse/DM-17263)]
+  [[DM-17263](https://rubinobs.atlassian.net/browse/DM-17263)]
 
 - Added the following projects to the intersphinx inventory of stack-based projects:
 
   - `firefly_client`
   - `astro_metadata_translator`
 
 ## 0.4.5 (2019-02-06)
 
 - Added a new `lso` role for linking to LSST Operations documents in DocuShare.
 
 ## 0.4.4 (2019-02-05)
 
 - Updated scikit-learn's intersphinx inventory URL (now available as HTTPS) in the `documenteer.sphinxconfig.stackconf`.
-- Fixed the `lsst-task-config-subtasks` directive so that it can introspect items in an `lsst.pex.config` `Registry` that are wrapped by a `ConfigurableWrapper`. [(DM-17661)[https://jira.lsstcorp.org/browse/DM-17661]]
+- Fixed the `lsst-task-config-subtasks` directive so that it can introspect items in an `lsst.pex.config` `Registry` that are wrapped by a `ConfigurableWrapper`. [(DM-17661)[https://rubinobs.atlassian.net/browse/DM-17661]]
 
 ## 0.4.3 (2018-11-30)
 
 - Pin [sphinxcontrib-bibtex](https://github.com/mcmtroffaes/sphinxcontrib-bibtex) to version 0.4.0 since later versions are incompatible with Sphinx <1.8.0.
-  [[DM-16651](https://jira.lsstcorp.org/browse/DM-16651)]
+  [[DM-16651](https://rubinobs.atlassian.net/browse/DM-16651)]
 
 ## 0.4.2 (2018-11-01)
 
 - Handle cases where an object does not have a docstring in `documenteer.sphinxext.lssttasks.taskutils.get_docstring`.
   This improves the reliability of the `lsst-task-api-summary` directive.
-  See (DM-16102)(https://jira.lsstcorp.org/browse/DM-16102).
+  See (DM-16102)(https://rubinobs.atlassian.net/browse/DM-16102).
 
 ## 0.4.1 (2018-10-15)
 
 - Add `documenteer.sphinxext.lssttasks` to the Sphinx extensions available for pipelines.lsst.io documentation builds.
 
 - For pipelines.lsst.io builds, Documenteer ignores the `home/` directory that's created at the root of the `pipelines_lsst_io` directory.
   This directory is created as part of the ci.lsst.codes `sqre/infra/documenteer` job and shouldn't be part of the documentation build.
@@ -517,15 +526,15 @@
 
 - Added Astropy to the intersphinx configuration.
 
 - Enabled `automodsumm_inherited_members` in the stackconf for stack documentation.
   This configuration is critical:
 
   1. It is actually responsible for ensuring that inherited members of classes appear in our docs.
-  2. Without this, classes that have a `__slots__` attribute (typically through inheritance of a `collections.abc` class) won't have *any* of their members documented. See (DM-16102)(https://jira.lsstcorp.org/browse/DM-16102) for discussion.
+  2. Without this, classes that have a `__slots__` attribute (typically through inheritance of a `collections.abc` class) won't have *any* of their members documented. See (DM-16102)(https://rubinobs.atlassian.net/browse/DM-16102) for discussion.
 
 - `todo` directives are now hidden when using `build_pipelines_lsst_io_configs`.
   They are still shown, by default, for standalone package documentation builds, which are primarily developer-facing.
 
 ## 0.3.0 (2018-09-19)
 
 - New `remote-code-block`, which works like the `literalinclude` directive, but allows you to include content from a URL over the web.
@@ -646,15 +655,15 @@
 ## 0.1.11 (2017-03-01)
 
 - Add `documenteer.sphinxconfig.utils.form_ltd_edition_name` to form LSST the Docs-like edition names for Git refs.
 - Configure automated PyPI deployments with Travis.
 
 ## 0.1.10 (2016-12-14)
 
-Includes prototype support for LSST Science Pipelines documentation, as part of `DM-6199 <https://jira.lsstcorp.org/browse/DM-6199>`__:
+Includes prototype support for LSST Science Pipelines documentation, as part of `DM-6199 <https://rubinobs.atlassian.net/browse/DM-6199>`__:
 
 - Added dependencies to [breathe](http://breathe.readthedocs.io/en/latest/), [astropy-helpers](https://github.com/astropy/astropy-helpers) and the [lsst-sphinx-bootstrap-theme](https://github.com/lsst-sqre/lsst-sphinx-bootstrap-theme) to generally coordinate LSST Science Pipelines documentation dependencies.
 - Created `documenteer.sphinxconfig.stackconf` module to centrally coordinate Science Pipelines documentation configuration. Much of the configuration is based on [astropy-helper's Sphinx configuration](https://github.com/astropy/astropy-helpers/blob/master/astropy_helpers/sphinx/conf.py) since the LSST Science Pipelines documentation is heavily based upon Astropy's Sphinx theme and API reference generation infrastructure.
   Also includes prototype configuration for breathe (the doxygen XML bridge).
 - Updated test harness (pytest and plugin versions).
 
 ## 0.1.9 (2016-07-08)
@@ -681,15 +690,15 @@
 
 ## 0.1.4 (2016-05-27)
 
 - Add roles for making mock references to code objects that don't have API references yet. E.g. `lclass`, `lfunc`. DM-6326.
 
 ## 0.1.3 (2016-05-24)
 
-- Add roles for linking to ls.st links: `lpm`, `ldm`, and `lse`. DM-6181.
+- Add roles for linking to `ls.st` links: `lpm`, `ldm`, and `lse`. DM-6181.
 - Add roles for linking to JIRA tickets: `jira`, `jirab`, and `jirap`. DM-6181.
 
 ## 0.1.2 (2016-05-14)
 
 - Include [sphinxcontrib-bibtex](https://sphinxcontrib-bibtex.readthedocs.io/) to Sphinx extensions available in technote projects. DM-6033.
 
 ## 0.1.0 (2015-11-23)
```

### Comparing `documenteer-1.2.1/LICENSE` & `documenteer-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/PKG-INFO` & `documenteer-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 1.2.1
+Version: 1.2.2
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `documenteer-1.2.1/README.md` & `documenteer-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/demo/ipynb-technote/index.ipynb` & `documenteer-1.2.2/demo/ipynb-technote/index.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991319444444444%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(6, 'A parenthetical citation {cite:p}`SQR-083`. And a "*

 * *            "textual citation {cite:t}`SQR-083`.')], delete: [6]}}}"}*

```diff
@@ -17,15 +17,15 @@
             "source": [
                 "## Introduction\n",
                 "\n",
                 "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin facilisis pharetra neque, at semper nulla mattis auctor. Proin semper mollis enim eget interdum. Mauris eleifend eget diam vitae bibendum. Praesent ut aliquet odio, sodales imperdiet nisi. Nam interdum imperdiet tortor sed fringilla. Maecenas efficitur mi sodales nulla commodo rutrum. Ut ornare diam quam, sed commodo turpis aliquam et. In nec enim consequat, suscipit tortor sit amet, luctus ante. Integer dictum augue diam, non pulvinar massa euismod in. Morbi viverra condimentum auctor. Nullam et metus mauris. Cras risus ex, porta sit amet nibh et, dapibus auctor leo.\n",
                 "\n",
                 "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin facilisis pharetra neque, at semper nulla mattis auctor. Proin semper mollis enim eget interdum. Mauris eleifend eget diam vitae bibendum. Praesent ut aliquet odio, sodales imperdiet nisi. Nam interdum imperdiet tortor sed fringilla. Maecenas efficitur mi sodales nulla commodo rutrum. Ut ornare diam quam, sed commodo turpis aliquam et. In nec enim consequat, suscipit tortor sit amet, luctus ante. Integer dictum augue diam, non pulvinar massa euismod in. Morbi viverra condimentum auctor. Nullam et metus mauris. Cras risus ex, porta sit amet nibh et, dapibus auctor leo.\n",
                 "\n",
-                "A parenthetical citation {cite:p}`2017arXiv170309824V`. And a textual citation {cite:t}`2017arXiv170309824V`."
+                "A parenthetical citation {cite:p}`SQR-083`. And a textual citation {cite:t}`SQR-083`."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Method\n",
```

### Comparing `documenteer-1.2.1/demo/ipynb-technote/technote.toml` & `documenteer-1.2.2/demo/ipynb-technote/technote.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/demo/md-technote/index.md` & `documenteer-1.2.2/demo/md-technote/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## Introduction
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin facilisis pharetra neque, at semper nulla mattis auctor. Proin semper mollis enim eget interdum. Mauris eleifend eget diam vitae bibendum. Praesent ut aliquet odio, sodales imperdiet nisi. Nam interdum imperdiet tortor sed fringilla. Maecenas efficitur mi sodales nulla commodo rutrum. Ut ornare diam quam, sed commodo turpis aliquam et. In nec enim consequat, suscipit tortor sit amet, luctus ante. Integer dictum augue diam, non pulvinar massa euismod in. Morbi viverra condimentum auctor. Nullam et metus mauris. Cras risus ex, porta sit amet nibh et, dapibus auctor leo.
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin facilisis pharetra neque, at semper nulla mattis auctor. Proin semper mollis enim eget interdum. Mauris eleifend eget diam vitae bibendum. Praesent ut aliquet odio, sodales imperdiet nisi. Nam interdum imperdiet tortor sed fringilla. Maecenas efficitur mi sodales nulla commodo rutrum. Ut ornare diam quam, sed commodo turpis aliquam et. In nec enim consequat, suscipit tortor sit amet, luctus ante. Integer dictum augue diam, non pulvinar massa euismod in. Morbi viverra condimentum auctor. Nullam et metus mauris. Cras risus ex, porta sit amet nibh et, dapibus auctor leo.
 
-A parenthetical citation {cite:p}`2017arXiv170309824V`. And a textual citation {cite:t}`2017arXiv170309824V`.
+A parenthetical citation {cite:p}`SQR-083`. And a textual citation {cite:t}`SQR-083`.
 
 ## Method
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin facilisis pharetra neque, at semper nulla mattis auctor. Proin semper mollis enim eget interdum. Mauris eleifend eget diam vitae bibendum. Praesent ut aliquet odio, sodales imperdiet nisi. Nam interdum imperdiet tortor sed fringilla. Maecenas efficitur mi sodales nulla commodo rutrum. Ut ornare diam quam, sed commodo turpis aliquam et. In nec enim consequat, suscipit tortor sit amet, luctus ante. Integer dictum augue diam, non pulvinar massa euismod in. Morbi viverra condimentum auctor. Nullam et metus mauris. Cras risus ex, porta sit amet nibh et, dapibus auctor leo.
 
 A list:
```

### Comparing `documenteer-1.2.1/demo/md-technote/technote.toml` & `documenteer-1.2.2/demo/md-technote/technote.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/demo/rst-technote/index.rst` & `documenteer-1.2.2/demo/rst-technote/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Introduction
 ============
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin facilisis pharetra neque, at semper nulla mattis auctor. Proin semper mollis enim eget interdum. Mauris eleifend eget diam vitae bibendum. Praesent ut aliquet odio, sodales imperdiet nisi. Nam interdum imperdiet tortor sed fringilla. Maecenas efficitur mi sodales nulla commodo rutrum. Ut ornare diam quam, sed commodo turpis aliquam et. In nec enim consequat, suscipit tortor sit amet, luctus ante. Integer dictum augue diam, non pulvinar massa euismod in. Morbi viverra condimentum auctor. Nullam et metus mauris. Cras risus ex, porta sit amet nibh et, dapibus auctor leo.
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin facilisis pharetra neque, at semper nulla mattis auctor. Proin semper mollis enim eget interdum. Mauris eleifend eget diam vitae bibendum. Praesent ut aliquet odio, sodales imperdiet nisi. Nam interdum imperdiet tortor sed fringilla. Maecenas efficitur mi sodales nulla commodo rutrum. Ut ornare diam quam, sed commodo turpis aliquam et. In nec enim consequat, suscipit tortor sit amet, luctus ante. Integer dictum augue diam, non pulvinar massa euismod in. Morbi viverra condimentum auctor. Nullam et metus mauris. Cras risus ex, porta sit amet nibh et, dapibus auctor leo.
 
-A parenthetical citation :cite:p:`2017arXiv170309824V`. And a textual citation :cite:t:`2017arXiv170309824V`.
+A parenthetical citation :cite:p:`SQR-083`. And a textual citation :cite:t:`SQR-083`.
 
 Method
 ======
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin facilisis pharetra neque, at semper nulla mattis auctor. Proin semper mollis enim eget interdum. Mauris eleifend eget diam vitae bibendum. Praesent ut aliquet odio, sodales imperdiet nisi. Nam interdum imperdiet tortor sed fringilla. Maecenas efficitur mi sodales nulla commodo rutrum. Ut ornare diam quam, sed commodo turpis aliquam et. In nec enim consequat, suscipit tortor sit amet, luctus ante. Integer dictum augue diam, non pulvinar massa euismod in. Morbi viverra condimentum auctor. Nullam et metus mauris. Cras risus ex, porta sit amet nibh et, dapibus auctor leo.
 
 A list:
```

### Comparing `documenteer-1.2.1/demo/rst-technote/technote.toml` & `documenteer-1.2.2/demo/rst-technote/technote.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/Makefile` & `documenteer-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/_rst_epilog.rst` & `documenteer-1.2.2/docs/_rst_epilog.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/changelog.md` & `documenteer-1.2.2/docs/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Change Log
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-1.2.2'></a>
+## 1.2.2 (2024-04-11)
+
+### Bug fixes
+
+- Update `jira_uri_template` configuration default to `https://rubinobs.atlassian.net/browse/{issue}`. This will make all :jira:, :jirab:, and :jirap: roles point to the new Jira instance for Rubin Observatory.
+- Drop `jira.lsstcorp.org` from the linkcheck ignore list defaults for `documenteer.config.guide` since that instance is no longer being used.
+- Replace `jira.lsstcorp.org` URLs in documentation to `rubinobs.atlassian.net`.
+
 <a id='changelog-1.2.1'></a>
 ## 1.2.1 (2024-04-02)
 
 ### Bug fixes
 
 - Fix the "Source parser for markdown not registered" error for Markdown-based technotes. With the MyST-NB extension the Markdown parser is automatically registered, so the `documenteer.conf.technote` configuration now resets the `source_suffix` configuration originally created by the Technote package.
 
@@ -336,15 +345,15 @@
 - New Sphinx configuration facilities should prevent recursion issues by more cleanly populating the Python attributes in the configuration module:
 
   - Technote projects now import `documenteer.conf.technote` in their `conf.py` files.
   - Stack projects now import `documenteer.conf.pipelines` in their `conf.py` files.
   - Individual Stack packages now import `documenteer.conf.pipelinespkg` in their `conf.py` files.
 
   The previous configuration sub-package, `documenteer.sphinxconf` is deprecated.
-  [[DM-20866](https://jira.lsstcorp.org/browse/DM-20866)]
+  [[DM-20866](https://rubinobs.atlassian.net/browse/DM-20866)]
 
   Overall, the configurations are compatible with these exceptions:
 
   - ReStructuredText source files are no longer copied into the built site for Pipelines projects (`html_copy_source` is `False`).
     This change reduces the upload site of the pipelines.lsst.io site.
   - Updated the MathJax CDN URL to point to cdnjs.
 
@@ -359,85 +368,85 @@
   It's intended to be used equivalently to the `automodapi` extension.
 
   The built-in Doxygen build considers all Stack packages with a `doc/doxygen.conf.in` file.
   Documenteer creates a Doxygen configuration from the contents of each package's `doxygen.conf.in` file, along with built-in defaults appropriate for pipelines.lsst.io.
   For example, individual packages can add to the `EXCLUDE` tag.
   By default, each package's `include` directory is included in the Doxygen build.
 
-  [[DM-22698](https://jira.lsstcorp.org/browse/DM-22698), [DM-23094](https://jira.lsstcorp.org/browse/DM-23094), [DM-22461](https://jira.lsstcorp.org/browse/DM-22461)]
+  [[DM-22698](https://rubinobs.atlassian.net/browse/DM-22698), [DM-23094](https://rubinobs.atlassian.net/browse/DM-23094), [DM-22461](https://rubinobs.atlassian.net/browse/DM-22461)]
 
 - Improved Sphinx runner (`documenteer.sphinxrunner`).
-  [[DM-26768](https://jira.lsstcorp.org/browse/DM-26768)]
+  [[DM-26768](https://rubinobs.atlassian.net/browse/DM-26768)]
 
 - Added static type checking using [mypy](https://mypy.readthedocs.io/en/stable/).
-  [[DM-22717](https://jira.lsstcorp.org/browse/DM-22717), [DM-26288](https://jira.lsstcorp.org/browse/DM-26288)]
+  [[DM-22717](https://rubinobs.atlassian.net/browse/DM-22717), [DM-26288](https://rubinobs.atlassian.net/browse/DM-26288)]
 
 - Improved packaging, testing, and development environment:
 
   - PEP 518-ify the build process by adding a `pyproject.toml` file.
   - Removed the deprecated pytest-runner plugin.
   - Moved most of the packaging configuration to `setup.cfg`.
   - Adopted black and isort for code formatting.
   - Migrated to `tox` for running tests.
   - Migrated to `pre-commit` for running linters and code formatters.
   - Migrated to GitHub Actions from Travis CI.
 
-  [`DM-22957 <https://jira.lsstcorp.org/browse/DM-22957>`_, `DM-26288 <https://jira.lsstcorp.org/browse/DM-26288>`_]
+  [`DM-22957 <https://rubinobs.atlassian.net/browse/DM-22957>`_, `DM-26288 <https://rubinobs.atlassian.net/browse/DM-26288>`_]
 
 - Documentation improvements:
 
   - Added a new Developer guide and Release procedure guide.
   - Added an installation page.
   - Moved the Python API reference to its own page.
   - Improved the README to list features.
 
 - Added GitHub community health features: contributing, support, and code of conduct files.
 
 ## 0.5.5 (2019-12-09)
 
 - Technote configuration now uses `yaml.safe_load` instead of `yaml.load`.
   See the [pyyaml docs for details](https://github.com/yaml/pyyaml/wiki/PyYAML-yaml.load(input)-Deprecation).
-  [[DM-22537](https://jira.lsstcorp.org/browse/DM-22537)]
+  [[DM-22537](https://rubinobs.atlassian.net/browse/DM-22537)]
 
 ## 0.5.4 (2019-11-03)
 
 - This new version of the technote sphinx theme should fix the edition link in the sidebar for non-main editions.
-  [[DM-20839](https://jira.lsstcorp.org/browse/DM-20839)]
+  [[DM-20839](https://rubinobs.atlassian.net/browse/DM-20839)]
 
 ## 0.5.3 (2019-08-07)
 
 - Enabled the `html_use_index` and `html_domain_indices` configurations for Stack documentation projects to enable automatic index generation.
   The `genindex` contains links to all command-line options and Python objects (Sphinx's domains).
   This also opens us up to a more general content index by way of the [index directive](https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#index-generating-markup).
-  [[DM-20850](https://jira.lsstcorp.org/browse/DM-20850)]
+  [[DM-20850](https://rubinobs.atlassian.net/browse/DM-20850)]
 
 - Fixed compatibility with docutils 0.15.
   Now Sphinx will control which version of docutils is used, which should now be 0.15.
 
 - Also updated the intersphinx URL for Pandas to use https.
 
 ## 0.5.2 (2019-08-01)
 
 - Add [sphinxcontrib.autoprogram](https://sphinxcontrib-autoprogram.readthedocs.io/en/stable/) to enable automated reference documentation of argparse-based command-line scripts.
   This extension is available with the `documenteer[pipelines]` installation extra and enabled by default for LSST Science Pipelines projects.
-  [[DM-20767](https://jira.lsstcorp.org/browse/)]
+  [[DM-20767](https://rubinobs.atlassian.net/browse/)]
 
 - Update the official list of tested and supported Python versions to Python 3.6 and 3.7.
 
 ## 0.5.1 (2019-07-22)
 
 - Pin docutils temporarily to `0.14`.
   The latest release, 0.15, is currently incompatible with the `:jira:` role.
 
 ## 0.5.0 (2019-02-11)
 
 - The stack documentation build now requires that packages be explicitly required by the main documentation project's EUPS table file.
   Before, a package only needed a `doc/manifest.yaml` file and to be currently set up in the EUPS environment to be linked into the documentation build.
   This would lead to packages being included in a documentation build despite not being a part of that stack product.
-  [[DM-17765](https://jira.lsstcorp.org/browse/DM-17765)]
+  [[DM-17765](https://rubinobs.atlassian.net/browse/DM-17765)]
 
 - This release adds the [sphinx-jinja](https://github.com/tardyp/sphinx-jinja) extension for `documenteer[pipelines]` installations.
   This extension makes it possible to dynamically create content with Jinja templating.
 
   The `documenteer.sphinxconfig.stackconf` module sets up a `default` context for the `jinja` directive that includes all module attributes in the Sphinx config module.
 
 - The `documenteer.sphinxconfig.stackconf` module includes several new configuration attributes that are driven by the presence of an `EUPS_TAG` environment variable.
@@ -449,54 +458,54 @@
   - `release`
   - `version`
   - `scipipe_conda_ref`
   - `newinstall_ref`
   - `pipelines_demo_ref`
 
   These variables are accessible from the `jinja` directive's context.
-  [[DM-17065](https://jira.lsstcorp.org/browse/DM-17065)]
+  [[DM-17065](https://rubinobs.atlassian.net/browse/DM-17065)]
 
 - This release also added some new substitutions to the `rst_epilog` of stack-based projects:
 
   - `|eups-tag|` --- the current EUPS tag, based on the `EUPS_TAG` environment variable.
   - `|eups-tag-mono|` --- monospace typeface version of `|eups-tag|`.
   - `|eups-tag-bold|` --- bold typeface version of `|eups-tag|`.
 
   The `|current-release|` substitution is no longer available.
 
 - Fixed some bugs with the display of copyrights in stack-based projects.
 
 - The project's name is also used as the `logotext` at the top of the page for stack-based projects.
   Previously the `logotext` would always be "LSST Science Pipelines."
-  [[DM-17263](https://jira.lsstcorp.org/browse/DM-17263)]
+  [[DM-17263](https://rubinobs.atlassian.net/browse/DM-17263)]
 
 - Added the following projects to the intersphinx inventory of stack-based projects:
 
   - `firefly_client`
   - `astro_metadata_translator`
 
 ## 0.4.5 (2019-02-06)
 
 - Added a new `lso` role for linking to LSST Operations documents in DocuShare.
 
 ## 0.4.4 (2019-02-05)
 
 - Updated scikit-learn's intersphinx inventory URL (now available as HTTPS) in the `documenteer.sphinxconfig.stackconf`.
-- Fixed the `lsst-task-config-subtasks` directive so that it can introspect items in an `lsst.pex.config` `Registry` that are wrapped by a `ConfigurableWrapper`. [(DM-17661)[https://jira.lsstcorp.org/browse/DM-17661]]
+- Fixed the `lsst-task-config-subtasks` directive so that it can introspect items in an `lsst.pex.config` `Registry` that are wrapped by a `ConfigurableWrapper`. [(DM-17661)[https://rubinobs.atlassian.net/browse/DM-17661]]
 
 ## 0.4.3 (2018-11-30)
 
 - Pin [sphinxcontrib-bibtex](https://github.com/mcmtroffaes/sphinxcontrib-bibtex) to version 0.4.0 since later versions are incompatible with Sphinx <1.8.0.
-  [[DM-16651](https://jira.lsstcorp.org/browse/DM-16651)]
+  [[DM-16651](https://rubinobs.atlassian.net/browse/DM-16651)]
 
 ## 0.4.2 (2018-11-01)
 
 - Handle cases where an object does not have a docstring in `documenteer.sphinxext.lssttasks.taskutils.get_docstring`.
   This improves the reliability of the `lsst-task-api-summary` directive.
-  See (DM-16102)(https://jira.lsstcorp.org/browse/DM-16102).
+  See (DM-16102)(https://rubinobs.atlassian.net/browse/DM-16102).
 
 ## 0.4.1 (2018-10-15)
 
 - Add `documenteer.sphinxext.lssttasks` to the Sphinx extensions available for pipelines.lsst.io documentation builds.
 
 - For pipelines.lsst.io builds, Documenteer ignores the `home/` directory that's created at the root of the `pipelines_lsst_io` directory.
   This directory is created as part of the ci.lsst.codes `sqre/infra/documenteer` job and shouldn't be part of the documentation build.
@@ -517,15 +526,15 @@
 
 - Added Astropy to the intersphinx configuration.
 
 - Enabled `automodsumm_inherited_members` in the stackconf for stack documentation.
   This configuration is critical:
 
   1. It is actually responsible for ensuring that inherited members of classes appear in our docs.
-  2. Without this, classes that have a `__slots__` attribute (typically through inheritance of a `collections.abc` class) won't have *any* of their members documented. See (DM-16102)(https://jira.lsstcorp.org/browse/DM-16102) for discussion.
+  2. Without this, classes that have a `__slots__` attribute (typically through inheritance of a `collections.abc` class) won't have *any* of their members documented. See (DM-16102)(https://rubinobs.atlassian.net/browse/DM-16102) for discussion.
 
 - `todo` directives are now hidden when using `build_pipelines_lsst_io_configs`.
   They are still shown, by default, for standalone package documentation builds, which are primarily developer-facing.
 
 ## 0.3.0 (2018-09-19)
 
 - New `remote-code-block`, which works like the `literalinclude` directive, but allows you to include content from a URL over the web.
@@ -646,15 +655,15 @@
 ## 0.1.11 (2017-03-01)
 
 - Add `documenteer.sphinxconfig.utils.form_ltd_edition_name` to form LSST the Docs-like edition names for Git refs.
 - Configure automated PyPI deployments with Travis.
 
 ## 0.1.10 (2016-12-14)
 
-Includes prototype support for LSST Science Pipelines documentation, as part of `DM-6199 <https://jira.lsstcorp.org/browse/DM-6199>`__:
+Includes prototype support for LSST Science Pipelines documentation, as part of `DM-6199 <https://rubinobs.atlassian.net/browse/DM-6199>`__:
 
 - Added dependencies to [breathe](http://breathe.readthedocs.io/en/latest/), [astropy-helpers](https://github.com/astropy/astropy-helpers) and the [lsst-sphinx-bootstrap-theme](https://github.com/lsst-sqre/lsst-sphinx-bootstrap-theme) to generally coordinate LSST Science Pipelines documentation dependencies.
 - Created `documenteer.sphinxconfig.stackconf` module to centrally coordinate Science Pipelines documentation configuration. Much of the configuration is based on [astropy-helper's Sphinx configuration](https://github.com/astropy/astropy-helpers/blob/master/astropy_helpers/sphinx/conf.py) since the LSST Science Pipelines documentation is heavily based upon Astropy's Sphinx theme and API reference generation infrastructure.
   Also includes prototype configuration for breathe (the doxygen XML bridge).
 - Updated test harness (pytest and plugin versions).
 
 ## 0.1.9 (2016-07-08)
@@ -681,15 +690,15 @@
 
 ## 0.1.4 (2016-05-27)
 
 - Add roles for making mock references to code objects that don't have API references yet. E.g. `lclass`, `lfunc`. DM-6326.
 
 ## 0.1.3 (2016-05-24)
 
-- Add roles for linking to ls.st links: `lpm`, `ldm`, and `lse`. DM-6181.
+- Add roles for linking to `ls.st` links: `lpm`, `ldm`, and `lse`. DM-6181.
 - Add roles for linking to JIRA tickets: `jira`, `jirab`, and `jirap`. DM-6181.
 
 ## 0.1.2 (2016-05-14)
 
 - Include [sphinxcontrib-bibtex](https://sphinxcontrib-bibtex.readthedocs.io/) to Sphinx extensions available in technote projects. DM-6033.
 
 ## 0.1.0 (2015-11-23)
```

### Comparing `documenteer-1.2.1/docs/conf.py` & `documenteer-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/dev/api/documenteer.ext.rst` & `documenteer-1.2.2/docs/dev/api/documenteer.ext.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/dev/api/documenteer.stackdocs.rst` & `documenteer-1.2.2/docs/dev/api/documenteer.stackdocs.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/dev/development.rst` & `documenteer-1.2.2/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/dev/html-templates.rst` & `documenteer-1.2.2/docs/dev/html-templates.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/dev/release.rst` & `documenteer-1.2.2/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/dev/theme-assets.rst` & `documenteer-1.2.2/docs/dev/theme-assets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/documenteer.toml` & `documenteer-1.2.2/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/badges.rst` & `documenteer-1.2.2/docs/guides/badges.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/configuration.rst` & `documenteer-1.2.2/docs/guides/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/diagrams.rst` & `documenteer-1.2.2/docs/guides/diagrams.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/extend-conf-py.rst` & `documenteer-1.2.2/docs/guides/extend-conf-py.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/including-notebooks.ipynb` & `documenteer-1.2.2/docs/guides/including-notebooks.ipynb`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/index.rst` & `documenteer-1.2.2/docs/guides/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/markdown-primer.md` & `documenteer-1.2.2/docs/guides/markdown-primer.md`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/openapi.rst` & `documenteer-1.2.2/docs/guides/openapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/organization.rst` & `documenteer-1.2.2/docs/guides/organization.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/overview.rst` & `documenteer-1.2.2/docs/guides/overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/pipelines/build-overview.rst` & `documenteer-1.2.2/docs/guides/pipelines/build-overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/pipelines/configuration.rst` & `documenteer-1.2.2/docs/guides/pipelines/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/pipelines/cpp-api-linking.rst` & `documenteer-1.2.2/docs/guides/pipelines/cpp-api-linking.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/pipelines/index.rst` & `documenteer-1.2.2/docs/guides/pipelines/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/pipelines/install.rst` & `documenteer-1.2.2/docs/guides/pipelines/install.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/pipelines/package-docs-cli.rst` & `documenteer-1.2.2/docs/guides/pipelines/package-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/pipelines/stack-docs-cli.rst` & `documenteer-1.2.2/docs/guides/pipelines/stack-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/pyproject-configuration.rst` & `documenteer-1.2.2/docs/guides/pyproject-configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/rst-epilog.rst` & `documenteer-1.2.2/docs/guides/rst-epilog.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/tabsets.rst` & `documenteer-1.2.2/docs/guides/tabsets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/guides/toml-reference.rst` & `documenteer-1.2.2/docs/guides/toml-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/index.rst` & `documenteer-1.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/sphinx-extensions/autocppapi.rst` & `documenteer-1.2.2/docs/sphinx-extensions/autocppapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/sphinx-extensions/autodocreset.rst` & `documenteer-1.2.2/docs/sphinx-extensions/autodocreset.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/sphinx-extensions/docushare-reference.rst` & `documenteer-1.2.2/docs/sphinx-extensions/docushare-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/sphinx-extensions/githubbibcache.rst` & `documenteer-1.2.2/docs/sphinx-extensions/githubbibcache.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/sphinx-extensions/jira-reference.rst` & `documenteer-1.2.2/docs/sphinx-extensions/jira-reference.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. default-domain:: rst
 
 ####################
 Jira reference roles
 ####################
 
-Documenteer provides reStructuredText roles to simplify linking to issues in LSST's Jira ticketing system at https://jira.lsstcorp.org.
+Documenteer provides reStructuredText roles to simplify linking to issues in LSST's Jira ticketing system at https://rubinobs.atlassian.net.
 
 To use these roles, add the ``documenteer.ext.jira`` extension to your :file:`conf.py` file:
 
 .. code-block:: python
 
    extensions = ["documenteer.ext.jira"]
```

### Comparing `documenteer-1.2.1/docs/sphinx-extensions/lsst-pybtex-style.rst` & `documenteer-1.2.2/docs/sphinx-extensions/lsst-pybtex-style.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/sphinx-extensions/lssttasks.rst` & `documenteer-1.2.2/docs/sphinx-extensions/lssttasks.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/sphinx-extensions/openapi.rst` & `documenteer-1.2.2/docs/sphinx-extensions/openapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/sphinx-extensions/package-toctree.rst` & `documenteer-1.2.2/docs/sphinx-extensions/package-toctree.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/sphinx-extensions/remote-code-block.rst` & `documenteer-1.2.2/docs/sphinx-extensions/remote-code-block.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/technotes/_templates/README.md` & `documenteer-1.2.2/docs/technotes/_templates/README.md`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/technotes/_templates/README.rst` & `documenteer-1.2.2/docs/technotes/_templates/README.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/technotes/author-metadata.rst` & `documenteer-1.2.2/docs/technotes/author-metadata.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/technotes/configuration.rst` & `documenteer-1.2.2/docs/technotes/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/technotes/document-status.rst` & `documenteer-1.2.2/docs/technotes/document-status.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/technotes/edit-locally.rst` & `documenteer-1.2.2/docs/technotes/edit-locally.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/technotes/edit-on-github.rst` & `documenteer-1.2.2/docs/technotes/edit-on-github.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/technotes/extensions.rst` & `documenteer-1.2.2/docs/technotes/extensions.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/technotes/how-your-technote-gets-published.rst` & `documenteer-1.2.2/docs/technotes/how-your-technote-gets-published.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/technotes/index.rst` & `documenteer-1.2.2/docs/technotes/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/technotes/migrate.rst` & `documenteer-1.2.2/docs/technotes/migrate.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/docs/technotes/start-a-technote.rst` & `documenteer-1.2.2/docs/technotes/start-a-technote.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/licenses/astropy-helpers.txt` & `documenteer-1.2.2/licenses/astropy-helpers.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/licenses/sphinx-issue.txt` & `documenteer-1.2.2/licenses/sphinx-issue.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/licenses/sphinx.txt` & `documenteer-1.2.2/licenses/sphinx.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/package-lock.json` & `documenteer-1.2.2/package-lock.json`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/package.json` & `documenteer-1.2.2/package.json`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/pyproject.toml` & `documenteer-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/assets/rubin-technote/styles/SourceSans3VF-Italic.ttf.woff2` & `documenteer-1.2.2/src/assets/rubin-technote/styles/SourceSans3VF-Italic.ttf.woff2`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/assets/rubin-technote/styles/SourceSans3VF-Upright.ttf.woff2` & `documenteer-1.2.2/src/assets/rubin-technote/styles/SourceSans3VF-Upright.ttf.woff2`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/assets/rubin-technote/styles/_hacks.scss` & `documenteer-1.2.2/src/assets/rubin-technote/styles/_hacks.scss`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/assets/rubin-technote/styles/_properties.scss` & `documenteer-1.2.2/src/assets/rubin-technote/styles/_properties.scss`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/731c8feefe13e72a8691.woff2` & `documenteer-1.2.2/src/documenteer/assets/731c8feefe13e72a8691.woff2`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/b8bc3440ba2145e132f5.woff2` & `documenteer-1.2.2/src/documenteer/assets/b8bc3440ba2145e132f5.woff2`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/favicon.ico` & `documenteer-1.2.2/src/documenteer/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg` & `documenteer-1.2.2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg` & `documenteer-1.2.2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/rubin-favicon-transparent-32px.png` & `documenteer-1.2.2/src/documenteer/assets/rubin-favicon-transparent-32px.png`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/rubin-favicon.svg` & `documenteer-1.2.2/src/documenteer/assets/rubin-favicon.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/rubin-pydata-theme.css` & `documenteer-1.2.2/src/documenteer/assets/rubin-pydata-theme.css`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/rubin-technote.css` & `documenteer-1.2.2/src/documenteer/assets/rubin-technote.css`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/rubin-technote.css.map` & `documenteer-1.2.2/src/documenteer/assets/rubin-technote.css.map`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg` & `documenteer-1.2.2/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg` & `documenteer-1.2.2/src/documenteer/assets/rubin-titlebar-imagotype-light.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/scripts/rubin-technote.js` & `documenteer-1.2.2/src/documenteer/assets/scripts/rubin-technote.js`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/assets/scripts/rubin-technote.js.map` & `documenteer-1.2.2/src/documenteer/assets/scripts/rubin-technote.js.map`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/cli.py` & `documenteer-1.2.2/src/documenteer/cli.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/conf/_toml.py` & `documenteer-1.2.2/src/documenteer/conf/_toml.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/conf/_utils.py` & `documenteer-1.2.2/src/documenteer/conf/_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/conf/guide.py` & `documenteer-1.2.2/src/documenteer/conf/guide.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,17 +230,16 @@
 
 # ============================================================================
 # #LINKCHECK Linkcheck builder configuration
 # ============================================================================
 
 linkcheck_retries = 2
 
-# Tucson IT infrastructure sometimes goes down or has TLS issues
 linkcheck_ignore = [
-    r"^https://jira.lsstcorp.org/browse/",
+    # Tucson IT infrastructure sometimes goes down or has TLS issues
     r"^https://ls.st/",
 ]
 _conf.append_linkcheck_ignore(linkcheck_ignore)
 
 linkcheck_timeout = 15
 
 # ============================================================================
```

### Comparing `documenteer-1.2.1/src/documenteer/conf/pipelines.py` & `documenteer-1.2.2/src/documenteer/conf/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 # c['autoclass_content'] = "both"
 autoclass_content = "class"
 
 # Default flags for automodapi directives. Special members are dunder
 # methods.
 # NOTE: We want to used `inherited-members`, but it seems to be causing
 # documentation duplication in the automodapi listings. We're leaving
-# this out for now. See https://jira.lsstcorp.org/browse/DM-14782 for
+# this out for now. See https://rubinobs.atlassian.net/browse/DM-14782 for
 # additional notes.
 # NOTE: Without inherited members set, special-members doesn't need seem
 # to have an effect (even for special members where the docstrings are
 # directly written in the class, not inherited.
 # autodoc_default_flags = ['inherited-members']
 autodoc_default_flags = ["show-inheritance", "special-members"]
```

### Comparing `documenteer-1.2.1/src/documenteer/conf/pipelinespkg.py` & `documenteer-1.2.2/src/documenteer/conf/pipelinespkg.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/conf/technote.py` & `documenteer-1.2.2/src/documenteer/conf/technote.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/_utils.py` & `documenteer-1.2.2/src/documenteer/ext/_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/autocppapi.py` & `documenteer-1.2.2/src/documenteer/ext/autocppapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/autodocreset.py` & `documenteer-1.2.2/src/documenteer/ext/autodocreset.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/bibtex.py` & `documenteer-1.2.2/src/documenteer/ext/bibtex.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/githubbibcache.py` & `documenteer-1.2.2/src/documenteer/ext/githubbibcache.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/jira.py` & `documenteer-1.2.2/src/documenteer/ext/jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,13 +149,13 @@
         close_symbol=")",
     )
 
 
 def setup(app):
     app.add_config_value(
         "jira_uri_template",
-        default="https://jira.lsstcorp.org/browse/{ticket}",
+        default="https://rubinobs.atlassian.net/browse/{ticket}",
         rebuild="html",
     )
     app.add_role("jira", jira_role)
     app.add_role("jirab", jira_bracket_role)
     app.add_role("jirap", jira_parens_role)
```

### Comparing `documenteer-1.2.1/src/documenteer/ext/lsstdocushare.py` & `documenteer-1.2.2/src/documenteer/ext/lsstdocushare.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/lssttasks/__init__.py` & `documenteer-1.2.2/src/documenteer/ext/lssttasks/__init__.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/lssttasks/configfieldlists.py` & `documenteer-1.2.2/src/documenteer/ext/lssttasks/configfieldlists.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/lssttasks/crossrefs.py` & `documenteer-1.2.2/src/documenteer/ext/lssttasks/crossrefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/lssttasks/pyapisummary.py` & `documenteer-1.2.2/src/documenteer/ext/lssttasks/pyapisummary.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/lssttasks/taskutils.py` & `documenteer-1.2.2/src/documenteer/ext/lssttasks/taskutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/lssttasks/topiclists.py` & `documenteer-1.2.2/src/documenteer/ext/lssttasks/topiclists.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/lssttasks/topics.py` & `documenteer-1.2.2/src/documenteer/ext/lssttasks/topics.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/mockcoderefs.py` & `documenteer-1.2.2/src/documenteer/ext/mockcoderefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/openapi.py` & `documenteer-1.2.2/src/documenteer/ext/openapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/packagetoctree.py` & `documenteer-1.2.2/src/documenteer/ext/packagetoctree.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/ext/remotecodeblock.py` & `documenteer-1.2.2/src/documenteer/ext/remotecodeblock.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/packagemetadata.py` & `documenteer-1.2.2/src/documenteer/packagemetadata.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/requestsutils.py` & `documenteer-1.2.2/src/documenteer/requestsutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/services/technoteauthor.py` & `documenteer-1.2.2/src/documenteer/services/technoteauthor.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/services/technotemigration.py` & `documenteer-1.2.2/src/documenteer/services/technotemigration.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/sphinxrunner.py` & `documenteer-1.2.2/src/documenteer/sphinxrunner.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/stackdocs/build.py` & `documenteer-1.2.2/src/documenteer/stackdocs/build.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml` & `documenteer-1.2.2/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/stackdocs/data/doxygen.defaults.conf` & `documenteer-1.2.2/src/documenteer/stackdocs/data/doxygen.defaults.conf`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/stackdocs/doxygen.py` & `documenteer-1.2.2/src/documenteer/stackdocs/doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/stackdocs/doxygentag.py` & `documenteer-1.2.2/src/documenteer/stackdocs/doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/stackdocs/packagecli.py` & `documenteer-1.2.2/src/documenteer/stackdocs/packagecli.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/stackdocs/pkgdiscovery.py` & `documenteer-1.2.2/src/documenteer/stackdocs/pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/stackdocs/rootdiscovery.py` & `documenteer-1.2.2/src/documenteer/stackdocs/rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/stackdocs/stackcli.py` & `documenteer-1.2.2/src/documenteer/stackdocs/stackcli.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/storage/authordb.py` & `documenteer-1.2.2/src/documenteer/storage/authordb.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/storage/latex.py` & `documenteer-1.2.2/src/documenteer/storage/latex.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/README.rst` & `documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/README.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/storage/localtemplates/technote/tox.ini` & `documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/tox.ini`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/storage/localtemplates.py` & `documenteer-1.2.2/src/documenteer/storage/localtemplates.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/storage/technotetoml.py` & `documenteer-1.2.2/src/documenteer/storage/technotetoml.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/templates/technote/components/sidebar-source.html` & `documenteer-1.2.2/src/documenteer/templates/technote/components/sidebar-source.html`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/templates/technote/sections/header-article.html` & `documenteer-1.2.2/src/documenteer/templates/technote/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer/utils.py` & `documenteer-1.2.2/src/documenteer/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer.egg-info/PKG-INFO` & `documenteer-1.2.2/src/documenteer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 1.2.1
+Version: 1.2.2
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `documenteer-1.2.1/src/documenteer.egg-info/SOURCES.txt` & `documenteer-1.2.2/src/documenteer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/src/documenteer.egg-info/requires.txt` & `documenteer-1.2.2/src/documenteer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/conftest.py` & `documenteer-1.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/data/afw.doxygen.conf` & `documenteer-1.2.2/tests/data/afw.doxygen.conf`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/data/authordb.yaml` & `documenteer-1.2.2/tests/data/authordb.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/data/doxygen.tag.zip` & `documenteer-1.2.2/tests/data/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/ext/autocppapi_test.py` & `documenteer-1.2.2/tests/ext/autocppapi_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/ext/jira_test.py` & `documenteer-1.2.2/tests/ext/jira_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 try:
     from unittest.mock import Mock
 except ImportError:
     from mock import Mock
 
 
-URI = "https://jira.lsstcorp.org/browse/{ticket}"
+URI = "https://rubinobs.atlassian.net/browse/{ticket}"
 
 
 @pytest.fixture()
 def app(request):
     src = mkdtemp()
     doctree = mkdtemp()
     confdir = mkdtemp()
```

### Comparing `documenteer-1.2.1/tests/ext/lsstdocushare_test.py` & `documenteer-1.2.2/tests/ext/lsstdocushare_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/ext/lssttasks/taskutils_test.py` & `documenteer-1.2.2/tests/ext/lssttasks/taskutils_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/ext/mockcoderefs_test.py` & `documenteer-1.2.2/tests/ext/mockcoderefs_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/ext/packagetoctree_test.py` & `documenteer-1.2.2/tests/ext/packagetoctree_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/ext/utils_test.py` & `documenteer-1.2.2/tests/ext/utils_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/packagemetadata_test.py` & `documenteer-1.2.2/tests/packagemetadata_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/roots/test-autocppapi/conf.py` & `documenteer-1.2.2/tests/roots/test-autocppapi/conf.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/roots/test-autocppapi/doxygen.tag.zip` & `documenteer-1.2.2/tests/roots/test-autocppapi/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/services/technotemigration_test.py` & `documenteer-1.2.2/tests/services/technotemigration_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/storage/authordb_test.py` & `documenteer-1.2.2/tests/storage/authordb_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/storage/technotetoml_test.py` & `documenteer-1.2.2/tests/storage/technotetoml_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/test_conf_toml.py` & `documenteer-1.2.2/tests/test_conf_toml.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,20 +135,20 @@
     }
 
 
 def test_append_linkcheck_ignore() -> None:
     config = DocumenteerConfig.load(EXAMPLE)
 
     linkcheck_ignore = [
-        r"^https://jira.lsstcorp.org/browse/",
+        r"^https://rubinobs.atlassian.net/browse/",
         r"^https://ls.st/",
     ]
     config.append_linkcheck_ignore(linkcheck_ignore)
     assert linkcheck_ignore == [
-        r"^https://jira.lsstcorp.org/browse/",
+        r"^https://rubinobs.atlassian.net/browse/",
         r"^https://ls.st/",
         r"^https://confluence.lsstcorp.org/",
     ]
 
 
 def test_disable_primary_sidebars_defaults() -> None:
     """Test sphinx.disable_primary_sidebars defaults where it wasn't set."""
```

### Comparing `documenteer-1.2.1/tests/test_conf_utils.py` & `documenteer-1.2.2/tests/test_conf_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/test_stackdocs_build.py` & `documenteer-1.2.2/tests/test_stackdocs_build.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/test_stackdocs_doxygen.py` & `documenteer-1.2.2/tests/test_stackdocs_doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/test_stackdocs_doxygentag.py` & `documenteer-1.2.2/tests/test_stackdocs_doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/test_stackdocs_pkgdiscovery.py` & `documenteer-1.2.2/tests/test_stackdocs_pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tests/test_stackdocs_rootdiscovery.py` & `documenteer-1.2.2/tests/test_stackdocs_rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/tox.ini` & `documenteer-1.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.1/webpack.config.js` & `documenteer-1.2.2/webpack.config.js`

 * *Files identical despite different names*

