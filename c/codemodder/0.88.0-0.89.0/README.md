# Comparing `tmp/codemodder-0.88.0.tar.gz` & `tmp/codemodder-0.89.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codemodder-0.88.0.tar", last modified: Thu Apr  4 17:49:16 2024, max compression
+gzip compressed data, was "codemodder-0.89.0.tar", last modified: Thu Apr 11 13:38:08 2024, max compression
```

## Comparing `codemodder-0.88.0.tar` & `codemodder-0.89.0.tar`

### file list

```diff
@@ -1,485 +1,501 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.993865 codemodder-0.88.0/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-04 17:49:07.000000 codemodder-0.88.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.913864 codemodder-0.88.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/pixeebot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.917865 codemodder-0.88.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/autoformat-pixeebot-prs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/codemod_pygoat.yml
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/deploy_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/integration_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/pre-commit-autoupdate.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/sonar_pixee.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-04 17:49:07.000000 codemodder-0.88.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-04 17:49:07.000000 codemodder-0.88.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 17:49:07.000000 codemodder-0.88.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 17:49:07.000000 codemodder-0.88.0/.semgrepignore
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 17:49:07.000000 codemodder-0.88.0/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-04 17:49:07.000000 codemodder-0.88.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-04 17:49:07.000000 codemodder-0.88.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 17:49:07.000000 codemodder-0.88.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-04 17:49:07.000000 codemodder-0.88.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-04 17:49:07.000000 codemodder-0.88.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-04 17:49:07.000000 codemodder-0.88.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    44628 2024-04-04 17:49:16.993865 codemodder-0.88.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-04 17:49:07.000000 codemodder-0.88.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.917865 codemodder-0.88.0/ci_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-04 17:49:07.000000 codemodder-0.88.0/ci_tests/test_pygoat_findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 17:49:07.000000 codemodder-0.88.0/codecov.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.917865 codemodder-0.88.0/img/
--rw-r--r--   0 runner    (1001) docker     (127)    41511 2024-04-04 17:49:07.000000 codemodder-0.88.0/img/base-codemod.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-04 17:49:07.000000 codemodder-0.88.0/img/codemodder-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-04 17:49:07.000000 codemodder-0.88.0/img/codemodder-light.png
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-04 17:49:07.000000 codemodder-0.88.0/img/codemodder.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.929865 codemodder-0.88.0/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_add_requests_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_combine_startswith_endswith.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_django_session_cookie_secure_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_fix_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_lxml_safe_parser_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_multiple_codemods.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_process_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_request_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sonar_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_str_concat_in_seq_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_use_defusedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_use_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-04 17:49:07.000000 codemodder-0.88.0/integration_tests/test_with_threading_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-04 17:49:07.000000 codemodder-0.88.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-04 17:49:07.000000 codemodder-0.88.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 17:49:16.993865 codemodder-0.88.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.909865 codemodder-0.88.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.933865 codemodder-0.88.0/src/codemodder/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/code_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemodder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.937865 codemodder-0.88.0/src/codemodder/codemods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/base_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/base_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/base_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/check_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/import_modifier_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/imported_call_modifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/libcst_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/semgrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/sonar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.937865 codemodder-0.88.0/src/codemodder/codemods/test/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13148 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/test/integration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/test/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.937865 codemodder-0.88.0/src/codemodder/codemods/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/transformations/clean_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/transformations/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23555 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codemods/utils_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/codetf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.941865 codemodder-0.88.0/src/codemodder/dependency_management/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/base_dependency_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/codemod_dependencies.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/pyproject_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/requirements_txt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/setup_py_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/dependency_management/setupcfg_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/file_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.941865 codemodder-0.88.0/src/codemodder/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.941865 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/package_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/project_analysis/python_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/sarifs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.941865 codemodder-0.88.0/src/codemodder/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21045 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/scripts/generate_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/scripts/get_hashes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/semgrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/sonar_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.941865 codemodder-0.88.0/src/codemodder/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/utils/abc_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/utils/clean_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/utils/format_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/utils/linearize_string_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/codemodder/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.989865 codemodder-0.88.0/src/codemodder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44628 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 17:49:16.000000 codemodder-0.88.0/src/codemodder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.953865 codemodder-0.88.0/src/core_codemods/
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/add_requests_timeouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.953865 codemodder-0.88.0/src/core_codemods/api/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/api/core_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/combine_startswith_endswith.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.953865 codemodder-0.88.0/src/core_codemods/defectdojo/
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/defectdojo/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/defectdojo/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.953865 codemodder-0.88.0/src/core_codemods/defectdojo/semgrep/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/django_session_cookie_secure_off.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.965865 codemodder-0.88.0/src/core_codemods/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-debug-flag-on.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-json-response-type.md
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-session-cookie-secure-off.md
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_exception-without-raise.md
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-assert-tuple.md
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-async-task-instantiation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-hasattr-call.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-missing-self-or-cls.md
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_harden-ruamel.md
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_https-connection.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_lazy-logging.md
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_limit-readline.md
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_literal-or-new-object-identity.md
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_numpy-nan-equality.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-debug-breakpoint.md
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-future-imports.md
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-module-global.md
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-unnecessary-f-str.md
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_requests-verify.md
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-random.md
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-tempfile.md
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_sql-parameterization.md
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_str-concat-in-sequence-literals.md
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_unused-imports.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_url-sandbox.md
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-defusedxml.md
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-generator.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-set-literal.md
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-walrus-if.md
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_async_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/lxml_safe_parser_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/process_creation_sandbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.965865 codemodder-0.88.0/src/core_codemods/refactor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/refactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/refactor/refactor_new_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/remove_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/requests_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/secure_cookie_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/secure_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.969865 codemodder-0.88.0/src/core_codemods/sonar/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sonar/sonar_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)    22977 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/str_concat_in_seq_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/use_defused_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/use_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-04 17:49:07.000000 codemodder-0.88.0/src/core_codemods/with_threading_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.969865 codemodder-0.88.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.985865 codemodder-0.88.0/tests/codemods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:07.000000 codemodder-0.88.0/tests/codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.909865 codemodder-0.88.0/tests/codemods/defectdojo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.985865 codemodder-0.88.0/tests/codemods/defectdojo/semgrep/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_add_requests_timeouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_async_fix_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_base_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_base_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_combine_startswith_endswith.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_django_session_cookie_secure_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_include_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)    23091 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_lxml_safe_parameter_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_process_creation_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_remove_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_request_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sonar_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_str_concat_in_seq_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_use_defused_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/codemods/test_with_threading_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.985865 codemodder-0.88.0/tests/dependency_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/test_base_dependency_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/test_dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/test_pyproject_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/test_requirements_txt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/test_setup_py_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/dependency_management/test_setupcfgt_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.985865 codemodder-0.88.0/tests/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.985865 codemodder-0.88.0/tests/project_analysis/file_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/file_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/project_analysis/test_python_repo_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.989865 codemodder-0.88.0/tests/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/make_request.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/multiple_codemods.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/semgrep.sarif
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/sonar_hotspots.json
--rw-r--r--   0 runner    (1001) docker     (127)    77614 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/sonar_issues.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)   451117 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/samples/webgoat_v8.2.0_codeql.sarif
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_ancestorpatterns_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_basetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_code_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_codemod_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_codemodder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_codetf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_file_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_format_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_linearize_string_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_nameresolution_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_sarif_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:16.989865 codemodder-0.88.0/tests/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/transformations/test_clean_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/transformations/test_remove_empty_string_concatenation.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-04 17:49:08.000000 codemodder-0.88.0/tests/transformations/test_remove_unused_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.978706 codemodder-0.89.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-11 13:37:58.000000 codemodder-0.89.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.890705 codemodder-0.89.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-11 13:37:58.000000 codemodder-0.89.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-11 13:37:58.000000 codemodder-0.89.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 13:37:58.000000 codemodder-0.89.0/.github/pixeebot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-11 13:37:58.000000 codemodder-0.89.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.890705 codemodder-0.89.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-11 13:37:58.000000 codemodder-0.89.0/.github/workflows/autoformat-pixeebot-prs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-11 13:37:58.000000 codemodder-0.89.0/.github/workflows/codemod_pygoat.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 13:37:58.000000 codemodder-0.89.0/.github/workflows/deploy_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-11 13:37:58.000000 codemodder-0.89.0/.github/workflows/integration_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 13:37:58.000000 codemodder-0.89.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-11 13:37:58.000000 codemodder-0.89.0/.github/workflows/pre-commit-autoupdate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-11 13:37:58.000000 codemodder-0.89.0/.github/workflows/sonar_pixee.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-11 13:37:58.000000 codemodder-0.89.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-11 13:37:58.000000 codemodder-0.89.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-11 13:37:58.000000 codemodder-0.89.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-11 13:37:58.000000 codemodder-0.89.0/.semgrepignore
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 13:37:58.000000 codemodder-0.89.0/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-11 13:37:58.000000 codemodder-0.89.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-11 13:37:58.000000 codemodder-0.89.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-11 13:37:58.000000 codemodder-0.89.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 13:37:58.000000 codemodder-0.89.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-11 13:37:58.000000 codemodder-0.89.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-11 13:37:58.000000 codemodder-0.89.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    44628 2024-04-11 13:38:08.978706 codemodder-0.89.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-11 13:37:58.000000 codemodder-0.89.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.890705 codemodder-0.89.0/ci_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-11 13:37:58.000000 codemodder-0.89.0/ci_tests/test_pygoat_findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-11 13:37:58.000000 codemodder-0.89.0/codecov.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.890705 codemodder-0.89.0/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    41511 2024-04-11 13:37:58.000000 codemodder-0.89.0/img/base-codemod.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-11 13:37:58.000000 codemodder-0.89.0/img/codemodder-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-11 13:37:58.000000 codemodder-0.89.0/img/codemodder-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-11 13:37:58.000000 codemodder-0.89.0/img/codemodder.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.902705 codemodder-0.89.0/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.906705 codemodder-0.89.0/integration_tests/sonar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/sonar/test_sonar_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_add_requests_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_combine_startswith_endswith.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_django_session_cookie_secure_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_fix_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_lxml_safe_parser_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_multiple_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_process_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_request_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_str_concat_in_seq_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_use_defusedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_use_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-11 13:37:58.000000 codemodder-0.89.0/integration_tests/test_with_threading_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-11 13:37:58.000000 codemodder-0.89.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-11 13:37:58.000000 codemodder-0.89.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:38:08.978706 codemodder-0.89.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.882705 codemodder-0.89.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.906705 codemodder-0.89.0/src/codemodder/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-11 13:38:08.000000 codemodder-0.89.0/src/codemodder/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/code_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemodder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.910705 codemodder-0.89.0/src/codemodder/codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/base_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/base_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/base_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/check_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/import_modifier_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/imported_call_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/libcst_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/semgrep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.910705 codemodder-0.89.0/src/codemodder/codemods/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13137 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/test/integration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/test/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.914706 codemodder-0.89.0/src/codemodder/codemods/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/transformations/clean_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/transformations/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23555 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codemods/utils_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/codetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.914706 codemodder-0.89.0/src/codemodder/dependency_management/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/dependency_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/dependency_management/base_dependency_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/dependency_management/codemod_dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/dependency_management/dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/dependency_management/pyproject_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/dependency_management/requirements_txt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/dependency_management/setup_py_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/dependency_management/setupcfg_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/file_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.914706 codemodder-0.89.0/src/codemodder/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.914706 codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/package_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/project_analysis/python_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/sarifs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.918706 codemodder-0.89.0/src/codemodder/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19005 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/scripts/generate_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/scripts/get_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/semgrep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.918706 codemodder-0.89.0/src/codemodder/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/utils/abc_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/utils/clean_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/utils/format_string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/utils/linearize_string_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/codemodder/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.974707 codemodder-0.89.0/src/codemodder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44628 2024-04-11 13:38:08.000000 codemodder-0.89.0/src/codemodder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21130 2024-04-11 13:38:08.000000 codemodder-0.89.0/src/codemodder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:38:08.000000 codemodder-0.89.0/src/codemodder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-11 13:38:08.000000 codemodder-0.89.0/src/codemodder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-11 13:38:08.000000 codemodder-0.89.0/src/codemodder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-11 13:38:08.000000 codemodder-0.89.0/src/codemodder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.930706 codemodder-0.89.0/src/core_codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/add_requests_timeouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.930706 codemodder-0.89.0/src/core_codemods/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/api/core_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/combine_startswith_endswith.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.930706 codemodder-0.89.0/src/core_codemods/defectdojo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/defectdojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/defectdojo/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.930706 codemodder-0.89.0/src/core_codemods/defectdojo/semgrep/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/django_session_cookie_secure_off.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.942706 codemodder-0.89.0/src/core_codemods/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_django-debug-flag-on.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_django-json-response-type.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_django-session-cookie-secure-off.md
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_exception-without-raise.md
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-assert-tuple.md
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-async-task-instantiation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-float-equality.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-hasattr-call.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-missing-self-or-cls.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_harden-ruamel.md
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_https-connection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_lazy-logging.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_limit-readline.md
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_literal-or-new-object-identity.md
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_numpy-nan-equality.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_remove-debug-breakpoint.md
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_remove-future-imports.md
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_remove-module-global.md
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_remove-unnecessary-f-str.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_requests-verify.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_secure-random.md
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_secure-tempfile.md
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_sql-parameterization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_str-concat-in-sequence-literals.md
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_unused-imports.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_url-sandbox.md
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_use-defusedxml.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_use-generator.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_use-set-literal.md
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/docs/pixee_python_use-walrus-if.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/fix_async_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/lxml_safe_parser_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/process_creation_sandbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.942706 codemodder-0.89.0/src/core_codemods/refactor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/refactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/refactor/refactor_new_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/remove_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/requests_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/secure_cookie_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/secure_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.942706 codemodder-0.89.0/src/core_codemods/sonar/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sonar/sonar_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22977 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/str_concat_in_seq_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/use_defused_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/use_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-11 13:37:58.000000 codemodder-0.89.0/src/core_codemods/with_threading_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.946706 codemodder-0.89.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.958706 codemodder-0.89.0/tests/codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.882705 codemodder-0.89.0/tests/codemods/defectdojo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.958706 codemodder-0.89.0/tests/codemods/defectdojo/semgrep/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.962706 codemodder-0.89.0/tests/codemods/sonar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/sonar/test_sonar_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_add_requests_timeouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_async_fix_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_base_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_base_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_combine_startswith_endswith.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_django_session_cookie_secure_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_include_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23091 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_lxml_safe_parameter_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_process_creation_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_remove_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_request_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_str_concat_in_seq_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_use_defused_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/codemods/test_with_threading_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.962706 codemodder-0.89.0/tests/dependency_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/dependency_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/dependency_management/test_base_dependency_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/dependency_management/test_dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/dependency_management/test_pyproject_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/dependency_management/test_requirements_txt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/dependency_management/test_setup_py_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/dependency_management/test_setupcfgt_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.962706 codemodder-0.89.0/tests/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.966706 codemodder-0.89.0/tests/project_analysis/file_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/project_analysis/file_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/project_analysis/test_python_repo_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.974707 codemodder-0.89.0/tests/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/flask_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/make_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/multiple_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2680067 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/pygoat.semgrep.sarif.json
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/semgrep.sarif
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/sonar_hotspots.json
+-rw-r--r--   0 runner    (1001) docker     (127)    80805 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/sonar_issues.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   451117 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/samples/webgoat_v8.2.0_codeql.sarif
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_ancestorpatterns_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_basetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_code_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_codemod_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_codemodder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_codetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_file_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_format_string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_linearize_string_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_nameresolution_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_sarif_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:38:08.974707 codemodder-0.89.0/tests/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/transformations/test_clean_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/transformations/test_remove_empty_string_concatenation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-11 13:37:58.000000 codemodder-0.89.0/tests/transformations/test_remove_unused_imports.py
```

### Comparing `codemodder-0.88.0/.github/workflows/autoformat-pixeebot-prs.yaml` & `codemodder-0.89.0/.github/workflows/autoformat-pixeebot-prs.yaml`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/.github/workflows/codemod_pygoat.yml` & `codemodder-0.89.0/.github/workflows/codemod_pygoat.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/.github/workflows/deploy_to_pypi.yml` & `codemodder-0.89.0/.github/workflows/deploy_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/.github/workflows/integration_test.yml` & `codemodder-0.89.0/.github/workflows/integration_test.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/.github/workflows/lint.yml` & `codemodder-0.89.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/.github/workflows/pre-commit-autoupdate.yml` & `codemodder-0.89.0/.github/workflows/pre-commit-autoupdate.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/.github/workflows/sonar_pixee.yml` & `codemodder-0.89.0/.github/workflows/sonar_pixee.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/.github/workflows/test.yml` & `codemodder-0.89.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/.gitignore` & `codemodder-0.89.0/.gitignore`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/.pre-commit-config.yaml` & `codemodder-0.89.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: check-yaml
     -   id: check-json
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
         exclude: |
           (?x)^(
               src/core_codemods/docs/.*|
               src/codemodder/dependency.py |
               integration_tests/.*|
               tests/.*
           )$
     -   id: check-added-large-files
