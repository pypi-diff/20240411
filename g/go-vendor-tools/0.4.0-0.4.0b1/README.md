# Comparing `tmp/go_vendor_tools-0.4.0.tar.gz` & `tmp/go_vendor_tools-0.4.0b1.tar.gz`

## Comparing `go_vendor_tools-0.4.0.tar` & `go_vendor_tools-0.4.0b1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/.packit.yaml
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/NEWS.md
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/docs-requirements.txt
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/go-vendor-tools.spec
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/noxfile.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/pyrightconfig.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/pyrightconfig.json.license
--rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/rpmeval.sh
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/ruff.toml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/.reuse/dep5
--rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/contrib/integration-archive.sh
--rwxr-xr-x   0        0        0      391 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/contrib/main-archive.sh
--rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/contrib/verify-license.sh
--rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/contrib/wait-for-copr.sh
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/README.md -> ../README.md
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/architecture.md
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/config.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/contributing.md -> ../CONTRIBUTING.md
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/example-specfile.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/news.md -> ../NEWS.md
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/scenarios.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/man/.gitignore
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/man/go_vendor_archive.1.scd
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/man/go_vendor_archive_create.1.scd
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/man/go_vendor_archive_override.1.scd
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/man/mkdocs_mangen.py
--rwxr-xr-x   0        0        0     1241 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/doc/man/mkman.sh
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/rpm/macros.go_vendor_tools
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/__init__.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/archive.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/exceptions.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/gomod.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/hashing.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/licensing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/py.typed
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/specfile_sources.py
--rwxr-xr-x   0        0        0     9832 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/cli/go_vendor_archive.py
--rwxr-xr-x   0        0        0    20400 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/cli/go_vendor_license.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/cli/utils.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/config/archive.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/config/base.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/config/licenses.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/config/utils.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/license_detection/__init__.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/license_detection/askalono.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/license_detection/base.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/license_detection/load.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/src/go_vendor_tools/license_detection/trivy.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/integration/.gitignore
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/integration/autorestic/CHECKSUMS
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/integration/autorestic/autorestic.spec
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/integration/autorestic/expected-licenses.list
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/integration/autorestic/expected-licenses.list.license
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/integration/autorestic/go-vendor-tools.toml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/integration/fzf/CHECKSUMS
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/integration/fzf/CHECKSUMS.license
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/integration/fzf/expected-licenses.list
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/integration/fzf/expected-licenses.list.license
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/integration/fzf/fzf.spec
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/integration/fzf/go-vendor-tools.toml
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/pytests/conftest.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/pytests/test_archive.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/pytests/test_go_vendor_tools.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/pytests/test_licensing.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/pytests/test_data/case1/config-broken.toml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/pytests/test_data/case1/config.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/pytests/test_data/case1/licenses/LICENSE.BSD3
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/pytests/test_data/case1/licenses/LICENSE.MIT
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/tests/pytests/test_data/case2/licenses/LICENSE
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/.gitignore
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/README.md
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/.packit.yaml
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/LICENSE.md
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/NEWS.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/docs-requirements.txt
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/go-vendor-tools.spec
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/mkdocs.yml
+-rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/noxfile.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/pyrightconfig.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/pyrightconfig.json.license
+-rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/rpmeval.sh
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/ruff.toml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/.reuse/dep5
+-rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/contrib/integration-archive.sh
+-rwxr-xr-x   0        0        0      391 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/contrib/main-archive.sh
+-rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/contrib/verify-license.sh
+-rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/contrib/wait-for-copr.sh
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/README.md -> ../README.md
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/architecture.md
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/config.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/contributing.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/example-specfile.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/news.md -> ../NEWS.md
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/scenarios.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/.gitignore
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive.1.scd
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive_create.1.scd
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive_override.1.scd
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/mkdocs_mangen.py
+-rwxr-xr-x   0        0        0     1241 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/mkman.sh
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/rpm/macros.go_vendor_tools
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/__init__.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/archive.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/exceptions.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/gomod.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/hashing.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/licensing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/py.typed
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/specfile_sources.py
+-rwxr-xr-x   0        0        0     9832 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/go_vendor_archive.py
+-rwxr-xr-x   0        0        0    20400 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/go_vendor_license.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/utils.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/archive.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/base.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/licenses.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/utils.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/__init__.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/askalono.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/base.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/load.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/trivy.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/.gitignore
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/CHECKSUMS
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/autorestic.spec
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/expected-licenses.list
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/expected-licenses.list.license
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/go-vendor-tools.toml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/CHECKSUMS
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/CHECKSUMS.license
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/expected-licenses.list
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/expected-licenses.list.license
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/fzf.spec
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/go-vendor-tools.toml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/conftest.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_archive.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_go_vendor_tools.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_licensing.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/config-broken.toml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/config.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/licenses/LICENSE.BSD3
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/licenses/LICENSE.MIT
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case2/licenses/LICENSE
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/.gitignore
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/README.md
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/PKG-INFO
```

### Comparing `go_vendor_tools-0.4.0/.gitlab-ci.yml` & `go_vendor_tools-0.4.0b1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/.packit.yaml` & `go_vendor_tools-0.4.0b1/.packit.yaml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/CONTRIBUTING.md` & `go_vendor_tools-0.4.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/NEWS.md` & `go_vendor_tools-0.4.0b1/NEWS.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 <!--
 Copyright (C) 2024 Maxwell G <maxwell@gtmx.me>
 SPDX-License-Identifier: MIT
 -->
 
 # NEWS
 
