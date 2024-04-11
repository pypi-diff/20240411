# Comparing `tmp/kraken_build-0.36.4.tar.gz` & `tmp/kraken_build-0.36.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_build-0.36.4.tar", max compression
+gzip compressed data, was "kraken_build-0.36.5.tar", max compression
```

## Comparing `kraken_build-0.36.4.tar` & `kraken_build-0.36.5.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0        0        0      998 2023-11-08 11:28:21.661737 kraken_build-0.36.4/LICENSE
--rw-r--r--   0        0        0     2943 2024-03-21 08:57:52.723092 kraken_build-0.36.4/README.md
--rw-r--r--   0        0        0     2541 2024-03-26 12:46:20.041098 kraken_build-0.36.4/pyproject.toml
--rw-r--r--   0        0        0      918 2024-01-31 22:13:36.668069 kraken_build-0.36.4/src/kraken/build/__init__.py
--rw-r--r--   0        0        0     1162 2024-01-10 15:13:19.378902 kraken_build-0.36.4/src/kraken/build/tests/test_import.py
--rw-r--r--   0        0        0      858 2024-01-10 15:13:19.379377 kraken_build-0.36.4/src/kraken/build/utils/import_helper.py
--rw-r--r--   0        0        0     2120 2024-03-26 12:46:20.041865 kraken_build-0.36.4/src/kraken/common/__init__.py
--rw-r--r--   0        0        0      471 2023-11-08 11:28:21.664810 kraken_build-0.36.4/src/kraken/common/_argparse.py
--rw-r--r--   0        0        0     1944 2024-03-21 13:10:37.491682 kraken_build-0.36.4/src/kraken/common/_asciitable.py
--rw-r--r--   0        0        0      121 2023-11-08 11:28:21.665670 kraken_build-0.36.4/src/kraken/common/_auth.py
--rw-r--r--   0        0        0     5226 2024-03-21 08:57:52.724936 kraken_build-0.36.4/src/kraken/common/_buildscript.py
--rw-r--r--   0        0        0      666 2024-02-02 12:30:53.402992 kraken_build-0.36.4/src/kraken/common/_buildscript_test.py
--rw-r--r--   0        0        0      609 2023-11-08 11:28:21.667159 kraken_build-0.36.4/src/kraken/common/_date.py
--rw-r--r--   0        0        0      690 2024-02-02 12:30:54.702453 kraken_build-0.36.4/src/kraken/common/_date_test.py
--rw-r--r--   0        0        0     1410 2024-02-16 10:07:48.792940 kraken_build-0.36.4/src/kraken/common/_environment.py
--rw-r--r--   0        0        0     3088 2024-03-21 13:10:37.492849 kraken_build-0.36.4/src/kraken/common/_fs.py
--rw-r--r--   0        0        0      709 2023-11-08 11:28:21.669121 kraken_build-0.36.4/src/kraken/common/_generic.py
--rw-r--r--   0        0        0     1083 2024-03-17 14:51:02.594070 kraken_build-0.36.4/src/kraken/common/_importlib.py
--rw-r--r--   0        0        0     1605 2024-03-15 11:32:59.216933 kraken_build-0.36.4/src/kraken/common/_option_sets.py
--rw-r--r--   0        0        0     9392 2024-03-21 08:57:52.725278 kraken_build-0.36.4/src/kraken/common/_requirements.py
--rw-r--r--   0        0        0     1037 2024-02-02 12:30:59.846814 kraken_build-0.36.4/src/kraken/common/_requirements_test.py
--rw-r--r--   0        0        0     8177 2024-03-21 08:57:52.726092 kraken_build-0.36.4/src/kraken/common/_runner.py
--rw-r--r--   0        0        0     2920 2024-03-21 08:57:52.726619 kraken_build-0.36.4/src/kraken/common/_runner_test.py
--rw-r--r--   0        0        0      494 2023-11-08 11:28:21.681038 kraken_build-0.36.4/src/kraken/common/_terminal.py
--rw-r--r--   0        0        0     1267 2024-03-17 14:51:02.597745 kraken_build-0.36.4/src/kraken/common/_text.py
--rw-r--r--   0        0        0      197 2023-11-08 11:28:21.681910 kraken_build-0.36.4/src/kraken/common/_text_test.py
--rw-r--r--   0        0        0     1201 2023-11-08 11:28:21.682239 kraken_build-0.36.4/src/kraken/common/_tomlconfig.py
--rw-r--r--   0        0        0      811 2024-02-02 12:31:05.021605 kraken_build-0.36.4/src/kraken/common/_tomlconfig_test.py
--rw-r--r--   0        0        0      898 2023-11-08 11:28:21.682920 kraken_build-0.36.4/src/kraken/common/exceptions.py
--rw-r--r--   0        0        0     8963 2024-03-05 10:45:26.064616 kraken_build-0.36.4/src/kraken/common/findpython.py
--rw-r--r--   0        0        0     2218 2024-02-02 12:31:08.598281 kraken_build-0.36.4/src/kraken/common/http/__init__.py
--rw-r--r--   0        0        0     3449 2024-02-02 12:31:09.378251 kraken_build-0.36.4/src/kraken/common/http/lint_ban_bare_requests.py
--rw-r--r--   0        0        0      824 2023-11-08 11:28:21.684895 kraken_build-0.36.4/src/kraken/common/path.py
--rw-r--r--   0        0        0        0 2023-11-08 11:28:21.685098 kraken_build-0.36.4/src/kraken/common/py.typed
--rw-r--r--   0        0        0      326 2024-02-02 12:31:09.703397 kraken_build-0.36.4/src/kraken/common/pyenv/__init__.py
--rw-r--r--   0        0        0     4960 2024-02-02 12:31:11.217565 kraken_build-0.36.4/src/kraken/common/pyenv/_distributions.py
--rw-r--r--   0        0        0     1996 2024-02-02 12:31:11.604303 kraken_build-0.36.4/src/kraken/common/pyenv/_virtualenv.py
--rw-r--r--   0        0        0      266 2023-11-08 11:28:21.686711 kraken_build-0.36.4/src/kraken/common/strings.py
--rw-r--r--   0        0        0     8695 2024-03-17 14:51:02.599384 kraken_build-0.36.4/src/kraken/common/supplier.py
--rw-r--r--   0        0        0      869 2024-03-26 12:46:20.042001 kraken_build-0.36.4/src/kraken/core/__init__.py
--rw-r--r--   0        0        0      468 2024-02-02 12:31:14.013772 kraken_build-0.36.4/src/kraken/core/address/__init__.py
--rw-r--r--   0        0        0    21824 2024-02-02 12:31:16.781600 kraken_build-0.36.4/src/kraken/core/address/_address.py
--rw-r--r--   0        0        0    14459 2024-02-02 12:31:19.347678 kraken_build-0.36.4/src/kraken/core/address/_address_resolver.py
--rw-r--r--   0        0        0     6070 2024-02-02 12:31:24.045766 kraken_build-0.36.4/src/kraken/core/address/_address_resolver_test.py
--rw-r--r--   0        0        0     6658 2024-03-17 14:51:02.600547 kraken_build-0.36.4/src/kraken/core/address/_address_test.py
--rw-r--r--   0        0        0      525 2023-11-08 11:28:21.700868 kraken_build-0.36.4/src/kraken/core/address/_addressable.py
--rw-r--r--   0        0        0      263 2023-11-08 11:28:21.705031 kraken_build-0.36.4/src/kraken/core/base/__init__.py
--rw-r--r--   0        0        0     2201 2024-02-02 12:31:25.227810 kraken_build-0.36.4/src/kraken/core/base/currentable.py
--rw-r--r--   0        0        0     1141 2024-02-02 12:31:25.719094 kraken_build-0.36.4/src/kraken/core/base/metadata.py
--rw-r--r--   0        0        0     2396 2024-02-02 12:31:26.189806 kraken_build-0.36.4/src/kraken/core/cli/executor.py
--rw-r--r--   0        0        0      325 2023-11-08 11:28:21.713170 kraken_build-0.36.4/src/kraken/core/cli/executor_test.py
--rw-r--r--   0        0        0    27380 2024-03-14 10:28:12.317469 kraken_build-0.36.4/src/kraken/core/cli/main.py
--rw-r--r--   0        0        0     7401 2024-02-02 12:33:17.967295 kraken_build-0.36.4/src/kraken/core/cli/option_sets.py
--rw-r--r--   0        0        0     2000 2024-03-17 14:51:02.600851 kraken_build-0.36.4/src/kraken/core/cli/serialize.py
--rw-r--r--   0        0        0        0 2023-11-08 11:28:21.714848 kraken_build-0.36.4/src/kraken/core/py.typed
--rw-r--r--   0        0        0      132 2023-11-08 11:28:21.715479 kraken_build-0.36.4/src/kraken/core/system/__init__.py
--rw-r--r--   0        0        0    17516 2024-03-25 14:07:46.558775 kraken_build-0.36.4/src/kraken/core/system/context.py
--rw-r--r--   0        0        0     4367 2024-02-02 12:33:17.971885 kraken_build-0.36.4/src/kraken/core/system/context_test.py
--rw-r--r--   0        0        0     1366 2024-03-05 12:12:48.677983 kraken_build-0.36.4/src/kraken/core/system/errors.py
--rw-r--r--   0        0        0     2759 2024-03-17 14:51:02.603473 kraken_build-0.36.4/src/kraken/core/system/executor/__init__.py
--rw-r--r--   0        0        0     2332 2024-02-02 12:33:17.987518 kraken_build-0.36.4/src/kraken/core/system/executor/colored.py
--rw-r--r--   0        0        0     8511 2024-03-17 14:51:02.603790 kraken_build-0.36.4/src/kraken/core/system/executor/default.py
--rw-r--r--   0        0        0     9377 2024-03-21 13:10:37.494722 kraken_build-0.36.4/src/kraken/core/system/executor/default_test.py
--rw-r--r--   0        0        0     1554 2023-11-08 11:28:21.719202 kraken_build-0.36.4/src/kraken/core/system/executor/utils.py
--rw-r--r--   0        0        0    24343 2024-02-02 12:33:17.994833 kraken_build-0.36.4/src/kraken/core/system/graph.py
--rw-r--r--   0        0        0    15570 2024-02-02 12:33:17.996970 kraken_build-0.36.4/src/kraken/core/system/graph_test.py
--rw-r--r--   0        0        0      947 2023-11-08 11:28:21.720551 kraken_build-0.36.4/src/kraken/core/system/kraken_object.py
--rw-r--r--   0        0        0    16455 2024-03-25 14:08:59.235234 kraken_build-0.36.4/src/kraken/core/system/project.py
--rw-r--r--   0        0        0     2893 2024-03-21 13:10:37.496101 kraken_build-0.36.4/src/kraken/core/system/project_test.py
--rw-r--r--   0        0        0    18566 2024-02-02 12:33:18.050425 kraken_build-0.36.4/src/kraken/core/system/property.py
--rw-r--r--   0        0        0     7588 2024-02-02 12:33:18.171837 kraken_build-0.36.4/src/kraken/core/system/property_test.py
--rw-r--r--   0        0        0    28698 2024-03-21 08:57:52.729892 kraken_build-0.36.4/src/kraken/core/system/task.py
--rw-r--r--   0        0        0      776 2023-11-08 11:28:21.736459 kraken_build-0.36.4/src/kraken/core/system/task_supplier.py
--rw-r--r--   0        0        0     1458 2024-02-02 12:33:18.213991 kraken_build-0.36.4/src/kraken/core/system/task_test.py
--rw-r--r--   0        0        0     1200 2023-11-08 11:28:21.737040 kraken_build-0.36.4/src/kraken/core/testing/__init__.py
--rw-r--r--   0        0        0       23 2024-03-26 12:46:20.042115 kraken_build-0.36.4/src/kraken/std/__init__.py
--rw-r--r--   0        0        0     1950 2024-03-17 14:48:54.130313 kraken_build-0.36.4/src/kraken/std/buffrs/__init__.py
--rw-r--r--   0        0        0     1921 2024-02-16 10:07:48.794197 kraken_build-0.36.4/src/kraken/std/buffrs/manifest.py
--rw-r--r--   0        0        0     2338 2024-03-17 14:48:54.130625 kraken_build-0.36.4/src/kraken/std/buffrs/tasks.py
--rw-r--r--   0        0        0    18767 2024-03-21 13:10:37.497115 kraken_build-0.36.4/src/kraken/std/cargo/__init__.py
--rw-r--r--   0        0        0     2461 2024-02-02 12:33:18.236375 kraken_build-0.36.4/src/kraken/std/cargo/config.py
--rw-r--r--   0        0        0     9302 2024-03-05 10:45:26.071807 kraken_build-0.36.4/src/kraken/std/cargo/manifest.py
--rw-r--r--   0        0        0        0 2023-11-08 11:28:21.740176 kraken_build-0.36.4/src/kraken/std/cargo/tasks/__init__.py
--rw-r--r--   0        0        0      867 2024-02-02 12:33:18.260391 kraken_build-0.36.4/src/kraken/std/cargo/tasks/_cargo_sqlx.py
--rw-r--r--   0        0        0     4931 2024-03-21 13:10:37.497889 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py
--rw-r--r--   0        0        0     7126 2024-03-21 13:10:37.499505 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_build_task.py
--rw-r--r--   0        0        0     2177 2024-02-02 12:33:18.280727 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py
--rw-r--r--   0        0        0     1330 2024-02-08 17:22:55.921309 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_clippy_task.py
--rw-r--r--   0        0        0     1004 2024-03-17 14:51:02.608276 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_deny_task.py
--rw-r--r--   0        0        0     3527 2024-02-02 12:33:18.282085 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_fmt_task.py
--rw-r--r--   0        0        0     1180 2024-02-02 12:33:18.282659 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_generate_deb.py
--rw-r--r--   0        0        0     1503 2024-03-05 10:45:26.072918 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_login.py
--rw-r--r--   0        0        0     4642 2024-03-15 13:22:29.887179 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_publish_task.py
--rw-r--r--   0        0        0      368 2024-01-10 15:13:19.386111 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_sqlx_database_create.py
--rw-r--r--   0        0        0      360 2024-01-10 15:13:19.386628 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_sqlx_database_drop.py
--rw-r--r--   0        0        0      583 2024-01-10 15:13:19.387260 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_sqlx_migrate.py
--rw-r--r--   0        0        0      927 2024-01-10 15:13:19.387768 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_sqlx_prepare.py
--rw-r--r--   0        0        0     3144 2024-03-17 14:48:54.132991 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_sync_config_task.py
--rw-r--r--   0        0        0      462 2024-03-05 10:45:26.074889 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_test_task.py
--rw-r--r--   0        0        0      387 2024-02-02 12:33:18.284771 kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_update_task.py
--rw-r--r--   0        0        0      761 2024-02-02 12:33:18.286141 kraken_build-0.36.4/src/kraken/std/cargo/tasks/rustup_target_add_task.py
--rw-r--r--   0        0        0      720 2023-11-08 11:28:21.744640 kraken_build-0.36.4/src/kraken/std/cargo/version.py
--rw-r--r--   0        0        0        0 2023-11-08 11:28:21.744808 kraken_build-0.36.4/src/kraken/std/descriptors/__init__.py
--rw-r--r--   0        0        0      872 2024-02-02 12:33:18.287524 kraken_build-0.36.4/src/kraken/std/descriptors/resource.py
--rw-r--r--   0        0        0    10250 2024-02-02 12:33:18.289426 kraken_build-0.36.4/src/kraken/std/dist.py
--rw-r--r--   0        0        0     1574 2024-03-17 14:51:02.608626 kraken_build-0.36.4/src/kraken/std/docker/__init__.py
--rw-r--r--   0        0        0      399 2023-11-08 11:28:21.745402 kraken_build-0.36.4/src/kraken/std/docker/_test.py
--rw-r--r--   0        0        0        0 2023-11-08 11:28:21.745464 kraken_build-0.36.4/src/kraken/std/docker/py.typed
--rw-r--r--   0        0        0        0 2023-11-08 11:28:21.745621 kraken_build-0.36.4/src/kraken/std/docker/tasks/__init__.py
--rw-r--r--   0        0        0     2915 2024-02-02 12:33:18.306296 kraken_build-0.36.4/src/kraken/std/docker/tasks/base_build_task.py
--rw-r--r--   0        0        0     4013 2024-03-26 12:45:32.641202 kraken_build-0.36.4/src/kraken/std/docker/tasks/buildx_build_task.py
--rw-r--r--   0        0        0     3685 2024-02-02 12:33:18.317640 kraken_build-0.36.4/src/kraken/std/docker/tasks/docker_build_task.py
--rw-r--r--   0        0        0     8509 2024-03-21 13:10:37.500247 kraken_build-0.36.4/src/kraken/std/docker/tasks/kaniko_build_task.py
--rw-r--r--   0        0        0     1461 2024-02-02 12:33:18.328126 kraken_build-0.36.4/src/kraken/std/docker/tasks/manifest_tool_push_task.py
--rw-r--r--   0        0        0        0 2023-11-08 11:28:21.746701 kraken_build-0.36.4/src/kraken/std/docker/util/__init__.py
--rw-r--r--   0        0        0     1426 2024-02-02 12:33:18.329946 kraken_build-0.36.4/src/kraken/std/docker/util/dockerapi.py
--rw-r--r--   0        0        0     2273 2024-02-02 12:33:18.335087 kraken_build-0.36.4/src/kraken/std/docker/util/dockerfile.py
--rw-r--r--   0        0        0        0 2024-01-31 22:13:36.669105 kraken_build-0.36.4/src/kraken/std/docs/__init__.py
--rw-r--r--   0        0        0        5 2024-01-31 22:13:36.669598 kraken_build-0.36.4/src/kraken/std/docs/tasks/__init__.py
--rw-r--r--   0        0        0     2214 2024-03-21 13:10:37.501408 kraken_build-0.36.4/src/kraken/std/docs/tasks/mkdocs.py
--rw-r--r--   0        0        0     2414 2024-02-02 12:33:18.356252 kraken_build-0.36.4/src/kraken/std/docs/tasks/novella.py
--rw-r--r--   0        0        0     1574 2024-02-02 12:33:18.359025 kraken_build-0.36.4/src/kraken/std/git/__init__.py
--rw-r--r--   0        0        0     1119 2023-12-12 13:34:59.571312 kraken_build-0.36.4/src/kraken/std/git/config.py
--rw-r--r--   0        0        0       61 2023-11-08 11:28:21.747496 kraken_build-0.36.4/src/kraken/std/git/gitignore/__init__.py
--rw-r--r--   0        0        0     6157 2023-11-08 11:28:21.747702 kraken_build-0.36.4/src/kraken/std/git/gitignore/data/gitignore-io-tokens.json.gz
--rw-r--r--   0        0        0     2739 2024-02-02 12:33:18.359488 kraken_build-0.36.4/src/kraken/std/git/gitignore/generated.py
--rw-r--r--   0        0        0     1849 2024-02-02 12:33:18.360902 kraken_build-0.36.4/src/kraken/std/git/gitignore/generated_test.py
--rw-r--r--   0        0        0     3309 2024-02-02 12:33:18.374517 kraken_build-0.36.4/src/kraken/std/git/gitignore/gitignore_io.py
--rw-r--r--   0        0        0      687 2024-02-02 12:33:18.376524 kraken_build-0.36.4/src/kraken/std/git/gitignore/gitignore_io_test.py
--rw-r--r--   0        0        0     4369 2024-02-02 12:33:18.378085 kraken_build-0.36.4/src/kraken/std/git/gitignore/parser.py
--rw-r--r--   0        0        0        0 2023-11-08 11:28:21.748440 kraken_build-0.36.4/src/kraken/std/git/gitignore_test.py
--rw-r--r--   0        0        0      134 2023-11-08 11:28:21.748631 kraken_build-0.36.4/src/kraken/std/git/tasks/__init__.py
--rw-r--r--   0        0        0     3011 2024-03-17 14:51:02.608999 kraken_build-0.36.4/src/kraken/std/git/tasks/check_file_task.py
--rw-r--r--   0        0        0     2690 2024-02-02 12:33:18.380774 kraken_build-0.36.4/src/kraken/std/git/tasks/check_file_task_test.py
--rw-r--r--   0        0        0     3538 2024-02-02 12:33:18.381262 kraken_build-0.36.4/src/kraken/std/git/tasks/sync_task.py
--rw-r--r--   0        0        0     2349 2024-02-02 12:33:18.381776 kraken_build-0.36.4/src/kraken/std/git/tasks/sync_task_test.py
--rw-r--r--   0        0        0     3164 2024-03-17 14:51:02.609368 kraken_build-0.36.4/src/kraken/std/git/version.py
--rw-r--r--   0        0        0     6354 2024-02-02 12:33:18.383354 kraken_build-0.36.4/src/kraken/std/helm/__init__.py
--rw-r--r--   0        0        0     2328 2024-02-02 12:33:18.384124 kraken_build-0.36.4/src/kraken/std/helm/helmapi.py
--rw-r--r--   0        0        0     3292 2024-03-21 13:10:37.502309 kraken_build-0.36.4/src/kraken/std/mitm/__init__.py
--rw-r--r--   0        0        0      861 2023-11-08 11:28:21.751000 kraken_build-0.36.4/src/kraken/std/mitm/mitm_addon.py
--rw-r--r--   0        0        0     1347 2024-02-02 12:33:18.431734 kraken_build-0.36.4/src/kraken/std/protobuf/__init__.py
--rw-r--r--   0        0        0        0 2023-11-08 11:28:21.751583 kraken_build-0.36.4/src/kraken/std/py.typed
--rw-r--r--   0        0        0     1754 2023-11-08 11:28:21.751835 kraken_build-0.36.4/src/kraken/std/python/__init__.py
--rw-r--r--   0        0        0     6778 2024-03-17 14:51:02.609907 kraken_build-0.36.4/src/kraken/std/python/buildsystem/__init__.py
--rw-r--r--   0        0        0     1439 2024-03-17 14:48:54.143331 kraken_build-0.36.4/src/kraken/std/python/buildsystem/helpers.py
--rw-r--r--   0        0        0    10349 2024-03-17 14:48:54.144128 kraken_build-0.36.4/src/kraken/std/python/buildsystem/maturin.py
--rw-r--r--   0        0        0     9785 2024-03-17 14:51:02.611488 kraken_build-0.36.4/src/kraken/std/python/buildsystem/pdm.py
--rw-r--r--   0        0        0     2105 2024-02-02 12:33:18.438267 kraken_build-0.36.4/src/kraken/std/python/buildsystem/pdm_test.py
--rw-r--r--   0        0        0    10853 2024-03-17 14:51:02.614074 kraken_build-0.36.4/src/kraken/std/python/buildsystem/poetry.py
--rw-r--r--   0        0        0     3094 2024-02-02 12:33:18.439054 kraken_build-0.36.4/src/kraken/std/python/buildsystem/poetry_test.py
--rw-r--r--   0        0        0     5177 2024-03-17 14:48:54.147507 kraken_build-0.36.4/src/kraken/std/python/buildsystem/slap.py
--rw-r--r--   0        0        0     6251 2024-03-21 14:23:29.323655 kraken_build-0.36.4/src/kraken/std/python/pyproject.py
--rw-r--r--   0        0        0     8712 2024-03-21 14:25:11.966765 kraken_build-0.36.4/src/kraken/std/python/settings.py
--rw-r--r--   0        0        0        0 2023-11-08 11:28:21.753394 kraken_build-0.36.4/src/kraken/std/python/tasks/__init__.py
--rw-r--r--   0        0        0     3705 2024-03-05 10:45:26.075653 kraken_build-0.36.4/src/kraken/std/python/tasks/base_task.py
--rw-r--r--   0        0        0     3352 2024-03-17 14:51:02.616547 kraken_build-0.36.4/src/kraken/std/python/tasks/black_task.py
--rw-r--r--   0        0        0     2002 2024-03-17 14:51:02.621554 kraken_build-0.36.4/src/kraken/std/python/tasks/build_task.py
--rw-r--r--   0        0        0     2207 2024-03-17 14:51:02.623986 kraken_build-0.36.4/src/kraken/std/python/tasks/flake8_task.py
--rw-r--r--   0        0        0     2580 2024-03-17 14:51:02.624305 kraken_build-0.36.4/src/kraken/std/python/tasks/info_task.py
--rw-r--r--   0        0        0     3298 2024-03-17 14:51:02.624684 kraken_build-0.36.4/src/kraken/std/python/tasks/install_task.py
--rw-r--r--   0        0        0     3003 2024-03-17 14:51:02.632920 kraken_build-0.36.4/src/kraken/std/python/tasks/isort_task.py
--rw-r--r--   0        0        0      970 2023-11-08 11:28:21.754346 kraken_build-0.36.4/src/kraken/std/python/tasks/login_task.py
--rw-r--r--   0        0        0     2491 2024-02-02 11:58:57.807899 kraken_build-0.36.4/src/kraken/std/python/tasks/mypy_stubtest_task.py
--rw-r--r--   0        0        0     4522 2024-03-17 14:51:02.633944 kraken_build-0.36.4/src/kraken/std/python/tasks/mypy_task.py
--rw-r--r--   0        0        0     8000 2024-03-21 14:30:42.996863 kraken_build-0.36.4/src/kraken/std/python/tasks/pex_build_task.py
--rw-r--r--   0        0        0     1682 2024-02-02 11:58:57.809648 kraken_build-0.36.4/src/kraken/std/python/tasks/pex_build_test.py
--rw-r--r--   0        0        0     3447 2024-03-17 14:51:02.636441 kraken_build-0.36.4/src/kraken/std/python/tasks/publish_task.py
--rw-r--r--   0        0        0     2750 2024-03-17 14:51:02.639001 kraken_build-0.36.4/src/kraken/std/python/tasks/pycln_task.py
--rw-r--r--   0        0        0     2041 2024-03-17 14:51:02.639505 kraken_build-0.36.4/src/kraken/std/python/tasks/pylint_task.py
--rw-r--r--   0        0        0     3887 2024-03-17 14:51:02.639999 kraken_build-0.36.4/src/kraken/std/python/tasks/pytest_task.py
--rw-r--r--   0        0        0     5451 2024-03-21 13:10:37.503446 kraken_build-0.36.4/src/kraken/std/python/tasks/pyupgrade_task.py
--rw-r--r--   0        0        0     1689 2024-03-17 14:51:02.640697 kraken_build-0.36.4/src/kraken/std/python/tasks/update_lockfile_task.py
--rw-r--r--   0        0        0     1619 2023-11-08 11:28:21.755671 kraken_build-0.36.4/src/kraken/std/python/tasks/update_pyproject_task.py
--rw-r--r--   0        0        0     1144 2024-03-17 14:51:02.640897 kraken_build-0.36.4/src/kraken/std/python/version.py
--rw-r--r--   0        0        0     4115 2024-03-17 14:51:02.641209 kraken_build-0.36.4/src/kraken/std/sccache.py
--rw-r--r--   0        0        0     3841 2024-03-05 12:12:48.680071 kraken_build-0.36.4/src/kraken/std/shellcheck.py
--rw-r--r--   0        0        0      232 2024-02-02 12:33:57.905684 kraken_build-0.36.4/src/kraken/std/util/__init__.py
--rw-r--r--   0        0        0     2198 2024-02-02 12:33:57.906169 kraken_build-0.36.4/src/kraken/std/util/check_file_contents_task.py
--rw-r--r--   0        0        0      910 2024-02-02 11:47:20.603083 kraken_build-0.36.4/src/kraken/std/util/check_file_contents_task_test.py
--rw-r--r--   0        0        0     2838 2024-02-02 11:47:20.604291 kraken_build-0.36.4/src/kraken/std/util/copyright_task.py
--rw-r--r--   0        0        0     9660 2024-03-17 14:48:54.155395 kraken_build-0.36.4/src/kraken/std/util/daemon_controller.py
--rw-r--r--   0        0        0     1167 2024-03-21 13:10:37.504091 kraken_build-0.36.4/src/kraken/std/util/http.py
--rw-r--r--   0        0        0     3417 2024-02-02 11:47:20.606575 kraken_build-0.36.4/src/kraken/std/util/render_file_task.py
--rw-r--r--   0        0        0      625 2024-03-21 13:10:37.505214 kraken_build-0.36.4/src/kraken/std/util/url.py
--rw-r--r--   0        0        0     7175 2024-02-02 11:47:20.607400 kraken_build-0.36.4/src/kraken/std/util/validate_readme.py
--rw-r--r--   0        0        0     3173 2024-02-02 11:47:20.608013 kraken_build-0.36.4/src/kraken/std/util/validate_readme_test.py
--rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 kraken_build-0.36.4/PKG-INFO
+-rw-r--r--   0        0        0      998 2024-04-11 17:13:39.290367 kraken_build-0.36.5/LICENSE
+-rw-r--r--   0        0        0     2943 2024-04-11 18:13:27.437407 kraken_build-0.36.5/README.md
+-rw-r--r--   0        0        0     2422 2024-04-11 19:39:33.065166 kraken_build-0.36.5/pyproject.toml
+-rw-r--r--   0        0        0      918 2024-04-11 17:13:39.290864 kraken_build-0.36.5/src/kraken/build/__init__.py
+-rw-r--r--   0        0        0     1162 2024-04-11 17:13:39.291009 kraken_build-0.36.5/src/kraken/build/tests/test_import.py
+-rw-r--r--   0        0        0      858 2024-04-11 17:13:39.291155 kraken_build-0.36.5/src/kraken/build/utils/import_helper.py
+-rw-r--r--   0        0        0     2120 2024-04-11 19:39:33.065366 kraken_build-0.36.5/src/kraken/common/__init__.py
+-rw-r--r--   0        0        0      471 2024-04-11 17:13:39.291411 kraken_build-0.36.5/src/kraken/common/_argparse.py
+-rw-r--r--   0        0        0     1944 2024-04-11 18:13:27.438198 kraken_build-0.36.5/src/kraken/common/_asciitable.py
+-rw-r--r--   0        0        0      121 2024-04-11 17:13:39.291598 kraken_build-0.36.5/src/kraken/common/_auth.py
+-rw-r--r--   0        0        0     5226 2024-04-11 18:13:27.438496 kraken_build-0.36.5/src/kraken/common/_buildscript.py
+-rw-r--r--   0        0        0      666 2024-04-11 17:13:39.291855 kraken_build-0.36.5/src/kraken/common/_buildscript_test.py
+-rw-r--r--   0        0        0      609 2024-04-11 17:13:39.291954 kraken_build-0.36.5/src/kraken/common/_date.py
+-rw-r--r--   0        0        0      690 2024-04-11 17:13:39.292039 kraken_build-0.36.5/src/kraken/common/_date_test.py
+-rw-r--r--   0        0        0     1410 2024-04-11 17:13:39.292128 kraken_build-0.36.5/src/kraken/common/_environment.py
+-rw-r--r--   0        0        0     3088 2024-04-11 18:13:27.438669 kraken_build-0.36.5/src/kraken/common/_fs.py
+-rw-r--r--   0        0        0      709 2024-04-11 17:13:39.292310 kraken_build-0.36.5/src/kraken/common/_generic.py
+-rw-r--r--   0        0        0     1083 2024-04-11 17:13:39.292406 kraken_build-0.36.5/src/kraken/common/_importlib.py
+-rw-r--r--   0        0        0     1605 2024-04-11 17:13:39.292508 kraken_build-0.36.5/src/kraken/common/_option_sets.py
+-rw-r--r--   0        0        0     9392 2024-04-11 18:13:27.438927 kraken_build-0.36.5/src/kraken/common/_requirements.py
+-rw-r--r--   0        0        0     1037 2024-04-11 17:13:39.292777 kraken_build-0.36.5/src/kraken/common/_requirements_test.py
+-rw-r--r--   0        0        0     8177 2024-04-11 18:13:27.439229 kraken_build-0.36.5/src/kraken/common/_runner.py
+-rw-r--r--   0        0        0     2920 2024-04-11 18:13:27.439395 kraken_build-0.36.5/src/kraken/common/_runner_test.py
+-rw-r--r--   0        0        0      494 2024-04-11 17:13:39.293140 kraken_build-0.36.5/src/kraken/common/_terminal.py
+-rw-r--r--   0        0        0     1267 2024-04-11 17:13:39.293235 kraken_build-0.36.5/src/kraken/common/_text.py
+-rw-r--r--   0        0        0      197 2024-04-11 17:13:39.293316 kraken_build-0.36.5/src/kraken/common/_text_test.py
+-rw-r--r--   0        0        0     1201 2024-04-11 17:13:39.293404 kraken_build-0.36.5/src/kraken/common/_tomlconfig.py
+-rw-r--r--   0        0        0      811 2024-04-11 17:13:39.293492 kraken_build-0.36.5/src/kraken/common/_tomlconfig_test.py
+-rw-r--r--   0        0        0      898 2024-04-11 17:13:39.293575 kraken_build-0.36.5/src/kraken/common/exceptions.py
+-rw-r--r--   0        0        0     8963 2024-04-11 17:13:39.293717 kraken_build-0.36.5/src/kraken/common/findpython.py
+-rw-r--r--   0        0        0     2218 2024-04-11 17:13:39.293859 kraken_build-0.36.5/src/kraken/common/http/__init__.py
+-rw-r--r--   0        0        0     3449 2024-04-11 17:13:39.293954 kraken_build-0.36.5/src/kraken/common/http/lint_ban_bare_requests.py
+-rw-r--r--   0        0        0      824 2024-04-11 17:13:39.294041 kraken_build-0.36.5/src/kraken/common/path.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:13:39.294074 kraken_build-0.36.5/src/kraken/common/py.typed
+-rw-r--r--   0        0        0      326 2024-04-11 17:13:39.294230 kraken_build-0.36.5/src/kraken/common/pyenv/__init__.py
+-rw-r--r--   0        0        0     4960 2024-04-11 17:13:39.294672 kraken_build-0.36.5/src/kraken/common/pyenv/_distributions.py
+-rw-r--r--   0        0        0     1996 2024-04-11 17:13:39.294781 kraken_build-0.36.5/src/kraken/common/pyenv/_virtualenv.py
+-rw-r--r--   0        0        0      266 2024-04-11 17:13:39.294869 kraken_build-0.36.5/src/kraken/common/strings.py
+-rw-r--r--   0        0        0     8695 2024-04-11 17:13:39.295014 kraken_build-0.36.5/src/kraken/common/supplier.py
+-rw-r--r--   0        0        0      869 2024-04-11 19:39:33.065497 kraken_build-0.36.5/src/kraken/core/__init__.py
+-rw-r--r--   0        0        0      468 2024-04-11 17:13:39.295292 kraken_build-0.36.5/src/kraken/core/address/__init__.py
+-rw-r--r--   0        0        0    21824 2024-04-11 17:13:39.295415 kraken_build-0.36.5/src/kraken/core/address/_address.py
+-rw-r--r--   0        0        0    14459 2024-04-11 17:13:39.295627 kraken_build-0.36.5/src/kraken/core/address/_address_resolver.py
+-rw-r--r--   0        0        0     6070 2024-04-11 17:13:39.295923 kraken_build-0.36.5/src/kraken/core/address/_address_resolver_test.py
+-rw-r--r--   0        0        0     6658 2024-04-11 17:13:39.296105 kraken_build-0.36.5/src/kraken/core/address/_address_test.py
+-rw-r--r--   0        0        0      525 2024-04-11 17:13:39.296194 kraken_build-0.36.5/src/kraken/core/address/_addressable.py
+-rw-r--r--   0        0        0      263 2024-04-11 17:13:39.296326 kraken_build-0.36.5/src/kraken/core/base/__init__.py
+-rw-r--r--   0        0        0     2201 2024-04-11 17:13:39.296417 kraken_build-0.36.5/src/kraken/core/base/currentable.py
+-rw-r--r--   0        0        0     1141 2024-04-11 17:13:39.296508 kraken_build-0.36.5/src/kraken/core/base/metadata.py
+-rw-r--r--   0        0        0     2396 2024-04-11 17:13:39.296645 kraken_build-0.36.5/src/kraken/core/cli/executor.py
+-rw-r--r--   0        0        0      325 2024-04-11 17:13:39.296732 kraken_build-0.36.5/src/kraken/core/cli/executor_test.py
+-rw-r--r--   0        0        0    27380 2024-04-11 17:13:39.296887 kraken_build-0.36.5/src/kraken/core/cli/main.py
+-rw-r--r--   0        0        0     7401 2024-04-11 17:13:39.297101 kraken_build-0.36.5/src/kraken/core/cli/option_sets.py
+-rw-r--r--   0        0        0     2000 2024-04-11 17:13:39.297200 kraken_build-0.36.5/src/kraken/core/cli/serialize.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:13:39.297236 kraken_build-0.36.5/src/kraken/core/py.typed
+-rw-r--r--   0        0        0      132 2024-04-11 17:13:39.297388 kraken_build-0.36.5/src/kraken/core/system/__init__.py
+-rw-r--r--   0        0        0    17516 2024-04-11 18:13:27.439800 kraken_build-0.36.5/src/kraken/core/system/context.py
+-rw-r--r--   0        0        0     4367 2024-04-11 17:13:39.297911 kraken_build-0.36.5/src/kraken/core/system/context_test.py
+-rw-r--r--   0        0        0     1366 2024-04-11 18:13:27.440417 kraken_build-0.36.5/src/kraken/core/system/errors.py
+-rw-r--r--   0        0        0     2759 2024-04-11 17:13:39.298143 kraken_build-0.36.5/src/kraken/core/system/executor/__init__.py
+-rw-r--r--   0        0        0     2332 2024-04-11 17:13:39.298234 kraken_build-0.36.5/src/kraken/core/system/executor/colored.py
+-rw-r--r--   0        0        0     8511 2024-04-11 17:13:39.298375 kraken_build-0.36.5/src/kraken/core/system/executor/default.py
+-rw-r--r--   0        0        0     9377 2024-04-11 18:13:27.440716 kraken_build-0.36.5/src/kraken/core/system/executor/default_test.py
+-rw-r--r--   0        0        0     1554 2024-04-11 17:13:39.298600 kraken_build-0.36.5/src/kraken/core/system/executor/utils.py
+-rw-r--r--   0        0        0    24343 2024-04-11 17:13:39.298771 kraken_build-0.36.5/src/kraken/core/system/graph.py
+-rw-r--r--   0        0        0    15570 2024-04-11 17:13:39.299324 kraken_build-0.36.5/src/kraken/core/system/graph_test.py
+-rw-r--r--   0        0        0      947 2024-04-11 17:13:39.299412 kraken_build-0.36.5/src/kraken/core/system/kraken_object.py
+-rw-r--r--   0        0        0    16455 2024-04-11 18:13:27.440934 kraken_build-0.36.5/src/kraken/core/system/project.py
+-rw-r--r--   0        0        0     2893 2024-04-11 18:13:27.441140 kraken_build-0.36.5/src/kraken/core/system/project_test.py
+-rw-r--r--   0        0        0    18566 2024-04-11 17:13:39.299789 kraken_build-0.36.5/src/kraken/core/system/property.py
+-rw-r--r--   0        0        0     7588 2024-04-11 17:13:39.300117 kraken_build-0.36.5/src/kraken/core/system/property_test.py
+-rw-r--r--   0        0        0    28698 2024-04-11 18:13:27.441376 kraken_build-0.36.5/src/kraken/core/system/task.py
+-rw-r--r--   0        0        0      776 2024-04-11 17:13:39.300732 kraken_build-0.36.5/src/kraken/core/system/task_supplier.py
+-rw-r--r--   0        0        0     1458 2024-04-11 17:13:39.300820 kraken_build-0.36.5/src/kraken/core/system/task_test.py
+-rw-r--r--   0        0        0     1200 2024-04-11 17:13:39.300969 kraken_build-0.36.5/src/kraken/core/testing/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-11 19:39:33.065646 kraken_build-0.36.5/src/kraken/std/__init__.py
+-rw-r--r--   0        0        0     1950 2024-04-11 18:13:27.442173 kraken_build-0.36.5/src/kraken/std/buffrs/__init__.py
+-rw-r--r--   0        0        0     1921 2024-04-11 17:13:39.301351 kraken_build-0.36.5/src/kraken/std/buffrs/manifest.py
+-rw-r--r--   0        0        0     2338 2024-04-11 18:13:27.442334 kraken_build-0.36.5/src/kraken/std/buffrs/tasks.py
+-rw-r--r--   0        0        0    18824 2024-04-11 18:13:27.442552 kraken_build-0.36.5/src/kraken/std/cargo/__init__.py
+-rw-r--r--   0        0        0     2461 2024-04-11 17:13:39.302059 kraken_build-0.36.5/src/kraken/std/cargo/config.py
+-rw-r--r--   0        0        0     9339 2024-04-11 18:13:27.443555 kraken_build-0.36.5/src/kraken/std/cargo/manifest.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:13:39.302308 kraken_build-0.36.5/src/kraken/std/cargo/tasks/__init__.py
+-rw-r--r--   0        0        0      867 2024-04-11 17:13:39.302425 kraken_build-0.36.5/src/kraken/std/cargo/tasks/_cargo_sqlx.py
+-rw-r--r--   0        0        0     4931 2024-04-11 18:13:27.443851 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py
+-rw-r--r--   0        0        0     7126 2024-04-11 18:13:27.444135 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_build_task.py
+-rw-r--r--   0        0        0     2177 2024-04-11 17:13:39.302875 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py
+-rw-r--r--   0        0        0     1330 2024-04-11 17:13:39.302966 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_clippy_task.py
+-rw-r--r--   0        0        0     1004 2024-04-11 17:13:39.303057 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_deny_task.py
+-rw-r--r--   0        0        0     3527 2024-04-11 17:13:39.303157 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_fmt_task.py
+-rw-r--r--   0        0        0     1180 2024-04-11 17:13:39.303250 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_generate_deb.py
+-rw-r--r--   0        0        0     1503 2024-04-11 17:13:39.303339 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_login.py
+-rw-r--r--   0        0        0     4642 2024-04-11 17:13:39.303617 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_publish_task.py
+-rw-r--r--   0        0        0      368 2024-04-11 17:13:39.303702 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sqlx_database_create.py
+-rw-r--r--   0        0        0      360 2024-04-11 17:13:39.303798 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sqlx_database_drop.py
+-rw-r--r--   0        0        0      583 2024-04-11 17:13:39.303887 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sqlx_migrate.py
+-rw-r--r--   0        0        0      927 2024-04-11 17:13:39.303977 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sqlx_prepare.py
+-rw-r--r--   0        0        0     3144 2024-04-11 18:13:27.444320 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sync_config_task.py
+-rw-r--r--   0        0        0      462 2024-04-11 17:13:39.304158 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_test_task.py
+-rw-r--r--   0        0        0      387 2024-04-11 17:13:39.304245 kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_update_task.py
+-rw-r--r--   0        0        0      761 2024-04-11 17:13:39.304332 kraken_build-0.36.5/src/kraken/std/cargo/tasks/rustup_target_add_task.py
+-rw-r--r--   0        0        0      720 2024-04-11 17:13:39.304419 kraken_build-0.36.5/src/kraken/std/cargo/version.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:13:39.304507 kraken_build-0.36.5/src/kraken/std/descriptors/__init__.py
+-rw-r--r--   0        0        0      872 2024-04-11 17:13:39.304617 kraken_build-0.36.5/src/kraken/std/descriptors/resource.py
+-rw-r--r--   0        0        0    10250 2024-04-11 17:13:39.304775 kraken_build-0.36.5/src/kraken/std/dist.py
+-rw-r--r--   0        0        0     1574 2024-04-11 17:13:39.304924 kraken_build-0.36.5/src/kraken/std/docker/__init__.py
+-rw-r--r--   0        0        0      399 2024-04-11 17:13:39.305024 kraken_build-0.36.5/src/kraken/std/docker/_test.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:13:39.305059 kraken_build-0.36.5/src/kraken/std/docker/py.typed
+-rw-r--r--   0        0        0        0 2024-04-11 17:13:39.305170 kraken_build-0.36.5/src/kraken/std/docker/tasks/__init__.py
+-rw-r--r--   0        0        0     2915 2024-04-11 17:13:39.305281 kraken_build-0.36.5/src/kraken/std/docker/tasks/base_build_task.py
+-rw-r--r--   0        0        0     4013 2024-04-11 18:13:27.444511 kraken_build-0.36.5/src/kraken/std/docker/tasks/buildx_build_task.py
+-rw-r--r--   0        0        0     3685 2024-04-11 17:13:39.305489 kraken_build-0.36.5/src/kraken/std/docker/tasks/docker_build_task.py
+-rw-r--r--   0        0        0     8509 2024-04-11 18:13:27.444994 kraken_build-0.36.5/src/kraken/std/docker/tasks/kaniko_build_task.py
+-rw-r--r--   0        0        0     1461 2024-04-11 17:13:39.305732 kraken_build-0.36.5/src/kraken/std/docker/tasks/manifest_tool_push_task.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:13:39.305819 kraken_build-0.36.5/src/kraken/std/docker/util/__init__.py
+-rw-r--r--   0        0        0     1426 2024-04-11 17:13:39.305931 kraken_build-0.36.5/src/kraken/std/docker/util/dockerapi.py
+-rw-r--r--   0        0        0     2273 2024-04-11 17:13:39.306023 kraken_build-0.36.5/src/kraken/std/docker/util/dockerfile.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:13:39.306107 kraken_build-0.36.5/src/kraken/std/docs/__init__.py
+-rw-r--r--   0        0        0        5 2024-04-11 17:13:39.306257 kraken_build-0.36.5/src/kraken/std/docs/tasks/__init__.py
+-rw-r--r--   0        0        0     2214 2024-04-11 18:13:27.445215 kraken_build-0.36.5/src/kraken/std/docs/tasks/mkdocs.py
+-rw-r--r--   0        0        0     2414 2024-04-11 17:13:39.306433 kraken_build-0.36.5/src/kraken/std/docs/tasks/novella.py
+-rw-r--r--   0        0        0     1574 2024-04-11 17:13:39.306568 kraken_build-0.36.5/src/kraken/std/git/__init__.py
+-rw-r--r--   0        0        0     1119 2024-04-11 17:13:39.306655 kraken_build-0.36.5/src/kraken/std/git/config.py
+-rw-r--r--   0        0        0       61 2024-04-11 17:13:39.306784 kraken_build-0.36.5/src/kraken/std/git/gitignore/__init__.py
+-rw-r--r--   0        0        0     6157 2024-04-11 17:13:39.306990 kraken_build-0.36.5/src/kraken/std/git/gitignore/data/gitignore-io-tokens.json.gz
+-rw-r--r--   0        0        0     2739 2024-04-11 17:13:39.307086 kraken_build-0.36.5/src/kraken/std/git/gitignore/generated.py
+-rw-r--r--   0        0        0     1849 2024-04-11 17:13:39.307171 kraken_build-0.36.5/src/kraken/std/git/gitignore/generated_test.py
+-rw-r--r--   0        0        0     3309 2024-04-11 17:13:39.307268 kraken_build-0.36.5/src/kraken/std/git/gitignore/gitignore_io.py
+-rw-r--r--   0        0        0      687 2024-04-11 17:13:39.307361 kraken_build-0.36.5/src/kraken/std/git/gitignore/gitignore_io_test.py
+-rw-r--r--   0        0        0     4369 2024-04-11 17:13:39.307524 kraken_build-0.36.5/src/kraken/std/git/gitignore/parser.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:13:39.307558 kraken_build-0.36.5/src/kraken/std/git/gitignore_test.py
+-rw-r--r--   0        0        0      134 2024-04-11 17:13:39.307707 kraken_build-0.36.5/src/kraken/std/git/tasks/__init__.py
+-rw-r--r--   0        0        0     3011 2024-04-11 17:13:39.307802 kraken_build-0.36.5/src/kraken/std/git/tasks/check_file_task.py
+-rw-r--r--   0        0        0     2690 2024-04-11 17:13:39.307892 kraken_build-0.36.5/src/kraken/std/git/tasks/check_file_task_test.py
+-rw-r--r--   0        0        0     3667 2024-04-11 18:13:27.445402 kraken_build-0.36.5/src/kraken/std/git/tasks/sync_task.py
+-rw-r--r--   0        0        0     2349 2024-04-11 17:13:39.308075 kraken_build-0.36.5/src/kraken/std/git/tasks/sync_task_test.py
+-rw-r--r--   0        0        0     3164 2024-04-11 17:13:39.308185 kraken_build-0.36.5/src/kraken/std/git/version.py
+-rw-r--r--   0        0        0     6354 2024-04-11 17:13:39.308407 kraken_build-0.36.5/src/kraken/std/helm/__init__.py
+-rw-r--r--   0        0        0     2328 2024-04-11 17:13:39.308498 kraken_build-0.36.5/src/kraken/std/helm/helmapi.py
+-rw-r--r--   0        0        0     3292 2024-04-11 18:13:27.445591 kraken_build-0.36.5/src/kraken/std/mitm/__init__.py
+-rw-r--r--   0        0        0      861 2024-04-11 17:13:39.308739 kraken_build-0.36.5/src/kraken/std/mitm/mitm_addon.py
+-rw-r--r--   0        0        0     1347 2024-04-11 17:13:39.308871 kraken_build-0.36.5/src/kraken/std/protobuf/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:13:39.308905 kraken_build-0.36.5/src/kraken/std/py.typed
+-rw-r--r--   0        0        0     1754 2024-04-11 17:13:39.309069 kraken_build-0.36.5/src/kraken/std/python/__init__.py
+-rw-r--r--   0        0        0     6778 2024-04-11 18:13:27.445891 kraken_build-0.36.5/src/kraken/std/python/buildsystem/__init__.py
+-rw-r--r--   0        0        0     1439 2024-04-11 18:13:27.446074 kraken_build-0.36.5/src/kraken/std/python/buildsystem/helpers.py
+-rw-r--r--   0        0        0    10349 2024-04-11 18:13:27.446339 kraken_build-0.36.5/src/kraken/std/python/buildsystem/maturin.py
+-rw-r--r--   0        0        0     9785 2024-04-11 18:13:27.446647 kraken_build-0.36.5/src/kraken/std/python/buildsystem/pdm.py
+-rw-r--r--   0        0        0     2105 2024-04-11 17:13:39.309833 kraken_build-0.36.5/src/kraken/std/python/buildsystem/pdm_test.py
+-rw-r--r--   0        0        0    10853 2024-04-11 18:13:27.446887 kraken_build-0.36.5/src/kraken/std/python/buildsystem/poetry.py
+-rw-r--r--   0        0        0     3094 2024-04-11 17:13:39.310049 kraken_build-0.36.5/src/kraken/std/python/buildsystem/poetry_test.py
+-rw-r--r--   0        0        0     5177 2024-04-11 18:13:27.447198 kraken_build-0.36.5/src/kraken/std/python/buildsystem/slap.py
+-rw-r--r--   0        0        0     6251 2024-04-11 18:13:27.447487 kraken_build-0.36.5/src/kraken/std/python/pyproject.py
+-rw-r--r--   0        0        0     8712 2024-04-11 18:13:27.447748 kraken_build-0.36.5/src/kraken/std/python/settings.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:13:39.310643 kraken_build-0.36.5/src/kraken/std/python/tasks/__init__.py
+-rw-r--r--   0        0        0     3705 2024-04-11 17:13:39.310759 kraken_build-0.36.5/src/kraken/std/python/tasks/base_task.py
+-rw-r--r--   0        0        0     3352 2024-04-11 17:13:39.310853 kraken_build-0.36.5/src/kraken/std/python/tasks/black_task.py
+-rw-r--r--   0        0        0     2002 2024-04-11 18:13:27.447939 kraken_build-0.36.5/src/kraken/std/python/tasks/build_task.py
+-rw-r--r--   0        0        0     2207 2024-04-11 18:13:27.448118 kraken_build-0.36.5/src/kraken/std/python/tasks/flake8_task.py
+-rw-r--r--   0        0        0     2580 2024-04-11 17:13:39.311161 kraken_build-0.36.5/src/kraken/std/python/tasks/info_task.py
+-rw-r--r--   0        0        0     3298 2024-04-11 17:13:39.311250 kraken_build-0.36.5/src/kraken/std/python/tasks/install_task.py
+-rw-r--r--   0        0        0     3003 2024-04-11 17:13:39.311344 kraken_build-0.36.5/src/kraken/std/python/tasks/isort_task.py
+-rw-r--r--   0        0        0      970 2024-04-11 17:13:39.311447 kraken_build-0.36.5/src/kraken/std/python/tasks/login_task.py
+-rw-r--r--   0        0        0     2491 2024-04-11 17:13:39.311535 kraken_build-0.36.5/src/kraken/std/python/tasks/mypy_stubtest_task.py
+-rw-r--r--   0        0        0     4522 2024-04-11 17:13:39.311734 kraken_build-0.36.5/src/kraken/std/python/tasks/mypy_task.py
+-rw-r--r--   0        0        0     8000 2024-04-11 18:13:27.448441 kraken_build-0.36.5/src/kraken/std/python/tasks/pex_build_task.py
+-rw-r--r--   0        0        0     1682 2024-04-11 17:13:39.312262 kraken_build-0.36.5/src/kraken/std/python/tasks/pex_build_test.py
+-rw-r--r--   0        0        0     3447 2024-04-11 17:13:39.312404 kraken_build-0.36.5/src/kraken/std/python/tasks/publish_task.py
+-rw-r--r--   0        0        0     2750 2024-04-11 18:13:27.448586 kraken_build-0.36.5/src/kraken/std/python/tasks/pycln_task.py
+-rw-r--r--   0        0        0     2041 2024-04-11 17:13:39.312616 kraken_build-0.36.5/src/kraken/std/python/tasks/pylint_task.py
+-rw-r--r--   0        0        0     3887 2024-04-11 17:13:39.312730 kraken_build-0.36.5/src/kraken/std/python/tasks/pytest_task.py
+-rw-r--r--   0        0        0     5451 2024-04-11 18:13:27.448873 kraken_build-0.36.5/src/kraken/std/python/tasks/pyupgrade_task.py
+-rw-r--r--   0        0        0     1689 2024-04-11 17:13:39.313043 kraken_build-0.36.5/src/kraken/std/python/tasks/update_lockfile_task.py
+-rw-r--r--   0        0        0     1619 2024-04-11 17:13:39.313145 kraken_build-0.36.5/src/kraken/std/python/tasks/update_pyproject_task.py
+-rw-r--r--   0        0        0     1144 2024-04-11 17:13:39.313244 kraken_build-0.36.5/src/kraken/std/python/version.py
+-rw-r--r--   0        0        0     4115 2024-04-11 17:13:39.313564 kraken_build-0.36.5/src/kraken/std/sccache.py
+-rw-r--r--   0        0        0     3841 2024-04-11 18:13:27.448980 kraken_build-0.36.5/src/kraken/std/shellcheck.py
+-rw-r--r--   0        0        0      232 2024-04-11 17:13:39.313831 kraken_build-0.36.5/src/kraken/std/util/__init__.py
+-rw-r--r--   0        0        0     2198 2024-04-11 17:13:39.313935 kraken_build-0.36.5/src/kraken/std/util/check_file_contents_task.py
+-rw-r--r--   0        0        0      910 2024-04-11 17:13:39.314041 kraken_build-0.36.5/src/kraken/std/util/check_file_contents_task_test.py
+-rw-r--r--   0        0        0     2838 2024-04-11 17:13:39.314147 kraken_build-0.36.5/src/kraken/std/util/copyright_task.py
+-rw-r--r--   0        0        0     9660 2024-04-11 18:13:27.449242 kraken_build-0.36.5/src/kraken/std/util/daemon_controller.py
+-rw-r--r--   0        0        0     1167 2024-04-11 18:13:27.449335 kraken_build-0.36.5/src/kraken/std/util/http.py
+-rw-r--r--   0        0        0     3417 2024-04-11 17:13:39.314517 kraken_build-0.36.5/src/kraken/std/util/render_file_task.py
+-rw-r--r--   0        0        0      625 2024-04-11 18:13:27.449424 kraken_build-0.36.5/src/kraken/std/util/url.py
+-rw-r--r--   0        0        0     7175 2024-04-11 17:13:39.314833 kraken_build-0.36.5/src/kraken/std/util/validate_readme.py
+-rw-r--r--   0        0        0     3173 2024-04-11 17:13:39.314950 kraken_build-0.36.5/src/kraken/std/util/validate_readme_test.py
+-rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 kraken_build-0.36.5/PKG-INFO
```

### Comparing `kraken_build-0.36.4/LICENSE` & `kraken_build-0.36.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/README.md` & `kraken_build-0.36.5/README.md`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/pyproject.toml` & `kraken_build-0.36.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 packages = [
   {include = "kraken/build", from = "src"},
   {include = "kraken/common", from = "src"},
   {include = "kraken/core", from = "src"},
   {include = "kraken/std", from = "src"},
 ]
 readme = "README.md"
-version = "0.36.4"
+version = "0.36.5"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kraken-build/kraken-build/issues"
 Documentation = "https://kraken-build.github.io/kraken-build/"
 Homepage = "https://kraken-build.github.io/kraken-build/"
 Repository = "https://github.com/kraken-build/kraken-build/"
 
@@ -37,46 +37,40 @@
 # ------------
 
 [tool.poetry.dependencies]
 databind-json = "^4.2.5"
 dataclasses = {version = "^0.6", python = "<3.7"}
 deprecated = "^1.2.13"
 dill = ">=0.3.8,<0.4.0"
-httpx = "^0.26.0"
-keyring = "^24.0.0"
+httpx = "^0.27.0"
+keyring = "^25.0.0"
 networkx = "^3.1"
 nr-io-graphviz = "^0.1.1"
 nr-stream = "^1.1.0"
 packaging = "^23.1"
 pex = "^2.1.156"
 python = ">=3.10"
 rich = "^13.4.2"
-termcolor = "^1.1.0"
+termcolor = "^2.0.0"
 tomli = "^2.0.1"
 tomli-w = "^1.0.0"
 tomlkit = "^0.12.4"
 typeapi = "^2.0.0"
 typing-extensions = ">=4.6.0"
 
 [tool.poetry.dev-dependencies]
 localimport = "^1.7.6"
-pyartifactory = "^1.10.0"
+pyartifactory = "^2.0.0"
 pytest = ">=6.0.0"
 types-Deprecated = "^1.2.9"
 types-requests = "^2.28.0"
 types-termcolor = "^1.1.5"
 pytest-xdist = {version = "^3.5.0", extras = ["psutil"]}
 mitmproxy = "^10.2.4"
 
-[tool.poetry.group.docs.dependencies]
-mkdocs = "*"
-mkdocs-material = "*"
-novella = "0.2.6"
-pydoc-markdown = "^4.6.0"
-
 # Slap configuration
 # ------------------
 
 [tool.slap]
 typed = true
 
 # Linter/Formatter configuration
```