+        exclude: |
+          (?x)^(
+              tests/samples/pygoat.semgrep.sarif.json
+          )$
 -   repo: https://github.com/psf/black
     rev: 24.3.0
     hooks:
     -   id: black
         exclude: |
           (?x)^(
               tests/samples/.*|
```

### Comparing `codemodder-0.88.0/CHANGELOG.md` & `codemodder-0.89.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/CONTRIBUTING.md` & `codemodder-0.89.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/LICENSE` & `codemodder-0.89.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/Makefile` & `codemodder-0.89.0/Makefile`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/PKG-INFO` & `codemodder-0.89.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codemodder
-Version: 0.88.0
+Version: 0.89.0
 Summary: A pluggable framework for building codemods in Python
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,15 +683,15 @@
 Requires-Dist: isort<5.14,>=5.12
 Requires-Dist: libcst<1.4,>=1.1
 Requires-Dist: packaging<25.0,>=23.2
 Requires-Dist: pydantic~=2.6.0
 Requires-Dist: pylint<3.2,>=3.0
 Requires-Dist: python-json-logger~=2.0.0
 Requires-Dist: PyYAML~=6.0.0
-Requires-Dist: semgrep<1.68,>=1.50
+Requires-Dist: semgrep<1.69,>=1.50
 Requires-Dist: toml~=0.10.2
 Requires-Dist: tomlkit~=0.12.0
 Requires-Dist: wrapt~=1.16.0
 Requires-Dist: chardet~=5.2.0
 Provides-Extra: test
 Requires-Dist: coverage<7.5,>=7.3; extra == "test"
 Requires-Dist: Flask<4; extra == "test"
```

### Comparing `codemodder-0.88.0/README.md` & `codemodder-0.89.0/README.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/ci_tests/test_pygoat_findings.py` & `codemodder-0.89.0/ci_tests/test_pygoat_findings.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/img/base-codemod.jpg` & `codemodder-0.89.0/img/base-codemod.jpg`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/img/codemodder-dark.png` & `codemodder-0.89.0/img/codemodder-dark.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/img/codemodder-light.png` & `codemodder-0.89.0/img/codemodder-light.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/img/codemodder.png` & `codemodder-0.89.0/img/codemodder.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_add_requests_timeout.py` & `codemodder-0.89.0/integration_tests/test_add_requests_timeout.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_combine_startswith_endswith.py` & `codemodder-0.89.0/integration_tests/test_combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_dependency_manager.py` & `codemodder-0.89.0/integration_tests/test_dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_django_debug_flag_on.py` & `codemodder-0.89.0/integration_tests/test_django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_django_json_response_type.py` & `codemodder-0.89.0/integration_tests/test_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_django_model_without_dunder_str.py` & `codemodder-0.89.0/integration_tests/test_django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_django_receiver_on_top.py` & `codemodder-0.89.0/integration_tests/test_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_django_session_cookie_secure_off.py` & `codemodder-0.89.0/integration_tests/test_django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_exception_without_raise.py` & `codemodder-0.89.0/integration_tests/test_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_file_resource_leak.py` & `codemodder-0.89.0/integration_tests/test_file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_fix_assert_tuple.py` & `codemodder-0.89.0/integration_tests/test_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_fix_dataclass_defaults.py` & `codemodder-0.89.0/integration_tests/test_fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_fix_deprecated_abstractproperty.py` & `codemodder-0.89.0/integration_tests/test_fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_fix_deprecated_logging_warn.py` & `codemodder-0.89.0/integration_tests/test_fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_fix_empty_sequence_comparison.py` & `codemodder-0.89.0/integration_tests/test_fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_fix_hasattr_call.py` & `codemodder-0.89.0/integration_tests/test_fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_fix_missing_self_or_cls.py` & `codemodder-0.89.0/integration_tests/test_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_fix_mutable_params.py` & `codemodder-0.89.0/integration_tests/test_fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_fix_task_instantiation.py` & `codemodder-0.89.0/integration_tests/test_fix_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_flask_enable_csrf_protection.py` & `codemodder-0.89.0/integration_tests/test_flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_flask_json_response_type.py` & `codemodder-0.89.0/integration_tests/test_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_harden_pickle_load.py` & `codemodder-0.89.0/integration_tests/test_harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_harden_pyyaml.py` & `codemodder-0.89.0/integration_tests/test_harden_pyyaml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_harden_ruamel.py` & `codemodder-0.89.0/integration_tests/test_harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_https_connection.py` & `codemodder-0.89.0/integration_tests/test_https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_jinja2_autoescape.py` & `codemodder-0.89.0/integration_tests/test_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_jwt_decode_verify.py` & `codemodder-0.89.0/integration_tests/test_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_lazy_logging.py` & `codemodder-0.89.0/integration_tests/test_lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_limit_readline.py` & `codemodder-0.89.0/integration_tests/test_limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_literal_or_new_object_identity.py` & `codemodder-0.89.0/integration_tests/test_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_lxml_safe_parser_defaults.py` & `codemodder-0.89.0/integration_tests/test_lxml_safe_parser_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_lxml_safe_parsing.py` & `codemodder-0.89.0/integration_tests/test_lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_multiple_codemods.py` & `codemodder-0.89.0/integration_tests/test_multiple_codemods.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_numpy_nan_equality.py` & `codemodder-0.89.0/integration_tests/test_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_order_imports.py` & `codemodder-0.89.0/integration_tests/test_order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_process_sandbox.py` & `codemodder-0.89.0/integration_tests/test_process_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_program.py` & `codemodder-0.89.0/integration_tests/test_program.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_remove_assertion_in_pytest_raises.py` & `codemodder-0.89.0/integration_tests/test_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_remove_debug_breakpoint.py` & `codemodder-0.89.0/integration_tests/test_remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_remove_future_imports.py` & `codemodder-0.89.0/integration_tests/test_remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_remove_module_global.py` & `codemodder-0.89.0/integration_tests/test_remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_remove_unused_imports.py` & `codemodder-0.89.0/integration_tests/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_replace_flask_send_file.py` & `codemodder-0.89.0/integration_tests/test_replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_request_verify.py` & `codemodder-0.89.0/integration_tests/test_request_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_secure_flask_cookie.py` & `codemodder-0.89.0/integration_tests/test_secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_secure_flask_session_config.py` & `codemodder-0.89.0/integration_tests/test_secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_secure_random.py` & `codemodder-0.89.0/integration_tests/test_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_django_json_response_type.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_django_receiver_on_top.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_exception_without_raise.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_fix_assert_tuple.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_fix_missing_self_or_cls.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_flask_json_response_type.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_jinja2_autoescape.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_jwt_decode_verify.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_literal_or_new_object_identity.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_numpy_nan_equality.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_remove_assertion_in_pytest_raises.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_secure_random.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sonar_tempfile_mktemp.py` & `codemodder-0.89.0/integration_tests/sonar/test_sonar_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_sql_parameterization.py` & `codemodder-0.89.0/integration_tests/test_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_str_concat_in_seq_literals.py` & `codemodder-0.89.0/integration_tests/test_str_concat_in_seq_literals.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_subprocess_shell_false.py` & `codemodder-0.89.0/integration_tests/test_subprocess_shell_false.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_tempfile_mktemp.py` & `codemodder-0.89.0/integration_tests/test_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_unnecessary_f_str.py` & `codemodder-0.89.0/integration_tests/test_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_upgrade_sslcontext_minimum_version.py` & `codemodder-0.89.0/integration_tests/test_upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_upgrade_sslcontext_tls.py` & `codemodder-0.89.0/integration_tests/test_upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_url_sandbox.py` & `codemodder-0.89.0/integration_tests/test_url_sandbox.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from codemodder.codemods.test import BaseIntegrationTest
 from codemodder.dependency import Security
-from core_codemods.url_sandbox import UrlSandbox
+from core_codemods.url_sandbox import UrlSandbox, UrlSandboxTransformer
 
 
 class TestUrlSandbox(BaseIntegrationTest):
     codemod = UrlSandbox
     original_code = """
     from test_sources import untrusted_data
     import requests
@@ -28,15 +28,15 @@
  url = untrusted_data()
 -requests.get(url)
 +safe_requests.get(url)
  var = "hello"
 """
 
     expected_line_change = "5"
-    change_description = UrlSandbox.change_description
+    change_description = UrlSandboxTransformer.change_description
     num_changed_files = 2
 
     requirements_file_name = "requirements.txt"
     original_requirements = (
         "# file used to test dependency management\n"
         "requests==2.31.0\n"
         "black==23.7.*\n"
```

### Comparing `codemodder-0.88.0/integration_tests/test_use_defusedxml.py` & `codemodder-0.89.0/integration_tests/test_use_defusedxml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_use_generator.py` & `codemodder-0.89.0/integration_tests/test_use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_use_set_literal.py` & `codemodder-0.89.0/integration_tests/test_use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_use_walrus_if.py` & `codemodder-0.89.0/integration_tests/test_use_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/integration_tests/test_with_threading_lock.py` & `codemodder-0.89.0/integration_tests/test_with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/pyproject.toml` & `codemodder-0.89.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "isort>=5.12,<5.14",
     "libcst>=1.1,<1.4",
     "packaging>=23.2,<25.0",
     "pydantic~=2.6.0",
     "pylint>=3.0,<3.2",
     "python-json-logger~=2.0.0",
     "PyYAML~=6.0.0",
-    "semgrep>=1.50,<1.68",
+    "semgrep>=1.50,<1.69",
     "toml~=0.10.2",
     "tomlkit~=0.12.0",
     "wrapt~=1.16.0",
     "chardet~=5.2.0",
 ]
 keywords = ["codemod", "codemods", "security", "fix", "fixes"]
 classifiers = [
@@ -79,14 +79,17 @@
 ]
 
 [project.entry-points.codemods]
 core = "core_codemods:registry"
 sonar = "core_codemods:sonar_registry"
 defectdojo = "core_codemods:defectdojo_registry"
 
+[project.entry-points.sarif_detectors]
+"semgrep" = "codemodder.semgrep:SemgrepSarifToolDetector"
+
 [tool.setuptools]
 
 [tool.setuptools.package-data]
 "core_codemods.semgrep" = ["src/core_codemods/semgrep/*.yaml"]
 "core_codemods.docs" = ["src/core_codemods/docs/*.md"]
 
 [tool.setuptools_scm]
```

### Comparing `codemodder-0.88.0/src/codemodder/cli.py` & `codemodder-0.89.0/src/codemodder/cli.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/code_directory.py` & `codemodder-0.89.0/src/codemodder/code_directory.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemodder.py` & `codemodder-0.89.0/src/codemodder/codemodder.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/api.py` & `codemodder-0.89.0/src/codemodder/codemods/api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/base_codemod.py` & `codemodder-0.89.0/src/codemodder/codemods/base_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/base_transformer.py` & `codemodder-0.89.0/src/codemodder/codemods/base_transformer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/base_visitor.py` & `codemodder-0.89.0/src/codemodder/codemods/base_visitor.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/check_annotations.py` & `codemodder-0.89.0/src/codemodder/codemods/check_annotations.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/import_modifier_codemod.py` & `codemodder-0.89.0/src/codemodder/codemods/import_modifier_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/imported_call_modifier.py` & `codemodder-0.89.0/src/codemodder/codemods/imported_call_modifier.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/libcst_transformer.py` & `codemodder-0.89.0/src/codemodder/codemods/libcst_transformer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/semgrep.py` & `codemodder-0.89.0/src/codemodder/codemods/semgrep.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import io
 import os
 import tempfile
+from functools import cache
 from pathlib import Path
 
 import yaml
 
 from codemodder.codemods.base_detector import BaseDetector
 from codemodder.context import CodemodExecutionContext
 from codemodder.result import ResultSet
+from codemodder.semgrep import SemgrepResultSet
 from codemodder.semgrep import run as semgrep_run
 
 
 def _populate_yaml(rule: str, codemod_id: str) -> str:
     rule_yaml = yaml.safe_load(io.StringIO(rule))
     config = {"rules": rule_yaml} if "rules" not in rule_yaml else rule_yaml
     config["rules"][0].setdefault("id", codemod_id)
@@ -43,7 +45,29 @@
         codemod_id: str,
         context: CodemodExecutionContext,
         files_to_analyze: list[Path],
     ) -> ResultSet:
         yaml_files = self.get_yaml_files(codemod_id)
         with context.timer.measure("semgrep"):
             return semgrep_run(context, yaml_files, files_to_analyze)