-## 0.4.0 - 2024-04-10 <a id='0.4.0'></a>
-
-See the notes for 0.4.0b1.
-
 ## 0.4.0b1 - 2024-04-10 <a id='0.4.0b1'></a>
 
 ### Added
 
 - `cli`: support compression algorithms other than `xz` (#7, #45)
 - `doc`: add manpages for go_vendor_archive commands (#40)
 - `go_vendor_archive create`: add `--idempotent` flag
```

### Comparing `go_vendor_tools-0.4.0/go-vendor-tools.spec` & `go_vendor_tools-0.4.0b1/go-vendor-tools.spec`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # License text: https://spdx.org/licenses/MIT
 
 %bcond manpages 1
 %global forgeurl https://gitlab.com/fedora/sigs/go/go-vendor-tools
 %define tag v%{version_no_tilde %{quote:%nil}}
 
 Name:           go-vendor-tools
-Version:        0.4.0
+Version:        0.4.0b1
 %forgemeta
 Release:        1%{?dist}
 Summary:        Tools for handling Go library vendoring in Fedora
 
 # BSD-3-Clause: src/go_vendor_tools/archive.py
 License:        MIT AND BSD-3-Clause
 URL:            %{forgeurl}
@@ -91,18 +91,15 @@
 
 %files doc
 %doc %{_docdir}/go-vendor-tools-doc/
 
 %pyproject_extras_subpkg -n go-vendor-tools all
 
 %changelog
-* Wed Apr 10 2024 Maxwell G <maxwell@gtmx.me> - 0.4.0-1
-- Release 0.4.0.
-
-* Wed Apr 10 2024 Maxwell G <maxwell@gtmx.me> - 0.4.0~b1-1
+* Wed Apr 10 2024 Maxwell G <maxwell@gtmx.me> - 0.4.0b1-1
 - Release 0.4.0b1.
 
 * Thu Mar 28 2024 Maxwell G <maxwell@gtmx.me> - 0.3.0-1
 - Release 0.3.0.
 
 * Sat Mar 16 2024 Maxwell G <maxwell@gtmx.me> - 0.2.0-1
 - Release 0.2.0.
```

### Comparing `go_vendor_tools-0.4.0/mkdocs.yml` & `go_vendor_tools-0.4.0b1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/noxfile.py` & `go_vendor_tools-0.4.0b1/noxfile.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/rpmeval.sh` & `go_vendor_tools-0.4.0b1/rpmeval.sh`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/ruff.toml` & `go_vendor_tools-0.4.0b1/ruff.toml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/contrib/integration-archive.sh` & `go_vendor_tools-0.4.0b1/contrib/integration-archive.sh`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/contrib/verify-license.sh` & `go_vendor_tools-0.4.0b1/contrib/verify-license.sh`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/doc/architecture.md` & `go_vendor_tools-0.4.0b1/doc/architecture.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/doc/config.md` & `go_vendor_tools-0.4.0b1/doc/config.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/doc/example-specfile.md` & `go_vendor_tools-0.4.0b1/doc/example-specfile.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/doc/scenarios.md` & `go_vendor_tools-0.4.0b1/doc/scenarios.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/doc/man/go_vendor_archive.1.scd` & `go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive.1.scd`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/doc/man/go_vendor_archive_create.1.scd` & `go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive_create.1.scd`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/doc/man/go_vendor_archive_override.1.scd` & `go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive_override.1.scd`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/doc/man/mkdocs_mangen.py` & `go_vendor_tools-0.4.0b1/doc/man/mkdocs_mangen.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/doc/man/mkman.sh` & `go_vendor_tools-0.4.0b1/doc/man/mkman.sh`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/rpm/macros.go_vendor_tools` & `go_vendor_tools-0.4.0b1/rpm/macros.go_vendor_tools`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/archive.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/archive.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/exceptions.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/gomod.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/gomod.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/hashing.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/hashing.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/licensing.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/licensing.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/specfile_sources.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/specfile_sources.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/cli/go_vendor_archive.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/go_vendor_archive.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/cli/go_vendor_license.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/go_vendor_license.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/config/archive.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/archive.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/config/base.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/base.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/config/licenses.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/licenses.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/license_detection/askalono.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/askalono.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/license_detection/base.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/base.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/license_detection/load.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/load.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/src/go_vendor_tools/license_detection/trivy.py` & `go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/trivy.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/tests/integration/autorestic/autorestic.spec` & `go_vendor_tools-0.4.0b1/tests/integration/autorestic/autorestic.spec`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/tests/integration/autorestic/expected-licenses.list` & `go_vendor_tools-0.4.0b1/tests/integration/autorestic/expected-licenses.list`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/tests/integration/autorestic/go-vendor-tools.toml` & `go_vendor_tools-0.4.0b1/tests/integration/autorestic/go-vendor-tools.toml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/tests/integration/fzf/expected-licenses.list` & `go_vendor_tools-0.4.0b1/tests/integration/fzf/expected-licenses.list`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/tests/integration/fzf/fzf.spec` & `go_vendor_tools-0.4.0b1/tests/integration/fzf/fzf.spec`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/tests/pytests/test_archive.py` & `go_vendor_tools-0.4.0b1/tests/pytests/test_archive.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/tests/pytests/test_go_vendor_tools.py` & `go_vendor_tools-0.4.0b1/tests/pytests/test_go_vendor_tools.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/tests/pytests/test_licensing.py` & `go_vendor_tools-0.4.0b1/tests/pytests/test_licensing.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/tests/pytests/test_data/case1/licenses/LICENSE.BSD3` & `go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/licenses/LICENSE.BSD3`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/tests/pytests/test_data/case1/licenses/LICENSE.MIT` & `go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/licenses/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/tests/pytests/test_data/case2/licenses/LICENSE` & `go_vendor_tools-0.4.0b1/tests/pytests/test_data/case2/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/README.md` & `go_vendor_tools-0.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/pyproject.toml` & `go_vendor_tools-0.4.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/LICENSES/BSD-3-Clause.txt` & `go_vendor_tools-0.4.0b1/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/LICENSES/MIT.txt` & `go_vendor_tools-0.4.0b1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0/PKG-INFO` & `go_vendor_tools-0.4.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: go-vendor-tools
-Version: 0.4.0
+Version: 0.4.0b1
 Summary: Tools for handling Go library vendoring in Fedora
 Project-URL: Homepage, https://fedora.gitlab.io/sigs/go/go-vendor-tools/
 Project-URL: Source, https://gitlab.com/fedora/sigs/go/go-vendor-tools
 Project-URL: Issue Tracker, https://gitlab.com/fedora/sigs/go/go-vendor-tools/-/issues
 Project-URL: Changelog, https://fedora.gitlab.io/sigs/go/go-vendor-tools/news/
 Author-email: Maxwell G <maxwell@gtmx.me>
 Maintainer-email: Maxwell G <maxwell@gtmx.me>, Fedora Go SIG <golang@lists.fedoraproject.org>
```

