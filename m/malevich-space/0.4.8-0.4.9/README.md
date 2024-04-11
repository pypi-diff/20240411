# Comparing `tmp/malevich_space-0.4.8.tar.gz` & `tmp/malevich_space-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malevich_space-0.4.8.tar", max compression
+gzip compressed data, was "malevich_space-0.4.9.tar", max compression
```

## Comparing `malevich_space-0.4.8.tar` & `malevich_space-0.4.9.tar`

### file list

```diff
@@ -1,115 +1,116 @@
--rw-r--r--   0        0        0    11357 2023-12-17 18:18:58.992055 malevich_space-0.4.8/LICENSE
--rw-r--r--   0        0        0        0 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/__init__.py
--rw-r--r--   0        0        0       92 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/ci/__init__.py
--rw-r--r--   0        0        0     4388 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/ci/manager.py
--rw-r--r--   0        0        0       70 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/ci/platform.py
--rw-r--r--   0        0        0      375 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/ci/report.py
--rw-r--r--   0        0        0       64 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/ci/status.py
--rw-r--r--   0        0        0        0 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/cli/__init__.py
--rw-r--r--   0        0        0      385 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/cli/cli.py
--rw-r--r--   0        0        0      158 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/cli/commands/__init__.py
--rw-r--r--   0        0        0     1714 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/cli/commands/ci.py
--rw-r--r--   0        0        0     4671 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/cli/commands/component.py
--rw-r--r--   0        0        0     1032 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/cli/commands/env.py
--rw-r--r--   0        0        0      426 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/cli/commands/schema.py
--rw-r--r--   0        0        0     1269 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/cli/commands/team.py
--rw-r--r--   0        0        0      573 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/constants.py
--rw-r--r--   0        0        0      211 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/__init__.py
--rw-r--r--   0        0        0       35 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/api_key/__init__.py
--rw-r--r--   0        0        0      224 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/api_key/get_api_key_by_name.py
--rw-r--r--   0        0        0       60 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/cfg/__init__.py
--rw-r--r--   0        0        0      376 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/cfg/cfg.py
--rw-r--r--   0        0        0      452 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/cfg/set_in_flow_component_cfg.py
--rw-r--r--   0        0        0      105 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/collection/__init__.py
--rw-r--r--   0        0        0      382 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/collection/ca_comp.py
--rw-r--r--   0        0        0      430 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/collection/ca_in_flow.py
--rw-r--r--   0        0        0      574 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/collection/collection_alias.py
--rw-r--r--   0        0        0      272 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/collection/update_ca.py
--rw-r--r--   0        0        0      619 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/__init__.py
--rw-r--r--   0        0        0      489 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/add_app_to_comp_flow.py
--rw-r--r--   0        0        0      496 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/add_ca_to_comp_flow.py
--rw-r--r--   0        0        0      328 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/add_cfg_2_av_app.py
--rw-r--r--   0        0        0      980 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/add_comp_in_flow.py
--rw-r--r--   0        0        0      422 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/add_dep_2_op.py
--rw-r--r--   0        0        0      442 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/add_op_to_av.py
--rw-r--r--   0        0        0      264 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/add_tag.py
--rw-r--r--   0        0        0      708 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/app_comp.py
--rw-r--r--   0        0        0      233 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/attach_tag_to_comp.py
--rw-r--r--   0        0        0      494 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/branch.py
--rw-r--r--   0        0        0     1523 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/component.py
--rw-r--r--   0        0        0      454 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/create_op.py
--rw-r--r--   0        0        0      242 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/flow_by_version_id.py
--rw-r--r--   0        0        0      423 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/flow_comp.py
--rw-r--r--   0        0        0      574 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/get_branch_by_name.py
--rw-r--r--   0        0        0     3641 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/get_comp_by_reverse_id.py
--rw-r--r--   0        0        0      642 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/invoke.py
--rw-r--r--   0        0        0     1095 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/link.py
--rw-r--r--   0        0        0      444 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/select_op_in_flow.py
--rw-r--r--   0        0        0     1354 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/update.py
--rw-r--r--   0        0        0      675 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/version.py
--rw-r--r--   0        0        0      206 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/component/wipe.py
--rw-r--r--   0        0        0      208 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/environment/__init__.py
--rw-r--r--   0        0        0      750 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/environment/add_user_secret.py
--rw-r--r--   0        0        0      591 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/environment/create_host.py
--rw-r--r--   0        0        0      699 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/environment/get_host.py
--rw-r--r--   0        0        0      166 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/environment/get_me.py
--rw-r--r--   0        0        0      572 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/environment/get_user_secret.py
--rw-r--r--   0        0        0      357 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/environment/invite_org.py
--rw-r--r--   0        0        0      222 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/environment/org.py
--rw-r--r--   0        0        0      412 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/environment/org_create.py
--rw-r--r--   0        0        0      112 2023-12-17 18:18:58.992055 malevich_space-0.4.8/malevich_space/gql/malevich/__init__.py
--rw-r--r--   0        0        0      839 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/malevich/add_pt.py
--rw-r--r--   0        0        0     1039 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/malevich/get_prompt_flow.py
--rw-r--r--   0        0        0     1756 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/malevich/regenerate.py
--rw-r--r--   0        0        0      690 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/malevich/subscribe_to_flow.py
--rw-r--r--   0        0        0       90 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/schema/__init__.py
--rw-r--r--   0        0        0      718 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/schema/create_schema_alias.py
--rw-r--r--   0        0        0      410 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/schema/create_scheme.py
--rw-r--r--   0        0        0      258 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/schema/get_schema.py
--rw-r--r--   0        0        0      215 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/task/__init__.py
--rw-r--r--   0        0        0      340 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/task/boot.py
--rw-r--r--   0        0        0      279 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/task/build.py
--rw-r--r--   0        0        0      284 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/task/change_state.py
--rw-r--r--   0        0        0      507 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/task/create_endpoint.py
--rw-r--r--   0        0        0      678 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/task/get_results.py
--rw-r--r--   0        0        0      380 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/task/run.py
--rw-r--r--   0        0        0      498 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/task/run_shaphost_components.py
--rw-r--r--   0        0        0      254 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/task/start_schema.py
--rw-r--r--   0        0        0       44 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/use_case/__init__.py
--rw-r--r--   0        0        0      332 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/use_case/attach.py
--rw-r--r--   0        0        0      372 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/gql/use_case/create.py
--rw-r--r--   0        0        0       77 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/ops/__init__.py
--rw-r--r--   0        0        0    15699 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/ops/component_manager.py
--rw-r--r--   0        0        0       66 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/ops/component_provider/__init__.py
--rw-r--r--   0        0        0      365 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/ops/component_provider/base.py
--rw-r--r--   0        0        0     1067 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/ops/component_provider/component.py
--rw-r--r--   0        0        0      725 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/ops/component_provider/local.py
--rw-r--r--   0        0        0      763 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/ops/env.py
--rw-r--r--   0        0        0     4770 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/ops/roller.py
--rw-r--r--   0        0        0       30 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/ops/service/__init__.py
--rw-r--r--   0        0        0     6817 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/ops/service/base.py
--rw-r--r--   0        0        0    25288 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/ops/space.py
--rw-r--r--   0        0        0       56 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/parser/__init__.py
--rw-r--r--   0        0        0      231 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/parser/abs.py
--rw-r--r--   0        0        0     8258 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/parser/yaml.py
--rw-r--r--   0        0        0      379 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/__init__.py
--rw-r--r--   0        0        0      300 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/branch.py
--rw-r--r--   0        0        0      225 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/cfg.py
--rw-r--r--   0        0        0      277 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/collection_alias.py
--rw-r--r--   0        0        0     3327 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/component.py
--rw-r--r--   0        0        0      168 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/dep.py
--rw-r--r--   0        0        0     2011 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/flow.py
--rw-r--r--   0        0        0      347 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/host.py
--rw-r--r--   0        0        0      967 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/op.py
--rw-r--r--   0        0        0      180 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/org.py
--rw-r--r--   0        0        0      235 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/payload.py
--rw-r--r--   0        0        0      215 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/result.py
--rw-r--r--   0        0        0      195 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/sa.py
--rw-r--r--   0        0        0      215 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/schema.py
--rw-r--r--   0        0        0     1517 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/setup.py
--rw-r--r--   0        0        0       77 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/stand.py
--rw-r--r--   0        0        0      276 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/task.py
--rw-r--r--   0        0        0      450 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/version.py
--rw-r--r--   0        0        0      133 2023-12-17 18:18:58.996055 malevich_space-0.4.8/malevich_space/schema/version_mode.py
--rw-r--r--   0        0        0     1546 2023-12-17 18:18:58.996055 malevich_space-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 malevich_space-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-19 12:02:36.109504 malevich_space-0.4.9/LICENSE
+-rw-r--r--   0        0        0        0 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/__init__.py
+-rw-r--r--   0        0        0       92 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/ci/__init__.py
+-rw-r--r--   0        0        0     4388 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/ci/manager.py
+-rw-r--r--   0        0        0       70 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/ci/platform.py
+-rw-r--r--   0        0        0      375 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/ci/report.py
+-rw-r--r--   0        0        0       64 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/ci/status.py
+-rw-r--r--   0        0        0        0 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/cli/__init__.py
+-rw-r--r--   0        0        0      385 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/cli/cli.py
+-rw-r--r--   0        0        0      158 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1714 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/cli/commands/ci.py
+-rw-r--r--   0        0        0     4671 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/cli/commands/component.py
+-rw-r--r--   0        0        0     1032 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/cli/commands/env.py
+-rw-r--r--   0        0        0      426 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/cli/commands/schema.py
+-rw-r--r--   0        0        0     1269 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/cli/commands/team.py
+-rw-r--r--   0        0        0      573 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/constants.py
+-rw-r--r--   0        0        0      211 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/gql/__init__.py
+-rw-r--r--   0        0        0       35 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/gql/api_key/__init__.py
+-rw-r--r--   0        0        0      224 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/gql/api_key/get_api_key_by_name.py
+-rw-r--r--   0        0        0       60 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/gql/cfg/__init__.py
+-rw-r--r--   0        0        0      376 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/gql/cfg/cfg.py
+-rw-r--r--   0        0        0      452 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/gql/cfg/set_in_flow_component_cfg.py
+-rw-r--r--   0        0        0      105 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/gql/collection/__init__.py
+-rw-r--r--   0        0        0      382 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/gql/collection/ca_comp.py
+-rw-r--r--   0        0        0      430 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/gql/collection/ca_in_flow.py
+-rw-r--r--   0        0        0      574 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/gql/collection/collection_alias.py
+-rw-r--r--   0        0        0      272 2023-12-19 12:02:36.109504 malevich_space-0.4.9/malevich_space/gql/collection/update_ca.py
+-rw-r--r--   0        0        0      651 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/__init__.py
+-rw-r--r--   0        0        0      489 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/add_app_to_comp_flow.py
+-rw-r--r--   0        0        0      496 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/add_ca_to_comp_flow.py
+-rw-r--r--   0        0        0      328 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/add_cfg_2_av_app.py
+-rw-r--r--   0        0        0      980 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/add_comp_in_flow.py
+-rw-r--r--   0        0        0      296 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/add_comp_to_org.py
+-rw-r--r--   0        0        0      422 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/add_dep_2_op.py
+-rw-r--r--   0        0        0      442 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/add_op_to_av.py
+-rw-r--r--   0        0        0      264 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/add_tag.py
+-rw-r--r--   0        0        0      708 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/app_comp.py
+-rw-r--r--   0        0        0      233 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/attach_tag_to_comp.py
+-rw-r--r--   0        0        0      494 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/branch.py
+-rw-r--r--   0        0        0     1523 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/component.py
+-rw-r--r--   0        0        0      454 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/create_op.py
+-rw-r--r--   0        0        0      242 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/flow_by_version_id.py
+-rw-r--r--   0        0        0      423 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/flow_comp.py
+-rw-r--r--   0        0        0      574 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/get_branch_by_name.py
+-rw-r--r--   0        0        0     3641 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/get_comp_by_reverse_id.py
+-rw-r--r--   0        0        0      642 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/invoke.py
+-rw-r--r--   0        0        0     1095 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/link.py
+-rw-r--r--   0        0        0      444 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/select_op_in_flow.py
+-rw-r--r--   0        0        0     1354 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/update.py
+-rw-r--r--   0        0        0      675 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/version.py
+-rw-r--r--   0        0        0      206 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/component/wipe.py
+-rw-r--r--   0        0        0      208 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/environment/__init__.py
+-rw-r--r--   0        0        0      750 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/environment/add_user_secret.py
+-rw-r--r--   0        0        0      591 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/environment/create_host.py
+-rw-r--r--   0        0        0      699 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/environment/get_host.py
+-rw-r--r--   0        0        0      166 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/environment/get_me.py
+-rw-r--r--   0        0        0      572 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/environment/get_user_secret.py
+-rw-r--r--   0        0        0      357 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/environment/invite_org.py
+-rw-r--r--   0        0        0      222 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/environment/org.py
+-rw-r--r--   0        0        0      412 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/environment/org_create.py
+-rw-r--r--   0        0        0      112 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/malevich/__init__.py
+-rw-r--r--   0        0        0      839 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/malevich/add_pt.py
+-rw-r--r--   0        0        0     1039 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/malevich/get_prompt_flow.py
+-rw-r--r--   0        0        0     1756 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/malevich/regenerate.py
+-rw-r--r--   0        0        0      690 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/malevich/subscribe_to_flow.py
+-rw-r--r--   0        0        0       90 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/schema/__init__.py
+-rw-r--r--   0        0        0      718 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/schema/create_schema_alias.py
+-rw-r--r--   0        0        0      410 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/schema/create_scheme.py
+-rw-r--r--   0        0        0      258 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/schema/get_schema.py
+-rw-r--r--   0        0        0      215 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/task/__init__.py
+-rw-r--r--   0        0        0      340 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/task/boot.py
+-rw-r--r--   0        0        0      279 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/task/build.py
+-rw-r--r--   0        0        0      284 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/task/change_state.py
+-rw-r--r--   0        0        0      507 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/task/create_endpoint.py
+-rw-r--r--   0        0        0      678 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/task/get_results.py
+-rw-r--r--   0        0        0      380 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/task/run.py
+-rw-r--r--   0        0        0      498 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/task/run_shaphost_components.py
+-rw-r--r--   0        0        0      254 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/task/start_schema.py
+-rw-r--r--   0        0        0       44 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/use_case/__init__.py
+-rw-r--r--   0        0        0      332 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/use_case/attach.py
+-rw-r--r--   0        0        0      372 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/gql/use_case/create.py
+-rw-r--r--   0        0        0       77 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/ops/__init__.py
+-rw-r--r--   0        0        0    15823 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/ops/component_manager.py
+-rw-r--r--   0        0        0       66 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/ops/component_provider/__init__.py
+-rw-r--r--   0        0        0      365 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/ops/component_provider/base.py
+-rw-r--r--   0        0        0     1067 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/ops/component_provider/component.py
+-rw-r--r--   0        0        0      725 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/ops/component_provider/local.py
+-rw-r--r--   0        0        0      763 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/ops/env.py
+-rw-r--r--   0        0        0     4770 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/ops/roller.py
+-rw-r--r--   0        0        0       30 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/ops/service/__init__.py
+-rw-r--r--   0        0        0     6947 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/ops/service/base.py
+-rw-r--r--   0        0        0    25689 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/ops/space.py
+-rw-r--r--   0        0        0       56 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/parser/__init__.py
+-rw-r--r--   0        0        0      231 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/parser/abs.py
+-rw-r--r--   0        0        0     8258 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/parser/yaml.py
+-rw-r--r--   0        0        0      379 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/__init__.py
+-rw-r--r--   0        0        0      300 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/branch.py
+-rw-r--r--   0        0        0      225 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/cfg.py
+-rw-r--r--   0        0        0      277 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/collection_alias.py
+-rw-r--r--   0        0        0     3327 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/component.py
+-rw-r--r--   0        0        0      168 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/dep.py
+-rw-r--r--   0        0        0     2011 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/flow.py
+-rw-r--r--   0        0        0      347 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/host.py
+-rw-r--r--   0        0        0      967 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/op.py
+-rw-r--r--   0        0        0      180 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/org.py
+-rw-r--r--   0        0        0      235 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/payload.py
+-rw-r--r--   0        0        0      215 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/result.py
+-rw-r--r--   0        0        0      195 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/sa.py
+-rw-r--r--   0        0        0      215 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/schema.py
+-rw-r--r--   0        0        0     1517 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/setup.py
+-rw-r--r--   0        0        0       77 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/stand.py
+-rw-r--r--   0        0        0      276 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/task.py
+-rw-r--r--   0        0        0      450 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/version.py
+-rw-r--r--   0        0        0      133 2023-12-19 12:02:36.113504 malevich_space-0.4.9/malevich_space/schema/version_mode.py
+-rw-r--r--   0        0        0     1546 2023-12-19 12:02:36.113504 malevich_space-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 malevich_space-0.4.9/PKG-INFO
```

### Comparing `malevich_space-0.4.8/LICENSE` & `malevich_space-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/ci/manager.py` & `malevich_space-0.4.9/malevich_space/ci/manager.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/cli/commands/ci.py` & `malevich_space-0.4.9/malevich_space/cli/commands/ci.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/cli/commands/component.py` & `malevich_space-0.4.9/malevich_space/cli/commands/component.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/cli/commands/env.py` & `malevich_space-0.4.9/malevich_space/cli/commands/env.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/cli/commands/team.py` & `malevich_space-0.4.9/malevich_space/cli/commands/team.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/constants.py` & `malevich_space-0.4.9/malevich_space/constants.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/collection/collection_alias.py` & `malevich_space-0.4.9/malevich_space/gql/collection/collection_alias.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/component/__init__.py` & `malevich_space-0.4.9/malevich_space/gql/component/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,7 +20,9 @@
 from .wipe import *
 
 from .flow_by_version_id import *
 
 from .invoke import *
 
 from .update import *