+
+
+class SemgrepSarifFileDetector(BaseDetector):
+    def apply(
+        self,
+        codemod_id: str,
+        context: CodemodExecutionContext,
+        files_to_analyze: list[Path],
+    ) -> ResultSet:
+        del codemod_id
+        del files_to_analyze
+        return process_semgrep_findings(
+            tuple(context.tool_result_files_map.get("semgrep", ()))
+        )  # Convert list to tuple for cache hashability
+
+
+@cache
+def process_semgrep_findings(semgrep_sarif_files: tuple[str]) -> ResultSet:
+    results = SemgrepResultSet()
+    for file in semgrep_sarif_files or ():
+        results |= SemgrepResultSet.from_sarif(file)
+    return results
```

### Comparing `codemodder-0.88.0/src/codemodder/codemods/sonar.py` & `codemodder-0.89.0/src/core_codemods/sonar/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 
 from codemodder.codemods.base_codemod import Metadata, Reference, ToolMetadata
 from codemodder.codemods.base_detector import BaseDetector
 from codemodder.codemods.base_transformer import BaseTransformerPipeline
 from codemodder.context import CodemodExecutionContext
 from codemodder.result import ResultSet
-from codemodder.sonar_results import SonarResultSet
 from core_codemods.api.core_codemod import CoreCodemod, SASTCodemod
+from core_codemods.sonar.results import SonarResultSet
 
 
 class SonarCodemod(SASTCodemod):
     @property
     def origin(self):
         return "sonar"
 
@@ -55,14 +55,16 @@
 class SonarDetector(BaseDetector):
     def apply(
         self,
         codemod_id: str,
         context: CodemodExecutionContext,
         files_to_analyze: list[Path],
     ) -> ResultSet:
+        del codemod_id
+        del files_to_analyze
         sonar_findings = process_sonar_findings(
             tuple(
                 context.tool_result_files_map.get("sonar", ())
             )  # Convert list to tuple for cache hashability
         )
         return sonar_findings
```

### Comparing `codemodder-0.88.0/src/codemodder/codemods/test/integration_utils.py` & `codemodder-0.89.0/src/codemodder/codemods/test/integration_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 from textwrap import dedent
 from types import ModuleType
 
 import jsonschema
 
 from codemodder import __version__, registry
+from core_codemods.sonar.api import process_sonar_findings
 
 from .validations import execute_code
 
 
 class DependencyTestMixin:
     # Only for codemods that modify requirements should these be overridden
     requirements_file_name = ""
@@ -278,16 +279,14 @@
         pathlib.Path(cls.output_path).unlink(missing_ok=True)
         # Revert code file
         with open(cls.code_path, mode="w", encoding="utf-8") as f:
             f.write(cls.original_code)
 
     @classmethod
     def check_sonar_issues(cls):
-        from codemodder.codemods.sonar import process_sonar_findings
-
         sonar_results = process_sonar_findings(
             (cls.sonar_issues_json, cls.sonar_hotspots_json)
         )
 
         assert (
             cls.codemod.rule_id in sonar_results
         ), f"Make sure to add a sonar issue/hotspot for {cls.codemod.rule_id} in {cls.sonar_issues_json} or {cls.sonar_hotspots_json}"
```

### Comparing `codemodder-0.88.0/src/codemodder/codemods/test/utils.py` & `codemodder-0.89.0/src/codemodder/codemods/test/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/test/validations.py` & `codemodder-0.89.0/src/codemodder/codemods/test/validations.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/transformations/clean_imports.py` & `codemodder-0.89.0/src/codemodder/codemods/transformations/clean_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py` & `codemodder-0.89.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/transformations/remove_unused_imports.py` & `codemodder-0.89.0/src/codemodder/codemods/transformations/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/utils.py` & `codemodder-0.89.0/src/codemodder/codemods/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codemods/utils_mixin.py` & `codemodder-0.89.0/src/codemodder/codemods/utils_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/codetf.py` & `codemodder-0.89.0/src/codemodder/codetf.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/context.py` & `codemodder-0.89.0/src/codemodder/context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/dependency.py` & `codemodder-0.89.0/src/codemodder/dependency.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/dependency_management/base_dependency_writer.py` & `codemodder-0.89.0/src/codemodder/dependency_management/base_dependency_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/dependency_management/dependency_manager.py` & `codemodder-0.89.0/src/codemodder/dependency_management/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/dependency_management/pyproject_writer.py` & `codemodder-0.89.0/src/codemodder/dependency_management/pyproject_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/dependency_management/requirements_txt_writer.py` & `codemodder-0.89.0/src/codemodder/dependency_management/requirements_txt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/dependency_management/setup_py_writer.py` & `codemodder-0.89.0/src/codemodder/dependency_management/setup_py_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/dependency_management/setupcfg_writer.py` & `codemodder-0.89.0/src/codemodder/dependency_management/setupcfg_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/diff.py` & `codemodder-0.89.0/src/codemodder/diff.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/file_context.py` & `codemodder-0.89.0/src/codemodder/file_context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/logging.py` & `codemodder-0.89.0/src/codemodder/logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/base_parser.py` & `codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/package_store.py` & `codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/package_store.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py` & `codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py` & `codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py` & `codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py` & `codemodder-0.89.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/project_analysis/python_repo_manager.py` & `codemodder-0.89.0/src/codemodder/project_analysis/python_repo_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/registry.py` & `codemodder-0.89.0/src/codemodder/registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import re
 from dataclasses import dataclass
 from importlib.metadata import entry_points
 from typing import TYPE_CHECKING, Optional
 
 from codemodder.logging import logger
 
 if TYPE_CHECKING:
@@ -60,44 +61,52 @@
         sast_only=False,
     ) -> list[BaseCodemod]:
         codemod_include = codemod_include or []
         codemod_exclude = codemod_exclude or DEFAULT_EXCLUDED_CODEMODS
 
         if codemod_exclude and not codemod_include:
             base_codemods = {}
+            patterns = [
+                re.compile(exclude.replace("*", ".*"))
+                for exclude in codemod_exclude
+                if "*" in exclude
+            ]
+            names = set(name for name in codemod_exclude if "*" not in name)
             for codemod in self.codemods:
