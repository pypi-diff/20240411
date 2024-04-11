# Comparing `tmp/onnxscript-0.1.0.dev20240409.tar.gz` & `tmp/onnxscript-0.1.0.dev20240410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240409.tar", last modified: Tue Apr  9 00:01:51 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240410.tar", last modified: Wed Apr 10 00:01:02 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240409.tar` & `onnxscript-0.1.0.dev20240410.tar`

### file list

```diff
@@ -1,212 +1,213 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.924615 onnxscript-0.1.0.dev20240409/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-09 00:01:51.924615 onnxscript-0.1.0.dev20240409/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.896615 onnxscript-0.1.0.dev20240409/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2151 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.900615 onnxscript-0.1.0.dev20240409/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.900615 onnxscript-0.1.0.dev20240409/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11068 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8872 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_legacy_ir/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5929 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_legacy_ir/protobuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36193 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.900615 onnxscript-0.1.0.dev20240409/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10580 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.900615 onnxscript-0.1.0.dev20240409/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.892615 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.900615 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.908615 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.892615 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.892615 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.908615 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.912615 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/_flags.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/graph_building.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.912615 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   288377 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.912615 onnxscript-0.1.0.dev20240409/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     1997 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50865 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1528 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2449 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      653 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1606 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2278 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15508 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1242 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/ir/convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43841 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.912615 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.920615 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.920615 onnxscript-0.1.0.dev20240409/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4288 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15445 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.920615 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1130 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6698 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2165 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8844 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43596 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.920615 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5082 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.924615 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39591 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.924615 onnxscript-0.1.0.dev20240409/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.924615 onnxscript-0.1.0.dev20240409/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 00:01:51.924615 onnxscript-0.1.0.dev20240409/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-09 00:01:51.000000 onnxscript-0.1.0.dev20240409/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     7932 2024-04-09 00:01:51.000000 onnxscript-0.1.0.dev20240409/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-09 00:01:51.000000 onnxscript-0.1.0.dev20240409/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-09 00:01:51.000000 onnxscript-0.1.0.dev20240409/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-09 00:01:51.000000 onnxscript-0.1.0.dev20240409/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6507 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-09 00:01:51.924615 onnxscript-0.1.0.dev20240409/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-09 00:00:47.000000 onnxscript-0.1.0.dev20240409/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.993492 onnxscript-0.1.0.dev20240410/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-10 00:01:02.993492 onnxscript-0.1.0.dev20240410/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.969492 onnxscript-0.1.0.dev20240410/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2151 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.969492 onnxscript-0.1.0.dev20240410/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.973492 onnxscript-0.1.0.dev20240410/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11068 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8872 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_legacy_ir/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5929 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_legacy_ir/protobuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36193 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.973492 onnxscript-0.1.0.dev20240410/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.973492 onnxscript-0.1.0.dev20240410/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.965492 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.973492 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.981492 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.965492 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.965492 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.981492 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.981492 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/_flags.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/graph_building.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.981492 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   288377 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.985492 onnxscript-0.1.0.dev20240410/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2306 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    59114 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10417 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2525 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17302 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1489 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/ir/convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44088 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.985492 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.989492 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.989492 onnxscript-0.1.0.dev20240410/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4288 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15445 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.989492 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1424 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6698 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2165 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8844 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43596 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.989492 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5082 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.989492 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39591 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.989492 onnxscript-0.1.0.dev20240410/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.993492 onnxscript-0.1.0.dev20240410/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 00:01:02.993492 onnxscript-0.1.0.dev20240410/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-10 00:01:02.000000 onnxscript-0.1.0.dev20240410/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     7962 2024-04-10 00:01:02.000000 onnxscript-0.1.0.dev20240410/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 00:01:02.000000 onnxscript-0.1.0.dev20240410/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-10 00:01:02.000000 onnxscript-0.1.0.dev20240410/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-10 00:01:02.000000 onnxscript-0.1.0.dev20240410/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6525 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-10 00:01:02.993492 onnxscript-0.1.0.dev20240410/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-10 00:00:40.000000 onnxscript-0.1.0.dev20240410/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240409/LICENSE` & `onnxscript-0.1.0.dev20240410/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/PKG-INFO` & `onnxscript-0.1.0.dev20240410/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240409
+Version: 0.1.0.dev20240410
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240409/README.md` & `onnxscript-0.1.0.dev20240410/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240410/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_legacy_ir/irbuilder.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_legacy_ir/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_legacy_ir/protobuilder.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_legacy_ir/protobuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240410/onnxscript/_thirdparty/asciichartpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     else:
         return color + char + reset
 
 
 _DEFAULT_SYMBOLS = ("┼", "┤", "╶", "╴", "─", "╰", "╭", "╮", "╯", "│")
 
 
-def plot(series, bin_edges=None, cfg=None):
+def plot(series, *, bin_edges=None, cfg=None):
     """Generate an ascii chart for a series of numbers.
 
     `series` should be a list of ints or floats. Missing data values in the
     series can be specified as a NaN. In Python versions less than 3.5, use
     float("nan") to specify an NaN. With 3.5 onwards, use math.nan to specify a
     NaN.
 
@@ -110,68 +110,68 @@
             3.00  ┤ ╭╯  ╰╮
             2.00  ┤╭╯    ╰╮
             1.00  ┼╯      ╰
 
     `series` can also be a list of lists to support multiple data series.
 
         >>> series = [[10,20,30,40,30,20,10], [40,30,20,10,20,30,40]]
-        >>> print(plot(series, {'height': 3}))
-            40.00  ┤╮ ╭╮ ╭
-            30.00  ┤╰╮╯╰╭╯
-            20.00  ┤╭╰╮╭╯╮
-            10.00  ┼╯ ╰╯ ╰
+        >>> print(plot(series, cfg={'height': 3}))
+           40.00  ┤╮ ╭╮ ╭
+           30.00  ┤╰╮╯╰╭╯
+           20.00  ┤╭╰╮╭╯╮
+           10.00  ┼╯ ╰╯ ╰
 
     `bin_edges` is an optional list of bin edges to display on the x-axis. If
     provided, the x-axis will be labeled with the bin edges. If there are too
     many bin edges to fit on the x-axis, some labels will be dropped and they
     will be spaced out evenly to fit the width of the chart.
     The labels will be formatted using the `x_format` option in `cfg`.
 
     `cfg` is an optional dictionary of various parameters to tune the appearance
     of the chart. `min` and `max` will clamp the y-axis and all values:
 
         >>> series = [1,2,3,4,float("nan"),4,3,2,1]
-        >>> print(plot(series, {'min': 0}))
+        >>> print(plot(series, cfg={'min': 0}))
             4.00  ┼  ╭╴╶╮
             3.00  ┤ ╭╯  ╰╮
             2.00  ┤╭╯    ╰╮
             1.00  ┼╯      ╰
             0.00  ┤
 
-        >>> print(plot(series, {'min': 2}))
+        >>> print(plot(series, cfg={'min': 2}))
             4.00  ┤  ╭╴╶╮
             3.00  ┤ ╭╯  ╰╮
             2.00  ┼─╯    ╰─
 
-        >>> print(plot(series, {'min': 2, 'max': 3}))
+        >>> print(plot(series, cfg={'min': 2, 'max': 3}))
             3.00  ┤ ╭─╴╶─╮
             2.00  ┼─╯    ╰─
 
     `height` specifies the number of rows the graph should occupy. It can be
     used to scale down a graph with large data values:
 
         >>> series = [10,20,30,40,50,40,30,20,10]
-        >>> print(plot(series, {'height': 4}))
-            50.00  ┤   ╭╮
-            40.00  ┤  ╭╯╰╮
-            30.00  ┤ ╭╯  ╰╮
-            20.00  ┤╭╯    ╰╮
-            10.00  ┼╯      ╰
+        >>> print(plot(series, cfg={'height': 4}))
+           50.00  ┤   ╭╮
+           40.00  ┤  ╭╯╰╮
+           30.00  ┤ ╭╯  ╰╮
+           20.00  ┤╭╯    ╰╮
+           10.00  ┼╯      ╰
 
     `format` specifies a Python format string used to format the labels on the
     y-axis. The default value is "{:8.2f} ". This can be used to remove the
     decimal point:
 
         >>> series = [10,20,30,40,50,40,30,20,10]
-        >>> print(plot(series, {'height': 4, 'format':'{:8.0f}'}))
-            50 ┤   ╭╮
-            40 ┤  ╭╯╰╮
-            30 ┤ ╭╯  ╰╮
-            20 ┤╭╯    ╰╮
-            10 ┼╯      ╰
+        >>> print(plot(series, cfg={'height': 4, 'format':'{:8.0f}'}))
+              50 ┤   ╭╮
+              40 ┤  ╭╯╰╮
+              30 ┤ ╭╯  ╰╮
+              20 ┤╭╯    ╰╮
+              10 ┼╯      ╰
     """
     if len(series) == 0:
         return ""
 
     if not isinstance(series[0], list):
         if all(isnan(n) for n in series):
             return ""
```

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240410/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240410/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240410/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240410/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240410/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/graph_building.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/graph_building.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240410/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240410/onnxscript/ir/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+# --------------------------------------------------------------------------
 """In-memory intermediate representation for ONNX graphs."""
 
 __all__ = [
     # Modules
     "serde",
     # IR classes
     "Attr",
@@ -48,14 +52,16 @@
     "ShapeProtocol",
     "TypeProtocol",
     "MapTypeProtocol",
     "FunctionProtocol",
     # Enums
     "AttributeType",
     "DataType",
+    # Types
+    "OperatorIdentifier",
 ]
 
 from onnxscript.ir import serde
 from onnxscript.ir._core import (
     Attr,
     AttrFloat32,
     AttrFloat32s,
@@ -96,14 +102,15 @@
     DimensionProtocol,
     DLPackCompatible,
     FunctionProtocol,
     GraphProtocol,
     MapTypeProtocol,
     ModelProtocol,
     NodeProtocol,
+    OperatorIdentifier,
     ReferenceAttributeProtocol,
     ShapeProtocol,
     SparseTensorProtocol,
     TensorProtocol,
     TypeProtocol,
     ValueProtocol,
 )
