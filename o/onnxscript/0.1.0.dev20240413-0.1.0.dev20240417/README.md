# Comparing `tmp/onnxscript-0.1.0.dev20240413.tar.gz` & `tmp/onnxscript-0.1.0.dev20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240413.tar", last modified: Sat Apr 13 00:01:16 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240417.tar", last modified: Wed Apr 17 00:01:34 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240413.tar` & `onnxscript-0.1.0.dev20240417.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.374487 onnxscript-0.1.0.dev20240413/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-13 00:01:16.374487 onnxscript-0.1.0.dev20240413/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.338487 onnxscript-0.1.0.dev20240413/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.342487 onnxscript-0.1.0.dev20240413/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.342487 onnxscript-0.1.0.dev20240413/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11068 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8872 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_legacy_ir/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5929 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_legacy_ir/protobuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36193 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.342487 onnxscript-0.1.0.dev20240413/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.342487 onnxscript-0.1.0.dev20240413/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.334487 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.346487 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.354487 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.334487 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.334487 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.354487 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.358487 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/_flags.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/graph_building.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.358487 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   288377 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.362487 onnxscript-0.1.0.dev20240413/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2338 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    64439 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10417 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2525 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18653 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1489 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/ir/convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44162 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.362487 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.366487 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.370487 onnxscript-0.1.0.dev20240413/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4288 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15445 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.370487 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1424 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6698 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2165 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8844 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43596 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.370487 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5082 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.374487 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39591 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.374487 onnxscript-0.1.0.dev20240413/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.374487 onnxscript-0.1.0.dev20240413/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 00:01:16.374487 onnxscript-0.1.0.dev20240413/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-13 00:01:16.000000 onnxscript-0.1.0.dev20240413/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     7995 2024-04-13 00:01:16.000000 onnxscript-0.1.0.dev20240413/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-13 00:01:16.000000 onnxscript-0.1.0.dev20240413/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-13 00:01:16.000000 onnxscript-0.1.0.dev20240413/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-13 00:01:16.000000 onnxscript-0.1.0.dev20240413/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6525 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-13 00:01:16.374487 onnxscript-0.1.0.dev20240413/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-13 00:00:57.000000 onnxscript-0.1.0.dev20240413/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.280448 onnxscript-0.1.0.dev20240417/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-17 00:01:34.280448 onnxscript-0.1.0.dev20240417/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.240448 onnxscript-0.1.0.dev20240417/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.240448 onnxscript-0.1.0.dev20240417/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.244448 onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11116 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8872 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6153 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/protobuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36193 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.244448 onnxscript-0.1.0.dev20240417/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.244448 onnxscript-0.1.0.dev20240417/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.232448 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.244448 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.256448 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.236448 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.236448 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.256448 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.256448 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/_flags.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/graph_building.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.260448 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.260448 onnxscript-0.1.0.dev20240417/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2338 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    65860 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10417 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2525 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18651 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1489 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44268 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.264448 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.268448 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.272448 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4288 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.276448 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1424 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6698 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2165 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8844 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46294 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.276448 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5082 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.276448 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39591 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.276448 onnxscript-0.1.0.dev20240417/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.280448 onnxscript-0.1.0.dev20240417/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.280448 onnxscript-0.1.0.dev20240417/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-17 00:01:34.000000 onnxscript-0.1.0.dev20240417/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     7995 2024-04-17 00:01:34.000000 onnxscript-0.1.0.dev20240417/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-17 00:01:34.000000 onnxscript-0.1.0.dev20240417/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-17 00:01:34.000000 onnxscript-0.1.0.dev20240417/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-17 00:01:34.000000 onnxscript-0.1.0.dev20240417/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-17 00:01:34.280448 onnxscript-0.1.0.dev20240417/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240413/LICENSE` & `onnxscript-0.1.0.dev20240417/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/PKG-INFO` & `onnxscript-0.1.0.dev20240417/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240413
+Version: 0.1.0.dev20240417
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
@@ -32,20 +32,21 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: onnx>=1.15
+Requires-Dist: onnx>=1.16
 Requires-Dist: typing_extensions
 
 # ONNX Script
 
 [![CI](https://github.com/microsoft/onnxscript/actions/workflows/main.yaml/badge.svg)](https://github.com/microsoft/onnxscript/actions/workflows/main.yaml)
 [![Dev Release](https://aiinfra.visualstudio.com/ONNX%20Converters/_apis/build/status%2Fonnxscript-release-dev?branchName=main&label=Dev%20Release)](https://aiinfra.visualstudio.com/ONNX%20Converters/_build/latest?definitionId=1258&branchName=main)
 [![PyPI - Version](https://img.shields.io/pypi/v/onnxscript.svg)](https://pypi.org/project/onnxscript)
```

### Comparing `onnxscript-0.1.0.dev20240413/README.md` & `onnxscript-0.1.0.dev20240417/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240417/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,15 @@
         self.op_type: str = node_proto.op_type
         if populate_io:
             self.inputs: list[Value | None] = [Value(i) for i in node_proto.input]
             self.outputs: list[Value | None] = [Value(i) for i in node_proto.output]
         else:
             self.inputs: list[Value | None] = []
             self.outputs: list[Value | None] = []
+        # TODO: attributes are never populated.
         self.attributes: dict[str, int | float | RefAttr | Graph | list[Graph]] = {}
 
     def __repr__(self) -> str:
         return (
             f"{self.op_type}({','.join(self.original_node_proto.input)})"
             f"->{','.join(self.original_node_proto.output)}"
         )
```

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_legacy_ir/irbuilder.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_legacy_ir/protobuilder.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/protobuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,14 +104,17 @@
             node_proto.input.append(i.name if i is not None else "")
         for o in ir_node.outputs:
             assert o is not None
             node_proto.output.append(o.name)
         for attr in ir_node.attributes.items():
             attr_proto = self.process_attribute(attr)
             node_proto.attribute.append(attr_proto)
+        if len(ir_node.attributes) == 0 and len(ir_node.original_node_proto.attribute) > 0:
+            # ir_node.attributes is never populated.
+            node_proto.attribute.extend(ir_node.original_node_proto.attribute)
         return node_proto
 
     def process_attribute(self, attr):
         attr_name, attr_val = attr
         if isinstance(attr_val, ir.RefAttr):
             return attr_val.to_proto()
         if isinstance(attr_val, ir.Graph):
```

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240417/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240417/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240417/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240417/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240417/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/graph_building.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/graph_building.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -2453,15 +2453,15 @@
 
 def aten_diagflat(self: TensorType, offset: int = 0) -> TensorType:
     """diagflat(Tensor self, int offset=0) -> Tensor"""
 
     raise NotImplementedError()
 
 
-@torch_op("aten::diagonal", trace_only=True)
+@torch_op(("aten::diagonal", "aten::diagonal_copy"), trace_only=True)
 def aten_diagonal(self: TReal, offset: int = 0, dim1: int = 0, dim2: int = 1) -> TReal:
     """diagonal(Tensor(a) self, int offset=0, int dim1=0, int dim2=1) -> Tensor(a)"""
 
     # perm is used to transpose the tensor to make dim1 and dim2 as the last 2 dims
     # [0,1,2] -> [2,0,1] when dim1=0 and dim2=1
     # [0,1,2] -> [1,0,2] when dim1=0 and dim2=2
     # [0,1,2] -> [0,1,2] when dim1=1 and dim2=2
@@ -3933,44 +3933,28 @@
 
 def _shape_of_broadcast_tensors(*args: TensorType) -> INT64:
     """Returns the broadcasted shape of the given tensors."""
     broadcasted = op.Max(*args)
     return op.Shape(broadcasted)
 
 
-@torch_op(("aten::index.Tensor", "aten::_unsafe_index.Tensor"), trace_only=True)
-def aten_index(self: TensorType, indices: Sequence[Optional[INT64]]) -> TensorType:
-    """index.Tensor(Tensor self, Tensor?[] indices) -> Tensor
-
-    NOTE: Understanding `aten::index`
-    For `arg0` with shape `[7, 3, 4, 5, 6]`
-    The indexing operation `arg0[0, :, 1:2, tensor([[4,5]])]` will be translated to
-
-    ```
-    +>  select: i64[3, 4, 5, 6] = torch.ops.aten.select.int(arg0, 0, 0);
-    +>  slice_1: i64[3, 4, 5, 6] = torch.ops.aten.slice.Tensor(select, 0, 0, 9223372036854775807);
-    +>  slice_2: i64[3, 1, 5, 6] = torch.ops.aten.slice.Tensor(slice_1, 1, 1, 2);
-    +>  index: i64[3, 1, 1, 2, 6] = torch.ops.aten.index.Tensor(slice_2, [None, None, arg1]);
-    ```
-
-    Here,
-    - `indices = [None, None, arg1]` is equivalent to `indices = [None, None, arg1, None]`
-    - The operation `arg0[0, :, 1:2, tensor([[4,5]])]` is equivalent to `arg0[0, :, 1:2, tensor([[4,5]]), :]`
-
-    None in `indices` are like fillers for dimensions that cannot be removed in the process.
-    """
-
+@torch_op("aten::index.Tensor", private=True, trace_only=True)
+def _aten_index_onnx(
+    self: TensorType,
+    indices: Sequence[Optional[INT64]],
+    index_ranks: Sequence[int],
+) -> TensorType:
     self_rank = len(self.shape)
-    index_ranks = [len(index.shape) for index in indices if index is not None]
     advanced_indexing_rank = max(index_ranks)
 
     # reordered_positions is the permutation of the index positions where
     # positions with None are move to the end of the list
     # For example, if indices = [None, 1, None, 2], then reordered_positions = [1, 3, 0, 2]
     reordered_positions = sorted(range(len(indices)), key=lambda i: (indices[i] is None, i))
+
     # Fill the list with the remaining indices up to the rank of the tensor self.
     # For example, if indices = [None, 1, None, 2], and the rank of self is 6,
     # then reordered_positions = [1, 3, 0, 2, 4, 5]
     reordered_positions = [
         *reordered_positions,
         *range(len(reordered_positions), self_rank),
     ]
@@ -4031,14 +4015,82 @@
             result_rank,
         ),  # None_back_1...None_back_m
     ]
 
     return op.Transpose(self, perm=perm)
 
 
+@torch_op(("aten::index.Tensor", "aten::_unsafe_index.Tensor"), trace_only=True)
+def aten_index(self: TensorType, indices: Sequence[Optional[INT64]]) -> TensorType:
+    """index.Tensor(Tensor self, Tensor?[] indices) -> Tensor
+
+    NOTE: Understanding `aten::index`
+    For `arg0` with shape `[7, 3, 4, 5, 6]`
+    The indexing operation `arg0[0, :, 1:2, tensor([[4,5]])]` will be translated to
+
+    ```
+    +>  select: i64[3, 4, 5, 6] = torch.ops.aten.select.int(arg0, 0, 0);
+    +>  slice_1: i64[3, 4, 5, 6] = torch.ops.aten.slice.Tensor(select, 0, 0, 9223372036854775807);
+    +>  slice_2: i64[3, 1, 5, 6] = torch.ops.aten.slice.Tensor(slice_1, 1, 1, 2);
+    +>  index: i64[3, 1, 1, 2, 6] = torch.ops.aten.index.Tensor(slice_2, [None, None, arg1]);
+    ```
+
+    Here,
+    - `indices = [None, None, arg1]` is equivalent to `indices = [None, None, arg1, None]`
+    - The operation `arg0[0, :, 1:2, tensor([[4,5]])]` is equivalent to `arg0[0, :, 1:2, tensor([[4,5]]), :]`
+
+    None in `indices` are like fillers for dimensions that cannot be removed in the process.
+    """
+
+    index_ranks = [len(index.shape) for index in indices if index is not None]
+
+    return _aten_index_onnx(self, indices, index_ranks)
+
+
+@torch_op(("aten::index.Tensor", "aten::_unsafe_index.Tensor"), trace_only=True)
+def aten_index_bool(self: TensorType, indices: Sequence[Optional[BOOL]]) -> TensorType:  # pylint: disable=inconsistent-return-statements
+    index_ranks = [len(index.shape) for index in indices if index is not None]
+
+    if index_ranks[0] == 1:
+        # indices contains scalar only.
+        new_indices = [
+            op.Transpose(op.NonZero(index), perm=[1, 0]) if index is not None else None
+            for index in indices
+        ]
+        new_indices = [
+            op.Squeeze(index, axes=[1]) if index is not None else None for index in new_indices
+        ]
+        return _aten_index_onnx(self, new_indices, index_ranks)
+    else:
+        input_rank = len(self.shape)
+        # Prepare perm for transposing self tensor.
+        # In indices, None meaning skip the corresponding dimension,
+        # so we need to move this dimension to the end of the list.
+        # After we gathered the final results, we transpose it back.
+        # For example,
+        # self's shape is [5, 5, 5, 5], indices is [None, (5, 5)]
+        # the final result's shape should be [5, 16, 5].
+        trans_perm = list(range(input_rank))
+        trans_perm.append(trans_perm.pop(0))
+        count_of_none = 0
+        for index in indices:
+            if index is None:
+                self = op.Transpose(self, perm=trans_perm)
+                count_of_none += 1
+            else:
+                new_indices = op.Transpose(op.NonZero(index), perm=[1, 0])
+                result = op.GatherND(self, new_indices, batch_dims=0)
+                finla_rank = input_rank - (len(index.shape) - 1)
+                trans_perm = list(range(finla_rank))
+                trans_perm = trans_perm[-1:] + trans_perm[:-1]
+                for _ in range(count_of_none):
+                    result = op.Transpose(result, perm=trans_perm)
+                return result
+
+
 def aten_index_add(
     self: TensorType, dim: int, index: TensorType, source: TensorType, alpha: float = 1
 ) -> TensorType:
     """index_add(Tensor self, int dim, Tensor index, Tensor source, *, Scalar alpha=1) -> Tensor"""
 
     raise NotImplementedError()
 
@@ -5784,37 +5836,45 @@
         input_sub_mean = op.Sub(input, mean)
         sqr_input_sub_mean = op.Mul(input_sub_mean, input_sub_mean)
         running_var = op.Squeeze(op.ReduceMean(sqr_input_sub_mean, axes))
 
     # We have to split to two private functions, because BatchNormalization returns
     # three outputs when training_mode=True and one when it is False.
     if training:
-        norm, input_mean, input_rstd, running_mean, running_var = (
-            _aten_native_batch_norm_training_onnx(
-                input,
-                weight,
-                bias,
-                running_mean,
-                running_var,
-                axes,
-                momentum=1.0 - momentum,
-                eps=eps,
-            )
+        (
+            norm,
+            input_mean,
+            input_rstd,
+            running_mean,
+            running_var,
+        ) = _aten_native_batch_norm_training_onnx(
+            input,
+            weight,
+            bias,
+            running_mean,
+            running_var,
+            axes,
+            momentum=1.0 - momentum,
+            eps=eps,
         )
     else:
-        norm, input_mean, input_rstd, running_mean, running_var = (
-            _aten_native_batch_norm_inference_onnx(
-                input,
-                weight,
-                bias,
-                running_mean,
-                running_var,
-                momentum=1.0 - momentum,
-                eps=eps,
-            )
+        (
+            norm,
+            input_mean,
+            input_rstd,
+            running_mean,
+            running_var,
+        ) = _aten_native_batch_norm_inference_onnx(
+            input,
+            weight,
+            bias,
+            running_mean,
+            running_var,
+            momentum=1.0 - momentum,
+            eps=eps,
         )
 
     return norm, input_mean, input_rstd, running_mean, running_var
 
 
 def aten_native_batch_norm_backward(
     grad_out: TensorType,
@@ -7856,22 +7916,14 @@
 
 
 @torch_op("aten::sym_size")
 def aten_sym_size(self: TReal, dim: int = 0) -> TReal:
     """sym_size(Tensor self, int dim) -> Tensor"""
     # NOTE: onnxscript doesn't support attribute process,
     # so op.Shape(self, start=dim, end=dim + 1) is not supported.
-
-    # TODO(titaiwang): ORT==1.15 fixes SegFault
-    # https://github.com/microsoft/onnxscript/pull/484#discussion_r1136105039
-    # Change the op to:
-    # shape = op.Shape(self)
-    # idx= op.Reshape(dim, [1])
-    # return op.Gather(shape, idx)
-
     shape = op.Shape(self)
     # Reshape helps dim from int to tensor, and
     # input arguments support attribute processing.
     start = op.Reshape(dim, op.Constant(value_ints=[1]))
     end = op.Reshape(dim + 1, op.Constant(value_ints=[1]))
     return op.Slice(shape, start, end)
```

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240417/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240417/onnxscript/ir/_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -426,17 +426,24 @@
     def value(self) -> int | str | None:
         return self._value
 
     @property
     def denotation(self) -> str | None:
         return self._denotation
 
-    def __repr__(self) -> str:
+    def __str__(self) -> str:
         return f"{self._value}"
 
+    def __repr__(self) -> str:
+        if self.denotation is not None:
+            denotation_text = f", denotation={self.denotation!r}"
+        else:
+            denotation_text = ""
+        return f"{self.__class__.__name__}({self._value}{denotation_text})"
+
 
 class Shape(_protocols.ShapeProtocol, _display.PrettyPrintable):
     __slots__ = ("_dims",)
 
     def __init__(self, dims: _protocols.SimpleShape | Sequence[Dimension]) -> None:
         # TODO: Support symbolic shapes with expressions?
         for dim in dims:
@@ -486,15 +493,15 @@
             return
 
         raise TypeError(
             f"Value must be int, str, None or DimensionProtocol. Got '{type(value)}'"
         )
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self._dims})"
+        return f"{self.__class__.__name__}({self._dims!r})"
 
     def __str__(self) -> str:
         """Return a string representation of the shape.
 
         E.g. [n,1,3]
         """
         return f"[{','.join([str(dim) for dim in self._dims])}]"
@@ -525,19 +532,19 @@
 class Node(_protocols.NodeProtocol, _display.PrettyPrintable):
     """IR Node.
 
     If the ``graph`` is provided, the node will be added to the graph. Otherwise,
     user is responsible to call ``graph.append(node)`` (or other mutation methods
     in :class:`Graph`) to add the node to the graph.
 
-    After the node is initialized, it will add itself as a user of the input values.
+    After the node is initialized, it will add itself as a consumer of the input values.
 
     The output values of the node are created during node initialization and are immutable.
-    To change the output values, create a new node and replace the output.users.inputs with
-    the new output values by calling :meth:`replace_input_with` on the user nodes
+    To change the output values, create a new node and replace the each of the inputs of ``output.consumers`` with
+    the new output values by calling :meth:`replace_input_with` on the consumer nodes
     of this node's outputs.
     """
 
     __slots__ = (
         "_name",
         "_domain",
         "_op_type",
@@ -562,15 +569,15 @@
         overload: str = "",
         num_outputs: int = 1,
         version: int | None = None,
         graph: Graph | None = None,
         name: str | None = None,
         doc_string: str | None = None,
     ):
-        """Initialize a node and add it as a user of the input values.
+        """Initialize a node and add it as a consumer of the input values.
 
         Args:
             domain: The domain of the operator. For onnx operators, this is an empty string.
             op_type: The name of the operator.
             inputs: The input values. When an input is None, it is an empty input.
             attributes: The attributes. RefAttr can be used only when the node is defined in a Function.
             overload: The overload name when the node is invoking a function.
@@ -586,31 +593,31 @@
         self._op_type: str = op_type
         # NOTE: Make inputs immutable with the assumption that they are not mutated
         # very often. This way all mutations can be tracked.
         # If necessary, we can cache the inputs and outputs as tuples.
         self._inputs: tuple[Value | None, ...] = tuple(inputs)
         # Values belong to their defining nodes. The values list is immutable
         self._outputs: tuple[Value, ...] = tuple(
-            Value(self, def_index=i) for i in range(num_outputs)
+            Value(self, index=i) for i in range(num_outputs)
         )
         self._attributes: OrderedDict[str, Attr | RefAttr] = OrderedDict(
             (attr.name, attr) for attr in attributes
         )
         self._overload: str = overload
         # TODO(justinchuby): Potentially support a version range
         self._version: int | None = version
         self._metadata: _metadata.MetadataStore | None = None
         self._metadata_props: dict[str, str] | None = None
         self._graph: Graph | None = graph
         self.doc_string = doc_string
 
-        # Add the node as a user of the inputs
+        # Add the node as a consumer of the inputs
         for i, input_value in enumerate(self._inputs):
             if input_value is not None:
-                input_value._add_user(self, i)  # pylint: disable=protected-access
+                input_value._add_consumer(self, i)  # pylint: disable=protected-access
 
         # Add the node to the graph if graph is specified
         if self._graph is not None:
             self._graph.append(self)
 
     def __str__(self) -> str:
         node_type_text = f"{self._domain}::{self._op_type}" + f":{self._overload}" * (
@@ -618,15 +625,15 @@
         )
         inputs_text = (
             "("
             + ", ".join(
                 [
                     (
                         f"%{_quoted(x.name) if x.name else 'anonymous:' + str(id(x))}"
-                        if x
+                        if x is not None
                         else "None"
                     )
                     for x in self._inputs
                 ]
             )
             + ")"
         )
@@ -702,17 +709,17 @@
         if index < 0 or index >= len(self.inputs):
             raise ValueError(f"Index out of range: {index}")
         old_input = self.inputs[index]
         self._inputs = tuple(
             value if i == index else old_input for i, old_input in enumerate(self.inputs)
         )
         if old_input is not None:
-            old_input._remove_user(self, index)  # pylint: disable=protected-access
+            old_input._remove_consumer(self, index)  # pylint: disable=protected-access
         if value is not None:
-            value._add_user(self, index)  # pylint: disable=protected-access
+            value._add_consumer(self, index)  # pylint: disable=protected-access
 
     def prepend(self, /, nodes: Node | Iterable[Node]) -> None:
         """Insert a node before this node in the list of nodes in the graph.
 
         It is the same as calling ``graph.insert_before(self, nodes)``.
 
         Example::
@@ -878,104 +885,128 @@
 
 
 class OptionalType(_RecursiveTypeBase):
     """A type that represents an optional element."""
 
 
 class Value(_protocols.ValueProtocol, _display.PrettyPrintable):
-    """IR Value."""
+    """IR Value.
+
+    A value is a named entity that can be used to represent an input or output of a graph,
+    a function, or a node. The information it stores generalizes over ``ValueInfoProto``
+    in the ONNX specification.
+
+    A :class:`Value` is always not owned or owned by exactly one node. When the value is not
+    owned, it must be an input of a graph or a function. ``producer`` and ``index``
+    are ``None``.
+
+    When the value is owned by a node, it is an output of the node.
+    The node that produces the value can be accessed with :meth:`producer`.
+    The index of the output of the node that produces the value can be accessed with
+    :meth:`index`.
+
+    To find all the nodes that use this value as an input, call :meth:`consumers`.
+
+    To check if the value is an output of a graph, call :meth:`is_graph_output`.
+
+    Attributes:
+        name: The name of the value. A value is always named when it is part of a graph.
+        shape: The shape of the value.
+        type: The type of the value.
+        metadata_props: Metadata.
+    """
 
     __slots__ = (
-        "_def_node",
-        "_def_index",
+        "_producer",
+        "_index",
         "_metadata",
         "_metadata_props",
         "_name",
         "_shape",
         "_type",
         "_const_value",
-        "_users",
+        "_consumers",
     )
 
     def __init__(
         self,
-        def_node: Node | None,
+        producer: Node | None,
         *,
-        def_index: int | None,
+        index: int | None,
         name: str | None = None,
         shape: Shape | None = None,
         type: _protocols.TypeProtocol | None = None,
         const_value: _protocols.TensorProtocol
         | Sequence[_protocols.TensorProtocol]
         | None = None,
     ) -> None:
-        # def_node is None when the value is an input or an initializer
-        self._def_node: Node | None = def_node
-        self._def_index: int | None = def_index
+        # producer is None when the value is an input or an initializer
+        self._producer: Node | None = producer
+        self._index: int | None = index
         self._metadata: _metadata.MetadataStore | None = None
         self._metadata_props: dict[str, str] | None = None
 
         self._name: str | None = name
         self._shape: Shape | None = shape
         self._type: _protocols.TypeProtocol | None = type
         # TODO(justinchuby): Handle initialization when a const value is provided
         # We can get shape and type information from the const value
         self._const_value = const_value
-        # Use a collection of (Node, int) to store users. This is needed
-        # because a single user can use the same value multiple times.
-        self._users: set[tuple[Node, int]] = set()
+        # Use a collection of (Node, int) to store consumers. This is needed
+        # because a single consumer can use the same value multiple times.
+        self._consumers: set[tuple[Node, int]] = set()
 
     def __repr__(self) -> str:
         value_name = self.name if self.name else "anonymous:" + str(id(self))
-        def_node = self.def_node()
-        def_node_text = (
-            def_node.name or "anonymous_node:" + str(id(def_node))
-            if def_node is not None
+        producer = self.producer()
+        producer_text = (
+            producer.name or "anonymous_node:" + str(id(producer))
+            if producer is not None
             else None
         )
-        return f"{self.__class__.__name__}({value_name!r}, type={self.type!r}, shape={self.shape}, def_node={def_node_text}, def_index={self.def_index()})"
+        return f"{self.__class__.__name__}({value_name!r}, type={self.type!r}, shape={self.shape}, producer={producer_text}, index={self.index()})"
 
     def __str__(self) -> str:
         value_name = self.name if self.name else "anonymous:" + str(id(self))
         shape_text = str(self.shape) if self.shape is not None else "?"
         type_text = str(self.type) if self.type is not None else "?"
 
         # Quote the name because in reality the names can have invalid characters
         # that make them hard to read
         return f"%{_quoted(value_name)}<{type_text},{shape_text}>"
 
-    def def_node(self) -> Node | None:
+    def producer(self) -> Node | None:
         """The node that produces this value."""
-        return self._def_node
+        return self._producer
 
-    def def_index(self) -> int | None:
+    def index(self) -> int | None:
         """The index of the output of the defining node."""
-        return self._def_index
+        return self._index
 
-    def users(self) -> frozenset[tuple[Node, int]]:
-        """Return a set of users of the value.
+    def consumers(self) -> frozenset[tuple[Node, int]]:
+        """Return a set of consumers of the value.
 
         The set contains tuples of ``(Node, index)`` where the index is the index of the input
-        of the node. For example, if ``node.inputs[1] == value``, then the user is ``(node, 1)``.
+        of the node. For example, if ``node.inputs[1] == value``, then the consumer is ``(node, 1)``.
         """
-        return frozenset(self._users)
+        return frozenset(self._consumers)
 
-    def _add_user(self, user: Node, index: int) -> None:
-        """Add a user node.
+    def _add_consumer(self, consumer: Node, index: int) -> None:
+        """Add a consumer node.
 
         This is an internal method. It should only be called by the Node class.
         """
-        self._users.add((user, index))
+        self._consumers.add((consumer, index))
 
-    def _remove_user(self, user: Node, index: int) -> None:
-        """Remove a node from the users of this value.
+    def _remove_consumer(self, consumer: Node, index: int) -> None:
+        """Remove a node from the consumers of this value.
 
         This is an internal method. It should only be called by the Node class.
         """
-        self._users.remove((user, index))
+        self._consumers.remove((consumer, index))
 
     @property
     def name(self) -> str | None:
         return self._name
 
     @name.setter
     def name(self, value: str | None) -> None:
@@ -1062,35 +1093,35 @@
     def metadata_props(self) -> dict[str, str]:
         if self._metadata_props is None:
             self._metadata_props = {}
         return self._metadata_props
 
     def is_graph_output(self) -> bool:
         """Whether the value is an output of a graph."""
-        def_node = self.def_node()
-        if def_node is None:
+        producer = self.producer()
+        if producer is None:
             return False
-        if def_node.graph is None:
+        if producer.graph is None:
             return False
-        return self in def_node.graph.outputs
+        return self in producer.graph.outputs
 
 
 class Input(Value):
     """Input of a Graph or a Function."""
 
     # Slots already defined in Value
     __slots__ = ()
 
     def __init__(
         self,
         name: str | None = None,
         shape: Shape | None = None,
         type: _protocols.TypeProtocol | None = None,
     ) -> None:
-        super().__init__(None, def_index=None)
+        super().__init__(None, index=None)
         self._name = name
         self._shape = shape
         self._type = type
 
 
 class Graph(_protocols.GraphProtocol, Sequence[Node], _display.PrettyPrintable):
     """IR Graph.
@@ -1307,19 +1338,19 @@
     initializers_text = ",\n".join(str(x) for x in graph.initializers.values())
     if initializers_text:
         initializers_text = (
             "\ninitializers=(\n" + textwrap.indent(initializers_text, " " * 4) + "\n),"
         )
     signature = f"""\
 graph(
-name={graph.name or 'anonymous_graph:' + str(id(graph))},
-inputs=({textwrap.indent(inputs_text, ' '*8)}
-),
-outputs=({textwrap.indent(outputs_text, ' '*8)}
-),{textwrap.indent(initializers_text, ' '*4)}
+    name={graph.name or 'anonymous_graph:' + str(id(graph))},
+    inputs=({textwrap.indent(inputs_text, ' '*8)}
+    ),
+    outputs=({textwrap.indent(outputs_text, ' '*8)}
+    ),{textwrap.indent(initializers_text, ' '*4)}
 )"""
     node_count = len(graph)
     number_width = len(str(node_count))
     node_lines = []
     for i, node in enumerate(graph.nodes):
         node_name = node.name if node.name else f":anonymous_node:{id(node)}"
         node_text = f"# {node_name}\n{node}"
```

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240417/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240417/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240417/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240417/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240417/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240417/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240417/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240417/onnxscript/ir/_protocols.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,27 +118,27 @@
 
 
 @typing.runtime_checkable
 class ValueProtocol(Protocol):
     """Protocol for values.
 
     A value is a named entity that can be used to represent an input or output of a graph,
-    a function, or a node. The information it stores corresponds to ``ValueInfoProto``
+    a function, or a node. The information it stores generalizes over ``ValueInfoProto``
     in the ONNX specification.
 
     A :class:`Value` is always not owned or owned by exactly one node. When the value is not
-    owned, it must be an input of a graph or a function. ``def_node`` and ``def_index``
+    owned, it must be an input of a graph or a function. ``producer`` and ``index``
     are ``None``.
 
     When the value is owned by a node, it is an output of the node.
-    The node that produces the value can be accessed with :meth:`def_node`.
+    The node that produces the value can be accessed with :meth:`producer`.
     The index of the output of the node that produces the value can be accessed with
-    :meth:`def_index`.
+    :meth:`index`.
 
-    To find all the nodes that use this value as an input, call :meth:`users`.
+    To find all the nodes that use this value as an input, call :meth:`consumers`.
 
     To check if the value is an output of a graph, call :meth:`is_graph_output`.
 
     Attributes:
         name: The name of the value. A value is always named when it is part of a graph.
         shape: The shape of the value.
         type: The type of the value.
@@ -147,23 +147,23 @@
 
     name: str
     shape: ShapeProtocol | None
     type: TypeProtocol | None
     metadata_props: Mapping[str, str]
     meta: Mapping[str, Any]
 
-    def def_node(self) -> NodeProtocol | None:
+    def producer(self) -> NodeProtocol | None:
         """The node that produces this value."""
         ...
 
-    def def_index(self) -> int | None:
+    def index(self) -> int | None:
         """The index of the output of the node that produces this value."""
         ...
 
-    def users(self) -> AbstractSet[tuple[NodeProtocol, int]]:
+    def consumers(self) -> AbstractSet[tuple[NodeProtocol, int]]:
         """The set of (node, input_index) with node being those that use this value as an input."""
         ...
 
     def is_graph_output(self) -> bool:
         """Whether this value is an output of a graph."""
         ...
```

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/ir/convenience.py` & `onnxscript-0.1.0.dev20240417/onnxscript/ir/convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240417/onnxscript/ir/serde.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,15 +386,15 @@
         if initializer.name in values:
             # The initializer is for an input
             values[initializer.name].const_value = initializer
         else:
             # The initializer is for some other value. Create this value first
             initializer_value = _core.Value(
                 None,
-                def_index=None,
+                index=None,
                 name=initializer.name,
                 # TODO(justinchuby): Fix type hinting for shape and dtype
                 shape=initializer.shape,  # type: ignore
                 type=_core.TensorType(initializer.dtype),
                 const_value=initializer,
             )
             values[initializer.name] = initializer_value
@@ -454,33 +454,32 @@
     )
 
 
 def deserialize_value_info_proto(
     proto: onnx.ValueInfoProto, value: _core.Value | None
 ) -> _core.Value:
     if value is None:
-        value = _core.Value(None, def_index=None)
+        value = _core.Value(None, index=None)
         value.name = proto.name
     value.shape = deserialize_type_proto_for_shape(proto.type)
     value.type = deserialize_type_proto_for_type(proto.type)
     return value
 
 
 def deserialize_type_proto_for_shape(proto: onnx.TypeProto) -> _core.Shape | None:
     if proto.HasField("tensor_type"):
         if (shape_proto := _get_field(proto.tensor_type, "shape")) is None:
             return None
-        if not (dim_protos := shape_proto.dim):
-            return None
+        # This logic handles when the shape is [] as well
+        dim_protos = shape_proto.dim
         return _core.Shape([deserialize_dimension(d) for d in dim_protos])
     if proto.HasField("sparse_tensor_type"):
         if (shape_proto := _get_field(proto.sparse_tensor_type, "shape")) is None:
             return None
-        if not (dim_protos := shape_proto.dim):
-            return None
+        dim_protos = shape_proto.dim
         return _core.Shape([deserialize_dimension(d) for d in dim_protos])
     if proto.HasField("sequence_type"):
         if (elem_type := _get_field(proto.sequence_type, "elem_type")) is None:
             return None
         return deserialize_type_proto_for_shape(elem_type)
     if proto.HasField("optional_type"):
         if (elem_type := _get_field(proto.optional_type, "elem_type")) is None:
@@ -651,15 +650,15 @@
     node = _core.Node(
         proto.domain,
         proto.op_type,
         node_inputs,
         [_deserialize_attribute(a, scoped_values) for a in proto.attribute],
         overload=getattr(proto, "overload", ""),
         num_outputs=len(proto.output),
-        name=_get_field(proto, "name"),
+        name=proto.name,
     )
 
     for output, value in zip(proto.output, node.outputs):
         value.name = output
         if output in value_info:
             deserialize_value_info_proto(value_info[output], value)
         else:
@@ -1124,14 +1123,16 @@
         serialize_type_into(optional_type_proto.elem_type, from_.elem_type)
     else:
         raise TypeError(f"Unsupported type: {from_}")
 
 
 def serialize_shape_into(type_proto: onnx.TypeProto, from_: _protocols.ShapeProtocol) -> None:
     tensor_type_proto = type_proto.tensor_type
+    # When from is empty, we still need to set the shape field to an empty list by touching it
+    tensor_type_proto.shape.ClearField("dim")
     for dim in from_:
         serialize_dimension_into(tensor_type_proto.shape.dim.add(), from_=dim)
 
 
 def serialize_dimension_into(
     dim_proto: onnx.TensorShapeProto.Dimension, from_: _protocols.DimensionProtocol
 ) -> None:
```

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240417/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/main.py` & `onnxscript-0.1.0.dev20240417/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240417/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/optimizer/copy_propagation.py` & `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/copy_propagation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,9 +426,13 @@
     position = context.get_input(node, 1)
     output = context.get_output(node, 0)
     if input is not None and position is not None:
         input_vals = input.symbolic_value
         position_val = position.value
         if isinstance(input_vals, list) and position_val is not None:
             output.symbolic_value = input_vals[position_val]
-            logger.debug("SquenceAt %s => %s", input, output.symbolic_value)
+            logger.debug("SequenceAt %s => %s", input, output.symbolic_value)
+            new_node = onnx.helper.make_node(
+                "Identity", [output.symbolic_value], [output.name]
+            )
+            return [new_node]
     return None
```

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/generic_pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import textwrap
 import typing
 
 import onnx
 import onnx.helper as oh
 
+import onnxscript
 import onnxscript._legacy_ir as oir
 import onnxscript.rewriter.pattern as orp
 
 
 def enumerate_subgraphs(
     node: oir.Node,
 ) -> typing.Iterator[tuple[typing.Any, ...]]:
@@ -290,14 +291,98 @@
             **kwargs,
         )
         if attributes:
             proto.attribute.extend(attributes)
         return proto
 
 
+class PatternMatchResult:
+    """Stores information about a match if a match was successful.
+
+    * pattern: the instance of :class:`GenericPattern` which found this result
+    * model_nodes: matched nodes coming from the model
+    * pattern_nodes: corresponding nodes coming from the pattern
+    * pattern_input_names: input names of the pattern
+    * pattern_ouptut_names: output names of the pattern
+    * kwargs: additional attributes the user may add through the method
+        :meth:`PatternMatchResult.add_kwargs`
+
+    The class creates one attributes `matched_pattern_to_model_name`,
+    which maps every result name from the pattern to the corresponding
+    result name in the model.
+    """
+
+    def __init__(
+        self,
+        pattern: GenericPattern,
+        model_nodes: typing.Sequence[oir.Node],
+        pattern_nodes: typing.Sequence[oir.Node],
+        pattern_input_names: typing.Sequence[str],
+        pattern_output_names: typing.Sequence[str],
+    ):
+        assert len(model_nodes) == len(pattern_nodes)
+        self.pattern = pattern
+        self.model_nodes = model_nodes
+        self.pattern_nodes = pattern_nodes
+        self.pattern_input_names = pattern_input_names
+        self.pattern_output_names = pattern_output_names
+        self.kwargs = {}
+
+        matched_pattern_to_model_name: dict[str, str] = {}
+        for gn, pn in zip(model_nodes, pattern_nodes):
+            assert (
+                gn.op_type == pn.op_type
+            ), f"Unexpected type mismatch {gn.op_type!r} != {pn.op_type!r}"
+            assert len(gn.input_names) == len(
+                pn.input_names
+            ), f"Unexpected number of inputs for type {gn.op_type}"
+            for a, b in zip(gn.input_names, pn.input_names):
+                if b == "":
+                    # optional input or not an interesting input
+                    continue
+                if b in matched_pattern_to_model_name:
+                    assert matched_pattern_to_model_name[b] == a, (
+                        f"Ambiguities, pattern name {b!r} means "
+                        f"{a!r} or {matched_pattern_to_model_name[b]}"
+                    )
+                else:
+                    matched_pattern_to_model_name[b] = a
+
+            assert len(gn.output_names) == len(
+                pn.output_names
+            ), f"Unexpected number of outputs for type {gn.op_type}"
+            for a, b in zip(gn.output_names, pn.output_names):
+                if b == "":
+                    # Only final outputs are interesting.
+                    continue
+                assert a != "", f"{a!r} cannot be optional"
+                if b in matched_pattern_to_model_name:
+                    assert matched_pattern_to_model_name[b] == a, (
+                        f"Ambiguities, pattern name {b!r} means "
+                        f"{a!r} or {matched_pattern_to_model_name[b]}"
+                    )
+                else:
+                    matched_pattern_to_model_name[b] = a
+
+        self.matched_pattern_to_model_name = matched_pattern_to_model_name
+
+    def add_kwargs(self, name: str, value: typing.Any):
+        """Adds an attribute, it can be done when the match is being validated,
+        this attribute can be used when building the replacement nodes.
+        """
+        self.kwargs[name] = value
+
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}([{self.pattern.__class__.__name__}], "
+            f"... {len(self.model_nodes)} nodes ..., {self.pattern_input_names}, "
+            f"{self.pattern_output_names})"
+        )
+
+
 class GenericRewriteRule(orp.RewriteRule):
     """
     Defines a rewriting rule.
 
     :param pattern: a pattern defines by :class:`GenericPattern`.
     """
 
@@ -317,38 +402,40 @@
             bridge = model
         else:
             bridge = ModelWithGraphStructure(model)
         deleted_nodes = []
         added_nodes = []
         marked = set()
         matched = 0
-        for matched_nodes in self.pattern.enumerate_matches(bridge, node):
-            assert all(isinstance(i, oir.Node) for i in matched_nodes)
+        for match_result in self.pattern.enumerate_matches(bridge, node):
             conflict = False
-            for node in matched_nodes:
+            for node in match_result.model_nodes:
                 if id(node) in marked:
                     conflict = True
                     break
             if conflict:
                 # Some nodes are already marked as rewritten.
                 continue
 
             # Let's build the new nodes
-            new_nodes = self.pattern.apply(bridge, *matched_nodes)
+            if not self.pattern.validate_mapping(bridge, match_result):
+                match_result._hint(
+                    "validate_mapping", "The pattern was rejected by the validation function."
+                )
+                continue
+
+            new_nodes = self.pattern.apply(bridge, match_result)
             assert all(
                 isinstance(i, oir.Node) for i in new_nodes
             ), f"Unexpected types {[type(n) for n in new_nodes]}"
 
-            if not self.pattern.validate_mapping(bridge, matched_nodes, new_nodes):
-                continue
-
             # Everything is good.
-            marked |= set(map(id, matched_nodes))
+            marked |= set(map(id, match_result.model_nodes))
             added_nodes.extend(new_nodes)
-            deleted_nodes.extend(matched_nodes)
+            deleted_nodes.extend(match_result.model_nodes)
             matched += 1
 
         if matched > 0:
             return matched, deleted_nodes, added_nodes
         return None
 
     def count_matches(self, model: oir.Model, *, commute: bool = False) -> int:
@@ -374,17 +461,15 @@
     * It does not compares attributes either (easy fix as well).
     """
 
     def __init__(self, verbose: int = 0):
         self.verbose = verbose
         self._cache: dict = {}
 
-    def validate_mapping(
-        self, g: oir.Model, deleted_nodes: list[oir.Node], added_nodes: list[oir.Node]
-    ) -> bool:
+    def validate_mapping(self, g: oir.Model, match_result: PatternMatchResult) -> bool:
         """Evaluates the consistency of the replacements."""
         raise NotImplementedError(
             "This method could return True but it is better to let you know "
             "that it exists. You need to overwrite it to return True."
         )
 
     def enumerate_matches(
@@ -473,18 +558,27 @@
         **kwargs: typing.Any,
     ) -> list[oir.Node] | None:
         """Builds the pattern to match."""
         raise NotImplementedError(
             f"Class {cls.__name__!r} must overwrite method match_pattern."
         )
 
-    @classmethod
     def _build_pattern(
-        cls, g: ModelWithGraphStructure, fct: typing.Callable
+        self,
+        g: ModelWithGraphStructure,
+        fct: typing.Callable | None = None,
+        match: bool = True,
+        kwargs: dict[str, typing.Any] | None = None,
     ) -> BuilderWithGraphStructure:
+        del match
+        assert fct, f"Not implemented if fct is None in class {self.__class__.__name__}"
+        assert not kwargs, (
+            f"Not implemented when kwargs is not empty but {kwargs} "
+            f"in class {self.__class__.__name__}"
+        )
         kwargs = {}
         args = []
 
         # There should be a better way.
         sig = inspect.signature(fct)
         for i, p in enumerate(sig.parameters.values()):
             if i == 0:
@@ -510,41 +604,27 @@
         return g2
 
     def _get_match_pattern(self, g: ModelWithGraphStructure) -> BuilderWithGraphStructure:
         cache_key = 0, tuple(sorted(g.opsets.items()))
         if cache_key in self._cache:
             return self._cache[cache_key]
 
-        pat = self._build_pattern(g, self.match_pattern)
+        pat = self._build_pattern(g, fct=self.match_pattern, match=True)
         self._cache[cache_key] = pat
         return pat
 
     def _get_apply_pattern(self, g: ModelWithGraphStructure) -> BuilderWithGraphStructure:
         cache_key = 1, tuple(sorted(g.opsets.items()))
         if cache_key in self._cache:
             return self._cache[cache_key]
 
-        pat = self._build_pattern(g, self.apply_pattern)
+        pat = self._build_pattern(g, fct=self.apply_pattern, match=False)
         self._cache[cache_key] = pat
         return pat
 
-    def display_pattern(self, g: ModelWithGraphStructure, fct: typing.Callable) -> str:
-        """Shows the pattern to match or to apply."""
-        pat = self._build_pattern(g, fct)
-        rows = []
-        rows.append(
-            f"{fct.__name__}({', '.join(pat.input_names)}) -> {', '.join(pat.output_names)}"
-        )
-        for node in pat.nodes:
-            rows.append(
-                f"{node.op_type}({', '.join(node.input_names)}) -> "
-                f"{', '.join(node.output_names)}"
-            )
-        return "\n".join(rows)
-
     def print_match(self, n1: oir.Node, n2: oir.Node) -> str:
         s1 = f"{n1.op_type}({','.join(n1.input_names)})"
         s2 = f"{n2.op_type}({','.join(n2.input_names)})"
         return f"match {s1} with {s2} (pattern)"
 
     def _debug_print(self) -> str:
         if not hasattr(self, "_debug"):
@@ -825,15 +905,15 @@
             print(f"[GenericPattern._match_forward] add {res} nodes")
         return res
 
     def match(
         self,
         g: ModelWithGraphStructure,
         node: oir.Node,
-    ) -> list[oir.Node] | None:
+    ) -> PatternMatchResult | None:
         self._debug = {}
 
         pat = self._get_match_pattern(g)
 
         # Let's match the last node.
         # Then we need to match successors and predecessors.
         p_node = pat.nodes[-1]  # the last one
@@ -844,16 +924,15 @@
         check_ids = {id(n) for n in pat.nodes}
         if self.verbose > 5:
             print(
                 f"[GenericPattern.match] starts with "
                 f"{node.op_type}({', '.join(node.input_names)})"
             )
             if self.verbose >= 10:
-                print("[GenericPattern.match] match pattern")
-                print(textwrap.indent(self.display_pattern(g, self.match_pattern), "    "))
+                print(f"[GenericPattern.match] match pattern {self!r}")
 
         marked = {id(p_node): (node, p_node)}
         stacked = [id(p_node)]
         iteration = 0
 
         if self.verbose > 5:
             self._debug = dict(
@@ -921,15 +1000,17 @@
             f"and {len(pat.nodes)} nodes in the pattern, marked is {marked}"
         )
         assert len(stacked) == 0, f"There are still {len(stacked)} nodes to explore."
 
         # We order the matched nodes in the same order than the pattern
         # to let next functions to be able to build the matching again.
         matched_nodes = [marked[id(n)][0] for i, n in enumerate(pat.nodes)]
-        return matched_nodes
+        return PatternMatchResult(
+            self, matched_nodes, pat.nodes, pat.input_names, pat.output_names
+        )
 
     @classmethod
     def apply_pattern(
         cls,
         g: ModelWithGraphStructure,
         *args: typing.Any,
         **kwargs: typing.Any,
@@ -938,94 +1019,52 @@
         raise NotImplementedError(
             f"Class {cls.__name__!r} must overwrite method 'apply_pattern'."
         )
 
     def apply(
         self,
         g: ModelWithGraphStructure,
-        *nodes: typing.Sequence[oir.Node],
+        match_result: PatternMatchResult,
     ) -> list[oir.Node]:
-        assert all(isinstance(n, oir.Node) for n in nodes)
-        pat = self._build_pattern(g, self.match_pattern)
-        assert len(nodes) == len(pat.nodes), (
-            f"Mismatch matched nodes pattern has {len(pat.nodes)} != {len(nodes)} = "
-            f"the number of matched nodes"
+        assert isinstance(match_result, PatternMatchResult)
+        new_pat = self._build_pattern(
+            g, fct=self.apply_pattern, kwargs=match_result.kwargs, match=False
         )
-        new_pat = self._build_pattern(g, self.apply_pattern)
-        assert len(new_pat.input_names) == len(pat.input_names), (
-            f"Not the same number of inputs, matched inputs={len(new_pat.input_names)}, "
-            f"got {len(pat.input_names)} in the applied pattern."
+        assert len(new_pat.input_names) == len(match_result.pattern_input_names), (
+            f"Not the same number of inputs, "
+            f"matched inputs={len(new_pat.input_names)}, "
+            f"got {len(match_result.pattern_input_names)} in the applied pattern."
         )
-        assert len(new_pat.output_names) == len(pat.output_names), (
-            f"Not the same number of outputs, matched outputs={pat.output_names}, "
+        assert len(new_pat.output_names) == len(match_result.pattern_output_names), (
+            f"Not the same number of outputs, matched "
+            f"outputs={match_result.pattern_output_names}, "
             f"got {new_pat.output_names} in the applied pattern."
         )
-        assert all(isinstance(n, oir.Node) for n in pat.nodes)
 
         if g.verbose > 5:
             print(
-                f"[GenericPattern.apply] replace {len(nodes)} nodes, "
+                f"[GenericPattern.apply] replace {len(match_result.model_nodes)} nodes, "
                 f"applied {self.display_pattern(g, self.apply_pattern)}"
             )
 
-        matched_pattern_to_applied_pattern = {}
-        for i, j in zip(pat.input_names, new_pat.input_names):
-            matched_pattern_to_applied_pattern[i] = j
-        for i, j in zip(pat.output_names, new_pat.output_names):
-            matched_pattern_to_applied_pattern[i] = j
-
-        matched_pattern_to_graph_name: dict = {}
-        input_names = set(pat.input_names)
-        output_names = set(pat.output_names)
-
-        matched_pairs = list(zip(nodes, pat.nodes))
-        for gn, pn in matched_pairs:
-            assert (
-                gn.op_type == pn.op_type
-            ), f"Unexpected type mismatch {gn.op_type!r} != {pn.op_type!r}"
-            assert len(gn.input_names) == len(
-                pn.input_names
-            ), f"Unexpected number of inputs for type {gn.op_type}"
-            for a, b in zip(gn.input_names, pn.input_names):
-                if b not in input_names or b == "":
-                    # optional input or not an interesting input
-                    continue
-                if b in matched_pattern_to_graph_name:
-                    assert matched_pattern_to_graph_name[b] == a, (
-                        f"Ambiguities, pattern name {b!r} means "
-                        f"{a!r} or {matched_pattern_to_graph_name[b]}"
-                    )
-                else:
-                    matched_pattern_to_graph_name[b] = a
-
-            assert len(gn.output_names) == len(
-                pn.output_names
-            ), f"Unexpected number of outputs for type {gn.op_type}"
-            for a, b in zip(gn.output_names, pn.output_names):
-                if b not in output_names or b == "":
-                    # Only final outputs are interesting.
-                    continue
-                assert a != "", f"{a!r} cannot be optional"
-                if b in matched_pattern_to_graph_name:
-                    assert matched_pattern_to_graph_name[b] == a, (
-                        f"Ambiguities, pattern name {b!r} means "
-                        f"{a!r} or {matched_pattern_to_graph_name[b]}"
-                    )
-                else:
-                    matched_pattern_to_graph_name[b] = a
-
         # TODO: handle initializers here
         # for name, init in pattern.initializers.items():
         #   # We add them to the graph, they will be removed if unused.
         #   new_name = g.make_initializer(name, init)
         #   replacements[new_name] = name
 
+        applied_pattern_to_match_pattern = {}
+        for i, j in zip(match_result.pattern_input_names, new_pat.input_names):
+            applied_pattern_to_match_pattern[j] = i
+        for i, j in zip(match_result.pattern_output_names, new_pat.output_names):
+            applied_pattern_to_match_pattern[j] = i
+
         replacements = {}
-        for k, v in matched_pattern_to_graph_name.items():
-            replacements[matched_pattern_to_applied_pattern[k]] = v
+        for k, v in applied_pattern_to_match_pattern.items():
+            replacements[k] = match_result.matched_pattern_to_model_name[v]
 
         # Creation of the new node.
         new_nodes = []
         for node in new_pat.nodes:
             new_inputs = []
             for i in node.input_names:
                 assert i in replacements, f"Unable to find {i!r} in {replacements}"
@@ -1037,15 +1076,15 @@
                     new_outputs.append(replacements[o])
                 else:
                     # We give it a new name.
                     n = g.unique_name(o)
                     replacements[o] = n
                     new_outputs.append(n)
             new_node = g.make_node(node.op_type, new_inputs, new_outputs, domain=node.domain)
-            new_node.attribute.extend(node.attribute)
+            new_node.attribute.extend(node.original_node_proto.attribute)
             new_nodes.append(oir.Node(new_node, True))
 
         if g.verbose > 5:
             print(f"[GenericPattern.apply] done with {len(new_nodes)} nodes")
 
         return new_nodes
 
@@ -1058,73 +1097,94 @@
     """An instance of GenericPattern taking onnx model.
 
     It defines the matching pattern and its replacement.
 
     :param match_proto: the onnx function defining the matching pattern
     :param apply_proto: the onnx function defining the new pattern
     :param validate_mapping: the function used to validate a pattern
+    :param use_onnxscript: tells if the apply_proto is an onnxscript function or
+        a regular function returning a FunctionProto
+    :param opsets: opset to consider when converting the function into ONNX,
+        if not specified, it is opset 18 for the main opset, and opset 1
+        for domain com.microsoft.
     :param verbose: in [0, 10], increase the verbosity to understand why a pattern
         does not match
     """
 
     def __init__(
         self,
         match_proto: onnx.FunctionProto,
-        apply_proto: onnx.FunctionProto,
+        apply_proto: onnx.FunctionProto | typing.Callable,
         validate_mapping: typing.Callable,
+        use_onnxscript: bool = True,
+        opsets: dict[str, onnxscript.values.Opset] | None = None,
         verbose: int = 0,
     ):
         super().__init__(verbose=verbose)
         self.match_proto = match_proto
         self._validate_mapping = validate_mapping
         self.apply_proto = apply_proto
+        self.use_onnxscript = use_onnxscript
+        self.opsets = opsets
         self._cache = {}
 
-    def validate_mapping(
-        self, g: oir.Model, deleted_nodes: list[oir.Node], added_nodes: list[oir.Node]
-    ) -> bool:
+    def validate_mapping(self, g: oir.Model, match_result: PatternMatchResult) -> bool:
         """Evaluates the consistency of the replacements."""
-        return self._validate_mapping(g, deleted_nodes, added_nodes)
+        return self._validate_mapping(g, match_result)
 
     def _build_pattern(
-        self, g: ModelWithGraphStructure, fct: typing.Callable
+        self,
+        g: ModelWithGraphStructure,
+        fct: typing.Callable | None = None,
+        kwargs: dict[str, typing.Any] | None = None,
+        match: bool = True,
     ) -> BuilderWithGraphStructure:
-        if fct == self.match_pattern:
-            key = id(g), "match"
-            if key in self._cache:
-                return self._cache[key]
-            onx = self.match_proto
-        elif fct == self.apply_pattern:
-            key = id(g), "apply"
-            if key in self._cache:
-                return self._cache[key]
-            onx = self.apply_proto
+        del fct
+        if match:
+            key = id(g), match, str(kwargs)
         else:
-            raise AssertionError(
-                f"Function {fct} is not {self.match_pattern} or {self.apply_pattern}."
-            )
+            key = id(g), match, str(kwargs)
+            assert not callable(self.apply_proto) or isinstance(kwargs, dict)
+        if key in self._cache:
+            return self._cache[key]
+
+        if match:
+            onx = self.match_proto
+        elif callable(self.apply_proto):
+            if self.use_onnxscript:
+                onx = onnxscript.script(**self.opsets)(self.apply_proto).to_function_proto()
+            else:
+                sig = inspect.signature(self.apply_proto)
+                args = []
+                for p in sig.parameters.values():
+                    if p.default is not inspect._empty:
+                        continue
+                    args.append(p.name)
+                onx = self.apply_proto(*args, **kwargs)
+        self._cache[key] = onx
 
         g2 = g.make_opset()
         for name in onx.input:
             g2.make_input(name)
         for node in onx.node:
             g2.make_node_with_proto(node)
         for name in onx.output:
             g2.make_output(name)
         g2._build()
         self._cache[key] = g2
         return g2
 
 
 def make_pattern_rule(
-    match_pattern: typing.Callable,
-    apply_pattern: typing.Callable,
+    match_pattern: typing.Callable | onnx.FunctionProto,
+    apply_pattern: typing.Callable | onnx.FunctionProto,
     validate_mapping: typing.Callable | None = None,
     verbose: int = 0,
-    opsets: dict[str, "onnxscript.Opset"] | None = None,  # noqa: F821
+    use_onnxscript: bool = True,
+    opsets: dict[str, onnxscript.values.Opset] | None = None,
 ) -> orp.RewriteRule:
     """
     Creates a rewriting rule.
 
     :param match_pattern: a function interpreted by onnx-script
         and converted into an onnx model, this model defines the
         nodes to be replaced
@@ -1133,33 +1193,36 @@
         replacing the matched nodes
     :param validate_mapping: a function validating the matching once
         it has happened, it is not valid, the pattern is not applied,
         if not specified, the function always return True
     :param opsets: opset to consider when converting the function into ONNX,
         if not specified, it is opset 18 for the main opset, and opset 1
         for domain com.microsoft.
+    :param use_onnxscript: tells if the apply_proto is an onnxscript function or
+        a regular function returning a FunctionProto
     :return: the rewriting rule
     """
     import onnxscript
 
     if opsets is None:
         opsets = dict(
             op=onnxscript.opset18, msft_op=onnxscript.values.Opset("com.microsoft", 1)
         )
 
     if verbose > 5:
         print(f"[make_pattern_rule] Converting {match_pattern} into ONNX.")
-    match = onnxscript.script(**opsets)(match_pattern).to_function_proto()
-    if verbose > 5:
-        print("[make_pattern_rule] done.")
-        print(f"[make_pattern_rule] Converting {apply_pattern} into ONNX.")
-    apply = onnxscript.script(**opsets)(apply_pattern).to_function_proto()
-    if verbose > 5:
-        print("[make_pattern_rule] done.")
+
+    if isinstance(match_pattern, onnx.FunctionProto):
+        match = match_pattern
+    else:
+        match = onnxscript.script(**opsets)(match_pattern).to_function_proto()
+    assert match.node, f"The match pattern has no node, function={match_pattern}."
 
     pat = OnnxGenericPattern(
         match,
-        apply,
+        apply_pattern,
         validate_mapping or (lambda *_, **__: True),
         verbose=verbose,
+        use_onnxscript=use_onnxscript,
+        opsets=opsets,
     )
     return pat.make_rule()
```

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240417/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240417/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240417/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240417/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240417/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240417/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240417/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript/values.py` & `onnxscript-0.1.0.dev20240417/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240417/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240413
+Version: 0.1.0.dev20240417
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
@@ -32,20 +32,21 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: onnx>=1.15
+Requires-Dist: onnx>=1.16
 Requires-Dist: typing_extensions
 
 # ONNX Script
 
 [![CI](https://github.com/microsoft/onnxscript/actions/workflows/main.yaml/badge.svg)](https://github.com/microsoft/onnxscript/actions/workflows/main.yaml)
 [![Dev Release](https://aiinfra.visualstudio.com/ONNX%20Converters/_apis/build/status%2Fonnxscript-release-dev?branchName=main&label=Dev%20Release)](https://aiinfra.visualstudio.com/ONNX%20Converters/_build/latest?definitionId=1258&branchName=main)
 [![PyPI - Version](https://img.shields.io/pypi/v/onnxscript.svg)](https://pypi.org/project/onnxscript)
```

### Comparing `onnxscript-0.1.0.dev20240413/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240417/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240413/pyproject.toml` & `onnxscript-0.1.0.dev20240417/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -17,28 +17,29 @@
   "Operating System :: POSIX",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "License :: OSI Approved :: MIT License",
 ]
-dependencies = ["numpy", "onnx>=1.15", "typing_extensions"]
+dependencies = ["numpy", "onnx>=1.16", "typing_extensions"]
 
 [tool.setuptools.packages.find]
 include = ["onnxscript*"]
 
 [tool.setuptools.package-data]
 onnxscript = ["py.typed"]
 onnx = ["py.typed"]
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore::UserWarning", "ignore::DeprecationWarning"]
-addopts = "-rsfEX --tb=short --color=yes --doctest-modules"
+addopts = "-rsfEX --tb=short --color=yes"
 
 [tool.mypy]
 # TODO disallow_incomplete_defs = true
 check_untyped_defs = true
 disable_error_code = 'override,import-untyped'
 disallow_any_generics = false
 disallow_untyped_decorators = true
@@ -68,45 +69,45 @@
 module = [
   "setup",
   "tests.models.*",
   "tests.onnx_backend_test_code.*",
 ]
 ignore_errors = true
 
+# FIXME(#1378): Remove this overrides section
 [[tool.mypy.overrides]]
 module = [
   "onnxrewriter.rewriter.generic_pattern_test.*",
 ]
 check_untyped_defs = false
 disable_error_code = 'override,import-untyped,no-untyped-def,assignment'
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 disallow_untyped_decorators = true
 show_column_numbers = true
 strict_optional = true
 warn_incomplete_stub = true
 warn_no_return = true
-warn_redundant_casts = true
 warn_unused_configs = true
 warn_unused_ignores = false
 
+# FIXME(#1378): Remove this overrides section
 [[tool.mypy.overrides]]
 module = [
   "onnxrewriter.rewriter.generic_pattern.*",
 ]
 check_untyped_defs = false
 disable_error_code = 'override,import-untyped,no-untyped-def,assignment,union-attr,func-returns-value,annotation-unchecked,arg-type,index,name-defined,attr-defined'
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 disallow_untyped_decorators = true
 show_column_numbers = true
 strict_optional = true
 warn_incomplete_stub = true
 warn_no_return = true
-warn_redundant_casts = true
 warn_unused_configs = true
 warn_unused_ignores = false
 
 [tool.black]
 target-version = ["py38", "py39", "py310", "py311"]
 # Black's extend-exclude needs to be a regex string
 extend-exclude = "/tests/models|/tests/onnx_backend_test_code"
@@ -195,16 +196,14 @@
 "pathlib".msg = "Using pathlib can impact performance. Use os.path instead"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["TID252"] # Allow relative imports in init files
 "setup.py" = ["TID251"] # pathlib is allowed in supporting code
 "**/{examples,tests,docs,tools,utils,opgen}/*" = ["TID251"] # pathlib is allowed in supporting code
 "**/*_test.py" = ["TID251"] # pathlib is allowed in tests
-"**/generic_pattern.py" = ["FBT003", "UP037"]  # inline ignoring fails
-"**/generic_pattern_test.py" = ["ARG001", "ARG002", "PLR2004"]
 
 [tool.ruff.flake8-tidy-imports]
 # Disallow all relative imports.
 ban-relative-imports = "all"
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `onnxscript-0.1.0.dev20240413/setup.py` & `onnxscript-0.1.0.dev20240417/setup.py`

 * *Files identical despite different names*