-                if (sast_only and codemod.origin != "pixee") or (
-                    not sast_only and codemod.origin == "pixee"
+                if (
+                    codemod.id in names
+                    or (codemod.origin == "pixee" and codemod.name in names)
+                    or any(pat.match(codemod.id) for pat in patterns)
                 ):
-                    base_codemods[codemod.id] = codemod
-                    base_codemods[codemod.name] = codemod
-
-            for name_or_id in codemod_exclude:
-                try:
-                    codemod = base_codemods[name_or_id]
-                except KeyError:
-                    logger.warning(
-                        f"Requested codemod to exclude'{name_or_id}' does not exist."
-                    )
                     continue
 
-                # remove both by name and id since we don't know which `name_or_id` represented
-                base_codemods.pop(codemod.name, None)
-                base_codemods.pop(codemod.id, None)
+                if bool(sast_only) != bool(codemod.origin == "pixee"):
+                    base_codemods[codemod.id] = codemod
+
             # Remove duplicates and preserve order
-            return list(dict.fromkeys(base_codemods.values()))
+            return list(base_codemods.values())
 
         matched_codemods = []
         for name in codemod_include:
+            if "*" in name:
+                pat = re.compile(name.replace("*", ".*"))
+                pattern_matches = [code for code in self.codemods if pat.match(code.id)]
+                matched_codemods.extend(pattern_matches)
+                if not pattern_matches:
+                    logger.warning(
+                        "Given codemod pattern '%s' does not match any codemods.", name
+                    )
+                continue
+
             try:
                 matched_codemods.append(
                     self._codemods_by_name.get(name) or self._codemods_by_id[name]
                 )
             except KeyError:
-                logger.warning(f"Requested codemod to include'{name}' does not exist.")
+                logger.warning(f"Requested codemod to include '{name}' does not exist.")
         return matched_codemods
 
     def describe_codemods(
         self,
         codemod_include: Optional[list] = None,
         codemod_exclude: Optional[list] = None,
     ) -> list[dict]:
```

### Comparing `codemodder-0.88.0/src/codemodder/result.py` & `codemodder-0.89.0/src/codemodder/result.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/sarifs.py` & `codemodder-0.89.0/src/codemodder/semgrep.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,29 @@
+import itertools
 import json
-from abc import ABCMeta, abstractmethod
-from collections import defaultdict
-from importlib.metadata import entry_points
+import subprocess
 from pathlib import Path
-from typing import DefaultDict, Optional
+from tempfile import NamedTemporaryFile
+from typing import Iterable, Optional
 
 from typing_extensions import Self
 
+from codemodder.context import CodemodExecutionContext
 from codemodder.logging import logger
+from codemodder.result import LineInfo, Location, Result, ResultSet
+from codemodder.sarifs import AbstractSarifToolDetector
 
-from .result import LineInfo, Location, Result, ResultSet
 
-
-class AbstractSarifToolDetector(metaclass=ABCMeta):
+class SemgrepSarifToolDetector(AbstractSarifToolDetector):
     @classmethod
-    @abstractmethod
     def detect(cls, run_data: dict) -> bool:
-        pass
-
-
-def detect_sarif_tools(filenames: list[Path]) -> DefaultDict[str, list[str]]:
-    results: DefaultDict[str, list[str]] = defaultdict(list)
-
-    logger.debug("loading registered SARIF tool detectors")
-    detectors = {
-        ent.name: ent.load() for ent in entry_points().select(group="sarif_detectors")
-    }
-    for fname in filenames:
-        data = json.loads(fname.read_text())
-        for name, det in detectors.items():
-            # TODO: handle malformed sarif?
-            for run in data["runs"]:
-                try:
-                    if det.detect(run):
-                        logger.debug("detected %s sarif: %s", name, fname)
-                        results[name].append(str(fname))
-                except (KeyError, AttributeError, ValueError):
-                    continue
-
-    return results
+        return (
+            "tool" in run_data
+            and "semgrep" in run_data["tool"]["driver"]["name"].lower()
+        )
 
 
 def extract_rule_id(result, sarif_run) -> Optional[str]:
     if "ruleId" in result:
         # semgrep preprends the folders into the rule-id, we want the base name only
         return result["ruleId"].rsplit(".")[-1]
 
@@ -51,16 +32,15 @@
         tool_index = result["rule"]["toolComponent"]["index"]
         rule_index = result["rule"]["index"]
         return sarif_run["tool"]["extensions"][tool_index]["rules"][rule_index]["id"]
 
     return None
 
 
-# NOTE: These Sarif classes are actually specific to Semgrep and should be moved elsewhere
-class SarifLocation(Location):
+class SemgrepLocation(Location):
     @classmethod
     def from_sarif(cls, sarif_location) -> Self:
         artifact_location = sarif_location["physicalLocation"]["artifactLocation"]
         file = Path(artifact_location["uri"])
         start = LineInfo(
             line=sarif_location["physicalLocation"]["region"]["startLine"],
             column=sarif_location["physicalLocation"]["region"]["startColumn"],
@@ -70,34 +50,78 @@
             line=sarif_location["physicalLocation"]["region"]["endLine"],
             column=sarif_location["physicalLocation"]["region"]["endColumn"],
             snippet=sarif_location["physicalLocation"]["region"]["snippet"]["text"],
         )
         return cls(file=file, start=start, end=end)
 
 
-class SarifResult(Result):
+class SemgrepResult(Result):
     @classmethod
     def from_sarif(cls, sarif_result, sarif_run) -> Self:
         rule_id = extract_rule_id(sarif_result, sarif_run)
         if not rule_id:
             raise ValueError("Could not extract rule id from sarif result.")
 
         locations: list[Location] = []
         for location in sarif_result["locations"]:
-            artifact_location = SarifLocation.from_sarif(location)
+            artifact_location = SemgrepLocation.from_sarif(location)
             locations.append(artifact_location)
         return cls(rule_id=rule_id, locations=locations)
 
 
-class SarifResultSet(ResultSet):
+class SemgrepResultSet(ResultSet):
     @classmethod
     def from_sarif(cls, sarif_file: str | Path) -> Self:
         with open(sarif_file, "r", encoding="utf-8") as f:
             data = json.load(f)
 
         result_set = cls()
         for sarif_run in data["runs"]:
             for result in sarif_run["results"]:
-                sarif_result = SarifResult.from_sarif(result, sarif_run)
+                sarif_result = SemgrepResult.from_sarif(result, sarif_run)
                 result_set.add_result(sarif_result)
 
         return result_set
+
+
+def run(
+    execution_context: CodemodExecutionContext,
+    yaml_files: Iterable[Path],
+    files_to_analyze: Optional[Iterable[Path]] = None,
+) -> SemgrepResultSet:
+    """
+    Runs Semgrep and outputs a dict with the results organized by rule_id.
+    """
+    if not yaml_files:
+        raise ValueError("No Semgrep rules were provided")
+
+    with NamedTemporaryFile(prefix="semgrep", suffix=".sarif") as temp_sarif_file:
+        command = [
+            "semgrep",
+            "scan",
+            "--legacy",
+            "--no-error",
+            "--dataflow-traces",
+            "--sarif",
+            "-o",
+            temp_sarif_file.name,
+        ]
+        command.extend(
+            itertools.chain.from_iterable(
+                map(lambda f: ["--config", str(f)], yaml_files)
+            )
+        )
+        command.extend(map(str, files_to_analyze or [execution_context.directory]))
+        logger.debug("semgrep command: `%s`", " ".join(command))
+        call = subprocess.run(
+            command,
+            shell=False,
+            check=False,
+            stdout=None if execution_context.verbose else subprocess.PIPE,
+            stderr=None if execution_context.verbose else subprocess.PIPE,
+        )
+        if call.returncode != 0:
+            if not execution_context.verbose:
+                logger.error("captured semgrep stderr: %s", call.stderr)
+            raise subprocess.CalledProcessError(call.returncode, command)
+        results = SemgrepResultSet.from_sarif(temp_sarif_file.name)
+        return results
```

### Comparing `codemodder-0.88.0/src/codemodder/scripts/generate_docs.py` & `codemodder-0.89.0/src/codemodder/scripts/generate_docs.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     importance: str
     guidance_explained: str
     need_sarif: str = "No"
 
 
 # codemod-specific metadata that's used only for docs, not for codemod API
-CORE_METADATA = {
+CORE_CODEMODS = {
     "add-requests-timeouts": DocMetadata(
         importance="Medium",
         guidance_explained="This change makes your code safer but in some cases it may be necessary to adjust the timeout value for your particular application.",
     ),
     "django-debug-flag-on": DocMetadata(
         importance="Medium",
         guidance_explained="Django's `DEBUG` flag may be overridden somewhere else or the runtime settings file may be set with the `DJANGO_SETTINGS_MODULE` environment variable. This means that the `DEBUG` flag may intentionally be left on as a development aid.",
@@ -251,106 +251,68 @@
         importance="Medium",
         guidance_explained="This change is safe and will prevent runtime `ValueError`.",
     ),
     "fix-missing-self-or-cls": DocMetadata(
         importance="Medium",
         guidance_explained="This change is safe and will prevent errors when calling on these instance or class methods..",
     ),
-}
-
-METADATA = CORE_METADATA | {
-    "numpy-nan-equality-S6725": DocMetadata(
-        importance=CORE_METADATA["numpy-nan-equality"].importance,
-        guidance_explained=CORE_METADATA["numpy-nan-equality"].guidance_explained,
-        need_sarif="Yes (Sonar)",
-    ),
-    "literal-or-new-object-identity-S5796": DocMetadata(
-        importance=CORE_METADATA["literal-or-new-object-identity"].importance,
-        guidance_explained=CORE_METADATA[
-            "literal-or-new-object-identity"
-        ].guidance_explained,
-        need_sarif="Yes (Sonar)",
-    ),
-    "django-receiver-on-top-S6552": DocMetadata(
-        importance=CORE_METADATA["django-receiver-on-top"].importance,
-        guidance_explained=CORE_METADATA["django-receiver-on-top"].guidance_explained,
-        need_sarif="Yes (Sonar)",
-    ),
-    "exception-without-raise-S3984": DocMetadata(
-        importance=CORE_METADATA["exception-without-raise"].importance,
-        guidance_explained=CORE_METADATA["exception-without-raise"].guidance_explained,
-        need_sarif="Yes (Sonar)",
-    ),
-    "fix-assert-tuple-S5905": DocMetadata(
-        importance=CORE_METADATA["fix-assert-tuple"].importance,
-        guidance_explained=CORE_METADATA["fix-assert-tuple"].guidance_explained,
-        need_sarif="Yes (Sonar)",
-    ),
-    "remove-assertion-in-pytest-raises-S5915": DocMetadata(
-        importance=CORE_METADATA["remove-assertion-in-pytest-raises"].importance,
-        guidance_explained=CORE_METADATA[
-            "remove-assertion-in-pytest-raises"
-        ].guidance_explained,
-        need_sarif="Yes (Sonar)",
-    ),
-    "flask-json-response-type-S5131": DocMetadata(
-        importance=CORE_METADATA["flask-json-response-type"].importance,
-        guidance_explained=CORE_METADATA["flask-json-response-type"].guidance_explained,
-        need_sarif="Yes (Sonar)",
-    ),
-    "django-json-response-type-S5131": DocMetadata(
-        importance=CORE_METADATA["django-json-response-type"].importance,
-        guidance_explained=CORE_METADATA[
-            "django-json-response-type"
-        ].guidance_explained,
-        need_sarif="Yes (Sonar)",
-    ),
-    "jwt-decode-verify-S5659": DocMetadata(
-        importance=CORE_METADATA["jwt-decode-verify"].importance,
-        guidance_explained=CORE_METADATA["jwt-decode-verify"].guidance_explained,
-        need_sarif="Yes (Sonar)",
-    ),
-    "fix-missing-self-or-cls-S5719": DocMetadata(
-        importance=CORE_METADATA["fix-missing-self-or-cls"].importance,
-        guidance_explained=CORE_METADATA["fix-missing-self-or-cls"].guidance_explained,
-        need_sarif="Yes (Sonar)",
-    ),
-    "secure-tempfile-S5445": DocMetadata(
-        importance=CORE_METADATA["secure-tempfile"].importance,
-        guidance_explained=CORE_METADATA["secure-tempfile"].guidance_explained,
-        need_sarif="Yes (Sonar)",
-    ),
-    "secure-random-S2245": DocMetadata(
-        importance=CORE_METADATA["secure-random"].importance,
-        guidance_explained=CORE_METADATA["secure-random"].guidance_explained,
-        need_sarif="Yes (Sonar)",
-    ),
-    "enable-jinja2-autoescape-S5247": DocMetadata(
-        importance=CORE_METADATA["enable-jinja2-autoescape"].importance,
-        guidance_explained=CORE_METADATA["enable-jinja2-autoescape"].guidance_explained,
-        need_sarif="Yes (Sonar)",
+    "fix-float-equality": DocMetadata(
+        importance="Medium",
+        guidance_explained="This change makes your code more accurate but in some cases it may be necessary to adjust the `abs_tol` and `rel_tol` parameter values for your particular calculations.",
     ),
+}
+DEFECTDOJO_CODEMODS = {
     "django-secure-set-cookie": DocMetadata(
         importance="Medium",
         guidance_explained="Our change provides the most secure way to create cookies in Django. However, it's possible you have configured your Django application configurations to use secure cookies. In these cases, using the default parameters for `set_cookie` is safe.",
         need_sarif="Yes (DefectDojo)",
     ),
     "avoid-insecure-deserialization": DocMetadata(
         importance="High",
         guidance_explained="This change is generally safe and will prevent deserialization vulnerabilities.",
         need_sarif="Yes (DefectDojo)",
     ),
 }
 
+SONAR_CODEMOD_NAMES = [
+    "numpy-nan-equality-S6725",
+    "literal-or-new-object-identity-S5796",
+    "django-receiver-on-top-S6552",
+    "exception-without-raise-S3984",
+    "fix-assert-tuple-S5905",
+    "remove-assertion-in-pytest-raises-S5915",
+    "flask-json-response-type-S5131",
+    "django-json-response-type-S5131",
+    "jwt-decode-verify-S5659",
+    "fix-missing-self-or-cls-S5719",
+    "secure-tempfile-S5445",
+    "secure-random-S2245",
+    "enable-jinja2-autoescape-S5247",
+    "url-sandbox-S5144",
+    "fix-float-equality-S1244",
+]
+SONAR_CODEMODS = {
+    name: DocMetadata(
+        importance=CORE_CODEMODS[
+            core_codemod_name := "-".join(name.split("-")[:-1])
+        ].importance,
+        guidance_explained=CORE_CODEMODS[core_codemod_name].guidance_explained,
+        need_sarif="Yes (Sonar)",
+    )
+    for name in SONAR_CODEMOD_NAMES
+}
+
+ALL_CODEMODS_METADATA = CORE_CODEMODS | DEFECTDOJO_CODEMODS | SONAR_CODEMODS
+
 
 def generate_docs(codemod):
     try:
-        codemod_data = METADATA[codemod.name]
+        codemod_data = ALL_CODEMODS_METADATA[codemod.name]
     except KeyError as exc:
-        raise KeyError(f"Must add {codemod.name} to METADATA") from exc
+        raise KeyError(f"Must add {codemod.name} to ALL_CODEMODS_METADATA") from exc
 
     formatted_references = [
         f"* [{ref.description or ref.url}]({ref.url})" for ref in codemod.references
     ]
     markdown_references = "\n".join(formatted_references) or "N/A"
 
     # A bit of a hack but keeps the table aligned
```

### Comparing `codemodder-0.88.0/src/codemodder/scripts/get_hashes.py` & `codemodder-0.89.0/src/codemodder/scripts/get_hashes.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/sonar_results.py` & `codemodder-0.89.0/src/core_codemods/sonar/results.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/utils/clean_code.py` & `codemodder-0.89.0/src/codemodder/utils/clean_code.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/utils/format_string_parser.py` & `codemodder-0.89.0/src/codemodder/utils/format_string_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/utils/linearize_string_expression.py` & `codemodder-0.89.0/src/codemodder/utils/linearize_string_expression.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/utils/timer.py` & `codemodder-0.89.0/src/codemodder/utils/timer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder/utils/utils.py` & `codemodder-0.89.0/src/codemodder/utils/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/codemodder.egg-info/PKG-INFO` & `codemodder-0.89.0/src/codemodder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codemodder
-Version: 0.88.0
+Version: 0.89.0
 Summary: A pluggable framework for building codemods in Python
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,15 +683,15 @@
 Requires-Dist: isort<5.14,>=5.12
 Requires-Dist: libcst<1.4,>=1.1
 Requires-Dist: packaging<25.0,>=23.2
 Requires-Dist: pydantic~=2.6.0
 Requires-Dist: pylint<3.2,>=3.0
 Requires-Dist: python-json-logger~=2.0.0
 Requires-Dist: PyYAML~=6.0.0
-Requires-Dist: semgrep<1.68,>=1.50
+Requires-Dist: semgrep<1.69,>=1.50
 Requires-Dist: toml~=0.10.2
 Requires-Dist: tomlkit~=0.12.0
 Requires-Dist: wrapt~=1.16.0
 Requires-Dist: chardet~=5.2.0
 Provides-Extra: test
 Requires-Dist: coverage<7.5,>=7.3; extra == "test"
 Requires-Dist: Flask<4; extra == "test"
```

### Comparing `codemodder-0.88.0/src/codemodder.egg-info/SOURCES.txt` & `codemodder-0.89.0/src/codemodder.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 integration_tests/test_exception_without_raise.py
 integration_tests/test_file_resource_leak.py
 integration_tests/test_fix_assert_tuple.py
 integration_tests/test_fix_dataclass_defaults.py
 integration_tests/test_fix_deprecated_abstractproperty.py
 integration_tests/test_fix_deprecated_logging_warn.py
 integration_tests/test_fix_empty_sequence_comparison.py
+integration_tests/test_fix_float_equality.py
 integration_tests/test_fix_hasattr_call.py
 integration_tests/test_fix_missing_self_or_cls.py
 integration_tests/test_fix_mutable_params.py
 integration_tests/test_fix_task_instantiation.py
 integration_tests/test_flask_enable_csrf_protection.py
 integration_tests/test_flask_json_response_type.py
 integration_tests/test_harden_pickle_load.py
@@ -76,40 +77,42 @@
 integration_tests/test_remove_module_global.py
 integration_tests/test_remove_unused_imports.py
 integration_tests/test_replace_flask_send_file.py
 integration_tests/test_request_verify.py
 integration_tests/test_secure_flask_cookie.py
 integration_tests/test_secure_flask_session_config.py
 integration_tests/test_secure_random.py
-integration_tests/test_sonar_django_json_response_type.py
-integration_tests/test_sonar_django_receiver_on_top.py
-integration_tests/test_sonar_exception_without_raise.py
-integration_tests/test_sonar_fix_assert_tuple.py
-integration_tests/test_sonar_fix_missing_self_or_cls.py
-integration_tests/test_sonar_flask_json_response_type.py
-integration_tests/test_sonar_jinja2_autoescape.py
-integration_tests/test_sonar_jwt_decode_verify.py
-integration_tests/test_sonar_literal_or_new_object_identity.py
-integration_tests/test_sonar_numpy_nan_equality.py
-integration_tests/test_sonar_remove_assertion_in_pytest_raises.py
-integration_tests/test_sonar_secure_random.py
-integration_tests/test_sonar_tempfile_mktemp.py
 integration_tests/test_sql_parameterization.py
 integration_tests/test_str_concat_in_seq_literals.py
 integration_tests/test_subprocess_shell_false.py
 integration_tests/test_tempfile_mktemp.py
 integration_tests/test_unnecessary_f_str.py
 integration_tests/test_upgrade_sslcontext_minimum_version.py
 integration_tests/test_upgrade_sslcontext_tls.py
 integration_tests/test_url_sandbox.py
 integration_tests/test_use_defusedxml.py
 integration_tests/test_use_generator.py
 integration_tests/test_use_set_literal.py
 integration_tests/test_use_walrus_if.py
 integration_tests/test_with_threading_lock.py
+integration_tests/sonar/test_sonar_django_json_response_type.py
+integration_tests/sonar/test_sonar_django_receiver_on_top.py
+integration_tests/sonar/test_sonar_exception_without_raise.py
+integration_tests/sonar/test_sonar_fix_assert_tuple.py
+integration_tests/sonar/test_sonar_fix_float_equality.py
+integration_tests/sonar/test_sonar_fix_missing_self_or_cls.py
+integration_tests/sonar/test_sonar_flask_json_response_type.py
+integration_tests/sonar/test_sonar_jinja2_autoescape.py
+integration_tests/sonar/test_sonar_jwt_decode_verify.py
+integration_tests/sonar/test_sonar_literal_or_new_object_identity.py
+integration_tests/sonar/test_sonar_numpy_nan_equality.py
+integration_tests/sonar/test_sonar_remove_assertion_in_pytest_raises.py
+integration_tests/sonar/test_sonar_secure_random.py
+integration_tests/sonar/test_sonar_tempfile_mktemp.py
+integration_tests/sonar/test_sonar_url_sandbox.py
 src/codemodder/__init__.py
 src/codemodder/_version.py
 src/codemodder/cli.py
 src/codemodder/code_directory.py
 src/codemodder/codemodder.py
 src/codemodder/codetf.py
 src/codemodder/context.py
@@ -117,15 +120,14 @@
 src/codemodder/diff.py
 src/codemodder/file_context.py
 src/codemodder/logging.py
 src/codemodder/registry.py
 src/codemodder/result.py
 src/codemodder/sarifs.py
 src/codemodder/semgrep.py
-src/codemodder/sonar_results.py
 src/codemodder.egg-info/PKG-INFO
 src/codemodder.egg-info/SOURCES.txt
 src/codemodder.egg-info/dependency_links.txt
 src/codemodder.egg-info/entry_points.txt
 src/codemodder.egg-info/requires.txt
 src/codemodder.egg-info/top_level.txt
 src/codemodder/codemods/__init__.py
@@ -135,15 +137,14 @@
 src/codemodder/codemods/base_transformer.py
 src/codemodder/codemods/base_visitor.py
 src/codemodder/codemods/check_annotations.py
 src/codemodder/codemods/import_modifier_codemod.py
 src/codemodder/codemods/imported_call_modifier.py
 src/codemodder/codemods/libcst_transformer.py
 src/codemodder/codemods/semgrep.py
-src/codemodder/codemods/sonar.py
 src/codemodder/codemods/utils.py
 src/codemodder/codemods/utils_mixin.py
 src/codemodder/codemods/test/__init__.py
 src/codemodder/codemods/test/integration_utils.py
 src/codemodder/codemods/test/utils.py
 src/codemodder/codemods/test/validations.py
 src/codemodder/codemods/transformations/__init__.py
@@ -190,14 +191,15 @@
 src/core_codemods/file_resource_leak.py
 src/core_codemods/fix_assert_tuple.py
 src/core_codemods/fix_async_task_instantiation.py
 src/core_codemods/fix_dataclass_defaults.py
 src/core_codemods/fix_deprecated_abstractproperty.py
 src/core_codemods/fix_deprecated_logging_warn.py
 src/core_codemods/fix_empty_sequence_comparison.py
+src/core_codemods/fix_float_equality.py
 src/core_codemods/fix_hasattr_call.py
 src/core_codemods/fix_missing_self_or_cls.py
 src/core_codemods/fix_mutable_params.py
 src/core_codemods/flask_enable_csrf_protection.py
 src/core_codemods/flask_json_response_type.py
 src/core_codemods/harden_pickle_load.py
 src/core_codemods/harden_pyyaml.py
@@ -258,14 +260,15 @@
 src/core_codemods/docs/pixee_python_fix-assert-tuple.md
 src/core_codemods/docs/pixee_python_fix-async-task-instantiation.md
 src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md
 src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md
 src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md
 src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md
 src/core_codemods/docs/pixee_python_fix-file-resource-leak.md
+src/core_codemods/docs/pixee_python_fix-float-equality.md
 src/core_codemods/docs/pixee_python_fix-hasattr-call.md
 src/core_codemods/docs/pixee_python_fix-missing-self-or-cls.md
 src/core_codemods/docs/pixee_python_fix-mutable-params.md
 src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md
 src/core_codemods/docs/pixee_python_flask-json-response-type.md
 src/core_codemods/docs/pixee_python_harden-pickle-load.md
 src/core_codemods/docs/pixee_python_harden-pyyaml.md
@@ -299,27 +302,31 @@
 src/core_codemods/docs/pixee_python_url-sandbox.md
 src/core_codemods/docs/pixee_python_use-defusedxml.md
 src/core_codemods/docs/pixee_python_use-generator.md
 src/core_codemods/docs/pixee_python_use-set-literal.md
 src/core_codemods/docs/pixee_python_use-walrus-if.md
 src/core_codemods/refactor/__init__.py
 src/core_codemods/refactor/refactor_new_api.py
+src/core_codemods/sonar/api.py
+src/core_codemods/sonar/results.py
 src/core_codemods/sonar/sonar_django_json_response_type.py
 src/core_codemods/sonar/sonar_django_receiver_on_top.py
 src/core_codemods/sonar/sonar_enable_jinja2_autoescape.py
 src/core_codemods/sonar/sonar_exception_without_raise.py
 src/core_codemods/sonar/sonar_fix_assert_tuple.py
+src/core_codemods/sonar/sonar_fix_float_equality.py
 src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
 src/core_codemods/sonar/sonar_flask_json_response_type.py
 src/core_codemods/sonar/sonar_jwt_decode_verify.py
 src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
 src/core_codemods/sonar/sonar_numpy_nan_equality.py
 src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
 src/core_codemods/sonar/sonar_secure_random.py
 src/core_codemods/sonar/sonar_tempfile_mktemp.py
+src/core_codemods/sonar/sonar_url_sandbox.py
 tests/__init__.py
 tests/conftest.py
 tests/test_ancestorpatterns_mixin.py
 tests/test_basetype.py
 tests/test_cli.py
 tests/test_code_directory.py
 tests/test_codemod_docs.py
@@ -329,14 +336,15 @@
 tests/test_file_context.py
 tests/test_format_string_parser.py
 tests/test_linearize_string_expression.py
 tests/test_logging.py
 tests/test_nameresolution_mixin.py
 tests/test_results.py
 tests/test_sarif_processing.py
+tests/test_semgrep.py
 tests/test_version.py
 tests/codemods/__init__.py
 tests/codemods/conftest.py
 tests/codemods/test_add_requests_timeouts.py
 tests/codemods/test_async_fix_task_instantiation.py
 tests/codemods/test_base_codemod.py
 tests/codemods/test_base_visitor.py
@@ -350,14 +358,15 @@
 tests/codemods/test_exception_without_raise.py
 tests/codemods/test_file_resource_leak.py
 tests/codemods/test_fix_assert_tuple.py
 tests/codemods/test_fix_dataclass_defaults.py
 tests/codemods/test_fix_deprecated_abstractproperty.py
 tests/codemods/test_fix_deprecated_logging_warn.py
 tests/codemods/test_fix_empty_sequence_comparison.py
+tests/codemods/test_fix_float_equality.py
 tests/codemods/test_fix_hasattr_call.py
 tests/codemods/test_fix_missing_self_or_cls.py
 tests/codemods/test_fix_mutable_params.py
 tests/codemods/test_flask_enable_csrf_protection.py
 tests/codemods/test_flask_json_response_type.py
 tests/codemods/test_harden_pickle_load.py
 tests/codemods/test_harden_pyyaml.py
@@ -380,41 +389,43 @@
 tests/codemods/test_remove_unnecessary_f_str.py
 tests/codemods/test_remove_unused_imports.py
 tests/codemods/test_replace_flask_send_file.py
 tests/codemods/test_request_verify.py
 tests/codemods/test_secure_flask_cookie.py
 tests/codemods/test_secure_flask_session_config.py
 tests/codemods/test_secure_random.py
-tests/codemods/test_sonar_django_json_response_type.py
-tests/codemods/test_sonar_django_receiver_on_top.py
-tests/codemods/test_sonar_enable_jinja2_autoescape.py
-tests/codemods/test_sonar_exception_without_raise.py
-tests/codemods/test_sonar_fix_assert_tuple.py
-tests/codemods/test_sonar_fix_missing_self_or_cls.py
-tests/codemods/test_sonar_flask_json_response_type.py
-tests/codemods/test_sonar_jwt_decode_verify.py
-tests/codemods/test_sonar_literal_or_new_object_identity.py
-tests/codemods/test_sonar_numpy_nan_equality.py
-tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py
-tests/codemods/test_sonar_secure_random.py
-tests/codemods/test_sonar_tempfile_mktemp.py
 tests/codemods/test_sql_parameterization.py
 tests/codemods/test_str_concat_in_seq_literal.py
 tests/codemods/test_subprocess_shell_false.py
 tests/codemods/test_tempfile_mktemp.py
 tests/codemods/test_upgrade_sslcontext_minimum_version.py
 tests/codemods/test_upgrade_sslcontext_tls.py
 tests/codemods/test_url_sandbox.py
 tests/codemods/test_use_defused_xml.py
 tests/codemods/test_use_generator.py
 tests/codemods/test_use_set_literal.py
 tests/codemods/test_walrus_if.py
 tests/codemods/test_with_threading_lock.py
 tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py
 tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py
+tests/codemods/sonar/test_sonar_django_json_response_type.py
+tests/codemods/sonar/test_sonar_django_receiver_on_top.py
+tests/codemods/sonar/test_sonar_enable_jinja2_autoescape.py
+tests/codemods/sonar/test_sonar_exception_without_raise.py
+tests/codemods/sonar/test_sonar_fix_assert_tuple.py
+tests/codemods/sonar/test_sonar_fix_float_equality.py
+tests/codemods/sonar/test_sonar_fix_missing_self_or_cls.py
+tests/codemods/sonar/test_sonar_flask_json_response_type.py
+tests/codemods/sonar/test_sonar_jwt_decode_verify.py
+tests/codemods/sonar/test_sonar_literal_or_new_object_identity.py
+tests/codemods/sonar/test_sonar_numpy_nan_equality.py
+tests/codemods/sonar/test_sonar_remove_assertion_in_pytest_raises.py
+tests/codemods/sonar/test_sonar_secure_random.py
+tests/codemods/sonar/test_sonar_tempfile_mktemp.py
+tests/codemods/sonar/test_sonar_url_sandbox.py
 tests/dependency_management/__init__.py
 tests/dependency_management/test_base_dependency_writer.py
 tests/dependency_management/test_dependency_manager.py
 tests/dependency_management/test_pyproject_writer.py
 tests/dependency_management/test_requirements_txt_writer.py
 tests/dependency_management/test_setup_py_writer.py
 tests/dependency_management/test_setupcfgt_writer.py
@@ -425,22 +436,25 @@
 tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py
 tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py
 tests/project_analysis/file_parsers/test_setup_py_file_parser.py
 tests/samples/django_json_response_type.py
 tests/samples/django_receiver_on_top.py
 tests/samples/exception_without_raise.py
 tests/samples/fix_assert_tuple.py
+tests/samples/fix_float_equality.py
 tests/samples/fix_missing_self_or_cls.py
 tests/samples/flask_json_response_type.py
+tests/samples/flask_request.py
 tests/samples/jinja2_autoescape.py
 tests/samples/jwt_decode_verify.py
 tests/samples/literal_or_new_object_identity.py
 tests/samples/make_request.py
 tests/samples/multiple_codemods.py
 tests/samples/numpy_nan_equality.py
+tests/samples/pygoat.semgrep.sarif.json
 tests/samples/remove_assertion_in_pytest_raises.py
 tests/samples/secure_random.py
 tests/samples/semgrep.sarif
 tests/samples/sonar_hotspots.json
 tests/samples/sonar_issues.json
 tests/samples/tempfile_mktemp.py
 tests/samples/webgoat_v8.2.0_codeql.sarif
```

### Comparing `codemodder-0.88.0/src/codemodder.egg-info/requires.txt` & `codemodder-0.89.0/src/codemodder.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 isort<5.14,>=5.12
 libcst<1.4,>=1.1
 packaging<25.0,>=23.2
 pydantic~=2.6.0
 pylint<3.2,>=3.0
 python-json-logger~=2.0.0
 PyYAML~=6.0.0
-semgrep<1.68,>=1.50
+semgrep<1.69,>=1.50
 toml~=0.10.2
 tomlkit~=0.12.0
 wrapt~=1.16.0
 chardet~=5.2.0
 
 [all]
 codemodder[test]
```

### Comparing `codemodder-0.88.0/src/core_codemods/__init__.py` & `codemodder-0.89.0/src/core_codemods/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .file_resource_leak import FileResourceLeak
 from .fix_assert_tuple import FixAssertTuple
 from .fix_async_task_instantiation import FixAsyncTaskInstantiation
 from .fix_dataclass_defaults import FixDataclassDefaults
 from .fix_deprecated_abstractproperty import FixDeprecatedAbstractproperty
 from .fix_deprecated_logging_warn import FixDeprecatedLoggingWarn
 from .fix_empty_sequence_comparison import FixEmptySequenceComparison
+from .fix_float_equality import FixFloatEquality
 from .fix_hasattr_call import TransformFixHasattrCall
 from .fix_missing_self_or_cls import FixMissingSelfOrCls
 from .fix_mutable_params import FixMutableParams
 from .flask_enable_csrf_protection import FlaskEnableCSRFProtection
 from .flask_json_response_type import FlaskJsonResponseType
 from .harden_pickle_load import HardenPickleLoad
 from .harden_pyyaml import HardenPyyaml
@@ -50,24 +51,26 @@
 from .secure_flask_session_config import SecureFlaskSessionConfig
 from .secure_random import SecureRandom
 from .sonar.sonar_django_json_response_type import SonarDjangoJsonResponseType
 from .sonar.sonar_django_receiver_on_top import SonarDjangoReceiverOnTop
 from .sonar.sonar_enable_jinja2_autoescape import SonarEnableJinja2Autoescape
 from .sonar.sonar_exception_without_raise import SonarExceptionWithoutRaise
 from .sonar.sonar_fix_assert_tuple import SonarFixAssertTuple
+from .sonar.sonar_fix_float_equality import SonarFixFloatEquality
 from .sonar.sonar_fix_missing_self_or_cls import SonarFixMissingSelfOrCls
 from .sonar.sonar_flask_json_response_type import SonarFlaskJsonResponseType
 from .sonar.sonar_jwt_decode_verify import SonarJwtDecodeVerify
 from .sonar.sonar_literal_or_new_object_identity import SonarLiteralOrNewObjectIdentity
 from .sonar.sonar_numpy_nan_equality import SonarNumpyNanEquality
 from .sonar.sonar_remove_assertion_in_pytest_raises import (
     SonarRemoveAssertionInPytestRaises,
 )
 from .sonar.sonar_secure_random import SonarSecureRandom
 from .sonar.sonar_tempfile_mktemp import SonarTempfileMktemp
+from .sonar.sonar_url_sandbox import SonarUrlSandbox
 from .sql_parameterization import SQLQueryParameterization
 from .str_concat_in_seq_literal import StrConcatInSeqLiteral
 from .subprocess_shell_false import SubprocessShellFalse
 from .tempfile_mktemp import TempfileMktemp
 from .upgrade_sslcontext_minimum_version import UpgradeSSLContextMinimumVersion
 from .upgrade_sslcontext_tls import UpgradeSSLContextTLS
 from .url_sandbox import UrlSandbox
@@ -126,14 +129,15 @@
         CombineStartswithEndswith,
         FixDeprecatedLoggingWarn,
         FlaskEnableCSRFProtection,
         ReplaceFlaskSendFile,
         FixEmptySequenceComparison,
         RemoveAssertionInPytestRaises,
         FixAssertTuple,
+        FixFloatEquality,
         LazyLogging,
         StrConcatInSeqLiteral,
         FixAsyncTaskInstantiation,
         DjangoModelWithoutDunderStr,
         TransformFixHasattrCall,
         FixDataclassDefaults,
         FixMissingSelfOrCls,
@@ -152,14 +156,16 @@
         SonarFlaskJsonResponseType,
         SonarDjangoJsonResponseType,
         SonarJwtDecodeVerify,
         SonarFixMissingSelfOrCls,
         SonarTempfileMktemp,
         SonarSecureRandom,
         SonarEnableJinja2Autoescape,
+        SonarUrlSandbox,
+        SonarFixFloatEquality,
     ],
 )
 
 defectdojo_registry = CodemodCollection(
     origin="defectdojo",
     codemods=[
         AvoidInsecureDeserialization,
```

### Comparing `codemodder-0.88.0/src/core_codemods/add_requests_timeouts.py` & `codemodder-0.89.0/src/core_codemods/add_requests_timeouts.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/api/core_codemod.py` & `codemodder-0.89.0/src/core_codemods/api/core_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/combine_startswith_endswith.py` & `codemodder-0.89.0/src/core_codemods/combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/defectdojo/api.py` & `codemodder-0.89.0/src/core_codemods/defectdojo/api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/defectdojo/results.py` & `codemodder-0.89.0/src/core_codemods/defectdojo/results.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py` & `codemodder-0.89.0/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py` & `codemodder-0.89.0/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/django_debug_flag_on.py` & `codemodder-0.89.0/src/core_codemods/django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/django_json_response_type.py` & `codemodder-0.89.0/src/core_codemods/django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/django_model_without_dunder_str.py` & `codemodder-0.89.0/src/core_codemods/django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/django_receiver_on_top.py` & `codemodder-0.89.0/src/core_codemods/django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/django_session_cookie_secure_off.py` & `codemodder-0.89.0/src/core_codemods/django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md` & `codemodder-0.89.0/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md` & `codemodder-0.89.0/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-json-response-type.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_django-json-response-type.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_harden-ruamel.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_harden-ruamel.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_lazy-logging.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_lazy-logging.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_limit-readline.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_limit-readline.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_remove-future-imports.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_remove-future-imports.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_requests-verify.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_requests-verify.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_secure-random.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_secure-random.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_sql-parameterization.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_sql-parameterization.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_url-sandbox.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_url-sandbox.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-defusedxml.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_use-defusedxml.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-generator.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_use-generator.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/docs/pixee_python_use-walrus-if.md` & `codemodder-0.89.0/src/core_codemods/docs/pixee_python_use-walrus-if.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/enable_jinja2_autoescape.py` & `codemodder-0.89.0/src/core_codemods/enable_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/exception_without_raise.py` & `codemodder-0.89.0/src/core_codemods/exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/file_resource_leak.py` & `codemodder-0.89.0/src/core_codemods/file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/fix_assert_tuple.py` & `codemodder-0.89.0/src/core_codemods/fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/fix_async_task_instantiation.py` & `codemodder-0.89.0/src/core_codemods/fix_async_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/fix_dataclass_defaults.py` & `codemodder-0.89.0/src/core_codemods/fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/fix_deprecated_abstractproperty.py` & `codemodder-0.89.0/src/core_codemods/fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/fix_deprecated_logging_warn.py` & `codemodder-0.89.0/src/core_codemods/fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/fix_empty_sequence_comparison.py` & `codemodder-0.89.0/src/core_codemods/fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/fix_hasattr_call.py` & `codemodder-0.89.0/src/core_codemods/fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/fix_missing_self_or_cls.py` & `codemodder-0.89.0/src/core_codemods/fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/fix_mutable_params.py` & `codemodder-0.89.0/src/core_codemods/fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/flask_enable_csrf_protection.py` & `codemodder-0.89.0/src/core_codemods/flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/flask_json_response_type.py` & `codemodder-0.89.0/src/core_codemods/flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/harden_pickle_load.py` & `codemodder-0.89.0/src/core_codemods/harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/harden_pyyaml.py` & `codemodder-0.89.0/src/core_codemods/harden_pyyaml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/harden_ruamel.py` & `codemodder-0.89.0/src/core_codemods/harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/https_connection.py` & `codemodder-0.89.0/src/core_codemods/https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/jwt_decode_verify.py` & `codemodder-0.89.0/src/core_codemods/jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/lazy_logging.py` & `codemodder-0.89.0/src/core_codemods/lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/limit_readline.py` & `codemodder-0.89.0/src/core_codemods/limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/literal_or_new_object_identity.py` & `codemodder-0.89.0/src/core_codemods/literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/lxml_safe_parser_defaults.py` & `codemodder-0.89.0/src/core_codemods/lxml_safe_parser_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/lxml_safe_parsing.py` & `codemodder-0.89.0/src/core_codemods/lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/numpy_nan_equality.py` & `codemodder-0.89.0/src/core_codemods/numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/order_imports.py` & `codemodder-0.89.0/src/core_codemods/order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/process_creation_sandbox.py` & `codemodder-0.89.0/src/core_codemods/process_creation_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/refactor/refactor_new_api.py` & `codemodder-0.89.0/src/core_codemods/refactor/refactor_new_api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/remove_assertion_in_pytest_raises.py` & `codemodder-0.89.0/src/core_codemods/remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/remove_debug_breakpoint.py` & `codemodder-0.89.0/src/core_codemods/remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/remove_future_imports.py` & `codemodder-0.89.0/src/core_codemods/remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/remove_module_global.py` & `codemodder-0.89.0/src/core_codemods/remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/remove_unnecessary_f_str.py` & `codemodder-0.89.0/src/core_codemods/remove_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/remove_unused_imports.py` & `codemodder-0.89.0/src/core_codemods/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/replace_flask_send_file.py` & `codemodder-0.89.0/src/core_codemods/replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/requests_verify.py` & `codemodder-0.89.0/src/core_codemods/requests_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/secure_cookie_mixin.py` & `codemodder-0.89.0/src/core_codemods/secure_cookie_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/secure_flask_cookie.py` & `codemodder-0.89.0/src/core_codemods/secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/secure_flask_session_config.py` & `codemodder-0.89.0/src/core_codemods/secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/secure_random.py` & `codemodder-0.89.0/src/core_codemods/secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py` & `codemodder-0.89.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import libcst as cst
 
 from codemodder.codemods.libcst_transformer import LibcstTransformerPipeline
-from codemodder.codemods.sonar import SonarCodemod
 from codemodder.result import fuzzy_column_match, same_line
 from core_codemods.jwt_decode_verify import JwtDecodeVerify, JwtDecodeVerifyTransformer
+from core_codemods.sonar.api import SonarCodemod
 
 
 class JwtDecodeVerifySonarTransformer(JwtDecodeVerifyTransformer):
     def filter_by_result(self, node) -> bool:
         """
         Special case result-matching for this rule because the sonar
         results returned have a start/end column for the verify keyword
```

### Comparing `codemodder-0.88.0/src/core_codemods/sql_parameterization.py` & `codemodder-0.89.0/src/core_codemods/sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/str_concat_in_seq_literal.py` & `codemodder-0.89.0/src/core_codemods/str_concat_in_seq_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/subprocess_shell_false.py` & `codemodder-0.89.0/src/core_codemods/subprocess_shell_false.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/tempfile_mktemp.py` & `codemodder-0.89.0/src/core_codemods/tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/upgrade_sslcontext_minimum_version.py` & `codemodder-0.89.0/src/core_codemods/upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/upgrade_sslcontext_tls.py` & `codemodder-0.89.0/src/core_codemods/upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/url_sandbox.py` & `codemodder-0.89.0/src/core_codemods/url_sandbox.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,65 +3,34 @@
 import libcst as cst
 from libcst import CSTNode, matchers
 from libcst.codemod import CodemodContext, ContextAwareVisitor
 from libcst.codemod.visitors import AddImportsVisitor, ImportItem
 from libcst.metadata import PositionProvider, ScopeProvider
 
 from codemodder.codemods.base_visitor import UtilsMixin
+from codemodder.codemods.libcst_transformer import (
+    LibcstResultTransformer,
+    LibcstTransformerPipeline,
+)
+from codemodder.codemods.semgrep import SemgrepRuleDetector
 from codemodder.codemods.transformations.remove_unused_imports import (
     RemoveUnusedImportsCodemod,
 )
 from codemodder.codemods.utils import ReplaceNodes
 from codemodder.codetf import Change
 from codemodder.dependency import Security
 from codemodder.file_context import FileContext
-from core_codemods.api import Metadata, Reference, ReviewGuidance, SimpleCodemod
+from core_codemods.api import CoreCodemod, Metadata, Reference, ReviewGuidance
 
 replacement_import = "safe_requests"
 
 
-class UrlSandbox(SimpleCodemod):
-    metadata = Metadata(
-        name="url-sandbox",
-        summary="Sandbox URL Creation",
-        review_guidance=ReviewGuidance.MERGE_AFTER_CURSORY_REVIEW,
-        references=[
-            Reference(
-                url="https://github.com/pixee/python-security/blob/main/src/security/safe_requests/api.py"
-            ),
-            Reference(url="https://portswigger.net/web-security/ssrf"),
-            Reference(
-                url="https://cheatsheetseries.owasp.org/cheatsheets/Server_Side_Request_Forgery_Prevention_Cheat_Sheet.html"
-            ),
-            Reference(
-                url="https://www.rapid7.com/blog/post/2021/11/23/owasp-top-10-deep-dive-defending-against-server-side-request-forgery/"
-            ),
-            Reference(url="https://blog.assetnote.io/2021/01/13/blind-ssrf-chains/"),
-        ],
-    )
+class UrlSandboxTransformer(LibcstResultTransformer):
     change_description = "Switch use of requests for security.safe_requests"
-
-    detector_pattern = """
-    rules:
-      - id: url-sandbox
-        message: Unbounded URL creation
-        severity: WARNING
-        languages:
-          - python
-        pattern-either:
-          - patterns:
-            - pattern: requests.get(...)
-            - pattern-not: requests.get("...")
-            - pattern-inside: |
-                import requests
-                ...
-            """
-
     METADATA_DEPENDENCIES = (PositionProvider, ScopeProvider)
-
     adds_dependency = True
 
     def transform_module_impl(self, tree: cst.Module) -> cst.Module:
         # we first gather all the nodes we want to change together with their replacements
         find_requests_visitor = FindRequestCallsAndImports(
             self.context,
             self.file_context,
@@ -107,15 +76,15 @@
             self,
             results=results,
             line_include=file_context.line_include,
             line_exclude=file_context.line_exclude,
         )
 
     def leave_Call(self, original_node: cst.Call):
-        if not (self.node_is_selected(original_node)):
+        if not self.node_is_selected(original_node):
             return
 
         line_number = self.node_position(original_node).start.line
         match original_node.args[0].value:
             case cst.SimpleString():
                 return
 
@@ -135,15 +104,15 @@
                                     names=node.names,
                                 )
                             }
                         )
                         self.changes_in_file.append(
                             Change(
                                 lineNumber=line_number,
-                                description=UrlSandbox.change_description,
+                                description=UrlSandboxTransformer.change_description,
                             )
                         )
 
             # case req.get(...)
             case _:
                 self.nodes_to_change.update(
                     {
@@ -152,15 +121,15 @@
                             args=original_node.args,
                         )
                     }
                 )
                 self.changes_in_file.append(
                     Change(
                         lineNumber=line_number,
-                        description=UrlSandbox.change_description,
+                        description=UrlSandboxTransformer.change_description,
                     )
                 )
 
     def _find_assignments(self, node: CSTNode):
         """
         Given a MetadataWrapper and a CSTNode representing an access, find all the possible assignments that it refers.
         """
@@ -171,7 +140,47 @@
         """
         Given a MetadataWrapper and a CSTNode representing an access, find if there is a single assignment that it refers to.
         """
         assignments = self._find_assignments(node)
         if len(assignments) == 1:
             return next(iter(assignments)).node
         return None
+
+
+UrlSandbox = CoreCodemod(
+    metadata=Metadata(
+        name="url-sandbox",
+        summary="Sandbox URL Creation",
+        review_guidance=ReviewGuidance.MERGE_AFTER_CURSORY_REVIEW,
+        references=[
+            Reference(
+                url="https://github.com/pixee/python-security/blob/main/src/security/safe_requests/api.py"
+            ),
+            Reference(url="https://portswigger.net/web-security/ssrf"),
+            Reference(
+                url="https://cheatsheetseries.owasp.org/cheatsheets/Server_Side_Request_Forgery_Prevention_Cheat_Sheet.html"
+            ),
+            Reference(
+                url="https://www.rapid7.com/blog/post/2021/11/23/owasp-top-10-deep-dive-defending-against-server-side-request-forgery/"
+            ),
+            Reference(url="https://blog.assetnote.io/2021/01/13/blind-ssrf-chains/"),
+        ],
+    ),
+    detector=SemgrepRuleDetector(
+        """
+    rules:
+      - id: url-sandbox
+        message: Unbounded URL creation
+        severity: WARNING
+        languages:
+          - python
+        pattern-either:
+          - patterns:
+            - pattern: requests.get(...)
+            - pattern-not: requests.get("...")
+            - pattern-inside: |
+                import requests
+                ...
+            """
+    ),
+    transformer=LibcstTransformerPipeline(UrlSandboxTransformer),
+)
```

### Comparing `codemodder-0.88.0/src/core_codemods/use_defused_xml.py` & `codemodder-0.89.0/src/core_codemods/use_defused_xml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/use_generator.py` & `codemodder-0.89.0/src/core_codemods/use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/use_set_literal.py` & `codemodder-0.89.0/src/core_codemods/use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/src/core_codemods/use_walrus_if.py` & `codemodder-0.89.0/src/core_codemods/use_walrus_if.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import itertools
 from collections import namedtuple
 from typing import List, Optional, Tuple
 
 import libcst as cst
-from libcst import matchers as m
 from libcst._position import CodeRange
 from libcst.metadata import ParentNodeProvider, ScopeProvider
 
 from core_codemods.api import Metadata, Reference, ReviewGuidance, SimpleCodemod
 
 FoundAssign = namedtuple("FoundAssign", ["assign", "target", "value"])
 
@@ -84,57 +83,68 @@
         for a, b in pairwise(node.children):
             if not (found_assign := self._filter_assigns(a)):
                 continue
             if not (if_test := self._filter_if(b)):
                 continue
 
             assign, target, value = found_assign
-            # If test can be a comparison expression
+
             match if_test:
+                # If test can be a comparison expression
                 case cst.Comparison(
                     left=cst.Name() as left,
                     comparisons=[
                         cst.ComparisonTarget(
                             operator=(
                                 cst.Is() | cst.IsNot() | cst.Equal() | cst.NotEqual()
                             )
                         )
                     ],
                 ):
+
                     if left.value == target.value:
                         named_expr = self._build_named_expr(target, value, parens=True)
                         self.assigns[assign] = named_expr
-                # If test can also be a bare name
                 case cst.Name() as name:
+                    # If test can also be a bare name
                     if name.value == target.value:
                         named_expr = self._build_named_expr(target, value, parens=False)
                         self.assigns[assign] = named_expr
-
+                case cst.UnaryOperation(
+                    operator=cst.Not(), expression=cst.Name() as name
+                ):
+                    if name.value == target.value:
+                        named_expr = self._build_named_expr(target, value, parens=True)
+                        self.assigns[assign] = named_expr
         return super().on_visit(node)
 
     def visit_If(self, node: cst.If):
         del node
         self._if_stack.append(
             self._modify_next_if.pop() if len(self._modify_next_if) else None
         )
 
     def leave_If(self, original_node, updated_node):
         # TODO: add filter by include or exclude that works for nodes
         # that that have different start/end numbers.
+
         if (result := self._if_stack.pop()) is not None:
             position, named_expr = result
-            is_name = m.matches(updated_node.test, m.Name())
             self.add_change_from_position(position, self.change_description)
-            return (
-                updated_node.with_changes(test=named_expr)
-                if is_name
-                else updated_node.with_changes(
-                    test=updated_node.test.with_changes(left=named_expr)
-                )
-            )
+            match updated_node.test:
+                case cst.Name():
+                    return updated_node.with_changes(test=named_expr)
+                case cst.UnaryOperation():
+                    return updated_node.with_changes(
+                        test=updated_node.test.with_changes(expression=named_expr)
+                    )
+                case _:
+                    return updated_node.with_changes(
+                        test=updated_node.test.with_changes(left=named_expr)
+                    )
 
         return original_node
 
     def leave_Assign(self, original_node: cst.Assign, updated_node: cst.Assign):
         del updated_node
         if named_expr := self.assigns.get(original_node):
             position = self.node_position(original_node)
```

### Comparing `codemodder-0.88.0/src/core_codemods/with_threading_lock.py` & `codemodder-0.89.0/src/core_codemods/with_threading_lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class WithThreadingLock(SimpleCodemod, NameResolutionMixin):
     metadata = Metadata(
         name="bad-lock-with-statement",
         summary="Separate Lock Instantiation from `with` Call",
         review_guidance=ReviewGuidance.MERGE_WITHOUT_REVIEW,
         references=[
             Reference(
-                url="https://pylint.pycqa.org/en/latest/user_guide/messages/warning/useless-with-lock."
+                url="https://pylint.pycqa.org/en/latest/user_guide/messages/warning/useless-with-lock.html"
             ),
             Reference(
                 url="https://docs.python.org/3/library/threading.html#using-locks-conditions-and-semaphores-in-the-with-statement"
             ),
         ],
     )
     change_description = (
```

### Comparing `codemodder-0.88.0/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py` & `codemodder-0.89.0/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py` & `codemodder-0.89.0/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_add_requests_timeouts.py` & `codemodder-0.89.0/tests/codemods/test_add_requests_timeouts.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_async_fix_task_instantiation.py` & `codemodder-0.89.0/tests/codemods/test_async_fix_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_base_codemod.py` & `codemodder-0.89.0/tests/codemods/test_base_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_base_visitor.py` & `codemodder-0.89.0/tests/codemods/test_base_visitor.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_combine_startswith_endswith.py` & `codemodder-0.89.0/tests/codemods/test_combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_django_debug_flag_on.py` & `codemodder-0.89.0/tests/codemods/test_django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_django_json_response_type.py` & `codemodder-0.89.0/tests/codemods/test_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_django_model_without_dunder_str.py` & `codemodder-0.89.0/tests/codemods/test_django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_django_receiver_on_top.py` & `codemodder-0.89.0/tests/codemods/test_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_django_session_cookie_secure_off.py` & `codemodder-0.89.0/tests/codemods/test_django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_enable_jinja2_autoescape.py` & `codemodder-0.89.0/tests/codemods/test_enable_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_exception_without_raise.py` & `codemodder-0.89.0/tests/codemods/test_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_file_resource_leak.py` & `codemodder-0.89.0/tests/codemods/test_file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_fix_assert_tuple.py` & `codemodder-0.89.0/tests/codemods/test_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_fix_dataclass_defaults.py` & `codemodder-0.89.0/tests/codemods/test_fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_fix_deprecated_abstractproperty.py` & `codemodder-0.89.0/tests/codemods/test_fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_fix_deprecated_logging_warn.py` & `codemodder-0.89.0/tests/codemods/test_fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_fix_empty_sequence_comparison.py` & `codemodder-0.89.0/tests/codemods/test_fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_fix_hasattr_call.py` & `codemodder-0.89.0/tests/codemods/test_fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_fix_missing_self_or_cls.py` & `codemodder-0.89.0/tests/codemods/test_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_fix_mutable_params.py` & `codemodder-0.89.0/tests/codemods/test_fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_flask_enable_csrf_protection.py` & `codemodder-0.89.0/tests/codemods/test_flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_flask_json_response_type.py` & `codemodder-0.89.0/tests/codemods/test_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_harden_pickle_load.py` & `codemodder-0.89.0/tests/codemods/test_harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_harden_pyyaml.py` & `codemodder-0.89.0/tests/codemods/test_harden_pyyaml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_harden_ruamel.py` & `codemodder-0.89.0/tests/codemods/test_harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_https_connection.py` & `codemodder-0.89.0/tests/codemods/test_https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_include_exclude.py` & `codemodder-0.89.0/tests/codemods/test_include_exclude.py`

 * *Files 24% similar despite different names*

```diff
@@ -85,7 +85,54 @@
 
     def test_exclude_some_match(self):
         assert self.registry.match_codemods(None, ["doesntexist", "secure-random"]) == [
             c
             for c in self.registry.codemods
             if c.name not in "secure-random" and c.id in self.all_ids
         ]
+
+    def test_include_with_pattern(self):
+        assert self.registry.match_codemods(["*django*"], None) == [
+            c for c in self.registry.codemods if "django" in c.id
+        ]
+
+    def test_include_with_pattern_and_another(self):
+        assert self.registry.match_codemods(["*django*", "use-defusedxml"], None) == [
+            c for c in self.registry.codemods if "django" in c.id
+        ] + [self.codemod_map["use-defusedxml"]]
+
+    def test_include_sast_with_prefix(self):
+        assert self.registry.match_codemods(["sonar*"], None, sast_only=False) == [
+            c for c in self.registry.codemods if c.origin == "sonar"
+        ]
+
+    def test_warn_pattern_no_match(self, caplog):
+        assert self.registry.match_codemods(["*doesntexist*"], None) == []
+        assert (
+            "Given codemod pattern '*doesntexist*' does not match any codemods"
+            in caplog.text
+        )
+
+    def test_exclude_with_pattern(self):
+        assert self.registry.match_codemods(None, ["*django*"], sast_only=False) == [
+            c
+            for c in self.registry.codemods
+            if "django" not in c.id and c.id in self.all_ids
+        ]
+
+    def test_exclude_with_pattern_and_another(self):
+        assert self.registry.match_codemods(
+            None, ["*django*", "use-defusedxml"], sast_only=False
+        ) == [
+            c
+            for c in self.registry.codemods
+            if "django" not in c.id
+            and c.id in self.all_ids
+            and c.name != "use-defusedxml"
+        ]
+
+    def test_exclude_pixee_with_prefix(self):
+        assert self.registry.match_codemods(None, ["pixee*"], sast_only=False) == [
+            c
+            for c in self.registry.codemods
+            if not c.origin == "pixee" and c.id in self.all_ids
+        ]
```

### Comparing `codemodder-0.88.0/tests/codemods/test_jwt_decode_verify.py` & `codemodder-0.89.0/tests/codemods/test_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_lazy_logging.py` & `codemodder-0.89.0/tests/codemods/test_lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_limit_readline.py` & `codemodder-0.89.0/tests/codemods/test_limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_literal_or_new_object_identity.py` & `codemodder-0.89.0/tests/codemods/test_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_lxml_safe_parameter_defaults.py` & `codemodder-0.89.0/tests/codemods/test_lxml_safe_parameter_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_lxml_safe_parsing.py` & `codemodder-0.89.0/tests/codemods/test_lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_numpy_nan_equality.py` & `codemodder-0.89.0/tests/codemods/test_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_order_imports.py` & `codemodder-0.89.0/tests/codemods/test_order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_process_creation_sandbox.py` & `codemodder-0.89.0/tests/codemods/test_process_creation_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_remove_assertion_in_pytest_raises.py` & `codemodder-0.89.0/tests/codemods/test_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_remove_debug_breakpoint.py` & `codemodder-0.89.0/tests/codemods/test_remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_remove_future_imports.py` & `codemodder-0.89.0/tests/codemods/test_remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_remove_module_global.py` & `codemodder-0.89.0/tests/codemods/test_remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_remove_unnecessary_f_str.py` & `codemodder-0.89.0/tests/codemods/test_remove_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_remove_unused_imports.py` & `codemodder-0.89.0/tests/codemods/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_replace_flask_send_file.py` & `codemodder-0.89.0/tests/codemods/test_replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_request_verify.py` & `codemodder-0.89.0/tests/codemods/test_request_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_secure_flask_cookie.py` & `codemodder-0.89.0/tests/codemods/test_secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_secure_flask_session_config.py` & `codemodder-0.89.0/tests/codemods/test_secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_secure_random.py` & `codemodder-0.89.0/tests/codemods/test_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_django_json_response_type.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_django_receiver_on_top.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_enable_jinja2_autoescape.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_enable_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_exception_without_raise.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_fix_assert_tuple.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_fix_missing_self_or_cls.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_flask_json_response_type.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_jwt_decode_verify.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_literal_or_new_object_identity.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_numpy_nan_equality.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_remove_assertion_in_pytest_raises.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_secure_random.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sonar_tempfile_mktemp.py` & `codemodder-0.89.0/tests/codemods/sonar/test_sonar_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_sql_parameterization.py` & `codemodder-0.89.0/tests/codemods/test_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_str_concat_in_seq_literal.py` & `codemodder-0.89.0/tests/codemods/test_str_concat_in_seq_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_subprocess_shell_false.py` & `codemodder-0.89.0/tests/codemods/test_subprocess_shell_false.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_tempfile_mktemp.py` & `codemodder-0.89.0/tests/codemods/test_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py` & `codemodder-0.89.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_upgrade_sslcontext_tls.py` & `codemodder-0.89.0/tests/codemods/test_upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_url_sandbox.py` & `codemodder-0.89.0/tests/codemods/test_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_use_defused_xml.py` & `codemodder-0.89.0/tests/codemods/test_use_defused_xml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_use_generator.py` & `codemodder-0.89.0/tests/codemods/test_use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_use_set_literal.py` & `codemodder-0.89.0/tests/codemods/test_use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/codemods/test_walrus_if.py` & `codemodder-0.89.0/tests/codemods/test_walrus_if.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,26 @@
         """
         expected_output = """
         if val := do_something():
             do_something_else(val)
         """
         self.run_and_assert(tmpdir, input_code, expected_output)
 
+    def test_walrus_if_not(self, tmpdir):
+        input_code = """
+        val = do_something()
+        if not val:
+            do_something_else(val)
+        """
+        expected_output = """
+        if not (val := do_something()):
+            do_something_else(val)
+        """
+        self.run_and_assert(tmpdir, input_code, expected_output)
+
     def test_walrus_if_preserve_comments(self, tmpdir):
         input_code = """
         val = do_something() # comment
         if val is not None: # another comment
             do_something_else(val)
         """
         expected_output = """
```

### Comparing `codemodder-0.88.0/tests/codemods/test_with_threading_lock.py` & `codemodder-0.89.0/tests/codemods/test_with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/conftest.py` & `codemodder-0.89.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/dependency_management/test_base_dependency_writer.py` & `codemodder-0.89.0/tests/dependency_management/test_base_dependency_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/dependency_management/test_dependency_manager.py` & `codemodder-0.89.0/tests/dependency_management/test_dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/dependency_management/test_pyproject_writer.py` & `codemodder-0.89.0/tests/dependency_management/test_pyproject_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/dependency_management/test_requirements_txt_writer.py` & `codemodder-0.89.0/tests/dependency_management/test_requirements_txt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/dependency_management/test_setup_py_writer.py` & `codemodder-0.89.0/tests/dependency_management/test_setup_py_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/dependency_management/test_setupcfgt_writer.py` & `codemodder-0.89.0/tests/dependency_management/test_setupcfgt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py` & `codemodder-0.89.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py` & `codemodder-0.89.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py` & `codemodder-0.89.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py` & `codemodder-0.89.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/samples/semgrep.sarif` & `codemodder-0.89.0/tests/samples/semgrep.sarif`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/samples/sonar_hotspots.json` & `codemodder-0.89.0/tests/samples/sonar_hotspots.json`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/samples/sonar_issues.json` & `codemodder-0.89.0/tests/samples/sonar_issues.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9474358974358974%*

 * *Differences: {"'issues'": "{insert: [(37, OrderedDict([('key', 'AY6o8XTbdw-0_54hqn7F'), ('rule', "*

 * *             "'pythonsecurity:S5144'), ('severity', 'MAJOR'), ('component', "*

 * *             "'pixee_codemodder-python:flask_request.py'), ('project', 'pixee_codemodder-python'), "*

 * *             "('line', 10), ('hash', 'c864c19608fe39f9e580a5deefb67381'), ('textRange', "*

 * *             "OrderedDict([('startLine', 10), ('endLine', 10), ('startOffset', 4), ('endOffset', "*

 * *             "21)])), ('flows', [OrderedDict([('locations' […]*

```diff
@@ -2478,14 +2478,119 @@
                 "endLine": 23,
                 "endOffset": 80,
                 "startLine": 23,
                 "startOffset": 14
             },
             "type": "VULNERABILITY",
             "updateDate": "2023-12-12T19:21:07+0100"
+        },
+        {
+            "assignee": "clavedeluna@github",
+            "cleanCodeAttribute": "COMPLETE",
+            "cleanCodeAttributeCategory": "INTENTIONAL",
+            "component": "pixee_codemodder-python:flask_request.py",
+            "creationDate": "2024-04-04T13:49:07+0200",
+            "debt": "30min",
+            "effort": "30min",
+            "flows": [
+                {
+                    "locations": [
+                        {
+                            "component": "pixee_codemodder-python:flask_request.py",
+                            "msg": "Sink: this invocation is not safe; a malicious value can be used as argument",
+                            "textRange": {
+                                "endLine": 10,
+                                "endOffset": 21,
+                                "startLine": 10,
+                                "startOffset": 4
+                            }
+                        },
+                        {
+                            "component": "pixee_codemodder-python:flask_request.py",
+                            "msg": "A malicious value can be assigned to variable \u2018url\u2019",
+                            "textRange": {
+                                "endLine": 9,
+                                "endOffset": 29,
+                                "startLine": 9,
+                                "startOffset": 4
+                            }
+                        },
+                        {
+                            "component": "pixee_codemodder-python:flask_request.py",
+                            "msg": "Source: a user can craft an HTTP request with malicious content",
+                            "textRange": {
+                                "endLine": 9,
+                                "endOffset": 29,
+                                "startLine": 9,
+                                "startOffset": 10
+                            }
+                        }
+                    ]
+                }
+            ],
+            "hash": "c864c19608fe39f9e580a5deefb67381",
+            "impacts": [
+                {
+                    "severity": "MEDIUM",
+                    "softwareQuality": "SECURITY"
+                }
+            ],
+            "key": "AY6o8XTbdw-0_54hqn7F",
+            "line": 10,
+            "message": "Change this code to not construct the URL from user-controlled data.",
+            "organization": "pixee",
+            "project": "pixee_codemodder-python",
+            "pullRequest": "445",
+            "rule": "pythonsecurity:S5144",
+            "severity": "MAJOR",
+            "status": "OPEN",
+            "tags": [
+                "cwe"
+            ],
+            "textRange": {
+                "endLine": 10,
+                "endOffset": 21,
+                "startLine": 10,
+                "startOffset": 4
+            },
+            "type": "VULNERABILITY",
+            "updateDate": "2024-04-04T13:49:25+0200"
+        },
+        {
+            "assignee": "clavedeluna@github",
+            "cleanCodeAttributeCategory": "INTENTIONAL",
+            "component": "pixee_codemodder-python:fix_float_equality.py",
+            "creationDate": "2024-04-06T21:36:46+0200",
+            "debt": "5min",
+            "effort": "5min",
+            "flows": [],
+            "hash": "4f98731d8aeb7e5d80e02d5ab1fd1ad8",
+            "impacts": [
+                {
+                    "severity": "MEDIUM",
+                    "softwareQuality": "RELIABILITY"
+                }
+            ],
+            "key": "AY606lcc6hXAwyuO7dPZ",
+            "line": 7,
+            "message": "Do not perform equality checks with floating point values.",
+            "organization": "pixee",
+            "project": "pixee_codemodder-python",
+            "rule": "python:S1244",
+            "severity": "MAJOR",
+            "status": "OPEN",
+            "tags": [],
+            "textRange": {
+                "endLine": 2,
+                "endOffset": 23,
+                "startLine": 2,
+                "startOffset": 11
+            },
+            "type": "BUG",
+            "updateDate": "2024-04-06T21:37:06+0200"
         }
     ],
     "organizations": [
         {
             "key": "pixee",
             "name": "Pixee"
         }
@@ -2493,9 +2598,9 @@
     "p": 1,
     "paging": {
         "pageIndex": 1,
         "pageSize": 500,
         "total": 170
     },
     "ps": 500,
-    "total": 37
+    "total": 39
 }
```

### Comparing `codemodder-0.88.0/tests/samples/webgoat_v8.2.0_codeql.sarif` & `codemodder-0.89.0/tests/samples/webgoat_v8.2.0_codeql.sarif`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/test_ancestorpatterns_mixin.py` & `codemodder-0.89.0/tests/test_ancestorpatterns_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/test_basetype.py` & `codemodder-0.89.0/tests/test_basetype.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/test_cli.py` & `codemodder-0.89.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/test_code_directory.py` & `codemodder-0.89.0/tests/test_code_directory.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/test_codemod_docs.py` & `codemodder-0.89.0/tests/test_codemod_docs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from codemodder.codemods.api import BaseCodemod
 from codemodder.registry import load_registered_codemods
-from codemodder.scripts.generate_docs import METADATA
+from codemodder.scripts.generate_docs import ALL_CODEMODS_METADATA
 
 
 def pytest_generate_tests(metafunc):
     registry = load_registered_codemods()
     if "codemod" in metafunc.fixturenames:
         metafunc.parametrize("codemod", registry.codemods)
 
@@ -17,8 +17,8 @@
 
     assert codemod.description
     assert codemod.review_guidance in (
         "Merge After Review",
         "Merge After Cursory Review",
         "Merge Without Review",
     )
-    assert codemod.name in METADATA
+    assert codemod.name in ALL_CODEMODS_METADATA
```

### Comparing `codemodder-0.88.0/tests/test_codemodder.py` & `codemodder-0.89.0/tests/test_codemodder.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         run(args)
         write_report.assert_called_once()
 
         assert any("no codemods to run" in x[0][0] for x in info_logger.call_args_list)
         assert any(x[0] == ("scanned: %s files", 0) for x in info_logger.call_args_list)
 
         assert any(
-            f"Requested codemod to include'{bad_codemod}' does not exist." in x[0][0]
+            f"Requested codemod to include '{bad_codemod}' does not exist." in x[0][0]
             for x in warning_logger.call_args_list
         )
 
     @mock.patch("codemodder.registry.logger.warning")
     @mock.patch("codemodder.codemodder.logger.info")
     @mock.patch("codemodder.codetf.CodeTF.write_report")
     def test_codemod_include_some_match(
@@ -229,15 +229,15 @@
             str(codetf),
             f"--codemod-include={bad_codemod},{good_codemod}",
         ]
         run(args)
         write_report.assert_called_once()
         assert any("running codemod %s" in x[0][0] for x in info_logger.call_args_list)
         assert any(
-            f"Requested codemod to include'{bad_codemod}' does not exist." in x[0][0]
+            f"Requested codemod to include '{bad_codemod}' does not exist." in x[0][0]
             for x in warning_logger.call_args_list
         )
 
     @mock.patch("codemodder.registry.logger.warning")
     @mock.patch("codemodder.codemodder.logger.info")
     @mock.patch("codemodder.codetf.CodeTF.write_report")
     def test_codemod_exclude_some_match(
@@ -258,18 +258,14 @@
             x[0][1]
             for x in info_logger.call_args_list
             if x[0][0] == "running codemod %s"
         ]
 
         assert f"pixee:python/{good_codemod}" not in codemods_that_ran
         assert any("running codemod %s" in x[0][0] for x in info_logger.call_args_list)
-        assert any(
-            f"Requested codemod to exclude'{bad_codemod}' does not exist." in x[0][0]
-            for x in warning_logger.call_args_list
-        )
 
     @mock.patch("codemodder.registry.logger.warning")
     @mock.patch("codemodder.codemodder.logger.info")
     @mock.patch("codemodder.codetf.CodeTF.write_report")
     @mock.patch("codemodder.codemods.base_codemod.BaseCodemod.apply")
     def test_codemod_exclude_no_match(
         self, apply, write_report, info_logger, warning_logger, dir_structure
@@ -282,18 +278,14 @@
             str(codetf),
             f"--codemod-exclude={bad_codemod}",
         ]
 
         run(args)
         write_report.assert_called_once()
         assert any("running codemod %s" in x[0][0] for x in info_logger.call_args_list)
-        assert any(
-            f"Requested codemod to exclude'{bad_codemod}' does not exist." in x[0][0]
-            for x in warning_logger.call_args_list
-        )
 
     @mock.patch("codemodder.codemods.semgrep.semgrep_run")
     def test_exclude_all_registered_codemods(self, mock_semgrep_run, dir_structure):
         code_dir, codetf = dir_structure
         assert not codetf.exists()
 
         registry = load_registered_codemods()
```

### Comparing `codemodder-0.88.0/tests/test_codetf.py` & `codemodder-0.89.0/tests/test_codetf.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/test_context.py` & `codemodder-0.89.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/test_format_string_parser.py` & `codemodder-0.89.0/tests/test_format_string_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/test_linearize_string_expression.py` & `codemodder-0.89.0/tests/test_linearize_string_expression.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/test_logging.py` & `codemodder-0.89.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/test_nameresolution_mixin.py` & `codemodder-0.89.0/tests/test_nameresolution_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/test_results.py` & `codemodder-0.89.0/tests/test_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from pathlib import Path
 
-from codemodder.sonar_results import SonarResultSet
+from core_codemods.sonar.results import SonarResultSet
 
 
 class TestResults:
     def test_or(self, tmpdir):
         issues1 = {
             "issues": [
                 {
```

### Comparing `codemodder-0.88.0/tests/test_sarif_processing.py` & `codemodder-0.89.0/tests/test_sarif_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import subprocess
 from pathlib import Path
 
-from codemodder.sarifs import SarifResultSet, extract_rule_id
+from codemodder.semgrep import SemgrepResultSet, extract_rule_id
 
 
 class TestSarifProcessing:
     def test_extract_rule_id_codeql(self):
         sarif_file = Path("tests") / "samples" / "webgoat_v8.2.0_codeql.sarif"
 
         with open(sarif_file, "r", encoding="utf-8") as f:
@@ -27,15 +27,15 @@
         result = sarif_run["results"][0]
         rule_id = extract_rule_id(result, sarif_run)
         assert rule_id == "secure-random"
 
     def test_results_by_rule_id(self):
         sarif_file = Path("tests") / "samples" / "semgrep.sarif"
 
-        results = SarifResultSet.from_sarif(sarif_file)
+        results = SemgrepResultSet.from_sarif(sarif_file)
         expected_rule = "secure-random"
         assert list(results.keys()) == [expected_rule]
 
         expected_path = Path("tests/samples/insecure_random.py")
         assert list(results[expected_rule].keys()) == [expected_path]
 
         assert results[expected_rule][expected_path][0].rule_id == expected_rule
```

### Comparing `codemodder-0.88.0/tests/transformations/test_clean_code.py` & `codemodder-0.89.0/tests/transformations/test_clean_code.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/transformations/test_remove_empty_string_concatenation.py` & `codemodder-0.89.0/tests/transformations/test_remove_empty_string_concatenation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.88.0/tests/transformations/test_remove_unused_imports.py` & `codemodder-0.89.0/tests/transformations/test_remove_unused_imports.py`

 * *Files identical despite different names*