### Comparing `kraken_build-0.36.4/src/kraken/build/__init__.py` & `kraken_build-0.36.5/src/kraken/build/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/build/tests/test_import.py` & `kraken_build-0.36.5/src/kraken/build/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/build/utils/import_helper.py` & `kraken_build-0.36.5/src/kraken/build/utils/import_helper.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/__init__.py` & `kraken_build-0.36.5/src/kraken/common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.36.4"
+__version__ = "0.36.5"
 
 from . import path
 from ._argparse import propagate_argparse_formatter_to_subparser
 from ._asciitable import AsciiTable
 from ._auth import CredentialsWithHost
 from ._buildscript import BuildscriptMetadata, BuildscriptMetadataException, buildscript
 from ._date import datetime_to_iso8601, iso8601_to_datetime
```

### Comparing `kraken_build-0.36.4/src/kraken/common/_asciitable.py` & `kraken_build-0.36.5/src/kraken/common/_asciitable.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_buildscript.py` & `kraken_build-0.36.5/src/kraken/common/_buildscript.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_buildscript_test.py` & `kraken_build-0.36.5/src/kraken/common/_buildscript_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_date.py` & `kraken_build-0.36.5/src/kraken/common/_date.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_date_test.py` & `kraken_build-0.36.5/src/kraken/common/_date_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_environment.py` & `kraken_build-0.36.5/src/kraken/common/_environment.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_fs.py` & `kraken_build-0.36.5/src/kraken/common/_fs.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_generic.py` & `kraken_build-0.36.5/src/kraken/common/_generic.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_importlib.py` & `kraken_build-0.36.5/src/kraken/common/_importlib.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_option_sets.py` & `kraken_build-0.36.5/src/kraken/common/_option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_requirements.py` & `kraken_build-0.36.5/src/kraken/common/_requirements.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_requirements_test.py` & `kraken_build-0.36.5/src/kraken/common/_requirements_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_runner.py` & `kraken_build-0.36.5/src/kraken/common/_runner.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_runner_test.py` & `kraken_build-0.36.5/src/kraken/common/_runner_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_text.py` & `kraken_build-0.36.5/src/kraken/common/_text.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_tomlconfig.py` & `kraken_build-0.36.5/src/kraken/common/_tomlconfig.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/_tomlconfig_test.py` & `kraken_build-0.36.5/src/kraken/common/_tomlconfig_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/exceptions.py` & `kraken_build-0.36.5/src/kraken/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/findpython.py` & `kraken_build-0.36.5/src/kraken/common/findpython.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/http/__init__.py` & `kraken_build-0.36.5/src/kraken/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/http/lint_ban_bare_requests.py` & `kraken_build-0.36.5/src/kraken/common/http/lint_ban_bare_requests.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/path.py` & `kraken_build-0.36.5/src/kraken/common/path.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/pyenv/_distributions.py` & `kraken_build-0.36.5/src/kraken/common/pyenv/_distributions.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/pyenv/_virtualenv.py` & `kraken_build-0.36.5/src/kraken/common/pyenv/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/common/supplier.py` & `kraken_build-0.36.5/src/kraken/common/supplier.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/__init__.py` & `kraken_build-0.36.5/src/kraken/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.36.4"
+__version__ = "0.36.5"
 
 from kraken.core.address import Address
 from kraken.core.system.context import Context, ContextEvent
 from kraken.core.system.errors import BuildError, ProjectLoaderError
 from kraken.core.system.executor import Graph
 from kraken.core.system.graph import TaskGraph
 from kraken.core.system.project import Project
