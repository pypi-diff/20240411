# Comparing `tmp/openfeature_provider_flagd-0.1.4.tar.gz` & `tmp/openfeature_provider_flagd-0.1.5.tar.gz`

## Comparing `openfeature_provider_flagd-0.1.4.tar` & `openfeature_provider_flagd-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,92 @@
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/CHANGELOG.md
--rwxr-xr-x   0        0        0      362 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/scripts/gen_protos.sh
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/config.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/flag_type.py
--rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/provider.py
--rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/flagd/evaluation/v1/evaluation_pb2.py
--rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/flagd/evaluation/v1/evaluation_pb2_grpc.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/flagd/sync/v1/sync_pb2.py
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/flagd/sync/v1/sync_pb2_grpc.py
--rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/schema/v1/schema_pb2.py
--rw-r--r--   0        0        0    12393 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/schema/v1/schema_pb2_grpc.py
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/sync/v1/sync_service_pb2.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/sync/v1/sync_service_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/tests/test_config.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/tests/test_flagd.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/LICENSE
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/README.md
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    14518 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/CHANGELOG.md
+-rwxr-xr-x   0        0        0      362 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/scripts/gen_protos.sh
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/__init__.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/config.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/flag_type.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/provider.py
+-rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/flagd/evaluation/v1/evaluation_pb2.py
+-rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/flagd/evaluation/v1/evaluation_pb2_grpc.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/flagd/sync/v1/sync_pb2.py
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/flagd/sync/v1/sync_pb2_grpc.py
+-rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/schema/v1/schema_pb2.py
+-rw-r--r--   0        0        0    12393 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/schema/v1/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/sync/v1/sync_service_pb2.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/sync/v1/sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/resolvers/__init__.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/resolvers/grpc.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/resolvers/in_process.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/resolvers/process/custom_ops.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/resolvers/process/file_watcher.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/resolvers/process/flags.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/.gherkin-lintrc
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/.git
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/.release-please-manifest.json
+-rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/CHANGELOG.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/Makefile
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/README.md
+-rw-r--r--   0        0        0    27641 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/package-lock.json
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/package.json
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/release-please-config.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/renovate.json
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/.github/workflows/lint-pr.yml
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/.github/workflows/release-please.yml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/flagd/Dockerfile
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/flagd/Dockerfile.unstable
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/flags/changing-flag-bar.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/flags/changing-flag-foo.json
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/flags/custom-ops.json
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/flags/edge-case-flags.json
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/flags/evaluator-refs.json
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/flags/testing-flags.json
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/flags/zero-flags.json
+-rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/gherkin/flagd-json-evaluator.feature
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/gherkin/flagd-reconnect.feature
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/gherkin/flagd.feature
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/scripts/change-flag-wrapper.sh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/scripts/change-flag.sh
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/scripts/restart-wrapper.sh
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/sync/Dockerfile
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/sync/Dockerfile.unstable
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/sync/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/sync/go.mod
+-rw-r--r--   0        0        0   112423 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/sync/go.sum
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/sync/main.go
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/sync/pkg/config.go
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/sync/pkg/file_watcher.go
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/test-harness/sync/pkg/server.go
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/test_config.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/test_errors.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/test_file_store.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/test_flagd.py
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/e2e/conftest.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/e2e/parsers.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/e2e/test_inprocess_custom_ops.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/e2e/test_inprocess_edge_cases.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/e2e/test_inprocess_evaluator_reuse.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/e2e/test_inprocess_events.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/e2e/test_inprocess_testing_flags.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/e2e/test_inprocess_zero_evals.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/basic-flag-broken-default.json
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/basic-flag-broken-state.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/basic-flag-broken-targeting.json
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/basic-flag-broken-variants.json
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/basic-flag-disabled.json
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/basic-flag-invalid.not-json
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/basic-flag-no-state.json
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/basic-flag-wrong-structure.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/basic-flag-wrong-variant.json
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/basic-flag.json
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/basic-flag.yaml
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/invalid-fractional-args.json
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/invalid-fractional-weights.json
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/invalid-semver-args.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/invalid-semver-op.json
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/tests/flags/invalid-stringcomp-args.json
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/README.md
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    15005 2020-02-02 00:00:00.000000 openfeature_provider_flagd-0.1.5/PKG-INFO
```

### Comparing `openfeature_provider_flagd-0.1.4/CHANGELOG.md` & `openfeature_provider_flagd-0.1.5/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [0.1.5](https://github.com/open-feature/python-sdk-contrib/compare/openfeature-provider-flagd/v0.1.4...openfeature-provider-flagd/v0.1.5) (2024-04-11)
+
+
+### ✨ New Features
+
+* in-process offline flagd resolver ([#74](https://github.com/open-feature/python-sdk-contrib/issues/74)) ([8cea506](https://github.com/open-feature/python-sdk-contrib/commit/8cea5066ee96f637f3108a9dc3a7539c450a14be))
+
 ## [0.1.4](https://github.com/open-feature/python-sdk-contrib/compare/openfeature-provider-flagd/v0.1.3...openfeature-provider-flagd/v0.1.4) (2024-03-26)
 
 
 ### 🐛 Bug Fixes
 
 * include targetingKey in flagd serialized evaluation context ([#58](https://github.com/open-feature/python-sdk-contrib/issues/58)) ([ddd79a4](https://github.com/open-feature/python-sdk-contrib/commit/ddd79a49b765aa0679a2c1938447c61b37b6d0fe))
 * respect timeout setting in grpc method calls ([#60](https://github.com/open-feature/python-sdk-contrib/issues/60)) ([0149cf7](https://github.com/open-feature/python-sdk-contrib/commit/0149cf7ced8116f54a9b220549834a1970460bd9))
```

### Comparing `openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/flagd/evaluation/v1/evaluation_pb2.py` & `openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/flagd/evaluation/v1/evaluation_pb2.py`

 * *Files identical despite different names*

### Comparing `openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/flagd/evaluation/v1/evaluation_pb2_grpc.py` & `openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/flagd/evaluation/v1/evaluation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/flagd/sync/v1/sync_pb2.py` & `openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/flagd/sync/v1/sync_pb2.py`

 * *Files identical despite different names*

### Comparing `openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/flagd/sync/v1/sync_pb2_grpc.py` & `openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/flagd/sync/v1/sync_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/schema/v1/schema_pb2.py` & `openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/schema/v1/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/schema/v1/schema_pb2_grpc.py` & `openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/schema/v1/schema_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/sync/v1/sync_service_pb2.py` & `openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/sync/v1/sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `openfeature_provider_flagd-0.1.4/src/openfeature/contrib/provider/flagd/proto/sync/v1/sync_service_pb2_grpc.py` & `openfeature_provider_flagd-0.1.5/src/openfeature/contrib/provider/flagd/proto/sync/v1/sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openfeature_provider_flagd-0.1.4/tests/test_config.py` & `openfeature_provider_flagd-0.1.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `openfeature_provider_flagd-0.1.4/tests/test_flagd.py` & `openfeature_provider_flagd-0.1.5/tests/test_flagd.py`

 * *Files identical despite different names*

### Comparing `openfeature_provider_flagd-0.1.4/.gitignore` & `openfeature_provider_flagd-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `openfeature_provider_flagd-0.1.4/LICENSE` & `openfeature_provider_flagd-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openfeature_provider_flagd-0.1.4/README.md` & `openfeature_provider_flagd-0.1.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,27 @@
 ```python
 from openfeature import api
 from openfeature.contrib.provider.flagd import FlagdProvider
 
 api.set_provider(FlagdProvider())
 ```
 
+To use in-process evaluation in offline mode with a file as source:
+
+```python
+from openfeature import api
+from openfeature.contrib.provider.flagd import FlagdProvider
+from openfeature.contrib.provider.flagd.config import ResolverType
+
+api.set_provider(FlagdProvider(
+    resolver_type=ResolverType.IN_PROCESS,
+    offline_flag_source_path="my-flag.json",
+))
+```
+
 ### Configuration options
 
 The default options can be defined in the FlagdProvider constructor.
 
 | Option name    | Type & Values | Default   |
 |----------------|---------------|-----------|
 | host           | str           | localhost |
```

### Comparing `openfeature_provider_flagd-0.1.4/pyproject.toml` & `openfeature_provider_flagd-0.1.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 # pyproject.toml
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openfeature-provider-flagd"
-version = "0.1.4"
+version = "0.1.5"
 description = "OpenFeature provider for the flagd flag evaluation engine"
 readme = "README.md"
 authors = [{ name = "OpenFeature", email = "openfeature-core@groups.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = []
 dependencies = [
   "openfeature-sdk>=0.4.0",
   "grpcio>=1.60.0",
   "protobuf>=4.25.2",
+  "mmh3>=4.1.0",
+  "panzi-json-logic>=1.0.1",
+  "semver>=3,<4",
+  "pyyaml>=6.0.1",
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/open-feature/python-sdk-contrib"
 
 [tool.hatch]
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
+  "pytest-bdd",
 ]
 post-install-commands = [
   "./scripts/gen_protos.sh"
 ]
 
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "coverage xml",
+  "coverage html",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [tool.hatch.build.targets.sdist]
@@ -57,8 +63,9 @@
 [tool.hatch.build.targets.wheel]
 packages = ["src/openfeature"]
 
 [tool.coverage.run]
 omit = [
   # exclude generated files
   "src/openfeature/contrib/provider/flagd/proto/*",
+  "tests/**",
 ]
```

### Comparing `openfeature_provider_flagd-0.1.4/PKG-INFO` & `openfeature_provider_flagd-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openfeature-provider-flagd
-Version: 0.1.4
+Version: 0.1.5
 Summary: OpenFeature provider for the flagd flag evaluation engine
 Project-URL: Homepage, https://github.com/open-feature/python-sdk-contrib
 Author-email: OpenFeature <openfeature-core@groups.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -207,16 +207,20 @@
            limitations under the License.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: grpcio>=1.60.0
+Requires-Dist: mmh3>=4.1.0
 Requires-Dist: openfeature-sdk>=0.4.0
+Requires-Dist: panzi-json-logic>=1.0.1
 Requires-Dist: protobuf>=4.25.2
+Requires-Dist: pyyaml>=6.0.1
+Requires-Dist: semver<4,>=3
 Description-Content-Type: text/markdown
 
 # flagd Provider for OpenFeature
 
 This provider is designed to use flagd's [evaluation protocol](https://github.com/open-feature/schemas/blob/main/protobuf/schema/v1/schema.proto).
 
 ## Installation
@@ -232,14 +236,27 @@
 ```python
 from openfeature import api
 from openfeature.contrib.provider.flagd import FlagdProvider
 
 api.set_provider(FlagdProvider())
 ```
 
+To use in-process evaluation in offline mode with a file as source:
+
+```python
+from openfeature import api
+from openfeature.contrib.provider.flagd import FlagdProvider
+from openfeature.contrib.provider.flagd.config import ResolverType
+
+api.set_provider(FlagdProvider(
+    resolver_type=ResolverType.IN_PROCESS,
+    offline_flag_source_path="my-flag.json",
+))
+```
+
 ### Configuration options
 
 The default options can be defined in the FlagdProvider constructor.
 
 | Option name    | Type & Values | Default   |
 |----------------|---------------|-----------|
 | host           | str           | localhost |
```