+
+from .add_comp_to_org import *
```

### Comparing `malevich_space-0.4.8/malevich_space/gql/component/add_comp_in_flow.py` & `malevich_space-0.4.9/malevich_space/gql/component/add_comp_in_flow.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/component/app_comp.py` & `malevich_space-0.4.9/malevich_space/gql/component/app_comp.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/component/component.py` & `malevich_space-0.4.9/malevich_space/gql/component/component.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/component/get_branch_by_name.py` & `malevich_space-0.4.9/malevich_space/gql/component/get_branch_by_name.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/component/get_comp_by_reverse_id.py` & `malevich_space-0.4.9/malevich_space/gql/component/get_comp_by_reverse_id.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/component/invoke.py` & `malevich_space-0.4.9/malevich_space/gql/component/invoke.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/component/link.py` & `malevich_space-0.4.9/malevich_space/gql/component/link.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/component/update.py` & `malevich_space-0.4.9/malevich_space/gql/component/update.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/component/version.py` & `malevich_space-0.4.9/malevich_space/gql/component/version.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/environment/add_user_secret.py` & `malevich_space-0.4.9/malevich_space/gql/environment/add_user_secret.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/environment/create_host.py` & `malevich_space-0.4.9/malevich_space/gql/environment/create_host.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/environment/get_host.py` & `malevich_space-0.4.9/malevich_space/gql/environment/get_host.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/environment/get_user_secret.py` & `malevich_space-0.4.9/malevich_space/gql/environment/get_user_secret.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/malevich/add_pt.py` & `malevich_space-0.4.9/malevich_space/gql/malevich/add_pt.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/malevich/get_prompt_flow.py` & `malevich_space-0.4.9/malevich_space/gql/malevich/get_prompt_flow.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/malevich/regenerate.py` & `malevich_space-0.4.9/malevich_space/gql/malevich/regenerate.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/malevich/subscribe_to_flow.py` & `malevich_space-0.4.9/malevich_space/gql/malevich/subscribe_to_flow.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/schema/create_schema_alias.py` & `malevich_space-0.4.9/malevich_space/gql/schema/create_schema_alias.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/gql/task/get_results.py` & `malevich_space-0.4.9/malevich_space/gql/task/get_results.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/ops/component_manager.py` & `malevich_space-0.4.9/malevich_space/ops/component_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,14 +302,16 @@
             if comp.version.updates_markdown:
                 version_update_md = comp.version.updates_markdown
             if comp.version.status:
                 version_status = comp.version.status
             commit_digest = comp.version.commit_digest
         if loaded:
             self.update_component(loaded=loaded, update_comp=comp)