```

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240410/onnxscript/ir/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+# --------------------------------------------------------------------------
 """data structures for the intermediate representation."""
 
 # NOTES for developers:
 # NOTE: None of these classes will have a "to_onnx" or "from_protobuf" method because
 # We cannot assume that the build tool chain has protoc installed and would like
 # to keep this module protobuf free. This way we separate the concerns of the IR
 # and the serialization/deserialization.
@@ -29,14 +33,15 @@
 )
 
 import numpy as np
 
 from onnxscript.ir import (
     _display,
     _enums,
+    _linked_list,
     _metadata,
     _protocols,
 )
 
 if typing.TYPE_CHECKING:
     from typing_extensions import TypeGuard
 
@@ -128,15 +133,17 @@
             lines.append(f"Sparsity (abs<{sparse_threathold}): {sparsity:.2f}")
 
             # Compute histogram
             finite_numbers = array[np.isfinite(array)]
             lines.append("Histogram:")
             hist, bin_edges = np.histogram(finite_numbers, bins=80, density=False)
             lines.append(
-                asciichartpy.plot(hist, bin_edges, {"height": 8, "format": "{:8.0f}"})
+                asciichartpy.plot(
+                    hist, bin_edges=bin_edges, cfg={"height": 8, "format": "{:8.0f}"}
+                )
             )
 
             text = "\n".join(lines)
 
         if rich is None:
             print(text)
         elif page:
@@ -364,21 +371,57 @@
 class Dimension(_protocols.DimensionProtocol, _display.PrettyPrintable):
     __slots__ = ("_value", "_denotation")
 
     def __init__(self, value: int | str | None, denotation: str | None = None) -> None:
         self._value = value
         self._denotation = denotation
 
-    def __index__(self) -> int:
+    def __int__(self) -> int:
         if not isinstance(self.value, int):
             raise TypeError(
-                f"The value of this dim is not int, but {type(self.value)} ({self.value})"
+                f"The value of this Dimension is not int, but {type(self.value)} ({self.value})"
             )
         return self.value
 
+    def __index__(self) -> int:
+        return int(self)
+
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, (int, str)) or other is None:
+            return self.value == other
+        if not isinstance(other, Dimension):
+            return False
+        return self.value == other.value
+
+    def __ne__(self, value: object) -> bool:
+        return not self.__eq__(value)
+
+    def __lt__(self, other: object) -> bool:
+        if not isinstance(other, (int, Dimension)):
+            raise TypeError(f"Expected other to be Dimension or int, got {type(other)}")
+        return int(self) < int(other)
+
+    def __le__(self, other: object) -> bool:
+        if not isinstance(other, (int, Dimension)):
+            raise TypeError(f"Expected other to be Dimension or int, got {type(other)}")
+        return int(self) <= int(other)
+
+    def __gt__(self, other: object) -> bool:
+        if not isinstance(other, (int, Dimension)):
+            raise TypeError(f"Expected other to be Dimension or int, got {type(other)}")
+        return int(self) > int(other)
+
+    def __ge__(self, other: object) -> bool:
+        if not isinstance(other, (int, Dimension)):
+            raise TypeError(f"Expected other to be Dimension or int, got {type(other)}")
+        return int(self) >= int(other)
+
+    def __hash__(self) -> int:
+        return hash(self.value)
+
     @property
     def value(self) -> int | str | None:
         return self._value
 
     @property
     def denotation(self) -> str | None:
         return self._denotation
@@ -544,14 +587,18 @@
         self.doc_string = doc_string
 
         # Add the node as a user of the inputs
         for i, input_value in enumerate(self._inputs):
             if input_value is not None:
                 input_value.add_user(self, i)
 
+        # Add the node to the graph if graph is specified
+        if self._graph is not None:
+            self._graph.append(self)
+
     def __str__(self) -> str:
         node_type_text = f"{self._domain}::{self._op_type}" + f":{self._overload}" * (
             self._overload != ""
         )
         inputs_text = (
             "("
             + ", ".join(
@@ -629,26 +676,64 @@
 
     @inputs.setter
     def inputs(self, _: Any) -> None:
         raise AttributeError(
             "Directly mutating the input sequence is unsupported. Please use Node.replace_input_with() instead."
         )
 
-    def replace_input_with(self, index: int, new_input: Value | None) -> None:
+    def replace_input_with(self, index: int, value: Value | None) -> None:
         """Replace an input with a new value."""
         if index < 0 or index >= len(self.inputs):
             raise ValueError(f"Index out of range: {index}")
         old_input = self.inputs[index]
         self._inputs = tuple(
-            new_input if i == index else old_input for i, old_input in enumerate(self.inputs)
+            value if i == index else old_input for i, old_input in enumerate(self.inputs)
         )
         if old_input is not None:
             old_input.remove_user(self, index)
-        if new_input is not None:
-            new_input.add_user(self, index)
+        if value is not None:
+            value.add_user(self, index)
+
+    def prepend(self, /, nodes: Node | Iterable[Node]) -> None:
+        """Insert a node before this node in the list of nodes in the graph.
+
+        It is the same as calling ``graph.insert_before(self, nodes)``.
+
+        Example::
+
+            Before: previous_node -> self
+                    previous_node' -> node -> next_node'
+            After:  previous_node -> node -> self
+                    previous_node' -> next_node'
+
+        Args:
+            nodes: A node or a sequence of nodes to put before this node.
+        """
+        if self._graph is None:
+            raise ValueError("The node to prepend to does not belong to any graph.")
+        self._graph.insert_before(self, nodes)
+
+    def append(self, /, nodes: Node | Iterable[Node]) -> None:
+        """Insert a node after this node in the list of nodes in the graph.
+
+        It is the same as calling ``graph.insert_after(self, nodes)``.
+
+        Example::
+
+            Before: previous_node -> self
+                    previous_node' -> node -> next_node'
+            After:  previous_node -> self -> node
+                    previous_node' -> next_node'
+
+        Args:
+            nodes:  A node or a sequence of nodes to put after this node.
+        """
+        if self._graph is None:
+            raise ValueError("The node to append to does not belong to any graph.")
+        self._graph.insert_after(self, nodes)
 
     @property
     def outputs(self) -> Sequence[Value]:
         return self._outputs
 
     @outputs.setter
     def outputs(self, _: Sequence[Value]) -> None:
@@ -689,29 +774,32 @@
             print(f"Doc: {self.doc_string}")
         super().display(page=page)
 
 
 class _TensorTypeBase(_protocols.TypeProtocol, _display.PrettyPrintable):
     """Tensor types that are non recursive types."""
 
-    __slots__ = ("_dtype", "_elem_types", "denotation")
+    __slots__ = ("_dtype", "denotation")
 
     def __init__(self, dtype: _enums.DataType, *, denotation: str | None = None) -> None:
         self._dtype = dtype
-        self._elem_types = (self,)
         self.denotation = denotation
 
     @property
     def dtype(self) -> _enums.DataType:
         return self._dtype
 
+    @dtype.setter
+    def dtype(self, value: _enums.DataType) -> None:
+        self._dtype = value
+
     @property
-    def elem_type(self) -> None:
-        # TODO: docs: explain the None
-        return None
+    def elem_type(self) -> _enums.DataType:
+        """Return the element type of the tensor type"""
+        return self.dtype
 
     def __eq__(self, other: object) -> bool:
         if self.__class__ is not other.__class__:
             return False
         return self.dtype == other.dtype  # type: ignore[attr-defined]
 
     def __repr__(self) -> str:
@@ -730,26 +818,29 @@
 class SparseTensorType(_TensorTypeBase):
     """A type that represents a sparse tensor."""
 
 
 class _RecursiveTypeBase(_protocols.TypeProtocol, _display.PrettyPrintable):
     """Base for recursive types like Optional and Sequence."""
 
-    __slots__ = ("_dtype", "_elem_type", "denotation")
+    __slots__ = ("_elem_type", "denotation")
 
     def __init__(
         self, elem_type: _protocols.TypeProtocol, *, denotation: str | None = None
     ) -> None:
-        self._dtype = elem_type.dtype
         self._elem_type = elem_type
         self.denotation = denotation
 
     @property
     def dtype(self) -> _enums.DataType:
-        return self._dtype
+        return self._elem_type.dtype
+
+    @dtype.setter
+    def dtype(self, value: _enums.DataType) -> None:
+        self._elem_type.dtype = value
 
     @property
     def elem_type(self) -> _protocols.TypeProtocol:
         return self._elem_type
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, _RecursiveTypeBase):
@@ -814,46 +905,39 @@
         self._const_value = const_value
         # Use a collection of (Node, int) to store users. This is needed
         # because a single user can use the same value multiple times.
         self._users: set[tuple[Node, int]] = set()
 
     def __repr__(self) -> str:
         value_name = self.name if self.name else "anonymous:" + str(id(self))
+        def_node = self.def_node()
         def_node_text = (
-            self.def_node.name or "anonymous_node:" + str(id(self.def_node))
-            if self.def_node is not None
+            def_node.name or "anonymous_node:" + str(id(def_node))
+            if def_node is not None
             else None
         )
-        return f"{self.__class__.__name__}({value_name!r}, type={self.type!r}, shape={self.shape}, def_node={def_node_text}, def_index={self.def_index})"
+        return f"{self.__class__.__name__}({value_name!r}, type={self.type!r}, shape={self.shape}, def_node={def_node_text}, def_index={self.def_index()})"
 
     def __str__(self) -> str:
         value_name = self.name if self.name else "anonymous:" + str(id(self))
         shape_text = str(self.shape) if self.shape is not None else "?"
         type_text = str(self.type) if self.type is not None else "?"
 
         # Quote the name because in reality the names can have invalid characters
         # that make them hard to read
         return f"%{_quoted(value_name)}<{type_text},{shape_text}>"
 
-    @property
     def def_node(self) -> Node | None:
+        """The node that produces this value."""
         return self._def_node
 
-    @def_node.setter
-    def def_node(self, _: Any) -> None:
-        raise AttributeError("def_node is immutable. Please create a new value instead.")
-
-    @property
     def def_index(self) -> int | None:
+        """The index of the output of the defining node."""
         return self._def_index
 
-    @def_index.setter
-    def def_index(self, _: Any) -> None:
-        raise AttributeError("def_index is immutable. Please create a new value instead.")
-
     def users(self) -> frozenset[tuple[Node, int]]:
         return frozenset(self._users)
 
     def add_user(self, user: Node, index: int) -> None:
         self._users.add((user, index))
 
     def remove_user(self, user: Node, index: int) -> None:
@@ -866,21 +950,47 @@
 
     @name.setter
     def name(self, value: str | None) -> None:
         self._name = value
 
     @property
     def type(self) -> _protocols.TypeProtocol | None:
+        """The type of the tensor.
+
+        Example types can be ``TensorType``, ``SparseTensorType``, ``SequenceType``, ``OptionalType``.
+        To obtain the data type of the tensor, use ``type.dtype`` or conveniently
+        :attribute:`dtype`.
+        """
         return self._type
 
     @type.setter
     def type(self, value: _protocols.TypeProtocol | None) -> None:
         self._type = value
 
     @property
+    def dtype(self) -> _enums.DataType | None:
+        """The data type of the tensor."""
+        if self._type is None:
+            return None
+        return self._type.dtype
+
+    @dtype.setter
+    def dtype(self, value: _enums.DataType) -> None:
+        """Set the data type of the tensor.
+
+        If the type is not set, it will be initialized to a new TensorType. To
+        set the type as other types like ``SequenceType``, initialize the type
+        then set :attribute:`type` instead.
+        """
+        if self._type is None:
+            self._type = TensorType(value)
+        else:
+            self._type.dtype = value
+
+    @property
     def shape(self) -> Shape | None:
         return self._shape
 
     @shape.setter
     def shape(self, value: _protocols.SimpleShape | Shape | None) -> None:
         if value is None:
             self._shape = None
@@ -923,19 +1033,20 @@
     def metadata_props(self) -> dict[str, str]:
         if self._metadata_props is None:
             self._metadata_props = {}
         return self._metadata_props
 
     def is_graph_output(self) -> bool:
         """Whether the value is an output of a graph."""
-        if self.def_node is None:
+        def_node = self.def_node()
+        if def_node is None:
             return False
-        if self.def_node.graph is None:
+        if def_node.graph is None:
             return False
-        return self in self.def_node.graph.outputs
+        return self in def_node.graph.outputs
 
 
 class Input(Value):
     """Input of a Graph or a Function."""
 
     # Slots already defined in Value
     __slots__ = ()
@@ -981,36 +1092,36 @@
         nodes: Iterable[Node],
         initializers: Sequence[_protocols.TensorProtocol] = (),
         doc_string: str | None = None,
         opset_imports: dict[str, int] | None = None,
         name: str | None = None,
     ):
         self.name = name
-        self._inputs = tuple(inputs)
-        self._outputs = tuple(outputs)
+
+        # Private fields that are not to be accessed by any other classes
+        self._inputs = list(inputs)
+        self._outputs = list(outputs)
         for initializer in initializers:
             if initializer.name is None:
                 raise ValueError(f"Initializer must have a name: {initializer}")
         self._initializers = {tensor.name: tensor for tensor in initializers}
         self._doc_string = doc_string
         self._opset_imports = opset_imports or {}
         self._metadata: _metadata.MetadataStore | None = None
         self._metadata_props: dict[str, str] | None = None
-
-        # Assign this graph as the owning_graph of all nodes
-        self._nodes = list(nodes)
-        for node in self._nodes:
-            node.graph = self
+        self._nodes: _linked_list.DoublyLinkedSet[Node] = _linked_list.DoublyLinkedSet()
+        # Call self.extend not self._nodes.extend so the graph reference is added to the nodes
+        self.extend(nodes)
 
     @property
-    def inputs(self) -> tuple[Value, ...]:
+    def inputs(self) -> list[Input]:
         return self._inputs
 
     @property
-    def outputs(self) -> tuple[Value, ...]:
+    def outputs(self) -> list[Value]:
         return self._outputs
 
     @property
     def initializers(self) -> dict[str, _protocols.TensorProtocol]:
         return self._initializers
 
     @property
@@ -1023,19 +1134,112 @@
 
     @property
     def opset_imports(self) -> dict[str, int]:
         return self._opset_imports
 
     @property
     def nodes(self) -> Sequence[Node]:
-        return self._nodes
+        return tuple(self._nodes)
+
+    def __getitem__(self, index: int) -> Node:
+        return self._nodes[index]
+
+    def __len__(self) -> int:
+        return len(self._nodes)
+
+    def __iter__(self) -> Iterator[Node]:
+        return iter(self._nodes)
 
-    def topologically_sorted_nodes(self) -> Sequence[Node]:
+    def __reversed__(self) -> Iterator[Node]:
+        return reversed(self._nodes)
+
+    def _set_node_graph_to_self(self, node: Node) -> Node:
+        """Set the graph reference for the node."""
+        if node.graph is not None and node.graph is not self:
+            raise ValueError(
+                f"The node {node} belongs to another graph. Please remove it first with Graph.remove()."
+            )
+        node.graph = self
+        return node
+
+    # Mutation methods
+    def append(self, node: Node, /) -> None:
+        """Append a node to the graph in O(1) time.
+
+        Args:
+            node: The node to append.
+
+        Raises:
+            ValueError: If the node belongs to another graph.
+        """
+        self._set_node_graph_to_self(node)
+        self._nodes.append(node)
+
+    def extend(self, nodes: Iterable[Node], /) -> None:
+        """Extend the graph with the given nodes in O(#new_nodes) time.
+
+        Args:
+            nodes: The nodes to extend the graph with.
+
+        Raises:
+            ValueError: If any node belongs to another graph.
+        """
+        nodes = [self._set_node_graph_to_self(node) for node in nodes]
+        self._nodes.extend(nodes)
+
+    def remove(self, node: Node, /) -> None:
+        """Remove a node from the graph in O(1) time.
+
+        Args:
+            node: The node to remove.
+
+        Raises:
+            ValueError: If the node does not belong to this graph.
+        """
+        if node.graph is not self:
+            raise ValueError(f"The node {node} does not belong to this graph.")
+        node.graph = None
+        self._nodes.remove(node)
+
+    def insert_after(self, node: Node, new_nodes: Iterable[Node] | Node, /) -> None:
+        """Insert new nodes after the given node in O(#new_nodes) time.
+
+        Args:
+            node: The node to insert after.
+            new_nodes: The new nodes to insert.
+
+        Raises:
+            ValueError: If any node belongs to another graph.
+        """
+        if isinstance(new_nodes, Node):
+            new_nodes = (new_nodes,)
+        new_nodes = [self._set_node_graph_to_self(node) for node in new_nodes]
+        self._nodes.insert_after(node, new_nodes)
+
+    def insert_before(self, node: Node, new_nodes: Iterable[Node] | Node, /) -> None:
+        """Insert new nodes before the given node in O(#new_nodes) time.
+
+        Args:
+            node: The node to insert before.
+            new_nodes: The new nodes to insert.
+
+        Raises:
+            ValueError: If any node belongs to another graph.
+        """
+        if isinstance(new_nodes, Node):
+            new_nodes = (new_nodes,)
+        new_nodes = [self._set_node_graph_to_self(node) for node in new_nodes]
+        self._nodes.insert_before(node, new_nodes)
+
+    def sort(self) -> None:
+        """Topologically sort the nodes in the graph."""
         raise NotImplementedError("Not implemented yet")
 
+    # End of mutation methods
+
     @property
     def meta(self) -> _metadata.MetadataStore:
         """The metadata store for intermediate analysis.
 
         Write to the :attribute:`metadata_props` if you would like the metadata to be serialized
         to the ONNX proto.
         """
@@ -1045,23 +1249,14 @@
 
     @property
     def metadata_props(self) -> dict[str, str]:
         if self._metadata_props is None:
             self._metadata_props = {}
         return self._metadata_props
 
-    def __getitem__(self, index: int) -> Node:
-        return self._nodes[index]
-
-    def __len__(self) -> int:
-        return len(self._nodes)
-
-    def __iter__(self) -> Iterator[Node]:
-        return iter(self._nodes)
-
     def __str__(self) -> str:
         # TODO(justinchuby): Show docstrings and metadata
         inputs_text = "\n" + ",\n".join(str(x) for x in self.inputs)
         outputs_text = "\n" + ",\n".join(str(x) for x in self.outputs)
         initializers_text = ",\n".join(str(x) for x in self.initializers.values())
         if initializers_text:
             initializers_text = (
@@ -1151,15 +1346,15 @@
         producer_name: str | None = None,
         producer_version: str | None = None,
         domain: str | None = None,
         model_version: int | None = None,
         doc_string: str | None = None,
         functions: Sequence[Function] = (),
     ) -> None:
-        self.graph: Graph = graph
+        self.graph: Graph = graph  # type: ignore[assignment]
         self.ir_version = ir_version
         self.producer_name = producer_name
         self.producer_version = producer_version
         self.domain = domain
         self.model_version = model_version
         self.doc_string = doc_string
         self._functions = {func.identifier(): func for func in functions}
@@ -1242,61 +1437,14 @@
         self._name = name
         self._overload = overload
         self._graph = graph
         self._attributes = OrderedDict((attr.name, attr) for attr in attributes)
         self._metadata: _metadata.MetadataStore | None = None
         self._metadata_props: dict[str, str] | None = None
 
-    def __str__(self) -> str:
-        full_name = f"{self.domain}::{self.name}" + f":{self.overload}" * (self.overload != "")
-        inputs_text = ",\n".join(str(x) for x in self.inputs)
-        outputs_text = ",\n".join(str(x) for x in self.outputs)
-        attributes_text = ",\n".join(
-            attr.name + f": {attr.type}" + f"= {attr.value}" * (attr.value is None)
-            for attr in self.attributes.values()
-        )
-        if attributes_text:
-            attributes_text = (
-                "\nattributes={\n" + textwrap.indent(attributes_text, " " * 4) + "\n}"
-            )
-        signature = f"""\
-<
-    opset_imports={self.opset_imports!r},
->
-def {full_name}(
-    inputs=(
-{textwrap.indent(inputs_text, ' '*8)}
-    ),{textwrap.indent(attributes_text, ' '*4)}
-    outputs=(
-{textwrap.indent(outputs_text, ' '*8)}
-    ),
-)"""
-        node_count = len(self.nodes)
-        number_width = len(str(node_count))
-        node_lines = []
-        for i, node in enumerate(self.nodes):
-            node_name = node.name if node.name else f":anonymous_node:{id(node)}"
-            node_text = f"# {node_name}\n{node}"
-            indented_node_text = textwrap.indent(node_text, " " * (number_width + 4))
-            # Remove the leading spaces
-            indented_node_text = indented_node_text.strip()
-            node_lines.append(f"{i:>{number_width}} |  {indented_node_text}")
-        returns = ", ".join(str(x) for x in self.outputs)
-        body = (
-            "{\n"
-            + textwrap.indent("\n".join(node_lines), " " * 4)
-            + textwrap.indent(f"\nreturn {returns}", " " * 4)
-            + "\n}"
-        )
-
-        return f"{signature} {body}"
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self.domain!r}, {self.name!r}, {self.overload!r}, inputs={self.inputs!r}, attributes={self.attributes!r}), outputs={self.outputs!r})"
-
     def identifier(self) -> _protocols.OperatorIdentifier:
         return self.domain, self.name, self.overload
 
     @property
     def name(self) -> str:
         return self._name
 
@@ -1317,31 +1465,40 @@
         return self._overload
 
     @overload.setter
     def overload(self, value: str) -> None:
         self._overload = value
 
     @property
-    def inputs(self) -> Sequence[Value]:
+    def inputs(self) -> list[Input]:
         return self._graph.inputs
 
     @property
-    def outputs(self) -> Sequence[Value]:
+    def outputs(self) -> list[Value]:
         return self._graph.outputs
 
     @property
     def attributes(self) -> OrderedDict[str, Attr]:
         return self._attributes
 
     @property
     def nodes(self) -> Sequence[Node]:
         return self._graph.nodes
 
-    def topologically_sorted_nodes(self) -> Sequence[Node]:
-        raise NotImplementedError("Not implemented yet")
+    def __getitem__(self, index: int) -> Node:
+        return self._graph.__getitem__(index)
+
+    def __len__(self) -> int:
+        return self._graph.__len__()
+
+    def __iter__(self) -> Iterator[Node]:
+        return self._graph.__iter__()
+
+    def __reversed__(self) -> Iterator[Node]:
+        return self._graph.__reversed__()
 
     @property
     def doc_string(self) -> str | None:
         return self._graph.doc_string
 
     @doc_string.setter
     def doc_string(self, value: str | None) -> None:
@@ -1360,14 +1517,88 @@
 
     @property
     def metadata_props(self) -> dict[str, str]:
         if self._metadata_props is None:
             self._metadata_props = {}
         return self._metadata_props
 
+    # Mutation methods
+    def append(self, node: Node, /) -> None:
+        """Append a node to the function in O(1) time."""
+        self._graph.append(node)
+
+    def extend(self, nodes: Iterable[Node], /) -> None:
+        """Extend the function with the given nodes in O(#new_nodes) time."""
+        self._graph.extend(nodes)
+
+    def remove(self, node: Node, /) -> None:
+        """Remove a node from the function in O(1) time."""
+        self._graph.remove(node)
+
+    def insert_after(self, node: Node, new_nodes: Iterable[Node], /) -> None:
+        """Insert new nodes after the given node in O(#new_nodes) time."""
+        self._graph.insert_after(node, new_nodes)
+
+    def insert_before(self, node: Node, new_nodes: Iterable[Node], /) -> None:
+        """Insert new nodes before the given node in O(#new_nodes) time."""
+        self._graph.insert_before(node, new_nodes)
+
+    def sort(self) -> None:
+        """Topologically sort the nodes in the function."""
+        self._graph.sort()
+
+    # End of mutation methods
+
+    def __str__(self) -> str:
+        full_name = f"{self.domain}::{self.name}" + f":{self.overload}" * (self.overload != "")
+        inputs_text = ",\n".join(str(x) for x in self.inputs)
+        outputs_text = ",\n".join(str(x) for x in self.outputs)
+        attributes_text = ",\n".join(
+            attr.name + f": {attr.type}" + f"= {attr.value}" * (attr.value is None)
+            for attr in self.attributes.values()
+        )
+        if attributes_text:
+            attributes_text = (
+                "\nattributes={\n" + textwrap.indent(attributes_text, " " * 4) + "\n}"
+            )
+        signature = f"""\
+<
+    opset_imports={self.opset_imports!r},
+>
+def {full_name}(
+    inputs=(
+{textwrap.indent(inputs_text, ' '*8)}
+    ),{textwrap.indent(attributes_text, ' '*4)}
+    outputs=(
+{textwrap.indent(outputs_text, ' '*8)}
+    ),
+)"""
+        node_count = len(self.nodes)
+        number_width = len(str(node_count))
+        node_lines = []
+        for i, node in enumerate(self.nodes):
+            node_name = node.name if node.name else f":anonymous_node:{id(node)}"
+            node_text = f"# {node_name}\n{node}"
+            indented_node_text = textwrap.indent(node_text, " " * (number_width + 4))
+            # Remove the leading spaces
+            indented_node_text = indented_node_text.strip()
+            node_lines.append(f"{i:>{number_width}} |  {indented_node_text}")
+        returns = ", ".join(str(x) for x in self.outputs)
+        body = (
+            "{\n"
+            + textwrap.indent("\n".join(node_lines), " " * 4)
+            + textwrap.indent(f"\nreturn {returns}", " " * 4)
+            + "\n}"
+        )
+
+        return f"{signature} {body}"
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.domain!r}, {self.name!r}, {self.overload!r}, inputs={self.inputs!r}, attributes={self.attributes!r}), outputs={self.outputs!r})"
+
 
 class RefAttr(_protocols.ReferenceAttributeProtocol, _display.PrettyPrintable):
     """Reference attribute."""
 
     __slots__ = ("_name", "_ref_attr_name", "_type", "doc_string")
 
     def __init__(
```

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240410/onnxscript/ir/_display.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+# --------------------------------------------------------------------------
 """Internal utilities for displaying the intermediate representation of a model.
 
 NOTE: All third-party imports should be scoped and imported only when used to avoid
 importing unnecessary dependencies.
 """
 # pylint: disable=import-outside-toplevel
