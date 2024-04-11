# Comparing `tmp/dsp_tools-7.1.2.tar.gz` & `tmp/dsp_tools-7.1.2.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-7.1.2.tar", max compression
+gzip compressed data, was "dsp_tools-7.1.2.post0.tar", max compression
```

## Comparing `dsp_tools-7.1.2.tar` & `dsp_tools-7.1.2.post0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0    35149 2024-04-10 07:47:56.099636 dsp_tools-7.1.2/LICENSE
--rw-r--r--   0        0        0     4941 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/docs/index.md
--rw-r--r--   0        0        0     8357 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/cli/__init__.py
--rw-r--r--   0        0        0     7360 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/cli/call_action.py
--rw-r--r--   0        0        0    12476 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/cli/create_parsers.py
--rw-r--r--   0        0        0     9819 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/cli/entry_point.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/__init__.py
--rw-r--r--   0        0        0    15987 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/lists.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/models/__init__.py
--rw-r--r--   0        0        0     8065 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/models/input_error.py
--rw-r--r--   0        0        0      501 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/models/list_node_name.py
--rw-r--r--   0        0        0     6313 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/project.py
--rw-r--r--   0        0        0    13147 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/properties.py
--rw-r--r--   0        0        0    11830 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/resources.py
--rw-r--r--   0        0        0    11866 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/utils.py
--rw-r--r--   0        0        0      466 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2xml/__init__.py
--rw-r--r--   0        0        0    21350 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
--rw-r--r--   0        0        0    75692 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
--rw-r--r--   0        0        0     1981 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/excel2xml/propertyelement.py
--rw-r--r--   0        0        0     8275 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/id2iri.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/ingest_xmlupload/__init__.py
--rw-r--r--   0        0        0     2876 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
--rw-r--r--   0        0        0     2351 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
--rw-r--r--   0        0        0     4891 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/ingest_xmlupload/user_information.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/create/__init__.py
--rw-r--r--   0        0        0    45642 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/create/project_create.py
--rw-r--r--   0        0        0     8243 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/create/project_create_lists.py
--rw-r--r--   0        0        0    19520 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/create/project_validate.py
--rw-r--r--   0        0        0     5743 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/get.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/models/__init__.py
--rw-r--r--   0        0        0    12173 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/models/context.py
--rw-r--r--   0        0        0     8379 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/models/group.py
--rw-r--r--   0        0        0      850 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/models/helpers.py
--rw-r--r--   0        0        0    14910 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/models/listnode.py
--rw-r--r--   0        0        0      245 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/models/model.py
--rw-r--r--   0        0        0    12710 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/models/ontology.py
--rw-r--r--   0        0        0    11594 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/models/project.py
--rw-r--r--   0        0        0      306 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/models/project_definition.py
--rw-r--r--   0        0        0    17215 2024-04-10 07:47:56.115636 dsp_tools-7.1.2/src/dsp_tools/commands/project/models/propertyclass.py
--rw-r--r--   0        0        0    28334 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/project/models/resourceclass.py
--rw-r--r--   0        0        0    17030 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/project/models/user.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/resume_xmlupload/__init__.py
--rw-r--r--   0        0        0     4200 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
--rw-r--r--   0        0        0     4177 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/rosetta.py
--rw-r--r--   0        0        0    14112 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/start_stack.py
--rw-r--r--   0        0        0     1134 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/template.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/__init__.py
--rw-r--r--   0        0        0     2350 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/ark2iri.py
--rw-r--r--   0        0        0    10356 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
--rw-r--r--   0        0        0      625 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/iri_resolver.py
--rw-r--r--   0        0        0     3587 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/list_client.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/__init__.py
--rw-r--r--   0        0        0     1334 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
--rw-r--r--   0        0        0     5428 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
--rw-r--r--   0        0        0     6751 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
--rw-r--r--   0        0        0     2388 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/permission.py
--rw-r--r--   0        0        0      812 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/sipi.py
--rw-r--r--   0        0        0      675 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/upload_state.py
--rw-r--r--   0        0        0     2236 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/xmlallow.py
--rw-r--r--   0        0        0      548 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py
--rw-r--r--   0        0        0     1437 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/xmlpermission.py
--rw-r--r--   0        0        0     2026 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/xmlproperty.py
--rw-r--r--   0        0        0     5164 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/xmlresource.py
--rw-r--r--   0        0        0     4004 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/xmlvalue.py
--rw-r--r--   0        0        0     3466 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/ontology_client.py
--rw-r--r--   0        0        0     3063 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/project_client.py
--rw-r--r--   0        0        0     4653 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
--rw-r--r--   0        0        0    13023 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/resource_create_client.py
--rw-r--r--   0        0        0     4585 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/resource_multimedia.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/__init__.py
--rw-r--r--   0        0        0    12372 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
--rw-r--r--   0        0        0     2452 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/graph_models.py
--rw-r--r--   0        0        0     5724 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
--rw-r--r--   0        0        0     3068 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/stash_models.py
--rw-r--r--   0        0        0     4237 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
--rw-r--r--   0        0        0     7727 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
--rw-r--r--   0        0        0     2175 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/upload_config.py
--rw-r--r--   0        0        0      858 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
--rw-r--r--   0        0        0    22348 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/xmlupload.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0     2876 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/models/datetimestamp.py
--rw-r--r--   0        0        0     2536 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     8457 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0     1777 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/py.typed
--rw-r--r--   0        0        0     1488 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    24358 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    44347 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    33977 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0       61 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/resources/start-stack/docker-compose.override.yml
--rw-r--r--   0        0        0     3295 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0      164 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/resources/start-stack/start-stack-config.yml
--rw-r--r--   0        0        0        0 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/connection.py
--rw-r--r--   0        0        0    14126 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/connection_live.py
--rw-r--r--   0        0        0     4554 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/date_util.py
--rw-r--r--   0        0        0      457 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/iri_util.py
--rw-r--r--   0        0        0      893 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/json_ld_util.py
--rw-r--r--   0        0        0     1157 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/logger_config.py
--rw-r--r--   0        0        0      705 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/set_encoder.py
--rw-r--r--   0        0        0     5754 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0      545 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/uri_util.py
--rw-r--r--   0        0        0     4464 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/xml_utils.py
--rw-r--r--   0        0        0     7194 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/xml_validation.py
--rw-r--r--   0        0        0     2312 2024-04-10 07:47:56.119636 dsp_tools-7.1.2/src/dsp_tools/utils/xml_validation_models.py
--rw-r--r--   0        0        0     6311 1970-01-01 00:00:00.000000 dsp_tools-7.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-11 14:31:12.870561 dsp_tools-7.1.2.post0/LICENSE
+-rw-r--r--   0        0        0     4941 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/docs/index.md
+-rw-r--r--   0        0        0     8363 2024-04-11 14:31:49.178882 dsp_tools-7.1.2.post0/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/cli/__init__.py
+-rw-r--r--   0        0        0     7360 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/cli/call_action.py
+-rw-r--r--   0        0        0    12476 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/cli/create_parsers.py
+-rw-r--r--   0        0        0     9819 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/cli/entry_point.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/__init__.py
+-rw-r--r--   0        0        0    15987 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/lists.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/models/__init__.py
+-rw-r--r--   0        0        0     8065 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/models/input_error.py
+-rw-r--r--   0        0        0      501 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/models/list_node_name.py
+-rw-r--r--   0        0        0     6313 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/project.py
+-rw-r--r--   0        0        0    13147 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/properties.py
+-rw-r--r--   0        0        0    11830 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/resources.py
+-rw-r--r--   0        0        0    11866 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/utils.py
+-rw-r--r--   0        0        0      466 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/__init__.py
+-rw-r--r--   0        0        0    21350 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
+-rw-r--r--   0        0        0    75692 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
+-rw-r--r--   0        0        0     1981 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/propertyelement.py
+-rw-r--r--   0        0        0     8275 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/id2iri.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/__init__.py
+-rw-r--r--   0        0        0     2876 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
+-rw-r--r--   0        0        0     2351 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0     4891 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/user_information.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/__init__.py
+-rw-r--r--   0        0        0    45642 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/project_create.py
+-rw-r--r--   0        0        0     8243 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/project_create_lists.py
+-rw-r--r--   0        0        0    19520 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/project_validate.py
+-rw-r--r--   0        0        0     5743 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/get.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/__init__.py
+-rw-r--r--   0        0        0    12173 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/context.py
+-rw-r--r--   0        0        0     8379 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/group.py
+-rw-r--r--   0        0        0      850 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/helpers.py
+-rw-r--r--   0        0        0    14910 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/listnode.py
+-rw-r--r--   0        0        0      245 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/model.py
+-rw-r--r--   0        0        0    12710 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/ontology.py
+-rw-r--r--   0        0        0    11594 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/project.py
+-rw-r--r--   0        0        0      306 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/project_definition.py
+-rw-r--r--   0        0        0    17215 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/propertyclass.py
+-rw-r--r--   0        0        0    28334 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/resourceclass.py
+-rw-r--r--   0        0        0    17030 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/user.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/resume_xmlupload/__init__.py
+-rw-r--r--   0        0        0     4200 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
+-rw-r--r--   0        0        0     4177 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/rosetta.py
+-rw-r--r--   0        0        0    14112 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/start_stack.py
+-rw-r--r--   0        0        0     1134 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/template.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/__init__.py
+-rw-r--r--   0        0        0     2350 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/ark2iri.py
+-rw-r--r--   0        0        0    10356 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
+-rw-r--r--   0        0        0      625 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/iri_resolver.py
+-rw-r--r--   0        0        0     3587 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/list_client.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/__init__.py
+-rw-r--r--   0        0        0     1334 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
+-rw-r--r--   0        0        0     5428 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
+-rw-r--r--   0        0        0     6751 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
+-rw-r--r--   0        0        0     2388 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/permission.py
+-rw-r--r--   0        0        0      812 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/sipi.py
+-rw-r--r--   0        0        0      675 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/upload_state.py
+-rw-r--r--   0        0        0     2236 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlallow.py
+-rw-r--r--   0        0        0      548 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py
+-rw-r--r--   0        0        0     1437 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlpermission.py
+-rw-r--r--   0        0        0     2026 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlproperty.py
+-rw-r--r--   0        0        0     5164 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlresource.py
+-rw-r--r--   0        0        0     4004 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlvalue.py
+-rw-r--r--   0        0        0     3466 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/ontology_client.py
+-rw-r--r--   0        0        0     3063 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/project_client.py
+-rw-r--r--   0        0        0     4653 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
+-rw-r--r--   0        0        0    13023 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/resource_create_client.py
+-rw-r--r--   0        0        0     4585 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/resource_multimedia.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/__init__.py
+-rw-r--r--   0        0        0    12372 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
+-rw-r--r--   0        0        0     2452 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/graph_models.py
+-rw-r--r--   0        0        0     5724 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
+-rw-r--r--   0        0        0     3068 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/stash_models.py
+-rw-r--r--   0        0        0     4237 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
+-rw-r--r--   0        0        0     7727 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
+-rw-r--r--   0        0        0     2175 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/upload_config.py
+-rw-r--r--   0        0        0      858 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
+-rw-r--r--   0        0        0    22348 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/xmlupload.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0     2876 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/models/datetimestamp.py
+-rw-r--r--   0        0        0     2536 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     8457 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0     1777 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/py.typed
+-rw-r--r--   0        0        0     1488 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    24360 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    44347 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    33977 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0       61 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/start-stack/docker-compose.override.yml
+-rw-r--r--   0        0        0     3295 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0      164 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/start-stack/start-stack-config.yml
+-rw-r--r--   0        0        0        0 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/connection.py
+-rw-r--r--   0        0        0    14126 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/connection_live.py
+-rw-r--r--   0        0        0     4554 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/date_util.py
+-rw-r--r--   0        0        0      457 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/iri_util.py
+-rw-r--r--   0        0        0      893 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/json_ld_util.py
+-rw-r--r--   0        0        0     1157 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/logger_config.py
+-rw-r--r--   0        0        0      705 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/set_encoder.py
+-rw-r--r--   0        0        0     5754 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0      547 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/uri_util.py
+-rw-r--r--   0        0        0     4464 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/xml_utils.py
+-rw-r--r--   0        0        0     7194 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/xml_validation.py
+-rw-r--r--   0        0        0     2312 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/xml_validation_models.py
+-rw-r--r--   0        0        0     6317 1970-01-01 00:00:00.000000 dsp_tools-7.1.2.post0/PKG-INFO
```

### Comparing `dsp_tools-7.1.2/LICENSE` & `dsp_tools-7.1.2.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/docs/index.md` & `dsp_tools-7.1.2.post0/docs/index.md`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/pyproject.toml` & `dsp_tools-7.1.2.post0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#writing-pyproject-toml
 
 [tool.poetry]
 name = "dsp-tools"
-version = "7.1.2"
+version = "7.1.2.post0"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `dsp_tools-7.1.2/src/dsp_tools/cli/call_action.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/cli/call_action.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/cli/create_parsers.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/cli/create_parsers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/cli/entry_point.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/cli/entry_point.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/lists.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/models/input_error.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/models/input_error.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/project.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/properties.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/properties.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/resources.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/resources.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/excel2json/utils.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/excel2xml/excel2xml_cli.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/excel2xml_cli.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/excel2xml/excel2xml_lib.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/excel2xml_lib.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/excel2xml/propertyelement.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/id2iri.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/id2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/ingest_xmlupload/user_information.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/user_information.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/create/project_create.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/project_create.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/create/project_create_lists.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/project_create_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/create/project_validate.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/project_validate.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/get.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/get.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/models/context.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/context.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/models/group.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/group.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/models/helpers.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/models/listnode.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/listnode.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/models/ontology.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/models/project.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/models/propertyclass.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/propertyclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/models/resourceclass.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/resourceclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/project/models/user.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/user.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/rosetta.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/rosetta.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/start_stack.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/start_stack.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/template.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/template.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/ark2iri.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/ark2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/iri_resolver.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/iri_resolver.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/list_client.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/list_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/permission.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/sipi.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/sipi.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/upload_state.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/upload_state.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/xmlallow.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlallow.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/xmlpermission.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/xmlproperty.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlproperty.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/xmlresource.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlresource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/models/xmlvalue.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlvalue.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/ontology_client.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/ontology_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/project_client.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/project_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/resource_create_client.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/resource_create_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/resource_multimedia.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/resource_multimedia.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/graph_models.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/graph_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/stash_models.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/stash_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/upload_config.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/upload_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/commands/xmlupload/xmlupload.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/xmlupload.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/models/datetimestamp.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/models/datetimestamp.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/models/exceptions.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/models/langstring.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/models/langstring.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/models/projectContext.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-7.1.2.post0/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-7.1.2.post0/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/data.xsd`

 * *Files 0% similar despite different names*

#### Comparing `dsp_tools-7.1.2/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/data.xsd`

```diff
@@ -36,15 +36,15 @@
     <xs:restriction base="xs:token">
       <xs:pattern value="#([0-9a-fA-F]{3}){1,2}"/>
     </xs:restriction>
   </xs:simpleType>
   <!-- data type for knora uri -->
   <xs:simpleType name="knorauri_type">
     <xs:restriction base="xs:string">