```

### Comparing `kraken_build-0.36.4/src/kraken/core/address/_address.py` & `kraken_build-0.36.5/src/kraken/core/address/_address.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/address/_address_resolver.py` & `kraken_build-0.36.5/src/kraken/core/address/_address_resolver.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/address/_address_resolver_test.py` & `kraken_build-0.36.5/src/kraken/core/address/_address_resolver_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/address/_address_test.py` & `kraken_build-0.36.5/src/kraken/core/address/_address_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/address/_addressable.py` & `kraken_build-0.36.5/src/kraken/core/address/_addressable.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/base/currentable.py` & `kraken_build-0.36.5/src/kraken/core/base/currentable.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/base/metadata.py` & `kraken_build-0.36.5/src/kraken/core/base/metadata.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/cli/executor.py` & `kraken_build-0.36.5/src/kraken/core/cli/executor.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/cli/main.py` & `kraken_build-0.36.5/src/kraken/core/cli/main.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/cli/option_sets.py` & `kraken_build-0.36.5/src/kraken/core/cli/option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/cli/serialize.py` & `kraken_build-0.36.5/src/kraken/core/cli/serialize.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/context.py` & `kraken_build-0.36.5/src/kraken/core/system/context.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/context_test.py` & `kraken_build-0.36.5/src/kraken/core/system/context_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/errors.py` & `kraken_build-0.36.5/src/kraken/core/system/errors.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/executor/__init__.py` & `kraken_build-0.36.5/src/kraken/core/system/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/executor/colored.py` & `kraken_build-0.36.5/src/kraken/core/system/executor/colored.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/executor/default.py` & `kraken_build-0.36.5/src/kraken/core/system/executor/default.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/executor/default_test.py` & `kraken_build-0.36.5/src/kraken/core/system/executor/default_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/executor/utils.py` & `kraken_build-0.36.5/src/kraken/core/system/executor/utils.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/graph.py` & `kraken_build-0.36.5/src/kraken/core/system/graph.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/graph_test.py` & `kraken_build-0.36.5/src/kraken/core/system/graph_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/kraken_object.py` & `kraken_build-0.36.5/src/kraken/core/system/kraken_object.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/project.py` & `kraken_build-0.36.5/src/kraken/core/system/project.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/project_test.py` & `kraken_build-0.36.5/src/kraken/core/system/project_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/property.py` & `kraken_build-0.36.5/src/kraken/core/system/property.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/property_test.py` & `kraken_build-0.36.5/src/kraken/core/system/property_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/task.py` & `kraken_build-0.36.5/src/kraken/core/system/task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/task_supplier.py` & `kraken_build-0.36.5/src/kraken/core/system/task_supplier.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/system/task_test.py` & `kraken_build-0.36.5/src/kraken/core/system/task_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/core/testing/__init__.py` & `kraken_build-0.36.5/src/kraken/core/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/buffrs/__init__.py` & `kraken_build-0.36.5/src/kraken/std/buffrs/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/buffrs/manifest.py` & `kraken_build-0.36.5/src/kraken/std/buffrs/manifest.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/buffrs/tasks.py` & `kraken_build-0.36.5/src/kraken/std/buffrs/tasks.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/__init__.py` & `kraken_build-0.36.5/src/kraken/std/cargo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,14 +317,15 @@
     *,
     exclude: Collection[str] = (),
     group: str | None = "build",
     name: str | None = None,
     project: Project | None = None,
     features: list[str] | None = None,
     depends_on: Sequence[Task] = (),