```

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240410/onnxscript/ir/_enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+# --------------------------------------------------------------------------
 """ONNX IR enums that matches the ONNX spec."""
 
 from __future__ import annotations
 
 import enum
 import typing
```

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240410/onnxscript/ir/_graph_comparison.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+# --------------------------------------------------------------------------
 """Utilities for comparing IR graphs."""
 
 from __future__ import annotations
 
 from onnxscript.ir import _core
 
 # NOTE(justinchuby): We need to ensure a graph has valid inputs and outputs
```

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240410/onnxscript/ir/_invariants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+# --------------------------------------------------------------------------
 """Utilities to enforce invariants on the IR."""
 
 from __future__ import annotations
 
 import functools
 from typing import Any, Callable
```

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240410/onnxscript/ir/_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+# --------------------------------------------------------------------------
 """Class for storing metadata about the IR objects."""
 
 from __future__ import annotations
 
 from typing import Any, Iterator, Mapping
```

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240410/onnxscript/ir/_protocols.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,26 @@
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+# --------------------------------------------------------------------------
 """Protocols for the ONNX IR.
 
 This file defines the interfaces for tools to interact with the IR. The interfaces
 are designed such that tools leveraging the IR can be decoupled from the IR
 implementation. This allows for the implementation to evolve independently of the
 tools.
-
-The file contains two sets of interfaces:
-1. Topologically immutable interfaces:
-    These interfaces provide a complete view of the ONNX model and allows mutation
-    against any metadata fields like shape, type, and node attributes. However, the
-    interfaces are topologically immutable, meaning that the structure of the graph
-    cannot be changed. This is useful for tools that need to analyze the model
-    without modifying how nodes are connected.
-2. Mutable interfaces:
-    These interfaces provide a mutable view of the ONNX model. They allow for
-    modification of the graph structure. This is useful for tools that need to
-    transform the model.
 """
 
 from __future__ import annotations
 
 import typing
 from typing import (
     AbstractSet,
     Any,
+    Iterable,
     Iterator,
     Mapping,
     OrderedDict,
     Protocol,
     Sequence,
     Tuple,
     Union,
@@ -57,15 +50,15 @@
     """
 
     def __array__(self, dtype: Any) -> np.ndarray: ...
 
 
 @typing.runtime_checkable
 class DLPackCompatible(Protocol):
-    """Protocol objects that can support dlpack.
+    """Protocol for objects that can support dlpack.
 
     Computation backends can call __dlpack__ to obtain the underlying data in a
     tensor without copying the data. This allows use to use tensorflow tensors etc.
     without copying the data.
     """
 
     def __dlpack__(self, *, stream: Any = ...) -> Any:
@@ -121,61 +114,66 @@
     def tobytes(self) -> bytes:
         """Return the tensor as a byte string conformed to the ONNX specification, in little endian."""
         ...
 
 
 @typing.runtime_checkable
 class ValueProtocol(Protocol):
-    """Values.
+    """Protocol for values.
 
     A value is a named entity that can be used to represent an input or output of a graph,
-    a function, or a node. The information it stores corresponds to ValueInfoProto
+    a function, or a node. The information it stores corresponds to ``ValueInfoProto``
     in the ONNX specification.
 
     A :class:`Value` is always not owned or owned by exactly one node. When the value is not
-    owned, it must be an input of a graph or a function. The def_node and def_index
-    attributes are None.
+    owned, it must be an input of a graph or a function. ``def_node`` and ``def_index``
+    are ``None``.
 
     When the value is owned by a node, it is an output of the node.
-    The node that produces the value is stored in the :attr:`def_node` attribute.
-    The index of the output of the node that produces the value is stored in the
-    :attr:`def_index` attribute.
+    The node that produces the value can be accessed with :method:`def_node`.
+    The index of the output of the node that produces the value can be accessed with
+    :method:`def_index`.
 
     To find all the nodes that use this value as an input, call :meth:`users`.
 
     To check if the value is an output of a graph, call :meth:`is_graph_output`.
 
     Attributes:
         name: The name of the value. A value is always named when it is part of a graph.
-        def_node: The node that produces this value.
-        def_index: The index of the output of the node that produces this value.
         shape: The shape of the value.
         type: The type of the value.
         metadata_props: Metadata.
     """
 
     name: str
-    def_node: NodeProtocol | None
-    def_index: int | None
     shape: ShapeProtocol | None
     type: TypeProtocol | None
     metadata_props: Mapping[str, str]
+    meta: Mapping[str, Any]
+
+    def def_node(self) -> NodeProtocol | None:
+        """The node that produces this value."""
+        ...
+
+    def def_index(self) -> int | None:
+        """The index of the output of the node that produces this value."""
+        ...
 
     def users(self) -> AbstractSet[tuple[NodeProtocol, int]]:
         """The set of (node, input_index) with node being those that use this value as an input."""
         ...
 
     def is_graph_output(self) -> bool:
         """Whether this value is an output of a graph."""
         ...
 
 
 @typing.runtime_checkable
 class NodeProtocol(Protocol):
-    """Nodes.
+    """Protocol for nodes.
 
     A node represents an invocation of an operation on the :class:`Value` s in
     the computational graph.
 
     A node can be optionally named. A name should typically be assigned when the
     node is added to a graph.
 
@@ -215,19 +213,24 @@
     overload: str
     inputs: Sequence[ValueProtocol]
     outputs: Sequence[ValueProtocol]
     attributes: OrderedDict[str, AttributeProtocol | ReferenceAttributeProtocol]
     version: int | None
     doc_string: str | None
     metadata_props: Mapping[str, str]
+    meta: Mapping[str, Any]
+
+    def replace_input_with(self, index: int, value: ValueProtocol | None) -> None:
+        """Set the input at the given index to the given value, replacing the original value."""
+        ...
 
 
 @typing.runtime_checkable
 class GraphProtocol(Protocol):
-    """Graphs.
+    """Protocol for graphs.
 
     Graph represents a computation graph. In addition to the ONNX specification
     specified fields, it also contains a mapping of :attr:`opset_imports`. This
     allows different subgraphs to import different opsets. It is the responsibility
     of the deserializer to reconcile the different opsets.
 
     The :attr:`nodes` are not guaranteed to be topologically sorted. But the
@@ -250,23 +253,50 @@
     inputs: Sequence[ValueProtocol]
     outputs: Sequence[ValueProtocol]
     nodes: Sequence[NodeProtocol]
     initializers: Mapping[str, TensorProtocol]
     doc_string: str
     opset_imports: Mapping[str, int]
     metadata_props: Mapping[str, str]
+    meta: Mapping[str, Any]
 
-    def topologically_sorted_nodes(self) -> Sequence[NodeProtocol]:
-        """Return the nodes in topological order."""
+    def __getitem__(self, index: int) -> NodeProtocol: ...
+    def __len__(self) -> int: ...
+    def __iter__(self) -> Iterator[NodeProtocol]: ...
+    def __reversed__(self) -> Iterator[NodeProtocol]: ...
+
+    # Mutation methods
+    def append(self, node: NodeProtocol, /) -> None:
+        """Append a node to the graph."""
+        ...
+
+    def extend(self, nodes: Iterable[NodeProtocol], /) -> None:
+        """Extend the graph with the given nodes."""
+        ...
+
+    def remove(self, node: NodeProtocol, /) -> None:
+        """Remove a node from the graph."""
+        ...
+
+    def insert_after(self, node: NodeProtocol, new_nodes: Iterator[NodeProtocol], /) -> None:
+        """Insert new nodes after the given node."""
+        ...
+
+    def insert_before(self, node: NodeProtocol, new_nodes: Iterator[NodeProtocol], /) -> None:
+        """Insert new nodes before the given node."""
+        ...
+
+    def sort(self) -> None:
+        """Topologically sort the nodes in the graph."""
         ...
 
 
 @typing.runtime_checkable
 class ModelProtocol(Protocol):
-    """Models.
+    """Protocol for models.
 
     A model is a container for a graph and metadata. It is the top-level object
     that represents an ONNX model.
 
     Attributes:
         graph: The graph of the model.
         ir_version: The version of the IR.
@@ -286,14 +316,15 @@
     domain: str | None
     model_version: int | None
     doc_string: str | None
     functions: Mapping[str, FunctionProtocol]
     # TODO(justinchuby): Add training_info
     opset_imports: Mapping[str, int]
     metadata_props: Mapping[str, str]
+    meta: Mapping[str, Any]
 
 
 @typing.runtime_checkable
 class AttributeProtocol(Protocol):
     """Protocol for ONNX attributes.
 
     Attributes:
@@ -385,20 +416,20 @@
     Attributes:
         denotation: An optional denotation can be used to denote the whole
             type with a standard semantic description as to what is
             stored inside.
             Refer to https://github.com/onnx/onnx/blob/main/docs/TypeDenotation.md#type-denotation-definition
             for pre-defined type denotations.
         elem_type: The type of its elements for nested types like Sequence[Optional] tensors.
-            Or None if the type is not nested.
+            Or the DataType if the type is not nested.
         dtype: The data type of the tensor or the nested tensor.
     """
 
     denotation: str | None
-    elem_type: TypeProtocol | None
+    elem_type: TypeProtocol | _enums.DataType
     dtype: _enums.DataType
 
     def __eq__(self, __value: object) -> bool: ...
 
 
 @typing.runtime_checkable
 class MapTypeProtocol(Protocol):
@@ -447,15 +478,42 @@
     inputs: Sequence[ValueProtocol]
     attributes: OrderedDict[str, AttributeProtocol]
     outputs: Sequence[ValueProtocol]
     doc_string: str
     opset_imports: Mapping[str, int]
     nodes: Sequence[NodeProtocol]
     metadata_props: Mapping[str, str]
+    meta: Mapping[str, Any]
 
+    def __getitem__(self, index: int) -> NodeProtocol: ...
+    def __len__(self) -> int: ...
+    def __iter__(self) -> Iterator[NodeProtocol]: ...
+    def __reversed__(self) -> Iterator[NodeProtocol]: ...
     def identifier(self) -> OperatorIdentifier:
         """Return the unique identifier of the function."""
         ...
 
-    def topologically_sorted_nodes(self) -> Sequence[NodeProtocol]:
-        """Return the nodes in topological order."""
+    # Mutation methods
+    # End Block
+    def append(self, node: NodeProtocol, /) -> None:
+        """Append a node to the function."""
+        ...
+
+    def extend(self, nodes: Iterable[NodeProtocol], /) -> None:
+        """Extend the function with the given nodes."""
+        ...
+
+    def remove(self, node: NodeProtocol, /) -> None:
+        """Remove a node from the function."""
+        ...
+
+    def insert_after(self, node: NodeProtocol, new_nodes: Iterator[NodeProtocol], /) -> None:
+        """Insert new nodes after the given node."""
+        ...
+
+    def insert_before(self, node: NodeProtocol, new_nodes: Iterator[NodeProtocol], /) -> None:
+        """Insert new nodes before the given node."""
+        ...
+
+    def sort(self) -> None:
+        """Topologically sort the nodes in the function."""
         ...
```

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/ir/convenience.py` & `onnxscript-0.1.0.dev20240410/onnxscript/ir/convenience.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+# --------------------------------------------------------------------------
 """Convenience methods for constructing (and manipulating?) the IR."""
 
 from __future__ import annotations
 
 from typing import Any, Mapping, Sequence
 
 from onnxscript.ir import _core