-      <xs:pattern value="([a-z][a-z0-9+.\-]*):(//([\w_.\-~:\[\]]+)(:\d{0,6})?)(/[\w_.\-~:%()]*)*(\?[\w_.,\-:%=*&amp;]+)*(#[\w_.\-~:/]*)?"/>
+      <xs:pattern value="([a-z][a-z0-9+.\-]*):(//([\w_.\-~:\[\]]+)(:\d{0,6})?)(/[\w_.\-~:%()]*)*(\?[\w_.,;/\-:%=*&amp;]+)*(#[\w_.\-~:/]*)?"/>
     </xs:restriction>
   </xs:simpleType>
   <!-- data type for knora interval -->
   <xs:simpleType name="knorainterval_type">
     <xs:restriction base="xs:token">
       <xs:pattern value="([+-]?([0-9]+([.][0-9]*)?|[.][0-9]+)):([+-]?([0-9]+([.][0-9]*)?|[.][0-9]+))"/>
     </xs:restriction>
```

### Comparing `dsp_tools-7.1.2/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/resources/schema/project.json` & `dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-7.1.2.post0/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/utils/connection.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/utils/connection.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/utils/connection_live.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/utils/connection_live.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/utils/date_util.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/utils/date_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/utils/json_ld_util.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/utils/json_ld_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/utils/logger_config.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/utils/logger_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/utils/set_encoder.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/utils/set_encoder.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/utils/shared.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/utils/shared.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/utils/uri_util.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/utils/uri_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 def is_uri(s: str) -> bool:
     """Checks if the given string is a valid URI."""
     # URI = scheme ":" ["//" host [":" port]] path ["?" query] ["#" fragment]
     scheme = r"(?<scheme>[a-z][a-z0-9+.\-]*)"
     host = r"(?<host>[\w_.\-~:\[\]]+)"
     port = r"(?<port>:\d{0,6})"
     path = r"(?<path>/[\w_.\-~:%()]*)"
-    query = r"(?<query>\?[\w_.,\-:%=*&]+)"
+    query = r"(?<query>\?[\w_.,;/\-:%=*&]+)"
     fragment = r"(?<fragment>#[\w_.\-~:/]*)"
     m = regex.match(rf"{scheme}:(//{host}{port}?){path}*{query}*{fragment}?", s, flags=regex.UNICODE)
     return m is not None
```

### Comparing `dsp_tools-7.1.2/src/dsp_tools/utils/xml_utils.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/utils/xml_validation.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/utils/xml_validation.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/src/dsp_tools/utils/xml_validation_models.py` & `dsp_tools-7.1.2.post0/src/dsp_tools/utils/xml_validation_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2/PKG-INFO` & `dsp_tools-7.1.2.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 7.1.2
+Version: 7.1.2.post0
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

