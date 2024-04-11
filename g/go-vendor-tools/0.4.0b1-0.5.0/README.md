# Comparing `tmp/go_vendor_tools-0.4.0b1.tar.gz` & `tmp/go_vendor_tools-0.5.0.tar.gz`

## Comparing `go_vendor_tools-0.4.0b1.tar` & `go_vendor_tools-0.5.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/.gitlab-ci.yml
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/.packit.yaml
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/CONTRIBUTING.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/LICENSE.md
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/NEWS.md
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/docs-requirements.txt
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/go-vendor-tools.spec
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/mkdocs.yml
--rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/noxfile.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/pyrightconfig.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/pyrightconfig.json.license
--rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/rpmeval.sh
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/ruff.toml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/.reuse/dep5
--rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/contrib/integration-archive.sh
--rwxr-xr-x   0        0        0      391 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/contrib/main-archive.sh
--rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/contrib/verify-license.sh
--rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/contrib/wait-for-copr.sh
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/README.md -> ../README.md
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/architecture.md
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/config.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/contributing.md -> ../CONTRIBUTING.md
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/example-specfile.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/news.md -> ../NEWS.md
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/scenarios.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/.gitignore
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive.1.scd
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive_create.1.scd
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive_override.1.scd
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/mkdocs_mangen.py
--rwxr-xr-x   0        0        0     1241 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/doc/man/mkman.sh
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/rpm/macros.go_vendor_tools
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/__init__.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/archive.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/exceptions.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/gomod.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/hashing.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/licensing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/py.typed
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/specfile_sources.py
--rwxr-xr-x   0        0        0     9832 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/go_vendor_archive.py
--rwxr-xr-x   0        0        0    20400 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/go_vendor_license.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/utils.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/archive.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/base.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/licenses.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/utils.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/__init__.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/askalono.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/base.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/load.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/trivy.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/.gitignore
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/CHECKSUMS
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/autorestic.spec
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/expected-licenses.list
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/expected-licenses.list.license
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/autorestic/go-vendor-tools.toml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/CHECKSUMS
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/CHECKSUMS.license
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/expected-licenses.list
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/expected-licenses.list.license
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/fzf.spec
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/integration/fzf/go-vendor-tools.toml
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/conftest.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_archive.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_go_vendor_tools.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_licensing.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/config-broken.toml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/config.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/licenses/LICENSE.BSD3
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/licenses/LICENSE.MIT
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/tests/pytests/test_data/case2/licenses/LICENSE
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/.gitignore
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/README.md
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/LICENSES/MIT.txt
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 go_vendor_tools-0.4.0b1/PKG-INFO
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/.packit.yaml
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/NEWS.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/docs-requirements.txt
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/go-vendor-tools.spec
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/mkdocs.yml
+-rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/noxfile.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/pyrightconfig.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/pyrightconfig.json.license
+-rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/rpmeval.sh
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/ruff.toml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/.reuse/dep5
+-rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/contrib/integration-archive.sh
+-rwxr-xr-x   0        0        0      391 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/contrib/main-archive.sh
+-rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/contrib/verify-license.sh
+-rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/contrib/wait-for-copr.sh
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/README.md -> ../README.md
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/architecture.md
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/config.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/contributing.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/example-specfile.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/news.md -> ../NEWS.md
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/scenarios.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/man/.gitignore
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/man/go_vendor_archive.1.scd
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/man/go_vendor_archive_create.1.scd
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/man/go_vendor_archive_override.1.scd
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/man/mkdocs_mangen.py
+-rwxr-xr-x   0        0        0     1241 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/doc/man/mkman.sh
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/rpm/macros.go_vendor_tools
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/__init__.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/archive.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/exceptions.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/gomod.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/hashing.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/licensing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/py.typed
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/specfile_sources.py
+-rwxr-xr-x   0        0        0    10003 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/cli/go_vendor_archive.py
+-rwxr-xr-x   0        0        0    20598 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/cli/go_vendor_license.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/cli/utils.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/config/archive.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/config/base.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/config/licenses.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/config/utils.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/license_detection/__init__.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/license_detection/askalono.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/license_detection/base.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/license_detection/load.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/src/go_vendor_tools/license_detection/trivy.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/integration/.gitignore
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/integration/autorestic/CHECKSUMS
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/integration/autorestic/autorestic.spec
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/integration/autorestic/expected-licenses.list
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/integration/autorestic/expected-licenses.list.license
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/integration/autorestic/go-vendor-tools.toml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/integration/fzf/CHECKSUMS
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/integration/fzf/CHECKSUMS.license
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/integration/fzf/expected-licenses.list
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/integration/fzf/expected-licenses.list.license
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/integration/fzf/fzf.spec
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/integration/fzf/go-vendor-tools.toml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/pytests/conftest.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/pytests/test_archive.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/pytests/test_go_vendor_tools.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/pytests/test_licensing.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/pytests/test_data/case1/config-broken.toml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/pytests/test_data/case1/config.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/pytests/test_data/case1/licenses/LICENSE.BSD3
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/pytests/test_data/case1/licenses/LICENSE.MIT
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/tests/pytests/test_data/case2/licenses/LICENSE
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/.gitignore
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/README.md
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 go_vendor_tools-0.5.0/PKG-INFO
```

### Comparing `go_vendor_tools-0.4.0b1/.gitlab-ci.yml` & `go_vendor_tools-0.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/.packit.yaml` & `go_vendor_tools-0.5.0/.packit.yaml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/CONTRIBUTING.md` & `go_vendor_tools-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/NEWS.md` & `go_vendor_tools-0.5.0/NEWS.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 <!--
 Copyright (C) 2024 Maxwell G <maxwell@gtmx.me>
 SPDX-License-Identifier: MIT
 -->
 
 # NEWS
 
