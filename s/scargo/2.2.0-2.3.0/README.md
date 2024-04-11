# Comparing `tmp/scargo-2.2.0.tar.gz` & `tmp/scargo-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scargo-2.2.0.tar", last modified: Fri Jan  5 07:36:21 2024, max compression
+gzip compressed data, was "scargo-2.3.0.tar", last modified: Thu Apr 11 09:14:44 2024, max compression
```

## Comparing `scargo-2.2.0.tar` & `scargo-2.3.0.tar`

### file list

```diff
@@ -1,116 +1,117 @@
--rw-r--r--   0        0        0     4508 2024-01-05 07:36:16.879221 scargo-2.2.0/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     1066 2024-01-05 07:36:16.879221 scargo-2.2.0/LICENSE
--rw-r--r--   0        0        0     3641 2024-01-05 07:36:16.879221 scargo-2.2.0/README.md
--rw-r--r--   0        0        0     3644 2024-01-05 07:36:16.891221 scargo-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      108 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/__init__.py
--rwxr-xr-x   0        0        0    19736 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/certs/certGen.sh
--rwxr-xr-x   0        0        0     4632 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/certs/generateAllCertificates.sh
--rw-r--r--   0        0        0     3967 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/certs/openssl_device_intermediate_ca.cnf
--rw-r--r--   0        0        0     3957 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/certs/openssl_root_ca.cnf
--rw-r--r--   0        0        0    14090 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/cli.py
--rw-r--r--   0        0        0       86 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/__init__.py
--rw-r--r--   0        0        0     3403 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/build.py
--rw-r--r--   0        0        0    14502 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/check.py
--rw-r--r--   0        0        0     1829 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/clean.py
--rw-r--r--   0        0        0     4128 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/debug.py
--rw-r--r--   0        0        0     3398 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/doc.py
--rw-r--r--   0        0        0     3897 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/docker.py
--rw-r--r--   0        0        0     1124 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/fix.py
--rw-r--r--   0        0        0     8479 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/flash.py
--rw-r--r--   0        0        0     3953 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/gen.py
--rw-r--r--   0        0        0     4658 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/new.py
--rw-r--r--   0        0        0     2694 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/publish.py
--rw-r--r--   0        0        0     1933 2024-01-05 07:36:16.891221 scargo-2.2.0/scargo/commands/run.py
--rw-r--r--   0        0        0     4187 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/commands/test.py
--rw-r--r--   0        0        0     4182 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/commands/update.py
--rw-r--r--   0        0        0      228 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/commands/version.py
--rw-r--r--   0        0        0    11104 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/config.py
--rw-r--r--   0        0        0     3024 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/config_utils.py
--rw-r--r--   0        0        0       86 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/__init__.py
--rw-r--r--   0        0        0     1656 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/base_gen.py
--rw-r--r--   0        0        0     3496 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/cicd_gen.py
--rw-r--r--   0        0        0       86 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/clang_parser/__init__.py
--rw-r--r--   0        0        0     2251 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/clang_parser/data_classes.py
--rw-r--r--   0        0        0     1197 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/clang_parser/header_parser.py
--rw-r--r--   0        0        0     2385 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/clang_parser/params_extractor.py
--rw-r--r--   0        0        0      395 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/cmake_gen.py
--rw-r--r--   0        0        0     2105 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/conan_gen.py
--rw-r--r--   0        0        0     3937 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/cpp_gen.py
--rw-r--r--   0        0        0     3307 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/docker_gen.py
--rw-r--r--   0        0        0     1115 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/env_gen.py
--rwxr-xr-x   0        0        0     1607 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/mock_gen.py
--rw-r--r--   0        0        0      454 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/readme_gen.py
--rw-r--r--   0        0        0      119 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/.gitlab-ci-custom.yml.j2
--rw-r--r--   0        0        0     4980 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/.gitlab-ci.yml.j2
--rw-r--r--   0        0        0     2259 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/CMakeLists.txt.j2
--rw-r--r--   0        0        0     9664 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/README.md.j2
--rw-r--r--   0        0        0     3578 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/conan/conanfile.py.j2
--rw-r--r--   0        0        0     1534 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/conan/conanfiletest.j2
--rw-r--r--   0        0        0      890 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/conan/profile_atsam.j2
--rw-r--r--   0        0        0      739 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/conan/profile_esp32.j2
--rw-r--r--   0        0        0      905 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/conan/profile_stm32.j2
--rw-r--r--   0        0        0      885 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/conan/profile_x86.j2
--rw-r--r--   0        0        0      342 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/conan/test_package/CMakeLists.txt.j2
--rw-r--r--   0        0        0      749 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/conan/test_package/conanfile.py.j2
--rw-r--r--   0        0        0      118 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/conan/test_package/example.cpp.j2
--rw-r--r--   0        0        0     2902 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/conan/toolchain/arm_gcc_toolchain.cmake.j2
--rw-r--r--   0        0        0      469 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/conan/toolchain/stm32_gcc_toolchain.cmake.j2
--rw-r--r--   0        0        0     2183 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/cpp/cmake-src-atsam.j2
--rw-r--r--   0        0        0      150 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
--rw-r--r--   0        0        0       71 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/cpp/cmake-src-multitarget.j2
--rw-r--r--   0        0        0     2907 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
--rw-r--r--   0        0        0      796 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2
--rw-r--r--   0        0        0      240 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/cpp/lib.cpp.j2
--rw-r--r--   0        0        0      272 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/cpp/lib.h.j2
--rw-r--r--   0        0        0     1063 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/cpp/main.cpp.j2
--rw-r--r--   0        0        0      782 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/docker/Dockerfile-arm.j2
--rw-r--r--   0        0        0      613 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2
--rw-r--r--   0        0        0     1609 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
--rw-r--r--   0        0        0     2634 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/docker/Dockerfile.j2
--rw-r--r--   0        0        0      149 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/docker/atsam-gdb.script.j2
--rw-r--r--   0        0        0      123 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/docker/atsam-openocd.cfg.j2
--rw-r--r--   0        0        0     1120 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/docker/devcontainer.json.j2
--rw-r--r--   0        0        0      993 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2
--rw-r--r--   0        0        0      287 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/docker/env.txt.j2
--rw-r--r--   0        0        0       93 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/docker/stm32-openocd.cfg.j2
--rw-r--r--   0        0        0       39 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/mock/.clang-format
--rw-r--r--   0        0        0      475 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/mock/CMakeLists.txt
--rw-r--r--   0        0        0      594 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/mock/class_interface.h.j2
--rw-r--r--   0        0        0      835 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/mock/class_mock.cpp.j2
--rw-r--r--   0        0        0      697 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/mock/class_mock.h.j2
--rw-r--r--   0        0        0     2979 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/scargo.toml.j2
--rw-r--r--   0        0        0       91 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
--rw-r--r--   0        0        0      100 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
--rw-r--r--   0        0        0     1140 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
--rw-r--r--   0        0        0       84 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
--rw-r--r--   0        0        0      326 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
--rw-r--r--   0        0        0     1046 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/tests/static_mock/static_mock.h
--rw-r--r--   0        0        0       39 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/ut/.clang-format
--rw-r--r--   0        0        0      575 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2
--rw-r--r--   0        0        0      716 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/ut/ut.cpp.j2
--rw-r--r--   0        0        0      565 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/vscode/launch.json.j2
--rw-r--r--   0        0        0     1040 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/templates/vscode/tasks.json.j2
--rw-r--r--   0        0        0     1492 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/tests_gen.py
--rw-r--r--   0        0        0      550 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/toml_gen.py
--rw-r--r--   0        0        0     5357 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/ut_gen.py
--rw-r--r--   0        0        0     1789 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/file_generators/vscode_gen.py
--rw-r--r--   0        0        0      629 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/global_values.py
--rw-r--r--   0        0        0     2107 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/logger.py
--rw-r--r--   0        0        0        0 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/target_helpers/__init__.py
--rw-r--r--   0        0        0    40877 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/target_helpers/atmel.xml
--rw-r--r--   0        0        0     3057 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/target_helpers/atsam_helper.py
--rw-r--r--   0        0        0     3049 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/target_helpers/esp32_helper.py
--rw-r--r--   0        0        0      982 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/target_helpers/stm32_helper.py
--rw-r--r--   0        0        0     2953 2024-01-05 07:36:16.895221 scargo-2.2.0/scargo/templates/.clang-format
--rw-r--r--   0        0        0     8780 2024-01-05 07:36:16.899221 scargo-2.2.0/scargo/templates/.clang-tidy
--rw-r--r--   0        0        0     2362 2024-01-05 07:36:16.899221 scargo-2.2.0/scargo/templates/.gitignore
--rw-r--r--   0        0        0     1066 2024-01-05 07:36:16.899221 scargo-2.2.0/scargo/templates/LICENSE
--rw-r--r--   0        0        0        0 2024-01-05 07:36:16.899221 scargo-2.2.0/scargo/utils/__init__.py
--rw-r--r--   0        0        0      698 2024-01-05 07:36:16.899221 scargo-2.2.0/scargo/utils/clang_utils.py
--rw-r--r--   0        0        0     2396 2024-01-05 07:36:16.899221 scargo-2.2.0/scargo/utils/conan_utils.py
--rw-r--r--   0        0        0     2388 2024-01-05 07:36:16.899221 scargo-2.2.0/scargo/utils/docker_utils.py
--rw-r--r--   0        0        0     2800 2024-01-05 07:36:16.899221 scargo-2.2.0/scargo/utils/file_utils.py
--rw-r--r--   0        0        0      778 2024-01-05 07:36:16.899221 scargo-2.2.0/scargo/utils/path_utils.py
--rw-r--r--   0        0        0      596 2024-01-05 07:36:16.899221 scargo-2.2.0/scargo/utils/sys_utils.py
--rw-r--r--   0        0        0      573 2024-01-05 07:36:16.899221 scargo-2.2.0/setup.cfg
--rw-r--r--   0        0        0     6729 1970-01-01 00:00:00.000000 scargo-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4508 2024-04-11 09:14:40.212261 scargo-2.3.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     1066 2024-04-11 09:14:40.212261 scargo-2.3.0/LICENSE
+-rw-r--r--   0        0        0     3641 2024-04-11 09:14:40.212261 scargo-2.3.0/README.md
+-rw-r--r--   0        0        0     3644 2024-04-11 09:14:40.224261 scargo-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      108 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/__init__.py
+-rwxr-xr-x   0        0        0    19736 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/certs/certGen.sh
+-rwxr-xr-x   0        0        0     4632 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/certs/generateAllCertificates.sh
+-rw-r--r--   0        0        0     3967 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/certs/openssl_device_intermediate_ca.cnf
+-rw-r--r--   0        0        0     3957 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/certs/openssl_root_ca.cnf
+-rw-r--r--   0        0        0    14932 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/cli.py
+-rw-r--r--   0        0        0       86 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/__init__.py
+-rw-r--r--   0        0        0     3403 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/build.py
+-rw-r--r--   0        0        0    14502 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/check.py
+-rw-r--r--   0        0        0     1829 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/clean.py
+-rw-r--r--   0        0        0     4128 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/debug.py
+-rw-r--r--   0        0        0     3398 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/doc.py
+-rw-r--r--   0        0        0     3897 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/docker.py
+-rw-r--r--   0        0        0     1124 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/fix.py
+-rw-r--r--   0        0        0     9206 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/flash.py
+-rw-r--r--   0        0        0     3953 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/gen.py
+-rw-r--r--   0        0        0     4302 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/monitor.py
+-rw-r--r--   0        0        0     4658 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/new.py
+-rw-r--r--   0        0        0     2694 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/publish.py
+-rw-r--r--   0        0        0     1933 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/run.py
+-rw-r--r--   0        0        0     4187 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/test.py
+-rw-r--r--   0        0        0     4182 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/update.py
+-rw-r--r--   0        0        0      228 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/commands/version.py
+-rw-r--r--   0        0        0    11104 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/config.py
+-rw-r--r--   0        0        0     3024 2024-04-11 09:14:40.224261 scargo-2.3.0/scargo/config_utils.py
+-rw-r--r--   0        0        0       86 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/__init__.py
+-rw-r--r--   0        0        0     1656 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/base_gen.py
+-rw-r--r--   0        0        0     3496 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/cicd_gen.py
+-rw-r--r--   0        0        0       86 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/clang_parser/__init__.py
+-rw-r--r--   0        0        0     2251 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/clang_parser/data_classes.py
+-rw-r--r--   0        0        0     1197 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/clang_parser/header_parser.py
+-rw-r--r--   0        0        0     2385 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/clang_parser/params_extractor.py
+-rw-r--r--   0        0        0      395 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/cmake_gen.py
+-rw-r--r--   0        0        0     2105 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/conan_gen.py
+-rw-r--r--   0        0        0     3937 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/cpp_gen.py
+-rw-r--r--   0        0        0     3307 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/docker_gen.py
+-rw-r--r--   0        0        0     1115 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/env_gen.py
+-rwxr-xr-x   0        0        0     1607 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/mock_gen.py
+-rw-r--r--   0        0        0      454 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/readme_gen.py
+-rw-r--r--   0        0        0      119 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/.gitlab-ci-custom.yml.j2
+-rw-r--r--   0        0        0     4980 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/.gitlab-ci.yml.j2
+-rw-r--r--   0        0        0     2259 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/CMakeLists.txt.j2
+-rw-r--r--   0        0        0     9664 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/README.md.j2
+-rw-r--r--   0        0        0     3578 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/conan/conanfile.py.j2
+-rw-r--r--   0        0        0     1534 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/conan/conanfiletest.j2
+-rw-r--r--   0        0        0      890 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/conan/profile_atsam.j2
+-rw-r--r--   0        0        0      739 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/conan/profile_esp32.j2
+-rw-r--r--   0        0        0      905 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/conan/profile_stm32.j2
+-rw-r--r--   0        0        0      885 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/conan/profile_x86.j2
+-rw-r--r--   0        0        0      342 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/conan/test_package/CMakeLists.txt.j2
+-rw-r--r--   0        0        0      749 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/conan/test_package/conanfile.py.j2
+-rw-r--r--   0        0        0      118 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/conan/test_package/example.cpp.j2
+-rw-r--r--   0        0        0     2902 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/conan/toolchain/arm_gcc_toolchain.cmake.j2
+-rw-r--r--   0        0        0      469 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/conan/toolchain/stm32_gcc_toolchain.cmake.j2
+-rw-r--r--   0        0        0     2183 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/cpp/cmake-src-atsam.j2
+-rw-r--r--   0        0        0      150 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
+-rw-r--r--   0        0        0       71 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/cpp/cmake-src-multitarget.j2
+-rw-r--r--   0        0        0     2907 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
+-rw-r--r--   0        0        0      796 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2
+-rw-r--r--   0        0        0      240 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/cpp/lib.cpp.j2
+-rw-r--r--   0        0        0      272 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/cpp/lib.h.j2
+-rw-r--r--   0        0        0     1063 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/cpp/main.cpp.j2
+-rw-r--r--   0        0        0      782 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/docker/Dockerfile-arm.j2
+-rw-r--r--   0        0        0      613 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2
+-rw-r--r--   0        0        0     1609 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
+-rw-r--r--   0        0        0     2634 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/docker/Dockerfile.j2
+-rw-r--r--   0        0        0      149 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/docker/atsam-gdb.script.j2
+-rw-r--r--   0        0        0      123 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/docker/atsam-openocd.cfg.j2
+-rw-r--r--   0        0        0     1120 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/docker/devcontainer.json.j2
+-rw-r--r--   0        0        0      993 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2
+-rw-r--r--   0        0        0      287 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/docker/env.txt.j2
+-rw-r--r--   0        0        0       93 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/docker/stm32-openocd.cfg.j2
+-rw-r--r--   0        0        0       39 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/mock/.clang-format
+-rw-r--r--   0        0        0      475 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/mock/CMakeLists.txt
+-rw-r--r--   0        0        0      594 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/mock/class_interface.h.j2
+-rw-r--r--   0        0        0      835 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/mock/class_mock.cpp.j2
+-rw-r--r--   0        0        0      697 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/mock/class_mock.h.j2
+-rw-r--r--   0        0        0     2979 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/scargo.toml.j2
+-rw-r--r--   0        0        0       91 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
+-rw-r--r--   0        0        0      100 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
+-rw-r--r--   0        0        0     1140 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
+-rw-r--r--   0        0        0       84 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
+-rw-r--r--   0        0        0      326 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
+-rw-r--r--   0        0        0     1046 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/tests/static_mock/static_mock.h
+-rw-r--r--   0        0        0       39 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/ut/.clang-format
+-rw-r--r--   0        0        0      575 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2
+-rw-r--r--   0        0        0      716 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/ut/ut.cpp.j2
+-rw-r--r--   0        0        0      565 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/vscode/launch.json.j2
+-rw-r--r--   0        0        0     1040 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/templates/vscode/tasks.json.j2
+-rw-r--r--   0        0        0     1492 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/tests_gen.py
+-rw-r--r--   0        0        0      550 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/toml_gen.py
+-rw-r--r--   0        0        0     5357 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/ut_gen.py
+-rw-r--r--   0        0        0     1789 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/file_generators/vscode_gen.py
+-rw-r--r--   0        0        0      629 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/global_values.py
+-rw-r--r--   0        0        0     2138 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/logger.py
+-rw-r--r--   0        0        0        0 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/target_helpers/__init__.py
+-rw-r--r--   0        0        0    40877 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/target_helpers/atmel.xml
+-rw-r--r--   0        0        0     3057 2024-04-11 09:14:40.228261 scargo-2.3.0/scargo/target_helpers/atsam_helper.py
+-rw-r--r--   0        0        0     3049 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/target_helpers/esp32_helper.py
+-rw-r--r--   0        0        0      982 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/target_helpers/stm32_helper.py
+-rw-r--r--   0        0        0     2953 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/templates/.clang-format
+-rw-r--r--   0        0        0     8780 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/templates/.clang-tidy
+-rw-r--r--   0        0        0     2362 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/templates/.gitignore
+-rw-r--r--   0        0        0     1066 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/templates/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/utils/__init__.py
+-rw-r--r--   0        0        0      698 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/utils/clang_utils.py
+-rw-r--r--   0        0        0     2396 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/utils/conan_utils.py
+-rw-r--r--   0        0        0     2388 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/utils/docker_utils.py
+-rw-r--r--   0        0        0     2800 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/utils/file_utils.py
+-rw-r--r--   0        0        0      778 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/utils/path_utils.py
+-rw-r--r--   0        0        0      596 2024-04-11 09:14:40.232261 scargo-2.3.0/scargo/utils/sys_utils.py
+-rw-r--r--   0        0        0      573 2024-04-11 09:14:40.232261 scargo-2.3.0/setup.cfg
+-rw-r--r--   0        0        0     6729 1970-01-01 00:00:00.000000 scargo-2.3.0/PKG-INFO
```

### Comparing `scargo-2.2.0/CODE-OF-CONDUCT.md` & `scargo-2.3.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/LICENSE` & `scargo-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/README.md` & `scargo-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/pyproject.toml` & `scargo-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/certs/certGen.sh` & `scargo-2.3.0/scargo/certs/certGen.sh`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/certs/generateAllCertificates.sh` & `scargo-2.3.0/scargo/certs/generateAllCertificates.sh`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/certs/openssl_device_intermediate_ca.cnf` & `scargo-2.3.0/scargo/certs/openssl_device_intermediate_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/certs/openssl_root_ca.cnf` & `scargo-2.3.0/scargo/certs/openssl_root_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/cli.py` & `scargo-2.3.0/scargo/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     scargo_docker_build,
     scargo_docker_exec,
     scargo_docker_run,
 )
 from scargo.commands.fix import scargo_fix
 from scargo.commands.flash import scargo_flash
 from scargo.commands.gen import scargo_gen