```

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240410/onnxscript/ir/serde.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+# --------------------------------------------------------------------------
 """Serialize and deserialize the intermediate representation to/from ONNX protos."""
 
 # NOTES for developers:
 # NOTE: Do not import pathlib in the IR. It is slow. Use os.path methods instead.
 #
 # NOTE: Protobuf serialization
 #     Initializing a protobuf message with initialized protobuf messages incurs
```

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240410/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/main.py` & `onnxscript-0.1.0.dev20240410/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240410/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240410/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240410/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/optimizer/copy_propagation.py` & `onnxscript-0.1.0.dev20240410/onnxscript/optimizer/copy_propagation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240410/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240410/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240410/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240410/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240410/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240410/onnxscript/rewriter/pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240410/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240410/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240410/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240410/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240410/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240410/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240410/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript/values.py` & `onnxscript-0.1.0.dev20240410/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240410/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240409
+Version: 0.1.0.dev20240410
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240409/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240410/onnxscript.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 onnxscript/function_libs/torch_lib/ops/vision.py
 onnxscript/ir/__init__.py
 onnxscript/ir/_core.py
 onnxscript/ir/_display.py
 onnxscript/ir/_enums.py
 onnxscript/ir/_graph_comparison.py
 onnxscript/ir/_invariants.py
+onnxscript/ir/_linked_list.py
 onnxscript/ir/_metadata.py
 onnxscript/ir/_protocols.py
 onnxscript/ir/convenience.py
 onnxscript/ir/serde.py
 onnxscript/onnx_opset/__init__.py
 onnxscript/onnx_opset/_impl/opset1.py
 onnxscript/onnx_opset/_impl/opset10.py
```

### Comparing `onnxscript-0.1.0.dev20240409/pyproject.toml` & `onnxscript-0.1.0.dev20240410/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 [tool.setuptools.package-data]
 onnxscript = ["py.typed"]
 onnx = ["py.typed"]
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore::UserWarning", "ignore::DeprecationWarning"]
-addopts = "-rsfEX --tb=short --color=yes"
+addopts = "-rsfEX --tb=short --color=yes --doctest-modules"
 
 [tool.mypy]
 # TODO disallow_incomplete_defs = true
 check_untyped_defs = true
 disable_error_code = 'override,import-untyped'
 disallow_any_generics = false
 disallow_untyped_decorators = true
```

### Comparing `onnxscript-0.1.0.dev20240409/setup.py` & `onnxscript-0.1.0.dev20240410/setup.py`

 * *Files identical despite different names*