+## 0.5.0 - 2024-04-11 <a id='0.5.0'></a>
+
+### Added
+
+- `cli`: add argcomplete-generated shell completions
+
+### Fixed
+
+- `doc scenarios`: fix outdated info about go2rpm profile
+- `go_vendor_archive`: fix broken `--help` message
+
+## 0.4.0 - 2024-04-10 <a id='0.4.0'></a>
+
+See the notes for 0.4.0b1.
+
 ## 0.4.0b1 - 2024-04-10 <a id='0.4.0b1'></a>
 
 ### Added
 
 - `cli`: support compression algorithms other than `xz` (#7, #45)
 - `doc`: add manpages for go_vendor_archive commands (#40)
 - `go_vendor_archive create`: add `--idempotent` flag
```

### Comparing `go_vendor_tools-0.4.0b1/mkdocs.yml` & `go_vendor_tools-0.5.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/noxfile.py` & `go_vendor_tools-0.5.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/rpmeval.sh` & `go_vendor_tools-0.5.0/rpmeval.sh`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/ruff.toml` & `go_vendor_tools-0.5.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/contrib/integration-archive.sh` & `go_vendor_tools-0.5.0/contrib/integration-archive.sh`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/contrib/verify-license.sh` & `go_vendor_tools-0.5.0/contrib/verify-license.sh`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/doc/architecture.md` & `go_vendor_tools-0.5.0/doc/architecture.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/doc/config.md` & `go_vendor_tools-0.5.0/doc/config.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/doc/example-specfile.md` & `go_vendor_tools-0.5.0/doc/example-specfile.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/doc/scenarios.md` & `go_vendor_tools-0.5.0/doc/scenarios.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # Scenarios
 
 ## Generate specfile with go2rpm
 
 Example case: You wish to package `github.com/opencontainers/runc` using
 vendored dependencies.
 
-Once support for go-vendor-tools is merged into go2rpm, you will be able to
-generate a specfile with the vendor profile with the following command
+go2rpm versions 1.12.0 and later ship with a `vendor` profile that integrates
+with go-vendor-tools.
 
 1. Generate the base specfile
 
     ``` bash
     go2rpm --profile vendor -d --no-clean github.com/opencontainers/runc --name runc
     ```
```

### Comparing `go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive.1.scd` & `go_vendor_tools-0.5.0/doc/man/go_vendor_archive.1.scd`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive_create.1.scd` & `go_vendor_tools-0.5.0/doc/man/go_vendor_archive_create.1.scd`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/doc/man/go_vendor_archive_override.1.scd` & `go_vendor_tools-0.5.0/doc/man/go_vendor_archive_override.1.scd`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/doc/man/mkdocs_mangen.py` & `go_vendor_tools-0.5.0/doc/man/mkdocs_mangen.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/doc/man/mkman.sh` & `go_vendor_tools-0.5.0/doc/man/mkman.sh`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/rpm/macros.go_vendor_tools` & `go_vendor_tools-0.5.0/rpm/macros.go_vendor_tools`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/archive.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/archive.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/exceptions.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/gomod.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/gomod.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/hashing.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/hashing.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/licensing.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/licensing.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/specfile_sources.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/specfile_sources.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/go_vendor_archive.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/cli/go_vendor_archive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+# PYTHON_ARGCOMPLETE_OK
 # Copyright (C) 2024 Maxwell G <maxwell@gtmx.me>
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import argparse
 import dataclasses
@@ -33,14 +34,21 @@
     import tomlkit
 except ImportError:
     HAS_TOMLKIT = False
 else:
     HAS_TOMLKIT = True
     from go_vendor_tools.cli.utils import load_tomlkit_if_exists
 
+try:
+    import argcomplete
+except ImportError:
+    HAS_ARGCOMPLETE = False
+else:
+    HAS_ARGCOMPLETE = True
+
 if TYPE_CHECKING:
     from _typeshed import StrPath
 
 DEFAULT_OUTPUT = "vendor.tar.bz2"
 ARCHIVE_FILES = (Path("go.mod"), Path("go.sum"), Path("vendor"))
 OPTIONAL_FILES = frozenset({Path("go.sum")})
 GO_PROXY_ENV = {
@@ -151,15 +159,14 @@
     )
     create_subparser.add_argument(
         "-p", action="store_true", dest="use_module_proxy", default=argparse.SUPPRESS
     )
     create_subparser.add_argument("-c", "--config", type=Path, dest="config_path")
     create_subparser.add_argument(
         "--tidy",
-        help="%(default)s",
         action=argparse.BooleanOptionalAction,
         default=argparse.SUPPRESS,
     )
     create_subparser.add_argument(
         "-I",
         "--idempotent",
         action="store_true",
@@ -180,14 +187,16 @@
     override_subparser = subparsers.add_parser("override")
     override_subparser.add_argument(
         "--config", type=Path, dest="config_path", required=True
     )
     override_subparser.add_argument("import_path")
     override_subparser.add_argument("version")
 
+    if HAS_ARGCOMPLETE:
+        argcomplete.autocomplete(parser)
     args = parser.parse_args(argv)
     if args.subcommand == "create":
         return CreateArchiveArgs.construct(**vars(args))
     elif args.subcommand == "override":
         return OverrideArgs.construct(**vars(args))
     else:
         raise RuntimeError("unreachable")
```

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/cli/go_vendor_license.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/cli/go_vendor_license.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+# PYTHON_ARGCOMPLETE_OK
 # Copyright (C) 2024 Maxwell G <maxwell@gtmx.me>
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import argparse
 import json
@@ -38,14 +39,20 @@
 try:
     import tomlkit
 except ImportError:
     HAS_TOMLKIT = False
 else:
     HAS_TOMLKIT = True
     from go_vendor_tools.cli.utils import load_tomlkit_if_exists
+try:
+    import argcomplete
+except ImportError:
+    HAS_ARGCOMPLETE = False
+else:
+    HAS_ARGCOMPLETE = True
 
 COLOR: bool | None = None
 RED = "\033[31m"  # ]
 CLEAR = "\033[0m"  # ]
 
 
 def red(__msg: str, /, *, file: IO[str] = sys.stdout) -> None:
@@ -203,14 +210,16 @@
     )
     # TODO(gotmax23): Should we support writing JSON from the install command
     # or just reading it? _add_json_argument(install_parser)
     generate_buildrequires_parser = subparsers.add_parser(  # noqa F841
         "generate_buildrequires"
     )
 
+    if HAS_ARGCOMPLETE:
+        argcomplete.autocomplete(parser)
     args = parser.parse_args(argv)
     args.directory = list(map(Path, args.directory or (".")))
     if args.subcommand not in ("explicit",):
         loaded = load_config(
             args.config_path, allow_missing=getattr(args, "write_config", False)
         )
         args.config = loaded["licensing"]
```

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/archive.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/config/archive.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/base.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/config/base.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/config/licenses.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/config/licenses.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/askalono.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/license_detection/askalono.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/base.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/license_detection/base.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/load.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/license_detection/load.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/src/go_vendor_tools/license_detection/trivy.py` & `go_vendor_tools-0.5.0/src/go_vendor_tools/license_detection/trivy.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/tests/integration/autorestic/autorestic.spec` & `go_vendor_tools-0.5.0/tests/integration/autorestic/autorestic.spec`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/tests/integration/autorestic/expected-licenses.list` & `go_vendor_tools-0.5.0/tests/integration/autorestic/expected-licenses.list`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/tests/integration/autorestic/go-vendor-tools.toml` & `go_vendor_tools-0.5.0/tests/integration/autorestic/go-vendor-tools.toml`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/tests/integration/fzf/expected-licenses.list` & `go_vendor_tools-0.5.0/tests/integration/fzf/expected-licenses.list`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/tests/integration/fzf/fzf.spec` & `go_vendor_tools-0.5.0/tests/integration/fzf/fzf.spec`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/tests/pytests/test_archive.py` & `go_vendor_tools-0.5.0/tests/pytests/test_archive.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/tests/pytests/test_go_vendor_tools.py` & `go_vendor_tools-0.5.0/tests/pytests/test_go_vendor_tools.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/tests/pytests/test_licensing.py` & `go_vendor_tools-0.5.0/tests/pytests/test_licensing.py`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/licenses/LICENSE.BSD3` & `go_vendor_tools-0.5.0/tests/pytests/test_data/case1/licenses/LICENSE.BSD3`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/tests/pytests/test_data/case1/licenses/LICENSE.MIT` & `go_vendor_tools-0.5.0/tests/pytests/test_data/case1/licenses/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/tests/pytests/test_data/case2/licenses/LICENSE` & `go_vendor_tools-0.5.0/tests/pytests/test_data/case2/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/README.md` & `go_vendor_tools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/pyproject.toml` & `go_vendor_tools-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 [project.scripts]
 go_vendor_archive = "go_vendor_tools.cli.go_vendor_archive:main"
 go_vendor_license = "go_vendor_tools.cli.go_vendor_license:main"
 
 [project.optional-dependencies]
 # User-facing
 all = [
+    "argcomplete",
     "tomlkit",
 ]
 # Dev
 codeqa = [
     "pymarkdownlnt",
     "reuse",
     "ruff>=0.3.0",
```

### Comparing `go_vendor_tools-0.4.0b1/LICENSES/BSD-3-Clause.txt` & `go_vendor_tools-0.5.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/LICENSES/MIT.txt` & `go_vendor_tools-0.5.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `go_vendor_tools-0.4.0b1/PKG-INFO` & `go_vendor_tools-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: go-vendor-tools
-Version: 0.4.0b1
+Version: 0.5.0
 Summary: Tools for handling Go library vendoring in Fedora
 Project-URL: Homepage, https://fedora.gitlab.io/sigs/go/go-vendor-tools/
 Project-URL: Source, https://gitlab.com/fedora/sigs/go/go-vendor-tools
 Project-URL: Issue Tracker, https://gitlab.com/fedora/sigs/go/go-vendor-tools/-/issues
 Project-URL: Changelog, https://fedora.gitlab.io/sigs/go/go-vendor-tools/news/
 Author-email: Maxwell G <maxwell@gtmx.me>
 Maintainer-email: Maxwell G <maxwell@gtmx.me>, Fedora Go SIG <golang@lists.fedoraproject.org>
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Requires-Dist: license-expression
 Requires-Dist: tomli; python_version < '3.11'
 Requires-Dist: zstarfile
 Provides-Extra: all
+Requires-Dist: argcomplete; extra == 'all'
 Requires-Dist: tomlkit; extra == 'all'
 Provides-Extra: codeqa
 Requires-Dist: pymarkdownlnt; extra == 'codeqa'
 Requires-Dist: reuse; extra == 'codeqa'
 Requires-Dist: ruff>=0.3.0; extra == 'codeqa'
 Requires-Dist: shellcheck-py; extra == 'codeqa'
 Provides-Extra: dev
```