+            if org_id := self.space.org_id():
+                self.space.add_comp_to_org(comp_id=loaded.uid, org_id=org_id)
             if version_mode == schema.VersionMode.DEFAULT:
                 return loaded
             else:
                 old_version_name = None
                 if comp.branch and comp.branch.name:
                     branch = self.space.get_branch_by_name(
                         component_id=loaded.uid, branch_name=comp.branch.name
```

### Comparing `malevich_space-0.4.8/malevich_space/ops/component_provider/component.py` & `malevich_space-0.4.9/malevich_space/ops/component_provider/component.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/ops/component_provider/local.py` & `malevich_space-0.4.9/malevich_space/ops/component_provider/local.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/ops/env.py` & `malevich_space-0.4.9/malevich_space/ops/env.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/ops/roller.py` & `malevich_space-0.4.9/malevich_space/ops/roller.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/ops/service/base.py` & `malevich_space-0.4.9/malevich_space/ops/service/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,18 @@
         raise NotImplementedError
     
     @abstractmethod
     def update_component(self, *args, **kwargs) -> str:
         raise NotImplementedError
 
     @abstractmethod
+    def add_comp_to_org(self, *, comp_id: str, org_id: str) -> str | None:
+        raise NotImplementedError
+
+    @abstractmethod
     def create_component(
             self,
             name: str,
             type: str,
             description: str,
             reverse_id: str,
             repo_url: Optional[str] = None,
```

### Comparing `malevich_space-0.4.8/malevich_space/ops/space.py` & `malevich_space-0.4.9/malevich_space/ops/space.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,8 +585,18 @@
         }
         result = self.client.execute(client.invoke_component, variable_values=kwargs)
         if result["invoke"] is None:
             return None
         task = result["invoke"]["task"]
         run = result["invoke"]["run"]
         return task["details"]["uid"], run["details"]["uid"]
+    
+    def add_comp_to_org(self, *, comp_id: str, org_id: str) -> str | None:
+        kwargs = {
+            "comp_id": comp_id,
+            "org_id": org_id
+        }
+        result = self.client.execute(client.comp_to_org, variable_values=kwargs)
+        if "details" not in result["component"]["addToOrg"]:
+            return None
+        return result["component"]["addToOrg"]["details"]["uid"]
```

### Comparing `malevich_space-0.4.8/malevich_space/parser/yaml.py` & `malevich_space-0.4.9/malevich_space/parser/yaml.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/schema/component.py` & `malevich_space-0.4.9/malevich_space/schema/component.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/schema/flow.py` & `malevich_space-0.4.9/malevich_space/schema/flow.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/schema/op.py` & `malevich_space-0.4.9/malevich_space/schema/op.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/malevich_space/schema/setup.py` & `malevich_space-0.4.9/malevich_space/schema/setup.py`

 * *Files identical despite different names*

### Comparing `malevich_space-0.4.8/pyproject.toml` & `malevich_space-0.4.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "malevich-space"
-version = "0.4.8"
+version = "0.4.9"
 description = "SDK for Malevich Space"
 authors = ["Zak Davydov <zak@malevich.ai>"]
 license = "Apache 2"
 homepage = "https://github.com/MalevichAI/space"
 repository = "https://github.com/MalevichAI/space"
 
 [tool.poetry.dependencies]
```

### Comparing `malevich_space-0.4.8/PKG-INFO` & `malevich_space-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malevich-space
-Version: 0.4.8
+Version: 0.4.9
 Summary: SDK for Malevich Space
 Home-page: https://github.com/MalevichAI/space
 License: Apache 2
 Author: Zak Davydov
 Author-email: zak@malevich.ai
 Requires-Python: >=3.11,<3.13
 Classifier: License :: Other/Proprietary License
```