+    locked: bool | None = None,
 ) -> CargoBuildTask:
     """Creates a task that runs `cargo build`.
 
     :param mode: Whether to create a task that runs the debug or release build.
     :param incremental: Whether to build incrementally or not (with the `--incremental=` option). If not
         specified, the option is not specified and the default behaviour is used.
     :param env: Override variables for the build environment variables. Values in this dictionary override
@@ -355,14 +356,15 @@
         f"cargoBuild{mode.capitalize()}" if name is None else name,
         CargoBuildTask,
         group=group,
     )
     task.incremental = incremental
     task.target = mode
     task.additional_args = additional_args
+    task.locked = locked
     task.env = Supplier.of_callable(lambda: {**cargo.build_env, **(env or {})})
 
     task.depends_on(f":{CARGO_BUILD_SUPPORT_GROUP_NAME}?")
 
     for dependency in depends_on:
         task.depends_on(dependency)
```

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/config.py` & `kraken_build-0.36.5/src/kraken/std/cargo/config.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/manifest.py` & `kraken_build-0.36.5/src/kraken/std/cargo/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from dataclasses import dataclass, fields
 from enum import Enum
 from pathlib import Path
 from typing import Any
 
 import tomli
 import tomli_w
-from pydantic import ClassError
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Bin:
     name: str
@@ -236,15 +235,15 @@
     bin: list[Bin]
 
     @classmethod
     def read(cls, path: Path) -> CargoManifest:
         with path.open("rb") as fp:
             ret = cls.of(path, tomli.load(fp))
             if ret.package is None and ret.workspace is None:
-                raise ClassError
+                raise ValueError("Cargo manifest must have either a package or a workspace section.")
             return ret
 
     @classmethod
     def of(cls, path: Path, data: dict[str, Any]) -> CargoManifest:
         return cls(
             path,
             data,
```

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/_cargo_sqlx.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/_cargo_sqlx.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_build_task.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_clippy_task.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_clippy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_deny_task.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_deny_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_fmt_task.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_fmt_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_generate_deb.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_generate_deb.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_login.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_login.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_publish_task.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_publish_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_sqlx_migrate.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sqlx_migrate.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_sqlx_prepare.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sqlx_prepare.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/cargo_sync_config_task.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/cargo_sync_config_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/tasks/rustup_target_add_task.py` & `kraken_build-0.36.5/src/kraken/std/cargo/tasks/rustup_target_add_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/cargo/version.py` & `kraken_build-0.36.5/src/kraken/std/cargo/version.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/descriptors/resource.py` & `kraken_build-0.36.5/src/kraken/std/descriptors/resource.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/dist.py` & `kraken_build-0.36.5/src/kraken/std/dist.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/docker/__init__.py` & `kraken_build-0.36.5/src/kraken/std/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/docker/tasks/base_build_task.py` & `kraken_build-0.36.5/src/kraken/std/docker/tasks/base_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/docker/tasks/buildx_build_task.py` & `kraken_build-0.36.5/src/kraken/std/docker/tasks/buildx_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/docker/tasks/docker_build_task.py` & `kraken_build-0.36.5/src/kraken/std/docker/tasks/docker_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/docker/tasks/kaniko_build_task.py` & `kraken_build-0.36.5/src/kraken/std/docker/tasks/kaniko_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/docker/tasks/manifest_tool_push_task.py` & `kraken_build-0.36.5/src/kraken/std/docker/tasks/manifest_tool_push_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/docker/util/dockerapi.py` & `kraken_build-0.36.5/src/kraken/std/docker/util/dockerapi.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/docker/util/dockerfile.py` & `kraken_build-0.36.5/src/kraken/std/docker/util/dockerfile.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/docs/tasks/mkdocs.py` & `kraken_build-0.36.5/src/kraken/std/docs/tasks/mkdocs.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/docs/tasks/novella.py` & `kraken_build-0.36.5/src/kraken/std/docs/tasks/novella.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/git/__init__.py` & `kraken_build-0.36.5/src/kraken/std/git/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/git/config.py` & `kraken_build-0.36.5/src/kraken/std/git/config.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/git/gitignore/data/gitignore-io-tokens.json.gz` & `kraken_build-0.36.5/src/kraken/std/git/gitignore/data/gitignore-io-tokens.json.gz`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/git/gitignore/generated.py` & `kraken_build-0.36.5/src/kraken/std/git/gitignore/generated.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/git/gitignore/generated_test.py` & `kraken_build-0.36.5/src/kraken/std/git/gitignore/generated_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/git/gitignore/gitignore_io.py` & `kraken_build-0.36.5/src/kraken/std/git/gitignore/gitignore_io.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/git/gitignore/gitignore_io_test.py` & `kraken_build-0.36.5/src/kraken/std/git/gitignore/gitignore_io_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/git/gitignore/parser.py` & `kraken_build-0.36.5/src/kraken/std/git/gitignore/parser.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/git/tasks/check_file_task.py` & `kraken_build-0.36.5/src/kraken/std/git/tasks/check_file_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/git/tasks/check_file_task_test.py` & `kraken_build-0.36.5/src/kraken/std/git/tasks/check_file_task_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/git/tasks/sync_task.py` & `kraken_build-0.36.5/src/kraken/std/git/tasks/sync_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,19 +49,21 @@
 
         # When no generated section is found, the entire file content sits in user1. If we want our new generated
         # content to sit at the top, we need to swap user1 and user2.
         if not generated and self.where.get() == "top":
             user1, user2 = user2, user1
 
         # Replace the generated content.
-        generated = GitignoreFile.parse(self.generated_content.get())
+        generated = GitignoreFile()
         if tokens := self.gitignore_io_tokens.get():
             generated += GitignoreFile.parse(
                 gitignore_io_fetch_cached(tokens, backfill=self.gitignore_io_allow_http_request_backfill.get())
             )
+        # User-provided generated content, allowing for overrides to API-generated content.
+        generated += GitignoreFile.parse(self.generated_content.get())
 
         # Ensure there's at least one blank space between sections.
         if user1 and generated and (user1[-1] != "" and generated[0] != ""):
             user1.append(GitignoreEntry())
         if generated and user2 and (generated[-1] != "" and user2[0] != ""):
             user2.insert(0, GitignoreEntry())
```

### Comparing `kraken_build-0.36.4/src/kraken/std/git/tasks/sync_task_test.py` & `kraken_build-0.36.5/src/kraken/std/git/tasks/sync_task_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/git/version.py` & `kraken_build-0.36.5/src/kraken/std/git/version.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/helm/__init__.py` & `kraken_build-0.36.5/src/kraken/std/helm/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/helm/helmapi.py` & `kraken_build-0.36.5/src/kraken/std/helm/helmapi.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/mitm/__init__.py` & `kraken_build-0.36.5/src/kraken/std/mitm/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/mitm/mitm_addon.py` & `kraken_build-0.36.5/src/kraken/std/mitm/mitm_addon.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/protobuf/__init__.py` & `kraken_build-0.36.5/src/kraken/std/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/__init__.py` & `kraken_build-0.36.5/src/kraken/std/python/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/buildsystem/__init__.py` & `kraken_build-0.36.5/src/kraken/std/python/buildsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/buildsystem/helpers.py` & `kraken_build-0.36.5/src/kraken/std/python/buildsystem/helpers.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/buildsystem/maturin.py` & `kraken_build-0.36.5/src/kraken/std/python/buildsystem/maturin.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/buildsystem/pdm.py` & `kraken_build-0.36.5/src/kraken/std/python/buildsystem/pdm.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/buildsystem/pdm_test.py` & `kraken_build-0.36.5/src/kraken/std/python/buildsystem/pdm_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/buildsystem/poetry.py` & `kraken_build-0.36.5/src/kraken/std/python/buildsystem/poetry.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/buildsystem/poetry_test.py` & `kraken_build-0.36.5/src/kraken/std/python/buildsystem/poetry_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/buildsystem/slap.py` & `kraken_build-0.36.5/src/kraken/std/python/buildsystem/slap.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/pyproject.py` & `kraken_build-0.36.5/src/kraken/std/python/pyproject.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/settings.py` & `kraken_build-0.36.5/src/kraken/std/python/settings.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/base_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/black_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/black_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/build_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/flake8_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/flake8_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/info_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/info_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/install_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/install_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/isort_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/isort_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/login_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/login_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/mypy_stubtest_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/mypy_stubtest_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/mypy_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/mypy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/pex_build_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/pex_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/pex_build_test.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/pex_build_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/publish_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/publish_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/pycln_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/pycln_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/pylint_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/pylint_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/pytest_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/pytest_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/pyupgrade_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/pyupgrade_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/update_lockfile_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/update_lockfile_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/tasks/update_pyproject_task.py` & `kraken_build-0.36.5/src/kraken/std/python/tasks/update_pyproject_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/python/version.py` & `kraken_build-0.36.5/src/kraken/std/python/version.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/sccache.py` & `kraken_build-0.36.5/src/kraken/std/sccache.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/shellcheck.py` & `kraken_build-0.36.5/src/kraken/std/shellcheck.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/util/check_file_contents_task.py` & `kraken_build-0.36.5/src/kraken/std/util/check_file_contents_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/util/check_file_contents_task_test.py` & `kraken_build-0.36.5/src/kraken/std/util/check_file_contents_task_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/util/copyright_task.py` & `kraken_build-0.36.5/src/kraken/std/util/copyright_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/util/daemon_controller.py` & `kraken_build-0.36.5/src/kraken/std/util/daemon_controller.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/util/http.py` & `kraken_build-0.36.5/src/kraken/std/util/http.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/util/render_file_task.py` & `kraken_build-0.36.5/src/kraken/std/util/render_file_task.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/util/url.py` & `kraken_build-0.36.5/src/kraken/std/util/url.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/util/validate_readme.py` & `kraken_build-0.36.5/src/kraken/std/util/validate_readme.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/src/kraken/std/util/validate_readme_test.py` & `kraken_build-0.36.5/src/kraken/std/util/validate_readme_test.py`

 * *Files identical despite different names*

### Comparing `kraken_build-0.36.4/PKG-INFO` & `kraken_build-0.36.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: kraken-build
-Version: 0.36.4
+Version: 0.36.5
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: databind-json (>=4.2.5,<5.0.0)
 Requires-Dist: dataclasses (>=0.6,<0.7) ; python_version < "3.7"
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
-Requires-Dist: httpx (>=0.26.0,<0.27.0)
-Requires-Dist: keyring (>=24.0.0,<25.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: keyring (>=25.0.0,<26.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: nr-io-graphviz (>=0.1.1,<0.2.0)
 Requires-Dist: nr-stream (>=1.1.0,<2.0.0)
 Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: pex (>=2.1.156,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
-Requires-Dist: termcolor (>=1.1.0,<2.0.0)
+Requires-Dist: termcolor (>=2.0.0,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Requires-Dist: tomlkit (>=0.12.4,<0.13.0)
 Requires-Dist: typeapi (>=2.0.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.6.0)
 Project-URL: Bug Tracker, https://github.com/kraken-build/kraken-build/issues
 Project-URL: Documentation, https://kraken-build.github.io/kraken-build/
```