+from scargo.commands.monitor import scargo_monitor
 from scargo.commands.new import scargo_new
 from scargo.commands.publish import scargo_publish
 from scargo.commands.run import scargo_run
 from scargo.commands.test import scargo_test
 from scargo.commands.update import scargo_update
 from scargo.commands.version import scargo_version
 from scargo.config import ScargoTarget
@@ -247,26 +248,55 @@
         "-t",
         "--target",
         help="Target device. Defaults to first one from toml if not specified.",
     ),
     app: bool = Option(False, "--app", help="Flash app only"),
     file_system: bool = Option(False, "--fs", help="Flash filesystem only"),
     no_erase: bool = Option(False, help="(stm32 only) Don't erase target memory"),
+    bank: Optional[int] = Option(
+        None,
+        "--bank",
+        help="(esp32 only) Provide app flasg bank number for chosen target e.g. --bank 0",
+    ),
     base_dir: Optional[Path] = BASE_DIR_OPTION,
 ) -> None:
     """Flash the target."""
     if base_dir:
         os.chdir(base_dir)
-    scargo_flash(flash_profile, port, target, app, file_system, not no_erase)
+    scargo_flash(flash_profile, port, target, app, file_system, not no_erase, bank)
 
 
 ###############################################################################
 
 
 @cli.command()
+def monitor(
+    port: Optional[str] = Option(
+        None,
+        "-p",
+        "--port",
+        help="port where the serial monitor will be run"
+        " connected to, e.g. /dev/ttyUSB0",
+    ),
+    baudrate: Optional[int] = Option(
+        None,
+        "-b",
+        "--baudrate",
+        help="baudrate, default is 115200",
+    ),
+    base_dir: Optional[Path] = BASE_DIR_OPTION,
+) -> None:
+    """Monitor the target over serial port"""
+    if base_dir:
+        os.chdir(base_dir)
+    scargo_monitor(port, baudrate)
+
+
+###############################################################################
+@cli.command()
 def gen(
     profile: str = Option("Debug", "--profile", "-p"),
     gen_ut: Optional[Path] = Option(
         None,
         "--unit-test",
         "-u",
         exists=True,
```

### Comparing `scargo-2.2.0/scargo/commands/build.py` & `scargo-2.3.0/scargo/commands/build.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/commands/check.py` & `scargo-2.3.0/scargo/commands/check.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/commands/clean.py` & `scargo-2.3.0/scargo/commands/clean.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/commands/debug.py` & `scargo-2.3.0/scargo/commands/debug.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/commands/doc.py` & `scargo-2.3.0/scargo/commands/doc.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/commands/docker.py` & `scargo-2.3.0/scargo/commands/docker.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/commands/fix.py` & `scargo-2.3.0/scargo/commands/fix.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/commands/flash.py` & `scargo-2.3.0/scargo/commands/flash.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,20 +35,22 @@
         self,
         flash_profile: str,
         port: Optional[str],
         target: Optional[ScargoTarget],
         app: bool,
         file_system: bool,
         erase_memory: bool,
+        bank: Optional[int],
     ):
         self._flash_profile = flash_profile
         self._port = port
         self._app = app
         self._file_system = file_system
         self._erase_memory = erase_memory
+        self._bank = bank
 
         self._config = prepare_config()
         self._target = self._initialize_target(target)
         self._validate_target()
         self._validate_erase_memory()
 
     def _initialize_target(self, target: Optional[ScargoTarget]) -> Target:
@@ -133,14 +135,18 @@
         try:
             if self._app:
                 self._flash_esp32_app()
             elif self._file_system:
                 self._flash_esp32_fs()
             else:
                 self._flash_esp32_default()
+
+            if self._bank is not None:
+                self._switch_bank_esp32()
+
         except subprocess.CalledProcessError as e:
             logger.error("Failed to flash esp32 target: %s", e.stderr)
             sys.exit(1)
 
     def _flash_stm32(self) -> None:
         bin_path, elf_path = self._get_binary_and_elf_paths()
         self._check_bin_path(elf_path)
@@ -219,18 +225,32 @@
             command.extend(["--chip", chip])
 
         if partition_name:
             command.extend(["write_partition", f"--partition-name={partition_name}"])
         command.extend(extra_args)
         return command
 
+    def _switch_bank_esp32(self) -> None:
+        command = ["otatool.py", "switch_ota_partition", "--slot", str(self._bank)]
+
+        try:
+            logger.info("Bank switching to: [%d]", self._bank)
+            subprocess.run(command, cwd=self._config.project_root, check=True)
+        except subprocess.CalledProcessError as e:
+            logger.error("Command failed with return code %s", str(e.returncode))
+        except Exception as e:  # pylint: disable=broad-except
+            logger.error("An error occurred: %s", str(e))
+
 
 def scargo_flash(
     flash_profile: str,
     port: Optional[str],
     target: Optional[ScargoTarget],
     app: bool,
     file_system: bool,
     erase_memory: bool,
+    bank: Optional[int] = None,
 ) -> None:
-    flasher = _ScargoFlash(flash_profile, port, target, app, file_system, erase_memory)
+    flasher = _ScargoFlash(
+        flash_profile, port, target, app, file_system, erase_memory, bank
+    )
     flasher.flash_target()
```

### Comparing `scargo-2.2.0/scargo/commands/gen.py` & `scargo-2.3.0/scargo/commands/gen.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/commands/new.py` & `scargo-2.3.0/scargo/commands/new.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/commands/publish.py` & `scargo-2.3.0/scargo/commands/publish.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/commands/run.py` & `scargo-2.3.0/scargo/commands/run.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/commands/test.py` & `scargo-2.3.0/scargo/commands/test.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/commands/update.py` & `scargo-2.3.0/scargo/commands/update.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/config.py` & `scargo-2.3.0/scargo/config.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/config_utils.py` & `scargo-2.3.0/scargo/config_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/base_gen.py` & `scargo-2.3.0/scargo/file_generators/base_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/cicd_gen.py` & `scargo-2.3.0/scargo/file_generators/cicd_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/clang_parser/data_classes.py` & `scargo-2.3.0/scargo/file_generators/clang_parser/data_classes.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/clang_parser/header_parser.py` & `scargo-2.3.0/scargo/file_generators/clang_parser/header_parser.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/clang_parser/params_extractor.py` & `scargo-2.3.0/scargo/file_generators/clang_parser/params_extractor.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/conan_gen.py` & `scargo-2.3.0/scargo/file_generators/conan_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/cpp_gen.py` & `scargo-2.3.0/scargo/file_generators/cpp_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/docker_gen.py` & `scargo-2.3.0/scargo/file_generators/docker_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/env_gen.py` & `scargo-2.3.0/scargo/file_generators/env_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/mock_gen.py` & `scargo-2.3.0/scargo/file_generators/mock_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/.gitlab-ci.yml.j2` & `scargo-2.3.0/scargo/file_generators/templates/.gitlab-ci.yml.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/CMakeLists.txt.j2` & `scargo-2.3.0/scargo/file_generators/templates/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/README.md.j2` & `scargo-2.3.0/scargo/file_generators/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/conan/conanfile.py.j2` & `scargo-2.3.0/scargo/file_generators/templates/conan/conanfile.py.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/conan/conanfiletest.j2` & `scargo-2.3.0/scargo/file_generators/templates/conan/conanfiletest.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/conan/profile_atsam.j2` & `scargo-2.3.0/scargo/file_generators/templates/conan/profile_atsam.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/conan/profile_esp32.j2` & `scargo-2.3.0/scargo/file_generators/templates/conan/profile_esp32.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/conan/profile_stm32.j2` & `scargo-2.3.0/scargo/file_generators/templates/conan/profile_stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/conan/profile_x86.j2` & `scargo-2.3.0/scargo/file_generators/templates/conan/profile_x86.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/conan/test_package/conanfile.py.j2` & `scargo-2.3.0/scargo/file_generators/templates/conan/test_package/conanfile.py.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/conan/toolchain/arm_gcc_toolchain.cmake.j2` & `scargo-2.3.0/scargo/file_generators/templates/conan/toolchain/arm_gcc_toolchain.cmake.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/cpp/cmake-src-atsam.j2` & `scargo-2.3.0/scargo/file_generators/templates/cpp/cmake-src-atsam.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2` & `scargo-2.3.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2` & `scargo-2.3.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/cpp/main.cpp.j2` & `scargo-2.3.0/scargo/file_generators/templates/cpp/main.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/docker/Dockerfile-arm.j2` & `scargo-2.3.0/scargo/file_generators/templates/docker/Dockerfile-arm.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2` & `scargo-2.3.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2` & `scargo-2.3.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/docker/Dockerfile.j2` & `scargo-2.3.0/scargo/file_generators/templates/docker/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/docker/devcontainer.json.j2` & `scargo-2.3.0/scargo/file_generators/templates/docker/devcontainer.json.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2` & `scargo-2.3.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/mock/class_interface.h.j2` & `scargo-2.3.0/scargo/file_generators/templates/mock/class_interface.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/mock/class_mock.cpp.j2` & `scargo-2.3.0/scargo/file_generators/templates/mock/class_mock.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/mock/class_mock.h.j2` & `scargo-2.3.0/scargo/file_generators/templates/mock/class_mock.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/scargo.toml.j2` & `scargo-2.3.0/scargo/file_generators/templates/scargo.toml.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2` & `scargo-2.3.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/tests/static_mock/static_mock.h` & `scargo-2.3.0/scargo/file_generators/templates/tests/static_mock/static_mock.h`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2` & `scargo-2.3.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/ut/ut.cpp.j2` & `scargo-2.3.0/scargo/file_generators/templates/ut/ut.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/vscode/launch.json.j2` & `scargo-2.3.0/scargo/file_generators/templates/vscode/launch.json.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/templates/vscode/tasks.json.j2` & `scargo-2.3.0/scargo/file_generators/templates/vscode/tasks.json.j2`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/tests_gen.py` & `scargo-2.3.0/scargo/file_generators/tests_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/toml_gen.py` & `scargo-2.3.0/scargo/file_generators/toml_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/ut_gen.py` & `scargo-2.3.0/scargo/file_generators/ut_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/file_generators/vscode_gen.py` & `scargo-2.3.0/scargo/file_generators/vscode_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/global_values.py` & `scargo-2.3.0/scargo/global_values.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/logger.py` & `scargo-2.3.0/scargo/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,19 +19,19 @@
         lock_file = get_config_file_path(SCARGO_LOCK_FILE)
         if not lock_file:
             return console_log_level, file_log_level
         config = parse_config(lock_file)
         scargo_config = config.scargo
         console_log_level = logging.getLevelName(scargo_config.console_log_level)
         file_log_level = logging.getLevelName(scargo_config.file_log_level)
-    finally:
-        return (  # pylint: disable=[lost-exception,return-in-finally]
-            console_log_level,
-            file_log_level,
-        )
+    except Exception:  # pylint: disable=broad-except
+        console_log_level = logging.INFO
+        file_log_level = logging.WARNING
+
+    return (console_log_level, file_log_level)
 
 
 def get_logger(name: str = "scargo") -> logging.Logger:
     if logging.getLogger(name).handlers:
         return logging.getLogger(name)
 
     console_log_level, file_log_level = __get_logging_config()
```

### Comparing `scargo-2.2.0/scargo/target_helpers/atmel.xml` & `scargo-2.3.0/scargo/target_helpers/atmel.xml`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/target_helpers/atsam_helper.py` & `scargo-2.3.0/scargo/target_helpers/atsam_helper.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/target_helpers/esp32_helper.py` & `scargo-2.3.0/scargo/target_helpers/esp32_helper.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/target_helpers/stm32_helper.py` & `scargo-2.3.0/scargo/target_helpers/stm32_helper.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/templates/.clang-format` & `scargo-2.3.0/scargo/templates/.clang-format`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/templates/.clang-tidy` & `scargo-2.3.0/scargo/templates/.clang-tidy`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/templates/.gitignore` & `scargo-2.3.0/scargo/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/templates/LICENSE` & `scargo-2.3.0/scargo/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/utils/clang_utils.py` & `scargo-2.3.0/scargo/utils/clang_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/utils/conan_utils.py` & `scargo-2.3.0/scargo/utils/conan_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/utils/docker_utils.py` & `scargo-2.3.0/scargo/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/utils/file_utils.py` & `scargo-2.3.0/scargo/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/utils/path_utils.py` & `scargo-2.3.0/scargo/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/scargo/utils/sys_utils.py` & `scargo-2.3.0/scargo/utils/sys_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/setup.cfg` & `scargo-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scargo-2.2.0/PKG-INFO` & `scargo-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scargo
-Version: 2.2.0
+Version: 2.3.0
 Summary: C/C++ package and software development life cycle manager inspired by RUST cargo idea.
 Keywords: scargo,Package manager,C++
 Author-email: "Spyrosoft Solutions S.A." <aak@spyro-soft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

