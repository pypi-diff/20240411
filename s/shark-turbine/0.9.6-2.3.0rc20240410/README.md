# Comparing `tmp/shark_turbine-0.9.6-py3-none-any.whl.zip` & `tmp/shark_turbine-2.3.0rc20240410-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,83 +1,87 @@
-Zip file size: 154493 bytes, number of entries: 81
--rw-rw-r--  2.0 unx      313 b- defN 24-Mar-01 19:13 shark_turbine/aot/__init__.py
--rw-rw-r--  2.0 unx    20685 b- defN 24-Mar-02 22:11 shark_turbine/aot/compiled_module.py
--rw-rw-r--  2.0 unx     6938 b- defN 24-Mar-02 22:11 shark_turbine/aot/exporter.py
--rw-rw-r--  2.0 unx      884 b- defN 24-Mar-01 19:13 shark_turbine/aot/builtins/__init__.py
--rw-rw-r--  2.0 unx     5409 b- defN 24-Mar-01 19:13 shark_turbine/aot/builtins/globals.py
--rw-rw-r--  2.0 unx    17841 b- defN 24-Mar-01 19:13 shark_turbine/aot/builtins/jittable.py
--rw-rw-r--  2.0 unx      262 b- defN 24-Mar-01 19:13 shark_turbine/aot/passes/__init__.py
--rw-rw-r--  2.0 unx     3522 b- defN 24-Mar-01 19:13 shark_turbine/aot/passes/functorch.py
--rw-rw-r--  2.0 unx    14145 b- defN 24-Mar-01 19:13 shark_turbine/aot/support/ir_utils.py
--rw-rw-r--  2.0 unx     2158 b- defN 24-Mar-01 19:13 shark_turbine/aot/support/utils.py
--rw-rw-r--  2.0 unx      646 b- defN 24-Mar-01 19:13 shark_turbine/aot/support/procedural/__init__.py
--rw-rw-r--  2.0 unx     7470 b- defN 24-Mar-01 19:13 shark_turbine/aot/support/procedural/base.py
--rw-rw-r--  2.0 unx     9202 b- defN 24-Mar-01 19:13 shark_turbine/aot/support/procedural/globals.py
--rw-rw-r--  2.0 unx    12361 b- defN 24-Mar-01 19:13 shark_turbine/aot/support/procedural/iree_emitter.py
--rw-rw-r--  2.0 unx    11588 b- defN 24-Mar-01 19:13 shark_turbine/aot/support/procedural/primitives.py
--rw-rw-r--  2.0 unx     7157 b- defN 24-Mar-01 19:13 shark_turbine/aot/support/procedural/tracer.py
--rw-rw-r--  2.0 unx      287 b- defN 24-Mar-01 19:13 shark_turbine/dynamo/__init__.py
--rw-rw-r--  2.0 unx     8147 b- defN 24-Mar-01 19:13 shark_turbine/dynamo/executor.py
--rw-rw-r--  2.0 unx     2646 b- defN 24-Mar-01 19:13 shark_turbine/dynamo/passes.py
--rw-rw-r--  2.0 unx    21923 b- defN 24-Mar-01 19:13 shark_turbine/dynamo/tensor.py
--rw-rw-r--  2.0 unx     6986 b- defN 24-Mar-01 19:13 shark_turbine/dynamo/type_conversion.py
--rw-rw-r--  2.0 unx     3272 b- defN 24-Mar-01 19:13 shark_turbine/dynamo/utils.py
--rw-rw-r--  2.0 unx     2808 b- defN 24-Mar-01 19:13 shark_turbine/dynamo/backends/cpu.py
--rw-rw-r--  2.0 unx    67460 b- defN 24-Mar-01 19:13 shark_turbine/importers/fx_importer.py
--rw-rw-r--  2.0 unx      857 b- defN 24-Mar-01 19:13 shark_turbine/importers/ir.py
--rw-rw-r--  2.0 unx     2675 b- defN 24-Mar-01 19:13 shark_turbine/importers/utils.py
--rw-rw-r--  2.0 unx      518 b- defN 24-Mar-01 19:13 shark_turbine/kernel/__init__.py
--rw-rw-r--  2.0 unx     1484 b- defN 24-Mar-01 19:13 shark_turbine/kernel/_support/context.py
--rw-rw-r--  2.0 unx     1157 b- defN 24-Mar-01 19:13 shark_turbine/kernel/_support/dtype.py
--rw-rw-r--  2.0 unx    12390 b- defN 24-Mar-01 19:13 shark_turbine/kernel/_support/indexing.py
--rw-rw-r--  2.0 unx     5147 b- defN 24-Mar-01 19:13 shark_turbine/kernel/_support/regions.py
--rw-rw-r--  2.0 unx     3549 b- defN 24-Mar-01 19:13 shark_turbine/kernel/_support/shaped_type.py
--rw-rw-r--  2.0 unx    15676 b- defN 24-Mar-02 22:11 shark_turbine/kernel/_support/tracing.py
--rw-rw-r--  2.0 unx      103 b- defN 24-Mar-01 19:13 shark_turbine/kernel/compiler/base.py
--rw-rw-r--  2.0 unx    11457 b- defN 24-Mar-01 19:13 shark_turbine/kernel/compiler/builder.py
--rw-rw-r--  2.0 unx     8284 b- defN 24-Mar-01 19:13 shark_turbine/kernel/compiler/dispatch_codegen.py
--rw-rw-r--  2.0 unx     1796 b- defN 24-Mar-01 19:13 shark_turbine/kernel/compiler/host_codegen.py
--rw-rw-r--  2.0 unx      744 b- defN 24-Mar-01 19:13 shark_turbine/kernel/compiler/ir.py
--rw-rw-r--  2.0 unx     8658 b- defN 24-Mar-01 19:13 shark_turbine/kernel/compiler/kernel_codegen.py
--rw-rw-r--  2.0 unx     1770 b- defN 24-Mar-01 19:13 shark_turbine/kernel/compiler/op_matchers.py
--rw-rw-r--  2.0 unx    35543 b- defN 24-Mar-01 19:13 shark_turbine/kernel/compiler/vector_codegen.py
--rw-rw-r--  2.0 unx       94 b- defN 24-Mar-02 22:11 shark_turbine/kernel/gen/__init__.py
--rw-rw-r--  2.0 unx     5342 b- defN 24-Mar-02 22:11 shark_turbine/kernel/gen/kernel.py
--rw-rw-r--  2.0 unx     4886 b- defN 24-Mar-02 22:11 shark_turbine/kernel/gen/thread.py
--rw-rw-r--  2.0 unx      339 b- defN 24-Mar-01 19:13 shark_turbine/kernel/lang/__init__.py
--rw-rw-r--  2.0 unx     1454 b- defN 24-Mar-01 19:13 shark_turbine/kernel/lang/grid.py
--rw-rw-r--  2.0 unx     4476 b- defN 24-Mar-01 19:13 shark_turbine/kernel/lang/kernel_buffer.py
--rw-rw-r--  2.0 unx     1031 b- defN 24-Mar-01 19:13 shark_turbine/kernel/lang/prims.py
--rw-rw-r--  2.0 unx     1331 b- defN 24-Mar-01 19:13 shark_turbine/kernel/lang/types.py
--rw-rw-r--  2.0 unx      149 b- defN 24-Mar-01 19:13 shark_turbine/kernel/ops/__init__.py
--rw-rw-r--  2.0 unx     1237 b- defN 24-Mar-01 19:13 shark_turbine/kernel/ops/base.py
--rw-rw-r--  2.0 unx      638 b- defN 24-Mar-01 19:13 shark_turbine/kernel/ops/control_flow.py
--rw-rw-r--  2.0 unx      581 b- defN 24-Mar-01 19:13 shark_turbine/kernel/ops/core.py
--rw-rw-r--  2.0 unx      330 b- defN 24-Mar-01 19:13 shark_turbine/kernel/ops/math.py
--rw-rw-r--  2.0 unx      577 b- defN 24-Mar-01 19:13 shark_turbine/kernel/ops/memory.py
--rw-rw-r--  2.0 unx      487 b- defN 24-Mar-01 19:13 shark_turbine/kernel/ops/reduction.py
--rw-rw-r--  2.0 unx      555 b- defN 24-Mar-01 19:13 shark_turbine/kernel/ops/shape_manipulation.py
--rw-rw-r--  2.0 unx      248 b- defN 24-Mar-01 19:13 shark_turbine/ops/__init__.py
--rw-rw-r--  2.0 unx     2169 b- defN 24-Mar-01 19:13 shark_turbine/ops/iree.py
--rw-rw-r--  2.0 unx      272 b- defN 24-Mar-01 19:13 shark_turbine/runtime/__init__.py
--rw-rw-r--  2.0 unx    12431 b- defN 24-Mar-01 19:13 shark_turbine/runtime/device.py
--rw-rw-r--  2.0 unx      249 b- defN 24-Mar-01 19:13 shark_turbine/runtime/op_reg/__init__.py
--rw-rw-r--  2.0 unx    27042 b- defN 24-Mar-02 22:11 shark_turbine/runtime/op_reg/base.py
--rw-rw-r--  2.0 unx     4442 b- defN 24-Mar-01 19:13 shark_turbine/runtime/op_reg/compiler.py
--rw-rw-r--  2.0 unx     5673 b- defN 24-Mar-01 19:13 shark_turbine/runtime/op_reg/eager.py
--rw-rw-r--  2.0 unx      241 b- defN 24-Mar-01 19:13 shark_turbine/support/__init__.py
--rw-rw-r--  2.0 unx     4109 b- defN 24-Mar-01 19:13 shark_turbine/support/conversions.py
--rw-rw-r--  2.0 unx     1341 b- defN 24-Mar-01 19:13 shark_turbine/support/exceptions.py
--rw-rw-r--  2.0 unx     1128 b- defN 24-Mar-01 19:13 shark_turbine/support/ir_imports.py
--rw-rw-r--  2.0 unx      305 b- defN 24-Mar-01 19:13 shark_turbine/support/logging.py
--rw-rw-r--  2.0 unx     2365 b- defN 24-Mar-01 19:13 shark_turbine/transforms/builder.py
--rw-rw-r--  2.0 unx     7910 b- defN 24-Mar-01 19:13 shark_turbine/transforms/merger.py
--rw-rw-r--  2.0 unx    10697 b- defN 24-Mar-01 19:13 shark_turbine/transforms/rewriter.py
--rw-rw-r--  2.0 unx     8563 b- defN 24-Mar-01 19:13 shark_turbine/transforms/general/custom_op_expansion.py
--rw-rw-r--  2.0 unx     4989 b- defN 24-Mar-01 19:13 shark_turbine/transforms/general/rename_parameters.py
--rw-rw-r--  2.0 unx     7693 b- defN 24-Mar-01 19:13 shark_turbine/transforms/quantization/mm_group_quant.py
--rw-rw-r--  2.0 unx     6229 b- defN 24-Mar-02 22:13 shark_turbine-0.9.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-02 22:13 shark_turbine-0.9.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       80 b- defN 24-Mar-02 22:13 shark_turbine-0.9.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       14 b- defN 24-Mar-02 22:13 shark_turbine-0.9.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7612 b- defN 24-Mar-02 22:13 shark_turbine-0.9.6.dist-info/RECORD
-81 files, 485319 bytes uncompressed, 142185 bytes compressed:  70.7%
+Zip file size: 150382 bytes, number of entries: 85
+-rw-rw-r--  2.0 unx      700 b- defN 24-Apr-10 21:52 iree/turbine/__init__.py
+-rw-rw-r--  2.0 unx      430 b- defN 24-Apr-10 21:46 shark_turbine/aot/__init__.py
+-rw-rw-r--  2.0 unx    23347 b- defN 24-Apr-10 21:46 shark_turbine/aot/compiled_module.py
+-rw-rw-r--  2.0 unx     2815 b- defN 24-Mar-29 02:54 shark_turbine/aot/decompositions.py
+-rw-rw-r--  2.0 unx     9666 b- defN 24-Apr-10 21:46 shark_turbine/aot/exporter.py
+-rw-rw-r--  2.0 unx    12219 b- defN 24-Mar-29 02:54 shark_turbine/aot/fx_programs.py
+-rw-rw-r--  2.0 unx     4751 b- defN 24-Apr-10 21:46 shark_turbine/aot/params.py
+-rw-rw-r--  2.0 unx     1023 b- defN 24-Apr-10 21:46 shark_turbine/aot/tensor_traits.py
+-rw-rw-r--  2.0 unx      884 b- defN 24-Mar-21 23:46 shark_turbine/aot/builtins/__init__.py
+-rw-rw-r--  2.0 unx     5431 b- defN 24-Apr-10 21:46 shark_turbine/aot/builtins/globals.py
+-rw-rw-r--  2.0 unx    18037 b- defN 24-Mar-29 02:54 shark_turbine/aot/builtins/jittable.py
+-rw-rw-r--  2.0 unx      262 b- defN 24-Feb-05 20:48 shark_turbine/aot/passes/__init__.py
+-rw-rw-r--  2.0 unx     3537 b- defN 24-Mar-05 20:36 shark_turbine/aot/passes/functorch.py
+-rw-rw-r--  2.0 unx    15795 b- defN 24-Apr-10 21:46 shark_turbine/aot/support/ir_utils.py
+-rw-rw-r--  2.0 unx      646 b- defN 24-Feb-05 20:48 shark_turbine/aot/support/procedural/__init__.py
+-rw-rw-r--  2.0 unx     7507 b- defN 24-Mar-05 20:36 shark_turbine/aot/support/procedural/base.py
+-rw-rw-r--  2.0 unx    11775 b- defN 24-Apr-10 21:46 shark_turbine/aot/support/procedural/exported_program.py
+-rw-rw-r--  2.0 unx     9338 b- defN 24-Mar-05 20:36 shark_turbine/aot/support/procedural/globals.py
+-rw-rw-r--  2.0 unx    12373 b- defN 24-Mar-05 20:36 shark_turbine/aot/support/procedural/iree_emitter.py
+-rw-rw-r--  2.0 unx    11744 b- defN 24-Mar-05 20:36 shark_turbine/aot/support/procedural/primitives.py
+-rw-rw-r--  2.0 unx     7211 b- defN 24-Mar-05 20:36 shark_turbine/aot/support/procedural/tracer.py
+-rw-rw-r--  2.0 unx      287 b- defN 24-Feb-05 20:48 shark_turbine/dynamo/__init__.py
+-rw-rw-r--  2.0 unx     4096 b- defN 24-Mar-29 02:54 shark_turbine/dynamo/decompositions.py
+-rw-rw-r--  2.0 unx     8179 b- defN 24-Mar-05 20:36 shark_turbine/dynamo/executor.py
+-rw-rw-r--  2.0 unx      814 b- defN 24-Mar-29 02:54 shark_turbine/dynamo/passes.py
+-rw-rw-r--  2.0 unx    21970 b- defN 24-Mar-21 20:49 shark_turbine/dynamo/tensor.py
+-rw-rw-r--  2.0 unx     7017 b- defN 24-Mar-05 20:36 shark_turbine/dynamo/type_conversion.py
+-rw-rw-r--  2.0 unx     2816 b- defN 24-Mar-21 20:49 shark_turbine/dynamo/backends/cpu.py
+-rw-rw-r--  2.0 unx      857 b- defN 24-Feb-23 23:17 shark_turbine/importers/ir.py
+-rw-rw-r--  2.0 unx     1192 b- defN 24-Mar-05 20:36 shark_turbine/importers/utils.py
+-rw-rw-r--  2.0 unx      518 b- defN 24-Feb-05 20:48 shark_turbine/kernel/__init__.py
+-rw-rw-r--  2.0 unx     1484 b- defN 24-Feb-05 20:48 shark_turbine/kernel/_support/context.py
+-rw-rw-r--  2.0 unx     1157 b- defN 24-Feb-26 22:45 shark_turbine/kernel/_support/dtype.py
+-rw-rw-r--  2.0 unx    12390 b- defN 24-Feb-26 22:45 shark_turbine/kernel/_support/indexing.py
+-rw-rw-r--  2.0 unx     5147 b- defN 24-Feb-26 22:45 shark_turbine/kernel/_support/regions.py
+-rw-rw-r--  2.0 unx     3549 b- defN 24-Feb-26 22:45 shark_turbine/kernel/_support/shaped_type.py
+-rw-rw-r--  2.0 unx    15676 b- defN 24-Mar-02 22:06 shark_turbine/kernel/_support/tracing.py
+-rw-rw-r--  2.0 unx      103 b- defN 24-Feb-05 20:48 shark_turbine/kernel/compiler/base.py
+-rw-rw-r--  2.0 unx    11457 b- defN 24-Feb-26 22:45 shark_turbine/kernel/compiler/builder.py
+-rw-rw-r--  2.0 unx     8284 b- defN 24-Feb-26 22:45 shark_turbine/kernel/compiler/dispatch_codegen.py
+-rw-rw-r--  2.0 unx     1796 b- defN 24-Feb-22 02:07 shark_turbine/kernel/compiler/host_codegen.py
+-rw-rw-r--  2.0 unx      744 b- defN 24-Feb-22 02:07 shark_turbine/kernel/compiler/ir.py
+-rw-rw-r--  2.0 unx     8658 b- defN 24-Feb-26 22:45 shark_turbine/kernel/compiler/kernel_codegen.py
+-rw-rw-r--  2.0 unx     1770 b- defN 24-Feb-05 20:48 shark_turbine/kernel/compiler/op_matchers.py
+-rw-rw-r--  2.0 unx    35543 b- defN 24-Feb-26 22:45 shark_turbine/kernel/compiler/vector_codegen.py
+-rw-rw-r--  2.0 unx       94 b- defN 24-Mar-02 22:06 shark_turbine/kernel/gen/__init__.py
+-rw-rw-r--  2.0 unx     5342 b- defN 24-Mar-02 22:06 shark_turbine/kernel/gen/kernel.py
+-rw-rw-r--  2.0 unx     4886 b- defN 24-Mar-02 22:06 shark_turbine/kernel/gen/thread.py
+-rw-rw-r--  2.0 unx      339 b- defN 24-Feb-26 22:45 shark_turbine/kernel/lang/__init__.py
+-rw-rw-r--  2.0 unx     1454 b- defN 24-Feb-26 22:45 shark_turbine/kernel/lang/grid.py
+-rw-rw-r--  2.0 unx     4476 b- defN 24-Feb-26 22:45 shark_turbine/kernel/lang/kernel_buffer.py
+-rw-rw-r--  2.0 unx     1031 b- defN 24-Feb-26 22:45 shark_turbine/kernel/lang/prims.py
+-rw-rw-r--  2.0 unx     1331 b- defN 24-Feb-05 20:48 shark_turbine/kernel/lang/types.py
+-rw-rw-r--  2.0 unx      149 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/__init__.py
+-rw-rw-r--  2.0 unx     1237 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/base.py
+-rw-rw-r--  2.0 unx      638 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/control_flow.py
+-rw-rw-r--  2.0 unx      581 b- defN 24-Feb-26 22:45 shark_turbine/kernel/ops/core.py
+-rw-rw-r--  2.0 unx      330 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/math.py
+-rw-rw-r--  2.0 unx      577 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/memory.py
+-rw-rw-r--  2.0 unx      487 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/reduction.py
+-rw-rw-r--  2.0 unx      555 b- defN 24-Feb-05 20:48 shark_turbine/kernel/ops/shape_manipulation.py
+-rw-rw-r--  2.0 unx      248 b- defN 24-Feb-05 20:48 shark_turbine/ops/__init__.py
+-rw-rw-r--  2.0 unx     1832 b- defN 24-Mar-28 03:11 shark_turbine/ops/iree.py
+-rw-rw-r--  2.0 unx      272 b- defN 24-Feb-05 20:48 shark_turbine/runtime/__init__.py
+-rw-rw-r--  2.0 unx    12469 b- defN 24-Mar-05 20:36 shark_turbine/runtime/device.py
+-rw-rw-r--  2.0 unx      249 b- defN 24-Feb-05 20:48 shark_turbine/runtime/op_reg/__init__.py
+-rw-rw-r--  2.0 unx    28076 b- defN 24-Mar-29 00:40 shark_turbine/runtime/op_reg/base.py
+-rw-rw-r--  2.0 unx     4442 b- defN 24-Feb-05 20:48 shark_turbine/runtime/op_reg/compiler.py
+-rw-rw-r--  2.0 unx     6341 b- defN 24-Mar-05 20:36 shark_turbine/runtime/op_reg/eager.py
+-rw-rw-r--  2.0 unx      241 b- defN 24-Feb-05 20:48 shark_turbine/support/__init__.py
+-rw-rw-r--  2.0 unx     4118 b- defN 24-Mar-21 20:49 shark_turbine/support/conversions.py
+-rw-rw-r--  2.0 unx     1341 b- defN 24-Feb-05 20:48 shark_turbine/support/exceptions.py
+-rw-rw-r--  2.0 unx     1128 b- defN 24-Apr-10 21:46 shark_turbine/support/ir_imports.py
+-rw-rw-r--  2.0 unx      357 b- defN 24-Mar-05 20:36 shark_turbine/support/logging.py
+-rw-rw-r--  2.0 unx     2365 b- defN 24-Feb-05 20:48 shark_turbine/transforms/builder.py
+-rw-rw-r--  2.0 unx     8202 b- defN 24-Apr-10 21:43 shark_turbine/transforms/merger.py
+-rw-rw-r--  2.0 unx    10997 b- defN 24-Apr-10 21:43 shark_turbine/transforms/rewriter.py
+-rw-rw-r--  2.0 unx     9012 b- defN 24-Mar-28 03:11 shark_turbine/transforms/general/custom_op_expansion.py
+-rw-rw-r--  2.0 unx     4995 b- defN 24-Mar-05 20:36 shark_turbine/transforms/general/rename_parameters.py
+-rw-rw-r--  2.0 unx     7793 b- defN 24-Mar-05 20:36 shark_turbine/transforms/quantization/mm_group_quant.py
+-rw-rw-r--  2.0 unx     6263 b- defN 24-Apr-11 00:12 shark_turbine-2.3.0rc20240410.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-11 00:12 shark_turbine-2.3.0rc20240410.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       80 b- defN 24-Apr-11 00:12 shark_turbine-2.3.0rc20240410.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       19 b- defN 24-Apr-11 00:12 shark_turbine-2.3.0rc20240410.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8034 b- defN 24-Apr-11 00:12 shark_turbine-2.3.0rc20240410.dist-info/RECORD
+85 files, 457468 bytes uncompressed, 137380 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -1,16 +1,31 @@
+Filename: iree/turbine/__init__.py
+Comment: 
+
 Filename: shark_turbine/aot/__init__.py
 Comment: 
 
 Filename: shark_turbine/aot/compiled_module.py
 Comment: 
 
+Filename: shark_turbine/aot/decompositions.py
+Comment: 
+
 Filename: shark_turbine/aot/exporter.py
 Comment: 
 
+Filename: shark_turbine/aot/fx_programs.py
+Comment: 
+
+Filename: shark_turbine/aot/params.py
+Comment: 
+
+Filename: shark_turbine/aot/tensor_traits.py
+Comment: 
+
 Filename: shark_turbine/aot/builtins/__init__.py
 Comment: 
 
 Filename: shark_turbine/aot/builtins/globals.py
 Comment: 
 
 Filename: shark_turbine/aot/builtins/jittable.py
@@ -21,23 +36,23 @@
 
 Filename: shark_turbine/aot/passes/functorch.py
 Comment: 
 
 Filename: shark_turbine/aot/support/ir_utils.py
 Comment: 
 
-Filename: shark_turbine/aot/support/utils.py
-Comment: 
-
 Filename: shark_turbine/aot/support/procedural/__init__.py
 Comment: 
 
 Filename: shark_turbine/aot/support/procedural/base.py
 Comment: 
 
+Filename: shark_turbine/aot/support/procedural/exported_program.py
+Comment: 
+
 Filename: shark_turbine/aot/support/procedural/globals.py
 Comment: 
 
 Filename: shark_turbine/aot/support/procedural/iree_emitter.py
 Comment: 
 
 Filename: shark_turbine/aot/support/procedural/primitives.py
@@ -45,35 +60,32 @@
 
 Filename: shark_turbine/aot/support/procedural/tracer.py
 Comment: 
 
 Filename: shark_turbine/dynamo/__init__.py
 Comment: 
 
+Filename: shark_turbine/dynamo/decompositions.py
+Comment: 
+
 Filename: shark_turbine/dynamo/executor.py
 Comment: 
 
 Filename: shark_turbine/dynamo/passes.py
 Comment: 
 
 Filename: shark_turbine/dynamo/tensor.py
 Comment: 
 
 Filename: shark_turbine/dynamo/type_conversion.py
 Comment: 
 
-Filename: shark_turbine/dynamo/utils.py
-Comment: 
-
 Filename: shark_turbine/dynamo/backends/cpu.py
 Comment: 
 
-Filename: shark_turbine/importers/fx_importer.py
-Comment: 
-
 Filename: shark_turbine/importers/ir.py
 Comment: 
 
 Filename: shark_turbine/importers/utils.py
 Comment: 
 
 Filename: shark_turbine/kernel/__init__.py
@@ -222,23 +234,23 @@
 
 Filename: shark_turbine/transforms/general/rename_parameters.py
 Comment: 
 
 Filename: shark_turbine/transforms/quantization/mm_group_quant.py
 Comment: 
 
-Filename: shark_turbine-0.9.6.dist-info/METADATA
+Filename: shark_turbine-2.3.0rc20240410.dist-info/METADATA
 Comment: 
 
-Filename: shark_turbine-0.9.6.dist-info/WHEEL
+Filename: shark_turbine-2.3.0rc20240410.dist-info/WHEEL
 Comment: 
 
-Filename: shark_turbine-0.9.6.dist-info/entry_points.txt
+Filename: shark_turbine-2.3.0rc20240410.dist-info/entry_points.txt
 Comment: 
 
-Filename: shark_turbine-0.9.6.dist-info/top_level.txt
+Filename: shark_turbine-2.3.0rc20240410.dist-info/top_level.txt
 Comment: 
 
-Filename: shark_turbine-0.9.6.dist-info/RECORD
+Filename: shark_turbine-2.3.0rc20240410.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shark_turbine/aot/__init__.py

```diff
@@ -1,10 +1,13 @@
 # Copyright 2023 Nod Labs, Inc
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
-from .compiled_module import CompiledModule
-from .exporter import export
-
 from .builtins import *
+from .compiled_module import *
+from .decompositions import *
+from .exporter import *
+from .fx_programs import FxPrograms, FxProgramsBuilder
+from .tensor_traits import *
+from .params import *
```

## shark_turbine/aot/compiled_module.py

```diff
@@ -1,50 +1,52 @@
 # Copyright 2023 Nod Labs, Inc
 # Portions Copyright 2022 The IREE Authors
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
-from typing import Callable, Dict, Generator, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Union
 
 import enum
 import inspect
 import logging
 from pathlib import Path
 import re
 import weakref
 import sys
 
+from torch.export import ExportedProgram
+
 from . import builtins
 
 from ..support.ir_imports import (
     Context,
     Location,
     MLIRError,
     Module,
     Operation,
     PassManager,
     StringAttr,
 )
+from ..support.logging import aot_logger as logger
 from ..transforms.general.custom_op_expansion import ExpandCustomOpsPass
 
 from .support.procedural import (
     GlobalsDef,
     ProcedureTrace,
     current_ir_trace,
 )
 
+from .support.procedural.exported_program import import_exported_program
+
 from .support.ir_utils import (
     ModuleBuilder,
 )
 
-from .support.utils import (
-    logger,
-)
 
 __all__ = [
     "CompiledModule",
 ]
 
 ################################################################################
 # Data structures
@@ -128,15 +130,36 @@
     def copy(self) -> "ExportProcDef":
         return ExportProcDef(self.export_name, self.callable, signature=self.signature)
 
     def __repr__(self):
         return f"<def {self.export_name}({self.signature})>"
 
 
-Exportable = Union[ExportProcDef, PyOnlyDef, GlobalsDef]
+class ExportedProgramDef:
+    def __init__(
+        self,
+        ep: ExportedProgram,
+        *,
+        export_name: Optional[str] = None,
+        public: bool = False,
+    ):
+        self.export_name = export_name
+        self.exported_program = ep
+        self.public = public
+
+    def copy(self) -> "ExportedProgramDef":
+        return ExportedProgramDef(
+            self.exported_program, export_name=self.export_name, public=self.public
+        )
+
+    def __repr__(self):
+        return f"<exported_program {self.exported_program}>"
+
+
+Exportable = Union[ExportProcDef, ExportedProgramDef, PyOnlyDef, GlobalsDef]
 
 
 class CompiledModuleClassInfo:
     __slots__ = [
         "all_exports",
         "ir_module_name",
     ]
@@ -151,52 +174,73 @@
         self.all_exports[key] = value
 
     @property
     def export_procs(self) -> Generator[Tuple[str, ExportProcDef], None, None]:
         return filter(
             lambda kv_tuple: isinstance(kv_tuple[1], ExportProcDef),
             self.all_exports.items(),
-        )
+        )  # type: ignore
+
+    @property
+    def exported_programs(
+        self,
+    ) -> Generator[Tuple[str, ExportedProgramDef], None, None]:
+        return filter(
+            lambda kv_tuple: isinstance(kv_tuple[1], ExportedProgramDef),
+            self.all_exports.items(),
+        )  # type: ignore
 
     @property
     def py_only_defs(self) -> Generator[Tuple[str, PyOnlyDef], None, None]:
         return filter(
             lambda kv_tuple: isinstance(kv_tuple[1], PyOnlyDef),
             self.all_exports.items(),
-        )
+        )  # type: ignore
 
     @property
     def globals_defs(self) -> Generator[Tuple[str, GlobalsDef], None, None]:
         return filter(
             lambda kv_tuple: isinstance(kv_tuple[1], GlobalsDef),
             self.all_exports.items(),
-        )
+        )  # type: ignore
 
     def def_attribute(self, key, value):
         # Some decorators, the only thing we do is convert them to PyOnlyDef.
         # Do that first so the generic descriptor code below handles them.
         if isinstance(value, builtins.jittable):
             value = PyOnlyDef(value)
 
+        # Promote a torch ExportedProgram to an ExportedProgramDef.
+        if isinstance(value, ExportedProgram):
+            value = ExportedProgramDef(
+                value, export_name=key, public=not key.startswith("_")
+            )
+
         # Detect our own descriptors.
         if isinstance(value, GlobalsDef):
             logging.debug("DEFINE GLOBALS: %s = %r", key, value)
             self.add_export(key, value)
             return value
         if isinstance(value, ExportProcDef):
             value = value.copy()
             if value.export_name is None:
                 value.export_name = key
             self.add_export(key, value)
             return value
-
         if isinstance(value, PyOnlyDef):
             logging.debug("DEFINE PY_ONLY: %s = %r", key, value)
             self.add_export(key, value)
             return value
+        if isinstance(value, ExportedProgramDef):
+            if value.export_name is None:
+                value = value.copy()
+                value.export_name = key
+            logging.debug("DEFINE EXPORTED_PROGRAM: %r", value.export_name)
+            self.add_export(key, value)
+            return value
 
         # Infer if it is an exported function.
         if callable(value) and inspect.isfunction(value):
             return self.def_export_proc(key, value)
 
         raise TypeError(
             f"cannot set arbitrary Python value '{key}' on "
@@ -205,19 +249,19 @@
 
     def def_export_proc(self, name, f) -> ExportProcDef:
         logging.debug("DEFINE EXPORT: %s = %r", name, f)
         # Get a reasonable location.
         file_line_loc = None
         try:
             sourcefile = inspect.getsourcefile(f)
-            _, linenums = sourcelines = inspect.getsourcelines(f)
-            if sourcefile and linenums:
-                file_line_loc = [sourcefile, linenums[0]]
-        except TypeError:
-            pass
+            _, linenum = sourcelines = inspect.getsourcelines(f)
+        except OSError:
+            ...
+        else:
+            file_line_loc = (sourcefile or "<unnamed>", linenum)
 
         sig = inspect.signature(f)
         if len(sig.parameters) < 1:
             raise TypeError(
                 f"export proc '{name}' is expected to have a 'self' parameter"
             )
 
@@ -263,50 +307,50 @@
     def __init__(
         self, class_info: CompiledModuleClassInfo, module_builder: ModuleBuilder
     ):
         self.class_info = class_info
         self.module_builder = module_builder
         # The shadow dict holds instance attributes. We stash them here and the
         # Program instance itself arbitrates access via getattr/setattr.
-        self.shadow_dict = dict()
+        self.shadow_dict: dict[str, Any] = dict()
         self.current_import_phase = ImportPhase.TORCH_IR
 
 
 ################################################################################
 # Live reference accounting
 ################################################################################
 
-_all_compiled_module_class_infos: Dict[
+_all_compiled_module_class_infos: weakref.WeakKeyDictionary[
     "CompiledModuleMeta", CompiledModuleClassInfo
 ] = weakref.WeakKeyDictionary()
-
-_all_compiled_module_instance_infos: Dict[
+_all_compiled_module_instance_infos: weakref.WeakKeyDictionary[
     "CompiledModule", CompiledModuleInstanceInfo
 ] = weakref.WeakKeyDictionary()
 
 
 ################################################################################
 # CompiledModule and metaclass
 ################################################################################
 
 # Gate that is set to True once metaclass setup is complete.
 _metaclass_setup_complete = False
 
 
-@property
+@property  # type: ignore
 def _blackhole_instance_attribute(self):
     # We're not here.
     raise AttributeError
 
 
 def _uncallable_public_export(*args, **kwargs):
     raise RuntimeError(f"Calls to exported functions not yet supported")
 
 
 _COMPILED_MODULE_API_ATTRIBUTES = [
+    "create_from_dict",
     "expand_custom_ops",
     "export_global",
     "get_class_info",
     "get_info",
     "get_module_builder",
     "get_mlir_module",
     "jittable",
@@ -381,14 +425,33 @@
         except KeyError:
             raise AttributeError
 
 
 class CompiledModule(metaclass=CompiledModuleMeta):
     """Base class for all staged modules."""
 
+    @classmethod
+    def create_from_dict(
+        cls: CompiledModuleMeta,
+        name: str,
+        dct: dict,
+        *,
+        export_name: Optional[str] = None,
+    ) -> CompiledModuleMeta:
+        """Creates a CompiledModule subclass with an explicit dictionary of members.
+
+        This is the unsugared form of:
+
+        ```
+        class Foo(CompiledModule, export_name="bar"):
+          def member(): ...
+        ```
+        """
+        return CompiledModuleMeta(name, (cls,), dct, export_name=export_name)
+
     @staticmethod
     def get_class_info(cls: CompiledModuleMeta) -> CompiledModuleClassInfo:
         return _all_compiled_module_class_infos[cls]
 
     @staticmethod
     def get_info(inst: "CompiledModule") -> CompiledModuleInstanceInfo:
         return _all_compiled_module_instance_infos[inst]
@@ -541,14 +604,25 @@
         for key, globals_def in info.class_info.globals_defs:
             info.shadow_dict[key] = globals_def.track(module_builder, key)
 
         # Make PyOnly defs visible.
         for key, py_def in info.class_info.py_only_defs:
             info.shadow_dict[key] = py_def.py_value
 
+        # Instantiate exported programs.
+        # TODO: This should be done in two phases along with export_procs
+        # in order to enable dependence.
+        for key, ep_def in info.class_info.exported_programs:
+            info.shadow_dict[key] = import_exported_program(
+                module_builder,
+                ep_def.exported_program,
+                symbol_name=ep_def.export_name or "main",
+                symbol_visibility=None if ep_def.public else "private",
+            )
+
         # Instantiate procs.
         # TODO: This should be done in two phases, first binding the symbols
         # and then defining them, enabling dependence.
         # See: https://github.com/nod-ai/SHARK-Turbine/issues/129
         for key, proc_def in info.class_info.export_procs:
 
             def do_export(proc_def: ExportProcDef):
```

## shark_turbine/aot/exporter.py

```diff
@@ -1,18 +1,18 @@
 # Copyright 2023 Nod Labs, Inc
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
-from typing import Optional, Sequence, Union
-import functools
+from typing import overload, Any, Dict, List, Optional, Sequence, Tuple, Type, Union
 import io
 from pathlib import Path
 import platform
+import warnings
 
 import torch
 
 from iree.compiler.api import (
     Session,
     Source,
     Output,
@@ -22,27 +22,33 @@
     Context,
     Operation,
 )
 
 from .builtins import *
 from .compiled_module import (
     CompiledModule,
-    CompiledModuleMeta,
-    ExportProcDef,
     ImportPhase,
 )
-from .support.procedural import (
-    AbstractTypedef,
-)
+from .fx_programs import FxPrograms
+from . import decompositions
 
+__all__ = [
+    "export",
+    "ExportOutput",
+]
 
 _is_windows = platform.system() == "Windows"
 
 
-ModuleLike = Union[torch.nn.Module, CompiledModuleMeta]
+ModuleLike = Union[
+    torch.nn.Module,
+    Type[CompiledModule],
+    torch.export.ExportedProgram,
+    FxPrograms,
+]
 SaveableTarget = Union[str, Path, None, Output]
 
 
 class ExportOutput:
     """Wrapper around a CompiledModule produced by `export`."""
 
     def __init__(
@@ -112,16 +118,16 @@
         if save_to is None:
             output = Output.open_membuffer()
             return_memory_view = True
         elif isinstance(save_to, (str, Path)):
             save_to = Path(save_to)
             output = Output.open_file(str(save_to))
         else:
-            assert isinstance(output, Output)
             output = save_to
+            assert isinstance(output, Output)
 
         target_backends = (
             target_backends
             if isinstance(target_backends, str)
             else ",".join(target_backends)
         )
         inv = self.session.invocation()
@@ -146,60 +152,149 @@
         output.keep()
         if return_memory_view:
             return output
         else:
             return None
 
 
-# Decorator which explicitly exports a function.
-# TODO: Make this a public API on CompiledModule.
-# See https://github.com/nod-ai/SHARK-Turbine/issues/126
-def export_proc(f=None, *, signature: Sequence[AbstractTypedef]) -> ExportProcDef:
-    if f is None:
-        return functools.partial(export_proc, signature=signature)
-    return ExportProcDef(f.__name__, f, signature=signature)
-
-
-def export(mdl: ModuleLike, *example_args: torch.Tensor) -> ExportOutput:
-    """One shot export of an nn.Module.
-
-    This is a very restrictive API vs the lower level `CompiledModule`
-    facility. It is suitable for one-shot modules, with a single
-    entrypoint and static example arguments where no additional
-    configuration is needed for mutable parameters/buffers or state
-    management. Dynamic shape constraints are also not presently
-    exposed via this API, but we expect to allow this in the future.
+@overload
+def export(
+    module: torch.nn.Module,
+    /,
+    *,
+    args: Optional[tuple] = None,
+    kwargs: Optional[Dict[str, Any]] = None,
+    dynamic_shapes: Dict[str, Any] | Tuple[Any] | List[Any] | None = None,
+    module_name: Optional[str] = None,
+    function_name: Optional[str] = None,
+) -> ExportOutput:
+    """Exports a torch.nn.Module.
+
+    This is done by first invoking torch.export.export with args, kwargs,
+    and dynamic_shapes.
+    """
+    ...
+
+
+@overload
+def export(compiled_module: Type[CompiledModule], /) -> ExportOutput:
+    """Exports a CompiledModule and returns the output."""
+    ...
+
+
+@overload
+def export(
+    exported_program: torch.export.ExportedProgram,
+    /,
+    *,
+    module_name: Optional[str] = None,
+    function_name: Optional[str] = None,
+) -> ExportOutput:
+    """Exports a single entry-point module consisting of an ExportedProgram."""
+    ...
+
+
+@overload
+def export(
+    exported_programs: FxPrograms,
+    /,
+    *,
+    module_name: Optional[str] = None,
+) -> ExportOutput:
+    """Exports a multi entry-point ExportedProgram."""
+    ...
+
+
+def export(
+    mdl: ModuleLike,
+    /,
+    *example_args: torch.Tensor,
+    args: Optional[tuple] = None,
+    kwargs: Optional[Dict[str, Any]] = None,
+    dynamic_shapes: Dict[str, Any] | Tuple[Any] | List[Any] | None = None,
+    module_name: Optional[str] = None,
+    function_name: Optional[str] = None,
+) -> ExportOutput:
+    """Generic export of supported entities.
+
+    See a more specific overload for accepted forms.
+
+    This function behaves differently based on the type of the `mdl` argument:
+
+    * nn.Module: The module is traced with torch.export.export passing it
+      `args`, `kwargs`, and `dynamic_shapes`.
+    * CompiledModule: The module is imported to IR. Additional arguments are
+      illegal in this case.
+    * torch.export.ExportedProgram: A pre-exported program can be passed and
+      it will be used to construct a single-entrypoint module.
 
     Args:
       mdl: The nn.Module to export.
       *example_args: Example tensors.
+      args: Example arguments to torch.export (if present, then *example_args
+        must be empty.
+      kwargs: Example keyword arguments.
+      dynamic_shapes: Dynamic shape specs to pass to torch.export.
 
     Returns:
       An ExportOutput object that wraps the compilation and provides
       easy access.
     """
-    if isinstance(mdl, torch.nn.Module):
-        signature = [abstractify(t) for t in example_args]
+    if len(example_args) > 0:
+        warnings.warn(
+            DeprecationWarning(
+                "extra `example_args` positional parameters are deprecated: pass `args=tuple(...)` instead."
+            )
+        )
+
+    TransformedModule: Any
+    current_decomps = decompositions.current_aot_decompositions()
+    if isinstance(mdl, torch.export.ExportedProgram):
+        TransformedModule = CompiledModule.create_from_dict(
+            "LambdaCompiledModule",
+            {(function_name or "main"): mdl},
+            export_name=module_name or "module",
+        )
 
-        class Exported(CompiledModule, export_name=mdl._get_name()):
-            params = export_parameters(mdl)
+    elif isinstance(mdl, FxPrograms):
+        TransformedModule = CompiledModule.create_from_dict(
+            "LambdaCompiledModule", mdl.programs, export_name=module_name or "module"
+        )
+    elif isinstance(mdl, torch.nn.Module):
+        # Normalize arguments for torch.export.
+        if args is None:
+            args = example_args
+        elif len(example_args) > 0:
+            raise ValueError(
+                "Cannot pass args= and positional example_args at the same time"
+            )
+        nn_module = mdl
+        exported_program = torch.export.export(
+            nn_module, args=args, kwargs=kwargs, dynamic_shapes=dynamic_shapes
+        )
+        if current_decomps:
+            from .decompositions import _patch_op_dispatch_for_export
 
-            @export_proc(signature=signature)
-            def main(self, *args):
-                return jittable(mdl.forward)(*args)
+            _patch_op_dispatch_for_export()
+            exported_program = exported_program.run_decompositions(current_decomps)
 
+        TransformedModule = CompiledModule.create_from_dict(
+            "LambdaCompiledModule",
+            {(function_name or "main"): exported_program},
+            export_name=module_name or "module",
+        )
     else:
-        assert isinstance(mdl, CompiledModuleMeta)
-        Exported = mdl
+        assert issubclass(type(mdl), CompiledModule)
+        TransformedModule = mdl
 
     session = Session()
     # There are some bugs with respect to Session/context interop that we
     # haven't squashed yet. For now, default everyone to round-tripping
     # via bytecode vs sharing the context between the importer/compiler.
     importer_uses_session = False and not _is_windows
     if importer_uses_session:
         context = session.context
     else:
         context = Context()
 
-    cm = Exported(context=context, import_to="import")
+    cm = TransformedModule(context=context, import_to="import")
     return ExportOutput(session, cm, importer_uses_session=importer_uses_session)
```

## shark_turbine/aot/builtins/globals.py

```diff
@@ -18,15 +18,15 @@
 )
 
 from ..support.ir_utils import (
     NameMapCallback,
     GlobalAttributes,
 )
 
-from ..support.utils import (
+from torch.utils._pytree import (
     TreeSpec,
     tree_flatten,
     tree_map,
 )
 
 
 class export_global(GlobalsDef, Abstractifiable):
@@ -44,15 +44,15 @@
         external_scope: Optional[str] = None,
         name_mapper: Optional[NameMapCallback] = None,
         uninitialized: Optional[bool] = None,
         attrs: Optional[GlobalAttributes] = None,
     ):
         if attrs is None:
             attrs = GlobalAttributes(
-                mutable=mutable,
+                mutable=bool(mutable),
                 external=external,
                 external_scope=external_scope,
                 name_mapper=name_mapper,
                 uninitialized=uninitialized,
             )
         super().__init__(attrs)
         self._name = name
@@ -81,15 +81,15 @@
         external_scope: Optional[str] = None,
         name_mapper: Optional[NameMapCallback] = None,
         uninitialized: Optional[bool] = None,
         attrs: Optional[GlobalAttributes] = None,
     ):
         if attrs is None:
             attrs = GlobalAttributes(
-                mutable=mutable,
+                mutable=bool(mutable),
                 external=external,
                 external_scope=external_scope,
                 name_mapper=name_mapper,
                 uninitialized=uninitialized,
             )
         super().__init__(attrs)
         self._tree = tree
@@ -131,15 +131,15 @@
         external_scope: Optional[str] = None,
         name_mapper: Optional[NameMapCallback] = None,
         uninitialized: Optional[bool] = None,
         attrs: Optional[GlobalAttributes] = None,
     ):
         if attrs is None:
             attrs = GlobalAttributes(
-                mutable=mutable,
+                mutable=bool(mutable),
                 external=external,
                 external_scope=external_scope,
                 name_mapper=name_mapper,
                 uninitialized=uninitialized,
             )
         super().__init__(attrs)
         self._param_list = list(nn_module.named_parameters())
```

## shark_turbine/aot/builtins/jittable.py

```diff
@@ -5,66 +5,52 @@
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 """Tracing builtins."""
 
 from typing import Any, Callable, Dict, List, Optional, Sequence, Set, Tuple, Union
 
+import warnings
+
 import torch
 from torch._decomp import get_decompositions
 import torch._dynamo as dynamo
-from torch.export import (
-    Constraint,
-    dynamic_dim,
-)
 from torch.fx import (
-    Graph,
     GraphModule,
 )
-from torch.fx.passes.shape_prop import TensorMetadata
-
-# TODO: Switch to upstream fx_importer vs local fork when ready.
-# from iree.compiler.extras.fx_importer import (
-#     GraphNodeImporter,
-#     FxImporter,
-#     FxImporterHooks,
-# )
+from torch.utils._pytree import (
+    tree_flatten,
+    tree_unflatten,
+)
 
-from ...importers.fx_importer import (
+from iree.compiler.extras.fx_importer import (
     GraphNodeImporter,
     FxImporter,
     FxImporterHooks,
 )
 
-from ...dynamo.passes import (
-    DEFAULT_DECOMPOSITIONS,
-)
-
 from ...support.ir_imports import (
     FlatSymbolRefAttr,
     FunctionType,
     Operation,
     StringAttr,
     SymbolTable,
     TypeAttr,
     Value,
     func_d,
     util_d,
 )
 
+from ...support.logging import aot_logger as logger
+
+from ..decompositions import current_aot_decompositions
 from ..passes import (
     functorch_functionalize,
 )
 
-from ..support.utils import (
-    logger,
-    tree_flatten,
-    tree_unflatten,
-)
-
 from ..support.ir_utils import (
     ModuleBuilder,
 )
 
 from ..support.procedural import (
     CallableIntrinsic,
     IrImmediateTensor,
@@ -149,27 +135,22 @@
         "_passes",
     ]
 
     def __init__(
         self,
         wrapped_f,
         *,
-        decompose_ops: Optional[List[torch._ops.OpOverload]] = None,
-        decomposition_table: Optional[
-            Dict[torch._ops.OpOverload, Callable[..., Any]]
-        ] = None,
-        constraints: Optional[List[Constraint]] = None,
+        decompose_ops: Optional[List[Any]] = None,
+        decomposition_table: Optional[Dict[Any, Callable[..., Any]]] = None,
+        constraints: Optional[List[Any]] = None,
         function_name: Optional[str] = None,
         passes: Sequence[str] = DEFAULT_PASSES,
     ):
         if decomposition_table is None:
-            decomposition_table = {}
-        if decompose_ops is None:
-            decompose_ops = DEFAULT_DECOMPOSITIONS
-
+            decomposition_table = current_aot_decompositions()
         if decompose_ops:
             decomposition_table.update(get_decompositions(decompose_ops))
 
         self.constraints = constraints
         self.decomposition_table = decomposition_table
         self.wrapped_f = wrapped_f
         self.function_name = function_name if function_name else wrapped_f.__name__
@@ -181,26 +162,37 @@
     def __repr__(self):
         return f"<Jittable PyTorch func: {self.wrapped_f}>"
 
     def resolve_call(
         self,
         proc_trace: IrTrace,
         *py_args,
-        constraints: Optional[List[Constraint]] = None,
+        constraints: Optional[List[Any]] = None,
         **py_kwargs,
     ):
         type_converter = proc_trace.module_builder.native_type_converter
         # Accumulate all constraints into a new list.
         if constraints is None:
             constraints = []
         else:
             constraints = list(constraints)
         if self.constraints is not None:
             constraints.extend(self.constraints)
 
+        export_kwargs = {}
+        if len(constraints) > 0:
+            warnings.warn(
+                "Compiling program with the old PyTorch constraints system "
+                "for dynamic shapes is deprecated and will break on PyTorch "
+                "nightlies after the 2.3 release cut (expect either a PyTorch "
+                "warning or exception to follow)",
+                DeprecationWarning,
+            )
+            export_kwargs["constraints"] = constraints
+
         # Convert procedural trace values to things that Dynamo can handle.
         flat_py_args, args_tree = tree_flatten((py_args, py_kwargs))
         flat_pytorch_args = []
         flat_ir_args = []
         for py_arg in flat_py_args:
             ir_arg, pytorch_arg = self._split_py_arg(py_arg, constraints=constraints)
             flat_ir_args.append(ir_arg)
@@ -224,17 +216,17 @@
 
         # Ask dynamo to give us an aten graph.
         # TODO: Cache this for repeated calls.
         logger.debug("Performing dynamo.export(constraints=%r)", constraints)
         exported_f = dynamo.export(
             transformed_f,
             aten_graph=True,
-            decomposition_table=self.decomposition_table,
-            constraints=constraints,
+            decomposition_table=self.decomposition_table,  # type: ignore
             assume_static_by_default=True,
+            **export_kwargs,  # type: ignore
         )
         logger.debug("Invoking dynamo trace")
         gm, guards = exported_f(*flat_pytorch_args)
         logger.debug("Dyanmo trace complete")
 
         # TODO: Add debug logging for the exported graph module.
         # gm.print_readable()
@@ -307,27 +299,28 @@
             flat_ir_results = func_d.CallOp(
                 target_ftype.results, target_symbol_ref, flat_ir_args
             ).results
 
         assert len(flat_ir_results) == len(result_tensor_infos)
         flat_py_results = []
         for ir_result, result_tensor_info in zip(flat_ir_results, result_tensor_infos):
+            assert result_tensor_info is not None
             (dtype,) = result_tensor_info
             native_ir_result = type_converter.materialize_torch_to_native(ir_result)
             if dtype is not None:
                 flat_py_results.append(IrImmediateTensor(native_ir_result, dtype))
             else:
                 raise TypeError(
                     f"Unknown PyTorch->IREE value mapping for jittable result: {result_tensor_info}->{native_ir_result}"
                 )
 
         tree_py_results = tree_unflatten(flat_py_results, out_spec)
         return tree_py_results
 
-    def _split_py_arg(self, arg, constraints: List[Constraint]) -> Tuple[Value, Any]:
+    def _split_py_arg(self, arg, constraints: List[Any]) -> Tuple[Value, Any]:
         if isinstance(arg, IrTensor):
             meta_tensor, meta_constraints = arg._to_meta_tensor()
             constraints.extend(meta_constraints)
             return arg.ir_value, meta_tensor
 
         raise TypeError(f"Unsupported argument to jittable: {arg}")
 
@@ -474,9 +467,9 @@
             tensor_meta = flat_output_node.meta.get("tensor_meta")
             fake_val = flat_output_node.meta.get("val")
             dtype = None
             if tensor_meta is not None:
                 dtype = tensor_meta.dtype
             elif fake_val is not None:
                 dtype = fake_val.dtype
-            output_metadata.append((dtype,))
+            output_metadata.append((dtype,) if dtype is not None else None)
     return out_spec, output_metadata
```

## shark_turbine/aot/passes/functorch.py

```diff
@@ -1,14 +1,14 @@
 # Copyright 2023 Nod Labs, Inc
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
-from typing import Callable
+from typing import Any, Callable
 
 import torch
 from torch.fx import (
     GraphModule,
 )
 from torch.fx.experimental import proxy_tensor
 from torch.utils import _pytree as pytree
@@ -36,16 +36,16 @@
 # debugging the issues that can arise from all of this layering, we
 # should just do that.
 #
 # For the reasons above, we only use this as a *pre-export* transformation,
 # since that does not result in load bearing information loss. Note that
 # ONNX applies this post export, which suffers from the loss of output
 # destructuring rewrites that torch.export does.
-def functorch_functionalize(gm: GraphModule, *args) -> GraphModule:
-    functionalized_callable = _functionalize_callabale(gm)
+def functorch_functionalize(gm_callable: Any, *args) -> GraphModule:
+    functionalized_callable = _functionalize_callabale(gm_callable)
     # TODO: There is more of a dance needed if the user has entered with a fake_mode.
     with proxy_tensor.maybe_disable_fake_tensor_mode():
         new_gm = proxy_tensor.make_fx(
             functionalized_callable,
             decomposition_table={},
             tracing_mode="symbolic",
             _allow_non_fake_inputs=True,
```

## shark_turbine/aot/support/ir_utils.py

```diff
@@ -1,28 +1,27 @@
 # Copyright 2023 Nod Labs, Inc
 # Portions Copyright 2022 The IREE Authors
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
-from typing import Any, Callable, Generator, List, Optional, Sequence, Tuple
+from typing import Callable, Dict, Optional, Sequence, Tuple
 
 from pathlib import Path
 import tempfile
 
 import numpy as np
 import torch
 
-from ...importers.fx_importer import (
+from iree.compiler.extras.fx_importer import (
     ContextCache,
-)
-
-from ...importers.utils import (
-    RefTracker as FxRefTracker,
+    Empty,
+    EmptyType,
+    RefTracker,
 )
 
 from ...dynamo.type_conversion import (
     NativeTypeConverter,
 )
 
 from ...support.ir_imports import (
@@ -54,17 +53,18 @@
     tensor_d,
 )
 
 from ...support.conversions import (
     TORCH_DTYPE_TO_IREE_TYPE,
 )
 
-from .utils import (
-    RefTracker,
-    logger,
+from ...support.logging import aot_logger as logger
+
+from ..tensor_traits import (
+    ExternalTensorTrait,
 )
 
 ###############################################################################
 # Configuration
 ###############################################################################
 
 # Maps a name to an altered name. If returns None, then the original
@@ -86,15 +86,15 @@
 
     def __init__(
         self,
         mutable: bool = False,
         external: Optional[bool] = None,
         external_scope: Optional[str] = None,
         name_mapper: Optional[NameMapCallback] = None,
-        noinline: bool = True,
+        noinline: bool = False,
         uninitialized: Optional[bool] = None,
     ):
         if external and uninitialized:
             raise ValueError(
                 f"Globals with external=True cannot also have uninitialized=True"
             )
         if uninitialized and not mutable:
@@ -111,14 +111,40 @@
     def map_name(self, name: str) -> str:
         if self.name_mapper:
             new_name = self.name_mapper(name)
             if new_name is not None:
                 return new_name
         return name
 
+    def infer_external_from_tensor(
+        self, t: torch.Tensor
+    ) -> Tuple[bool, Optional[str], Optional[str]]:
+        """If externality is not specified, infers it from the tensor."""
+        # We check for the first item in a list because this lets us in the
+        # future extend the list by unwrapping.
+        check_tensors = [t]
+        for check_t in check_tensors:
+            trait = ExternalTensorTrait.get(check_t)
+            if trait is None:
+                continue
+            try:
+                external_scope = trait.external_scope
+                external_name = trait.external_name
+            except AttributeError as e:
+                raise AttributeError(
+                    f"Tensor defines _is_turbine_external_tensor but not other fields: {type(t)} = {t}"
+                )
+            return (
+                True,
+                external_scope if self.external_scope is None else self.external_scope,
+                external_name,
+            )
+
+        return bool(self.external), self.external_scope, None
+
 
 ###############################################################################
 # Builders
 ###############################################################################
 
 
 class ModuleBuilder:
@@ -131,14 +157,15 @@
         "fx_py_attr_tracker",
         "global_ip",
         "ip",
         "module_op",
         "symbol_table",
         "global_ref_tracker",
         "native_type_converter",
+        "_auto_symbol_counts",
     ]
 
     def __init__(self, module_op: Operation):
         self.module_op = module_op
         self.context = module_op.context
         self.body = module_op.regions[0].blocks[0]
         self.symbol_table = SymbolTable(module_op)
@@ -146,16 +173,25 @@
         self.ip = InsertionPoint(self.body)
         self.cache = ContextCache(self.context)
         # Tracks global references to a MaterializedGlobal.
         self.global_ref_tracker = RefTracker()
         # Usually the FxImporter makes a new ref tracker for each invocation,
         # but we want to preserve it across individual JIT evaluations so
         # as to better intern tensors to attributes.
-        self.fx_py_attr_tracker = FxRefTracker()
+        self.fx_py_attr_tracker = RefTracker()
         self.native_type_converter = NativeTypeConverter(self.context)
+        self._auto_symbol_counts: Dict[str, int] = {}
+
+    def unique_auto_symbol(self, requested_name: str) -> str:
+        if requested_name not in self._auto_symbol_counts:
+            self._auto_symbol_counts[requested_name] = 0
+            return requested_name
+        count = self._auto_symbol_counts[requested_name] + 1
+        self._auto_symbol_counts[requested_name] = count
+        return f"{requested_name}${count}"
 
     def handle_mlir_error(self, op: Operation, e: MLIRError, message: str):
         # TODO: Replace with a real dumping facility.
         # See: https://github.com/nod-ai/SHARK-Turbine/issues/136
         dump_path = Path(tempfile.gettempdir()) / "turbine_module_builder_error.mlir"
         logger.exception(f"{message} (dumping to {dump_path})")
         try:
@@ -207,30 +243,36 @@
         symbol_name: str,
         t: torch.Tensor,
         *,
         attrs: GlobalAttributes,
         logical_name: Optional[str] = None,
     ) -> Tuple[str, Operation, IrType]:
         element_type = self.torch_dtype_to_iree_type(t.dtype)
+        external, external_scope, external_name = attrs.infer_external_from_tensor(t)
+
         with self.global_ip, Location.unknown():
             tensor_type = RankedTensorType.get(list(t.shape), element_type)
             ir_attrs = {
                 "sym_name": StringAttr.get(symbol_name),
                 "sym_visibility": StringAttr.get("private"),
                 "type": TypeAttr.get(tensor_type),
             }
             if attrs.noinline:
                 ir_attrs["noinline"] = UnitAttr.get()
             if attrs.mutable:
                 ir_attrs["is_mutable"] = UnitAttr.get()
-            if attrs.external:
+            if external:
                 # Emit named external reference.
-                external_scope_attr = StringAttr.get(attrs.external_scope or "model")
-                external_name = attrs.map_name(
-                    logical_name if logical_name is not None else symbol_name
+                external_scope_attr = StringAttr.get(external_scope or "model")
+                external_name = (
+                    external_name
+                    if external_name is not None
+                    else attrs.map_name(
+                        logical_name if logical_name is not None else symbol_name
+                    )
                 )
                 external_name_attr = StringAttr.get(external_name)
                 # TODO: Have real Python builders for this.
                 ir_attrs["initial_value"] = Attribute.parse(
                     f"#stream.parameter.named<{external_scope_attr}::{external_name_attr}> : {tensor_type}"
                 )
             elif attrs.uninitialized:
@@ -242,16 +284,15 @@
                 )
             else:
                 # Emit inline initialized.
                 detached_tensor = t.detach().contiguous().cpu()
                 array = np.array(detached_tensor)
                 # We know that a Numpy array is a ReadableBuffer so ignore type error.
                 contents = memoryview(array)  # type: ignore
-                shape_desc = "_".join([str(d) for d in t.shape])
-                blob_name = f"torch_tensor_{shape_desc}_{str(t.dtype)}"
+                blob_name = symbol_name
                 elements_attr = DenseResourceElementsAttr.get_from_buffer(
                     contents, blob_name, tensor_type
                 )
                 ir_attrs["initial_value"] = elements_attr
 
             global_op = Operation.create("util.global", attributes=ir_attrs)
             self.symbol_table.insert(global_op)
```

## shark_turbine/aot/support/procedural/base.py

```diff
@@ -10,16 +10,18 @@
     Callable,
     List,
     Optional,
     Sequence,
 )
 
 from contextlib import contextmanager
+import threading
 
 import torch
+from torch.utils._pytree import tree_map
 
 from ....support.ir_imports import (
     F32Type,
     F64Type,
     IndexType,
     IntegerType,
     IrType,
@@ -30,20 +32,16 @@
 )
 
 from ..ir_utils import (
     FunctionBuilder,
     ModuleBuilder,
 )
 
-from ..utils import (
-    thread_state,
-    tree_map,
-)
-
 ShapedTypeDynamicSizeSentinel = ShapedType.get_dynamic_size()
+_thread_state = threading.local()
 
 ###############################################################################
 # Tracing intrinsics
 ###############################################################################
 
 
 class ProcedureTraceError(Exception):
@@ -67,17 +65,17 @@
         raise NotImplementedError(
             f"The current trace scope does not support assignment"
         )
 
 
 def _trace_scopes() -> List[IrTrace]:
     try:
-        trace_scopes = thread_state.trace_scopes
+        trace_scopes = _thread_state.trace_scopes
     except AttributeError:
-        trace_scopes = thread_state.trace_scopes = []
+        trace_scopes = _thread_state.trace_scopes = []
     return trace_scopes
 
 
 @contextmanager
 def new_ir_trace_scope(ir_trace: IrTrace):
     trace_scopes = _trace_scopes()
     trace_scopes.append(ir_trace)
```

## shark_turbine/aot/support/procedural/globals.py

```diff
@@ -15,32 +15,33 @@
     Optional,
     Sequence,
     Tuple,
 )
 
 import torch
 
+from torch.utils._pytree import (
+    TreeSpec,
+    tree_unflatten,
+)
+
 from ....support.ir_imports import (
     IrType,
     Operation,
     Value,
     util_d,
 )
 
+from ....support.logging import aot_logger as logger
+
 from ..ir_utils import (
     GlobalAttributes,
     ModuleBuilder,
 )
 
-from ..utils import (
-    TreeSpec,
-    logger,
-    tree_unflatten,
-)
-
 from .base import (
     AbstractScalar,
     AbstractTensor,
     Intrinsic,
     IrTrace,
     current_ir_trace,
 )
@@ -190,15 +191,18 @@
         else:
             return LiveGlobalCollectionProxy(tree_globals)
 
 
 class MaterializedGlobal:
     """Tags an Ir* that is duck-typed as a global."""
 
-    ...
+    ir_type: IrType
+    symbol_name: str
+    global_op: Operation
+    global_type: IrType
 
 
 class IrGlobalScalar(IrScalar, MaterializedGlobal):
     """An IrScalar that is loaded from a global and associated with its aggregate."""
 
     __slots__ = [
         "global_op",
```

## shark_turbine/aot/support/procedural/iree_emitter.py

```diff
@@ -111,15 +111,15 @@
 
 def cast_scalar_to_element_type(scalar: Value, element_type: IrType) -> Value:
     scalar_type = scalar.type
     # Support cast from Index -> Integer.
     if scalar_type == IndexType.get() and IntegerType.isinstance(element_type):
         return arith_d.IndexCastUIOp(element_type, scalar).result
     raise ValueError(
-        f"Provided splat value ({type(value)}) does not match dtype {dtype} (and cannot be cast)"
+        f"Provided splat value ({scalar_type}) does not match dtype {element_type} (and cannot be cast)"
     )
 
 
 def assert_value_is_index(x: Value):
     t = x.type
     if not IndexType.isinstance(t):
         raise ValueError(f"Expected an index value but got {t}")
@@ -341,15 +341,15 @@
         return result
 
     @emitter
     def tensor_trace(self, key: str, *ts: BuildableTensorType):
         dynamic_dims = []
         for t in ts:
             dynamic_dims.extend(t.get_only_dynamic_dim_values())
-        ts = [cast_tensor_value(t).ir_value for t in ts]
+        ts = tuple(cast_tensor_value(t).ir_value for t in ts)
         flow_d.TensorTraceOp(StringAttr.get(key), ts, dynamic_dims)
 
 
 # Circular imports to resolve typing.
 from .primitives import (
     IrScalar,
     IrTensor,
```

## shark_turbine/aot/support/procedural/primitives.py

```diff
@@ -5,14 +5,15 @@
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 # Live types during runtime of a procedure trace. User code will
 # operate on instances of these.
 
 from typing import (
+    cast,
     Dict,
     List,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
@@ -32,17 +33,14 @@
     arith_d,
 )
 
 from ..ir_utils import (
     build_tensor_dim_value,
     _is_float_type,
     _is_integer_like_type,
-)
-
-from ..utils import (
     Empty,
     EmptyType,
 )
 
 from .base import (
     Intrinsic,
     IrTrace,
@@ -120,24 +118,24 @@
                 )
 
 
 class IrImmediateScalar(IrScalar):
     """Represents an IR scalar value."""
 
     __slots__ = [
-        "ir_value",
+        "_ir_value",
     ]
 
     def __init__(self, ir_value: Value):
         super().__init__(ir_value.type)
         assert isinstance(ir_value, Value)
-        self.ir_value = ir_value
+        self._ir_value = ir_value
 
     def resolve_ir_values(self, proc_trace: IrTrace) -> Sequence[Value]:
-        return (self.ir_value,)
+        return (self._ir_value,)
 
 
 class IrTensor(Intrinsic):
     """An intrinsic that represents a tensor value.
 
     Carries additional metadata needed to resolve dimensions and original
     PyTorch attributes.
@@ -175,16 +173,16 @@
         # If we computed a dim, then stash it here for later use.
         self._cached_dim_values: List[Optional[Value]] = [None] * len(
             self._dynamic_dims
         )
 
     def dynamic_dim(self, i: int) -> Constraint:
         """Access the dynamic_dim constraint for the i'th dimension."""
-        self._populate_meta_tensor()
-        c = self._meta_tensor_constraints[i]
+        mt, constraints = self._get_meta_tensor_constraints()
+        c = constraints[i]
         if c is None:
             raise TypeError(
                 f"Requested dynamic_dim constraint for dimension {i} of {self.ir_type} which is not dynamic"
             )
         return c
 
     @property
@@ -276,17 +274,17 @@
                 )
         return values
 
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None):
         return NotImplemented
 
-    def _populate_meta_tensor(self):
-        if self._meta_tensor is not None:
-            return
+    def _get_meta_tensor_constraints(self) -> tuple[torch.Tensor, list[Constraint]]:
+        if self._meta_tensor is not None and self._meta_tensor_constraints is not None:
+            return self._meta_tensor, self._meta_tensor_constraints
 
         ir_tensor_type = self.ir_type
         shape = ir_tensor_type.shape
         # TODO: We shouldn't need to create a real tensor here, as Dynamo will
         # immediately convert it to fake. However, it will also set up the shape
         # environment and asserts that any fake tensor inputs are from its
         # internal FakeMode. There should be a way but needs more investigation.
@@ -297,35 +295,34 @@
         # a dynamic quantity. We therefore adjust the shape in this way and
         # add a dynamic_dim constraint.
         # See: https://github.com/nod-ai/SHARK-Turbine/issues/134
         extents = [2 if d < 0 else d for d in shape]
         mt = self._meta_tensor = torch.empty(extents, dtype=self.dtype)
         # Generate constraints that are aligned with any dynamic dimensions or None
         # if static.
-        self._meta_tensor_constraints = [
+        self._meta_tensor_constraints = constraints = [
             dynamic_dim(mt, i) if d < 0 else None for i, d in enumerate(shape)
         ]
+        return mt, constraints
 
     def _to_meta_tensor(self) -> Tuple[torch.Tensor, List[Constraint]]:
         """Converts to a fake Tensor that dynamo can handle."""
-        self._populate_meta_tensor()
-        return self._meta_tensor, [
-            c for c in self._meta_tensor_constraints if c is not None
-        ]
+        mt, constraints = self._get_meta_tensor_constraints()
+        return mt, [c for c in constraints if c is not None]
 
 
 class IrImmediateTensor(IrTensor):
     """Represents a Value in the IR under construction during procedural tracing."""
 
     __slots__ = [
-        "ir_value",
+        "_ir_value",
     ]
 
     def __init__(self, ir_value: Value, dtype: torch.dtype):
         super().__init__(ir_value.type, dtype)
-        self.ir_value = ir_value
+        self._ir_value = ir_value
 
     def __repr__(self):
         return f"IrValueTensor(@{self.ir_value})"
 
     def resolve_ir_values(self, proc_trace: IrTrace) -> Sequence[Value]:
-        return (self.ir_value,)
+        return (self._ir_value,)
```

## shark_turbine/aot/support/procedural/tracer.py

```diff
@@ -10,32 +10,33 @@
 from typing import (
     Any,
     Callable,
     List,
     Sequence,
 )
 
+from torch.utils._pytree import (
+    tree_flatten,
+    tree_unflatten,
+    treespec_dumps,
+)
+
 from ....support.ir_imports import (
     Location,
     StringAttr,
     Value,
     func_d,
 )
 
+from ....support.logging import aot_logger as logger
+
 from ..ir_utils import (
     ModuleBuilder,
 )
 
-from ..utils import (
-    logger,
-    tree_flatten,
-    tree_unflatten,
-    treespec_dumps,
-)
-
 from .base import (
     AbstractIntrinsic,
     Intrinsic,
     IrTrace,
     ProcedureTraceError,
     new_ir_trace_scope,
 )
```

## shark_turbine/dynamo/executor.py

```diff
@@ -115,15 +115,15 @@
         device = self.device_state.device
         num_returns = len(ret_list)
         user_returns = [None] * num_returns
         for i in range(num_returns):
             device_buffer_view = HalBufferView.__iree_vm_cast__(ret_list.get_as_ref(i))
             device_array = DeviceArray(device, device_buffer_view)
             host_array = device_array.to_host()
-            user_returns[i] = torch_from_numpy(host_array)
+            user_returns[i] = torch_from_numpy(host_array)  # type: ignore
 
         return user_returns
 
 
 @dataclass
 class EagerExecResult:
     buffer: HalBuffer
@@ -209,15 +209,15 @@
         num_returns = len(ret_list)
         user_returns = [None] * num_returns
         for i in range(num_returns):
             device_buffer_view = HalBufferView.__iree_vm_cast__(ret_list.get_as_ref(i))
             dtype = _element_type_to_dtype(device_buffer_view.element_type)
             size = torch.Size(device_buffer_view.shape)
             device_buffer = device_buffer_view.get_buffer()
-            user_returns[i] = EagerExecResult(device_buffer, size, dtype, signal)
+            user_returns[i] = EagerExecResult(device_buffer, size, dtype, signal)  # type: ignore
         return user_returns
 
     def _initialize_fences(self, device: Device, inputs: list, arg_list: VmVariantList):
         fence_capacity = device._fence_capacity
         tx_semaphore = device._tx_timeline
         current_tx_timepoint = device._tx_timepoint
```

## shark_turbine/dynamo/passes.py

```diff
@@ -1,67 +1,20 @@
 import torch
 from torch.fx.experimental.proxy_tensor import make_fx
 from torch._decomp import get_decompositions
-from shark_turbine.dynamo import utils
 from torch.func import functionalize
-from typing import List
+from typing import List, Optional
 
-# default decompositions pulled from SHARK / torch._decomp
-DEFAULT_DECOMPOSITIONS = [
-    torch.ops.aten.embedding_dense_backward,
-    torch.ops.aten.native_layer_norm_backward,
-    torch.ops.aten.slice_backward,
-    torch.ops.aten.select_backward,
-    torch.ops.aten.norm.ScalarOpt_dim,
-    torch.ops.aten.native_group_norm,
-    torch.ops.aten.upsample_bilinear2d.vec,
-    torch.ops.aten.split.Tensor,
-    torch.ops.aten.split_with_sizes,
-    torch.ops.aten.native_layer_norm,
-    torch.ops.aten.masked_fill.Tensor,
-    torch.ops.aten.masked_fill.Scalar,
-    torch.ops.aten.t,
-    torch.ops.aten.addmm,
-    # decompositions that aid us in handling nn.BatchNorm2d
-    torch.ops.aten._native_batch_norm_legit_functional,
-    torch.ops.aten._native_batch_norm_legit_no_training,
-    torch.ops.aten._native_batch_norm_legit,
-    torch.ops.aten._native_batch_norm_legit.no_stats,
-    torch.ops.aten.squeeze.dims,
-    # decompositions for miscellaneous ops that are not handled in torch-mlir but have available decompositions
-    torch.ops.aten.soft_margin_loss,
-    torch.ops.aten.im2col,
-    torch.ops.aten._euclidean_dist,
-    torch.ops.aten.index_copy,
-    torch.ops.aten.index_copy_,
-    torch.ops.aten.grid_sampler_2d,
-    torch.ops.aten.log_sigmoid_forward,
-    torch.ops.aten.unsafe_split.Tensor,
-    torch.ops.aten.binary_cross_entropy,
-    torch.ops.aten.dot,
-    torch.ops.aten._adaptive_avg_pool2d,
-    torch.ops.aten._prelu_kernel,
-    torch.ops.aten.full,
-    torch.ops.aten._log_softmax,
-    torch.ops.aten.nll_loss_forward,
-    torch.ops.aten.nll_loss_backward,
-    torch.ops.aten._to_copy,
-    torch.ops.aten._log_softmax_backward_data,
-    torch.ops.aten.lift_fresh_copy.default,
-    torch.ops.aten._unsafe_index.Tensor,
-    torch.ops.aten.unbind.int,
-    # decompositions added manually in this file
-    torch.ops.aten._scaled_dot_product_flash_attention.default,
-]
+from .decompositions import DEFAULT_DECOMPOSITIONS
 
 
 def apply_decompositions(
     gm: torch.fx.GraphModule,
     example_inputs,
-    decompose_ops: List[torch._ops.OpOverload] = None,
+    decompose_ops: Optional[List[torch._ops.OpOverload]] = None,
 ):
     if decompose_ops is None:
         return gm
 
     decompositions = get_decompositions(decompose_ops)
     gm = make_fx(
         functionalize(gm),
@@ -69,8 +22,8 @@
     )(*example_inputs)
 
     return gm
 
 
 def turbine_cpu_pass_pipeline(gm: torch.fx.GraphModule, example_inputs):
     decompose_ops = DEFAULT_DECOMPOSITIONS
-    return apply_decompositions(gm, example_inputs, decompose_ops)
+    return apply_decompositions(gm, example_inputs, decompose_ops)  # type: ignore
```

## shark_turbine/dynamo/tensor.py

```diff
@@ -47,15 +47,15 @@
     HalFence,
     VmModule,
 )
 
 from iree.compiler.api import Session, Output
 from iree.compiler.passmanager import PassManager
 
-from ..importers.fx_importer import FxImporter
+from iree.compiler.extras.fx_importer import FxImporter
 
 DEFAULT_COMPILER_FLAGS = ("--iree-input-type=torch",)
 
 ###############################################################################
 # Factories and device enablement
 ###############################################################################
 
@@ -63,16 +63,16 @@
 class TurbineMode(TorchFunctionMode):
     """Enables PyTorch tensor device= support for Tensor factory functions.
 
     This can be used in a `with` block to dynamically scope enablement, or
     it can be enabled globally via the `enable()` function.
     """
 
-    IMPLEMENTATIONS = {}
-    CACHED_IMPLEMENTATIONS = {}
+    IMPLEMENTATIONS: dict = {}
+    CACHED_IMPLEMENTATIONS: dict = {}
     COMPUTE_METHODS = set((torch.add, torch.sub, torch.mul, torch.abs))
 
     def __torch_function__(self, func, types, args=(), kwargs=None):
         def super_fn(*args, **kwargs):
             # Disable torch_function by hand because we don't want the wrapping behavior of
             # the super() impl
             with torch._C.DisableTorchFunction():
@@ -155,14 +155,15 @@
     if isinstance(device_arg, Device):
         return device_arg
     elif isinstance(device_arg, str):
         if device_arg == "turbine":
             return Device.current()
         elif device_arg.startswith(_TURBINE_PREFIX):
             return Device(device_arg[len(_TURBINE_PREFIX) :])
+    return None
 
 
 ###############################################################################
 # Turbine storage
 ###############################################################################
 
 
@@ -411,16 +412,16 @@
     else:
         return super_fn(self, device)
 
 
 @device_factory(torch.empty)
 def _empty(*size, device: Device, dtype=torch.float32):
     # Turbine empty.
-    size = _normalize_size(size)
-    return DeviceTensor._async_create_empty(size, device=device, dtype=dtype)
+    norm_size = _normalize_size(size)
+    return DeviceTensor._async_create_empty(norm_size, device=device, dtype=dtype)
 
 
 @device_factory(torch.zeros)
 def _zeros(*size, device: Device, dtype=torch.float32):
     t = DeviceTensor._async_create_empty(_normalize_size(size), device, dtype)
     t._async_fill_py_value(0)
     return t
```

## shark_turbine/dynamo/type_conversion.py

```diff
@@ -38,15 +38,15 @@
 DECOMPOSE_TENSOR_PARAMS_PATTERN = re.compile(r"\[([^\]]*)\],([^,]+)$")
 
 
 class NativeTypeConverter:
     def __init__(self, context: Context):
         self._context = context
         # Cache per instance.
-        self.torch_type_to_native = functools.lru_cache(maxsize=None)(
+        self.torch_type_to_native = functools.lru_cache(maxsize=None)(  # type: ignore[method-assign]
             self.torch_type_to_native
         )
 
     def torch_type_to_native(self, torch_type: IrType, signless: bool = True) -> IrType:
         """Converts a presumed torch type to a corresponding native type.
 
         This mirrors the type conversion in torch-mlir's BackendTypeConversion.cpp.
```

## shark_turbine/dynamo/backends/cpu.py

```diff
@@ -29,15 +29,15 @@
     PassManager,
 )
 
 from iree.runtime import (
     VmModule,
 )
 
-from ...importers.fx_importer import FxImporter
+from iree.compiler.extras.fx_importer import FxImporter
 
 import torch
 from torch._dynamo.backends.common import aot_autograd
 from ..passes import turbine_cpu_pass_pipeline
 
 DEFAULT_COMPILER_FLAGS = ("--iree-input-type=torch",)
```

## shark_turbine/importers/utils.py

```diff
@@ -39,64 +39,7 @@
         for t_super, value in self._mapping:
             if issubclass(t, t_super):
                 self._cache[t] = value
                 return value
         else:
             self._cache[t] = None
             return None
-
-
-###############################################################################
-# Reference mapping
-###############################################################################
-
-
-# Opaque value to indicate something is empty. Used in cases where 'None'
-# may have a different meaning.
-class EmptyType:
-    ...
-
-
-Empty = EmptyType()
-
-
-class RefMapping:
-    __slots__ = [
-        "_referrent",
-        "value",
-    ]
-
-    def __init__(self, referrent: Any):
-        if referrent is not Empty:
-            self._referrent = weakref.ref(referrent)
-        self.value = Empty
-
-    @property
-    def is_empty(self):
-        return self.value is Empty
-
-    def __repr__(self):
-        return (
-            f"<RefMapping {id(self._referrent) if self._referrent is not Empty else 'empty'} -> "
-            f"{self.value if self.value is not Empty else 'empty'}>"
-        )
-
-
-class RefTracker:
-    """Tracks live references from Python values to symbolic associations."""
-
-    def __init__(self):
-        self._refs: Dict[int, RefMapping] = {}
-
-    def track(self, referrent: Any) -> RefMapping:
-        ref_id = id(referrent)
-        existing = self._refs.get(ref_id)
-        if existing:
-            return existing
-        info = RefMapping(referrent)
-        if referrent is not Empty:
-            weakref.finalize(referrent, self._ref_finalizer, ref_id)
-        self._refs[ref_id] = info
-        return info
-
-    def _ref_finalizer(self, ref_id: int):
-        del self._refs[ref_id]
```

## shark_turbine/ops/iree.py

```diff
@@ -1,27 +1,29 @@
 # Copyright 2023 Advanced Micro Devices, Inc
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 """Custom ops for built-in IREE functionality."""
+from typing import cast
 
 from ..support.ir_imports import (
     RankedTensorType,
     StringAttr,
     Value,
     flow_d,
     tensor_d,
 )
 
 from ..runtime.op_reg import (
     CustomOp,
     KernelBuilder,
     KernelSelection,
+    AttrArg,
     def_library,
 )
 
 __all__ = [
     "trace",
 ]
 
@@ -44,31 +46,17 @@
             if rtt.is_dynamic_dim(i):
                 dynamic_dims.append(tensor_d.dim(t, kb.constant_index(i)))
     flow_d.TensorTraceOp(StringAttr.get(key), ts, dynamic_dims)
 
 
 @CustomOp.register(library=IREE_LIBRARY)
 class trace_tensor(CustomOp):
-    signature = "trace_tensor(str trace_key, Tensor tensor) -> ()"
+    signature = "trace_tensor(str trace_key, Tensor(a!) tensor) -> ()"
 
     def select(self, ksel: KernelSelection):
         ksel.attr_str(0)
-        ksel.arg_tensor(1)
+        ksel.arg_tensor(1, inplace_tied=True)
 
     def generate(self, ksel: KernelSelection, kb: KernelBuilder):
-        _emit_tensor_trace(kb, ksel.arg_descs[0].v, [kb.arg_bindings[1]])
-        kb.yield_results()
-
-
-@CustomOp.register(library=IREE_LIBRARY)
-class trace_tensors(CustomOp):
-    signature = "trace_tensors(str trace_key, Tensor[] tensors) -> ()"
-
-    def select(self, ksel: KernelSelection):
-        ksel.attr_str(0)
-        ksel.arg_tensor_list(1)
-
-    def generate(self, ksel: KernelSelection, kb: KernelBuilder):
-        ts = kb.arg_bindings[1]
-        if len(ts) >= 1:
-            _emit_tensor_trace(kb, ksel.arg_descs[0].v, ts)
-        kb.yield_results()
+        key = cast(AttrArg, ksel.arg_descs[0])
+        _emit_tensor_trace(kb, cast(str, key.v), [kb.arg_bindings[1]])
+        kb.yield_results(kb.arg_bindings[1])
```

## shark_turbine/runtime/device.py

```diff
@@ -213,26 +213,28 @@
     def vm_instance(self) -> VmInstance:
         return self._s.instance
 
     def create_hal_module(self) -> VmModule:
         s = self._s
         return create_hal_module(s.instance, s.device)
 
+    @staticmethod
     def current() -> "Device":
         try:
             return _CURRENT_THREAD.stack[-1]
         except (AttributeError, IndexError):
             raise NoCurrentDeviceError()
 
     def set(self) -> "Device":
         """Sets this device as the current device without a context manager."""
         try:
             _CURRENT_THREAD.stack.append(self)
         except AttributeError:
             _CURRENT_THREAD.stack = [self]
+        return self
 
     def clear(self):
         """Clears the current device without a context manager."""
         try:
             c = _CURRENT_THREAD.stack[-1]
             if _CURRENT_THREAD.stack[-1] is self:
                 _CURRENT_THREAD.stack.pop()
```

## shark_turbine/runtime/op_reg/base.py

```diff
@@ -4,15 +4,15 @@
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 """Base classes for registering custom operations with the PyTorch
 dispatcher.
 """
 
-from typing import Any, Callable, Optional, Sequence, Type, Union
+from typing import Any, Callable, Optional, Sequence, Type, Union, cast
 
 from abc import ABC, abstractmethod, abstractproperty
 import functools
 import logging
 import re
 import textwrap
 import threading
@@ -39,14 +39,15 @@
 
 from ...support.conversions import (
     TORCH_DTYPE_TO_IREE_TYPE_ASM,
 )
 
 __all__ = [
     "ArgDescriptor",
+    "AttrArg",
     "CustomOp",
     "FreeFuncKernelBuilder",
     "IntArg",
     "KernelBuilder",
     "KernelSelection",
     "TensorArg",
     "def_library",
@@ -234,22 +235,24 @@
     This mechanism also serves as the means for servicing `meta`
     registrations because it implicitly computes everything needed
     (i.e. shapes, etc).
     """
 
     __slots__ = [
         "arg_descs",
+        "inplace_tied_arg_descs",
         "op",
         "result_descs",
         "variant",
     ]
 
     def __init__(self, op: CustomOp, arg_arity: int):
         self.op = op
-        self.arg_descs: list[Optional[ArgDescriptor]] = arg_arity * [None]
+        self.arg_descs = cast(list[Optional[ArgDescriptor]], arg_arity * [None])
+        self.inplace_tied_arg_descs: list[ArgDescriptor] = []
         self.result_descs: list[ArgDescriptor] = []
         self.variant: str = "default"
 
     def __repr__(self):
         lines = [
             "KernelSelection<",
             f"  op = '{self.op.name}',",
@@ -275,31 +278,39 @@
             return None
         else:
             return tuple(results)
 
     @property
     def spec_key(self) -> str:
         try:
-            arg_keys = ",".join(d.spec_key for d in self.arg_descs)
-            return_keys = ",".join(d.spec_key for d in self.result_descs)
+            arg_keys = ",".join(
+                d.spec_key if d is not None else "None" for d in self.arg_descs
+            )
+            return_keys = ",".join(
+                d.spec_key if d is not None else "None" for d in self.result_descs
+            )
             return (
                 f"{self.op.cache_key_base}::{self.variant}({arg_keys})->({return_keys})"
             )
         except Exception as e:
             raise AssertionError(
                 f"Error generating spec_key from:\n{textwrap.indent(repr(self), '  ')}"
             ) from e
 
     @abstractmethod
-    def arg_tensor(self, arg: int) -> "TensorArg":
+    def arg_tensor(self, arg: int, *, inplace_tied: bool = False) -> "TensorArg":
         """Declares an argument to allow any ranked tensor and to specialize for each rank
         and dtype.
 
         Returns the argument descriptor, which can be used to further inspect or constrain
         the selection. It will default to allowing all dimensions to be dynamic.
+
+        If inplace_tied is True, then this argument participates in in-place
+        semantics. The kernel must yield the result-mutated after all normal
+        results in the order declared.
         """
         ...
 
     @abstractmethod
     def arg_tensor_list(self, arg: int) -> "TensorListArg":
         """Declares an argument to accept a list of tensors which will be specialized
         for the list size and each rank/dtype.
@@ -345,31 +356,33 @@
         "args",
     ]
 
     def __init__(self, op: CustomOp, args: list[Any]):
         super().__init__(op, len(args))
         self.args = args
 
-    def arg_tensor(self, arg: int) -> "TensorArg":
+    def arg_tensor(self, arg: int, *, inplace_tied: bool = False) -> "TensorArg":
         arg_descs = self.arg_descs
         arg_value = self.args[arg]
         assert arg_descs[arg] is None, f"Already constrained argument {arg}"
         assert isinstance(
             arg_value, Tensor
         ), f"Argument type mismatch from Torch for {arg}: Expected tensor, got {type(arg_value)}"
         arg_descs[arg] = desc = TensorArg(arg_value)
+        if inplace_tied:
+            self.inplace_tied_arg_descs.append(desc)
         return desc
 
     def arg_tensor_list(self, arg: int) -> "TensorListArg":
         arg_descs = self.arg_descs
         arg_value = self.args[arg]
         assert arg_descs[arg] is None, f"Already constrained argument {arg}"
         assert isinstance(
             arg_value, list
-        ), f"Argument type mismatch from Torch for {arg}: Expected tensor, got {type(arg_value)}"
+        ), f"Argument type mismatch from Torch for {arg}: Expected list, got {type(arg_value)}"
         arg_descs[arg] = desc = TensorListArg(arg_value)
         return desc
 
     def arg_int(self, arg: int) -> "IntArg":
         arg_descs = self.arg_descs
         arg_value = self.args[arg]
         assert arg_descs[arg] is None, f"Already constrained argument {arg}"
@@ -472,15 +485,15 @@
 
     ir_arity: int = 1
     is_list: bool = False
 
     def __init__(self, t: Tensor):
         self.t = t
         # Any static dims that we are specializing. Defaults to all dynamic.
-        self.spec_dims: list[Optional[int]] = len(t.shape) * [None]
+        self.spec_dims: Sequence[Optional[int]] = len(t.shape) * [None]
         # All descriptors have an attribute to indicate their value
         # as a tensor, and those that aren't are fixated to None.
         # This is to enable fast lookup in the hot path of determining
         # how to dispatch.
         self.maybe_tensor_value: Tensor = t
 
     def __repr__(self):
@@ -523,24 +536,24 @@
         "spec_dims",
         "ir_arity",
         "maybe_tensor_value",
     ]
 
     is_list: bool = True
 
-    def __init__(self, ts: Tensor):
+    def __init__(self, ts: list[Tensor]):
         self.ts = ts
         self.ir_arity = len(ts)
         # Any static dims that we are specializing. Defaults to all dynamic.
-        self.spec_dims: list[list[Optional[int]]] = [len(t.shape) * [None] for t in ts]
+        self.spec_dims: list[list[Optional[int]]] = [len(t.shape) * [None] for t in ts]  # type: ignore
         # All descriptors have an attribute to indicate their value
         # as a tensor, and those that aren't are fixated to None.
         # This is to enable fast lookup in the hot path of determining
         # how to dispatch.
-        self.maybe_tensor_value: Tensor = ts
+        self.maybe_tensor_value: list[Tensor] = ts
 
     def __repr__(self):
         return (
             f"TensorListArg(shape={[t.shape for t in self.ts]}, "
             f"dtype={[t.dtype for t in self.ts]}, "
             f"spec_dims={self.spec_dims}, ir_arity={self.ir_arity})"
         )
@@ -654,27 +667,28 @@
         context = self.module_op.context
         if func_name is None:
             func_name = ksel.op.name
         with context, Location.unknown(), InsertionPoint(module_body):
             # Assemble arg types.
             arg_types = []
             for d in ksel.arg_descs:
+                assert d is not None, "NYI: None arguments"
                 arity = d.ir_arity
                 if not d.is_list:
                     if arity == 1:
                         arg_types.append(IrType.parse(d.mlir_type_asm))
                     else:
                         continue
                 else:
                     for i in range(arity):
                         arg_types.append(IrType.parse(d.mlir_type_asm[i]))
 
             # Assemble result types.
             result_types = []
-            for d in ksel.result_descs:
+            for d in (*ksel.result_descs, *ksel.inplace_tied_arg_descs):
                 if not d.is_list:
                     if d.ir_arity == 1:
                         result_types.append(IrType.parse(d.mlir_type_asm))
                     else:
                         continue
                 else:
                     raise AssertionError("NYI: arity > 1 results")
@@ -688,14 +702,15 @@
             symbol_table.insert(func_op)
 
         # Map inputs to arg bindings, lining up with arguments that are elided.
         block_arguments = list(entry_block.arguments)
         block_arg_index = 0
         arg_bindings: list[Optional[Value]] = []
         for desc in ksel.arg_descs:
+            assert desc is not None, "NYI: None arguments"
             arity = desc.ir_arity
             if not desc.is_list:
                 if arity == 1:
                     arg_bindings.append(block_arguments[block_arg_index])
                     block_arg_index += 1
                 else:
                     arg_bindings.append(None)
@@ -733,14 +748,19 @@
                 func_name=func_name,
                 is_public=is_public,
             )
 
     def yield_results(self, *results: Value):
         """Yields results of the kernel computation."""
         assert not self.yielded, "yield_results has already been called"
+        ksel = self.ksel
+        expected_count = len(ksel.result_descs) + len(ksel.inplace_tied_arg_descs)
+        assert (
+            len(results) == expected_count
+        ), f"Mismatched yielded results and declared+inplace: Expected={expected_count}, Got={len(results)}"
         with self.ip, Location.unknown():
             func_d.ReturnOp(results)
         self.yielded = True
 
 
 ###############################################################################
 # Private utilities
```

## shark_turbine/runtime/op_reg/eager.py

```diff
@@ -26,14 +26,16 @@
 
 from ..device import (
     Device,
     lookup_device_from_torch,
 )
 
 from .base import (
+    AttrArg,
+    IntArg,
     KernelSelection,
 )
 
 from .compiler import (
     compile_standalone_kernel,
 )
 
@@ -46,43 +48,49 @@
     """Main entry-point for handling dispatch of a selected kernel via a generator."""
     # Scan arg descs and decide on a compute device.
     # For now, we compute on the first device that we support.
     # This is very simplisitic and will need to be extended for multi-device, etc.
     device: Optional[Device] = None
     torch_device: Optional[torch.device] = None
     for arg_desc in ksel.arg_descs:
+        assert arg_desc is not None, "NYI: None arguments"
         if not arg_desc.is_list:
             if arg_desc.ir_arity == 1:
                 # One arg has maybe_tensor_value as a single element (common case).
                 tensor_arg = arg_desc.maybe_tensor_value
                 if tensor_arg is None:
                     continue
+                assert isinstance(tensor_arg, torch.Tensor)
                 torch_device = tensor_arg.device
                 device = lookup_device_from_torch(torch_device)
                 if device is not None:
                     break
             else:
                 # Optional arg omitted.
                 assert arg_desc.ir_arity == 0
                 continue
         else:
             # List. maybe_tensor_value is a list. Uncommon case.
+            assert isinstance(arg_desc.maybe_tensor_value, list)
             for tensor_arg in arg_desc.maybe_tensor_value:
                 if tensor_arg is None:
                     continue
                 torch_device = tensor_arg.device
                 device = lookup_device_from_torch(torch_device)
                 if device is not None:
                     break
 
     # Default to CPU.
     if device is None:
         logger.debug("Fallback to CPU device due to no supported device in arguments")
         torch_device = torch.device("cpu")
         device = lookup_device_from_torch(torch_device)
+        assert (
+            device is not None
+        ), "Could not resolve lookup_device_from_torch for argument"
 
     # Compile.
     # TODO: We can do compilation asynchronously with the device movement
     vm_context, vm_f, config = compile_standalone_kernel(device, ksel)
 
     # Build the concrete args, issuing device movement as necessary.
     arg_list = VmVariantList(len(ksel.arg_descs))
@@ -107,34 +115,39 @@
                 )
             tensor_arg = tensor_arg.contiguous()
         # Since we know we are on the same device, we can use the unsafe
         # import_torch_tensor.
         arg_list.push_ref(device.import_torch_tensor(tensor_arg))
 
     for arg_desc in ksel.arg_descs:
+        assert arg_desc is not None, "NYI: None arguments"
         arity = arg_desc.ir_arity
         if not arg_desc.is_list:
             # Non-list.
             if arity == 1:
                 tensor_arg = arg_desc.maybe_tensor_value
                 if tensor_arg is not None:
                     push_tensor(tensor_arg)
                 else:
+                    assert isinstance(arg_desc, (IntArg, AttrArg))
                     push_scalar(arg_desc.v)
             else:
                 continue
         else:
             # List. Uncommon case.
             tensor_arg = arg_desc.maybe_tensor_value
             if tensor_arg is not None:
                 for i in range(arity):
                     push_tensor(tensor_arg[i])
             else:
                 for i in range(arity):
-                    push_scalar(arg_desc.v[i])
+                    assert isinstance(arg_desc, (IntArg, AttrArg))
+                    list_arg = arg_desc.v
+                    assert isinstance(list_arg, list)
+                    push_scalar(list_arg[i])
 
     if config.async_invocations:
         raise NotImplementedError("Async execution not yet implemented")
 
     # Invoke.
     ret_list = VmVariantList(len(ksel.result_descs))
     start = default_timer()
@@ -142,19 +155,21 @@
     invoke_time = default_timer() - start
     logger.debug("Kernel invocation %s: %sms", config.key, invoke_time * 1000)
 
     # Unpack results.
     results = []
     for i, result_desc in enumerate(ksel.result_descs):
         arity = result_desc.ir_arity
-        assert arity == 1, "NYI: Optional and result lists"
         meta_tensor_value = result_desc.maybe_tensor_value
         if meta_tensor_value is None:
             # Scalar return.
             raise NotImplementedError("CustomOp scalar return")
+        assert isinstance(
+            meta_tensor_value, torch.Tensor
+        ), "NYI: Optional and result lists"
 
         # Tensor return. The meta tensor value already has the correct torch
         # dtype and shape, so we just need to export and return it for the
         # appropriate device.
         bv: HalBufferView = HalBufferView.__iree_vm_cast__(ret_list.get_as_ref(i))
         results.append(device.export_torch_tensor(bv, meta_tensor_value))
```

## shark_turbine/support/conversions.py

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import torch
 
 from iree.runtime import (
     HalElementType,
 )
 
-from ..importers.fx_importer import (
+from iree.compiler.extras.fx_importer import (
     TORCH_DTYPE_TO_MLIR_TYPE_ASM,
 )
 
 from .exceptions import (
     UnknownDTypeError,
 )
```

## shark_turbine/support/logging.py

```diff
@@ -2,8 +2,9 @@
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
 import logging
 
+aot_logger = logging.getLogger("shark_turbine.aot")
 runtime_logger = logging.getLogger("shark_turbine.runtime")
```

## shark_turbine/transforms/merger.py

```diff
@@ -128,14 +128,21 @@
         # Merge initializers.
         initializers = get_top_level_ops(self.source_module, "util.initializer")
         for init_op in initializers:
             init_op.detach_from_parent()
             self._nested_symbol_table_ops.append(init_op)
             self._target_body.append(init_op)
 
+        # Merge external dispatches.
+        sources = get_top_level_ops(self.source_module, "hal.executable.source")
+        for source in sources:
+            source.detach_from_parent()
+            self._nested_symbol_table_ops.append(source)
+            self._target_body.append(source)
+
         # Merge functions.
         funcs = get_top_level_ops(self.source_module, "func.func")
         for func_op in funcs:
             self._import_symbol_op(func_op)
             self._nested_symbol_table_ops.append(func_op)
 
         self._logger(f"The following symbol renames will be made: {self._rename_map}")
```

## shark_turbine/transforms/rewriter.py

```diff
@@ -1,14 +1,14 @@
 # Copyright 2023 Nod Labs, Inc
 #
 # Licensed under the Apache License v2.0 with LLVM Exceptions.
 # See https://llvm.org/LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 
-from typing import Dict, List, Optional, Set, Union, Type, cast
+from typing import Dict, Generic, List, Optional, Set, Union, Type, TypeVar, cast
 
 import argparse
 import sys
 
 from iree.compiler.ir import (
     Block,
     BlockArgument,
@@ -42,32 +42,35 @@
     "pass_main",
 ]
 
 ###############################################################################
 # Matching
 ###############################################################################
 
+OpMatchT = TypeVar("OpMatchT", bound=Operation)
 
-class OpMatchResult:
-    def __init__(self, op: Operation):
+
+class OpMatchResult(Generic[OpMatchT]):
+    def __init__(self, op: OpMatchT):
         self.op = op
 
     def __repr__(self):
         return f"{type(self).__name__}({self.op})"
 
 
+OpMatchResultT = TypeVar("OpMatchResultT", bound=OpMatchResult)
 OperationParent = Union[None, Operation, OpView, Region, Block, OpMatchResult]
 OperationParentOrList = Union[OperationParent, List[OperationParent]]
 MaybeOperation = Union[None, Value, OpMatchResult, Operation, OpView]
 
 
-class OpMatcher:
+class OpMatcher(Generic[OpMatchResultT]):
     """Base class for things that match an operation."""
 
-    def __call__(self, maybe_op: MaybeOperation) -> Optional[OpMatchResult]:
+    def __call__(self, maybe_op: MaybeOperation) -> Optional[OpMatchResultT]:
         if maybe_op is None:
             return None
         if isinstance(maybe_op, OpMatchResult):
             op = maybe_op.op
         elif isinstance(maybe_op, Operation):
             op = maybe_op
         elif isinstance(maybe_op, OpView):
@@ -78,31 +81,31 @@
             elif BlockArgument.isinstance(maybe_op):
                 return None
         else:
             raise ValueError(f"Unexpected OpMatcher input: {type(maybe_op)}")
 
         return self._match(op)
 
-    def _match(self, op: Operation) -> Optional[OpMatchResult]:
+    def _match(self, op: Operation) -> Optional[OpMatchResultT]:
         raise NotImplementedError
 
 
-class NamedOpMatcher(OpMatcher):
+class NamedOpMatcher(OpMatcher[OpMatchResultT]):
     """Matches operations by name."""
 
     def __init__(self, *op_names: str):
         self.op_names = op_names
 
-    def _match(self, op: Operation) -> Optional[OpMatchResult]:
+    def _match(self, op: Operation) -> Optional[OpMatchResultT]:
         if op.name in self.op_names:
             return self.match(op)
         return None
 
-    def match(self, op: Operation) -> Optional[OpMatchResult]:
-        return OpMatchResult(op)
+    def match(self, op: Operation) -> Optional[OpMatchResultT]:
+        return OpMatchResult(op)  # type: ignore
 
 
 def get_child_blocks(of: OperationParentOrList) -> List[Block]:
     """Gets all child blocks of an Operation, Region, or Block (self)."""
     blocks: List[Block] = []
     if of is None:
         return blocks
@@ -161,15 +164,15 @@
 
 class GlobalOpResult(OpMatchResult):
     @property
     def sym_name(self) -> str:
         return StringAttr(self.op.attributes["sym_name"]).value
 
 
-class GlobalOpMatcher(NamedOpMatcher):
+class GlobalOpMatcher(NamedOpMatcher[GlobalOpResult]):
     """Matches global operations."""
 
     def __init__(self):
         super().__init__("util.global")
 
     def match(self, op: Operation) -> Optional[GlobalOpResult]:
         return GlobalOpResult(op)
@@ -177,15 +180,15 @@
 
 class Transpose2DResult(OpMatchResult):
     @property
     def input(self) -> Value:
         return self.op.operands[0]
 
 
-class Transpose2DMatcher(NamedOpMatcher):
+class Transpose2DMatcher(NamedOpMatcher[Transpose2DResult]):
     def __init__(self):
         super().__init__("torch.aten.transpose.int")
 
     def match(self, op: Operation) -> Optional[Transpose2DResult]:
         result = Transpose2DResult(op)
         if not ConstantIntMatcher(0)(op.operands[1]) or not ConstantIntMatcher(1)(
             op.operands[2]
@@ -212,15 +215,15 @@
         self.resolved_global: Optional[GlobalOpResult] = None
 
     @property
     def global_ref(self) -> str:
         return FlatSymbolRefAttr(self.op.attributes["global"]).value
 
 
-class GlobalLoadMatcher(NamedOpMatcher):
+class GlobalLoadMatcher(NamedOpMatcher[GlobalLoadResult]):
     def __init__(self, globals: Optional["GlobalsDict"] = None):
         super().__init__("util.global.load", "torch_c.from_builtin_tensor")
         self.globals = globals
 
     def match(self, op: Operation) -> Optional[GlobalLoadResult]:
         # Skip over any builtin tensor conversion.
         if op.name == "torch_c.from_builtin_tensor":
@@ -254,15 +257,15 @@
     @property
     def funcs(self) -> List[OpMatchResult]:
         return match_children(self.root_op, FuncOpMatcher())
 
     @property
     def globals(self) -> GlobalsDict:
         results = match_children(self.root_op, GlobalOpMatcher())
-        return {r.sym_name: r for r in results}
+        return {r.sym_name: r for r in cast(list[GlobalOpResult], results)}
 
     def merge_module(self, source_module: Operation) -> Merger:
         """Merges the given source module into the root.
 
         See documentation for the Merger for more information.
         """
         merger = Merger(source_module, self.root_op)
@@ -313,15 +316,15 @@
 
 
 def pass_main(pass_class: Type[Pass], *, argv=None):
     """Simple main entry-point which reads a file, runs a callback and outputs."""
     parser = argparse.ArgumentParser(description="Rewrite driver")
     parser.add_argument("input_file", help="File to process")
     parser.add_argument("-o", dest="output_file", help="Output file")
-    args = parser.parse_args(argv)
+    args, _ = parser.parse_known_args(argv)
 
     with Context() as context:
         with open(args.input_file, "r") as f:
             module_op = Operation.parse(f.read(), source_name=args.input_file)
 
         p = pass_class(module_op)
         p.run()
```

## shark_turbine/transforms/general/custom_op_expansion.py

```diff
@@ -120,15 +120,15 @@
         type_converter: NativeTypeConverter,
     ):
         super().__init__(op, len(operands))
         self.operands = operands
         self.results = results
         self.type_converter = type_converter
 
-    def arg_tensor(self, arg: int) -> TensorArg:
+    def arg_tensor(self, arg: int, *, inplace_tied: bool = False) -> TensorArg:
         # This is annoying: We have to go from the Torch MLIR type system to the
         # original torch.tensor Python type system. We do this by way of the native
         # type converter because it has the mapping pathway we need. This is one of the
         # only places in the code where we have to go this way to preserve the facade.
         # Everywhere else is going from Torch -> IREE native.
         arg_descs = self.arg_descs
         assert arg_descs[arg] is None, f"Already constrained argument {arg}"
@@ -150,14 +150,16 @@
             dtype = MLIR_TYPE_ASM_TO_TORCH_DTYPE[element_type_asm]
         except KeyError as e:
             raise AssertionError(
                 f"Could not find dtype mapping for {element_type_asm} in MLIR_TYPE_ASM_TO_TORCH_DTYPE"
             )
         t = torch.empty(rtt.shape, dtype=dtype, device="meta")
         arg_descs[arg] = desc = TensorArg(t)
+        if inplace_tied:
+            self.inplace_tied_arg_descs.append(desc)
         return desc
 
     def arg_tensor_list(self, arg: int) -> TensorListArg:
         raise NotImplementedError("NYI: AOT arg_tensor_list")
 
     def arg_int(self, arg: int) -> IntArg:
         raise NotImplementedError("NYI: AOT arg_int")
@@ -204,14 +206,15 @@
     ):
         location = torch_op.location
         ip = InsertionPoint(torch_op)
         with ip, location:
             operands = list(torch_op.operands)
             arg_bindings = []
             for desc, operand in zip(ksel.arg_descs, operands):
+                assert desc is not None, "NYI: None arguments"
                 arity = desc.ir_arity
                 if not desc.is_list:
                     if arity == 1:
                         arg_bindings.append(
                             type_converter.materialize_torch_to_native(operand)
                         )
                     else:
@@ -230,14 +233,19 @@
         self.location = location
         self.torch_op = torch_op
         self.type_converter = type_converter
 
     def yield_results(self, *results: Value):
         """Yields results of the kernel computation."""
         assert not self.yielded, "yield_results has already been called"
+        ksel = self.ksel
+        expected_count = len(ksel.result_descs) + len(ksel.inplace_tied_arg_descs)
+        assert (
+            len(results) == expected_count
+        ), f"Mismatched yielded results and declared+inplace: Expected={expected_count}, Got={len(results)}"
         with self.ip, self.location:
             torch_op_results: list[Value] = list(self.torch_op.results)
             assert len(results) == len(
                 torch_op_results
             ), f"Mismatched yield_results with custom op results"
             for new_result, old_result in zip(results, torch_op_results):
                 torch_type = old_result.type
```

## shark_turbine/transforms/general/rename_parameters.py

```diff
@@ -40,15 +40,15 @@
         rename_map: Optional[Dict[MaybeScopedName, MaybeScopedName]] = None,
         rename_callback: Callable[
             [Optional[str], str], Optional[ScopedName]
         ] = lambda scope, name: None,
     ):
         super().__init__(root_op)
         self.context = root_op.context
-        self.rename_map = rename_map
+        self.rename_map = rename_map or {}
         self.rename_callback = rename_callback
         with self.context:
             # Make a prototype named parameter attribute so we can get its
             # typeid.
             self.parameter_attr_typeid = Attribute.parse(
                 '#stream.parameter.named<""::"">'
             ).typeid
```

## shark_turbine/transforms/quantization/mm_group_quant.py

```diff
@@ -36,15 +36,15 @@
         self.k = k
         self.element_type = element_type
 
     def __repr__(self):
         return f"TransposedMM(weight={self.param_name}, m={self.m}, n={self.n}, k={self.k}, element_type={self.element_type})"
 
 
-class TransposedMMMatcher(NamedOpMatcher):
+class TransposedMMMatcher(NamedOpMatcher[TransposedMMResult]):
     def __init__(self, globals: GlobalsDict, builder: Builder):
         super().__init__("torch.aten.mm")
         self.globals = globals
         self.builder = builder
 
     def match(self, op: Operation):
         weight_transpose = Transpose2DMatcher()(op.operands[1])
@@ -142,25 +142,28 @@
             self.rewrite(mr)
 
         self.inline()
         self.cleanup()
 
     def rewrite(self, mr: TransposedMMResult):
         none_to_q = lambda x: "?" if x is None else x
+        static_n = mr.n
+        if static_n is None:
+            return
         # TODO (ian): make generalizable and not specific for brevitas
         if "lm_head.weight" not in mr.param_name:
             inline_module_asm = GROUP_MATMUL_TEMPLATE.format(
                 # TODO (ian): Fix skipping the "_params." portion of the name to match safetensor format with RenameParametersPass
                 param_name=mr.param_name[8:],
                 lowp_type="i4",
                 m=none_to_q(mr.m),
                 n=none_to_q(mr.n),
                 k=none_to_q(mr.k),
-                n_div=mr.n // 2,
-                group0=mr.n // self.group_size,
+                n_div=static_n // 2,
+                group0=static_n // self.group_size,
                 group1=self.group_size,
                 element_type=mr.element_type,
             )
 
             inline_module = Operation.parse(inline_module_asm, context=self.context)
             actual_callee_name = self.merge_module(inline_module).translate_symbol(
                 "compute_mm_group_quant"
```

## Comparing `shark_turbine-0.9.6.dist-info/METADATA` & `shark_turbine-2.3.0rc20240410.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: shark-turbine
-Version: 0.9.6
+Version: 2.3.0rc20240410
 Summary: SHARK Turbine Machine Learning Deployment Tools
 Home-page: https://github.com/nod-ai/SHARK-Turbine
 Author: SHARK Authors
 Author-email: stella@nod.ai
 License: Apache-2.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
-Requires-Dist: iree-compiler >=20240226.813
-Requires-Dist: iree-runtime >=20240226.813
+Requires-Dist: iree-compiler >=20240410.859
+Requires-Dist: iree-runtime >=20240410.859
 Requires-Dist: torch >=2.1.0
 Provides-Extra: onnx
 Requires-Dist: onnx ; extra == 'onnx'
 Provides-Extra: testing
 Requires-Dist: onnx ; extra == 'testing'
 Requires-Dist: pytest ; extra == 'testing'
 Requires-Dist: pytest-xdist ; extra == 'testing'
 Provides-Extra: torch-cpu-nightly
-Requires-Dist: torch >=2.1.0 ; extra == 'torch-cpu-nightly'
+Requires-Dist: torch ; extra == 'torch-cpu-nightly'
 
 # SHARK Turbine
 ![image](https://netl.doe.gov/sites/default/files/2020-11/Turbine-8412270026_83cfc8ee8f_c.jpg)
 
 Turbine is the set of development tools that the [SHARK Team](https://github.com/nod-ai/SHARK)
 is building for deploying all of our models for deployment to the cloud and devices. We
 are building it as we transition from our TorchScript-era 1-off export and compilation 
 to a unified approach based on PyTorch 2 and Dynamo. While we use it heavily ourselves, it 
 is intended to be a general purpose model compilation and execution tool.
 
 Turbine provides three primary tools:
 
 * *AOT Export*: For compiling one or more `nn.Module`s to compiled, deployment
-  ready artifacts. This operates via both a [simple one-shot export API](https://github.com/nod-ai/SHARK-Turbine/blob/main/python/shark_turbine/aot/exporter.py)
-  for simple models and an underlying [advanced API](https://github.com/nod-ai/SHARK-Turbine/blob/main/python/shark_turbine/aot/compiled_module.py) for complicated models
+  ready artifacts. This operates via both a simple one-shot export API (Already upstreamed to [torch-mlir](https://github.com/llvm/torch-mlir/blob/main/python/torch_mlir/extras/fx_importer.py))
+  for simple models and an underlying [advanced API](https://github.com/nod-ai/SHARK-Turbine/blob/main/core/shark_turbine/aot/compiled_module.py) for complicated models
   and accessing the full features of the runtime.
 * *Eager Execution*: A `torch.compile` backend is provided and a Turbine Tensor/Device
   is available for more native, interactive use within a PyTorch session.
 * *Turbine Kernels*: (coming soon) A union of the [Triton](https://github.com/openai/triton) approach and
   [Pallas](https://jax.readthedocs.io/en/latest/pallas/index.html) but based on
   native PyTorch constructs and tracing. It is intended to complement for simple
   cases where direct emission to the underlying, cross platform, vector programming model
@@ -60,42 +60,40 @@
 
 ## Quick Start for Users
 
 1. Install from source:
 
 ```
 pip install shark-turbine
-# Or editable: pip install -e core
+# Or for editable: see instructions under developers
 ```
 
 The above does install some unecessary cuda/cudnn packages for cpu use. To avoid this you
 can specify pytorch-cpu and install via:
 ```
-pip install --index-url https://download.pytorch.org/whl/cpu \
-    -r core/pytorch-cpu-requirements.txt \
-    -r core/torchvision-requirements.txt
+pip install -r core/pytorch-cpu-requirements.txt
 pip install shark-turbine
 ```
 
 (or follow the "Developers" instructions below for installing from head/nightly)
 
 2. Try one of the samples:
 
 Generally, we use Turbine to produce valid, dynamic shaped Torch IR (from the 
 [`torch-mlir torch` dialect](https://github.com/llvm/torch-mlir/tree/main/include/torch-mlir/Dialect/Torch/IR)
 with various approaches to handling globals). Depending on the use-case and status of the
 compiler, these should be compilable via IREE with `--iree-input-type=torch` for
 end to end execution. Dynamic shape support in torch-mlir is a work in progress,
 and not everything works at head with release binaries at present.
 
-  * [AOT MLP With Static Shapes](https://github.com/nod-ai/SHARK-Turbine/blob/main/examples/aot_mlp/mlp_export_simple.py)
-  * [AOT MLP with a dynamic batch size](https://github.com/nod-ai/SHARK-Turbine/blob/main/examples/aot_mlp/mlp_export_dynamic.py)
-  * [AOT llama2](https://github.com/nod-ai/SHARK-Turbine/blob/main/examples/llama2_inference/llama2.ipynb):
+  * [AOT MLP With Static Shapes](https://github.com/nod-ai/SHARK-Turbine/blob/main/core/examples/aot_mlp/mlp_export_simple.py)
+  * [AOT MLP with a dynamic batch size](https://github.com/nod-ai/SHARK-Turbine/blob/main/core/examples/aot_mlp/mlp_export_dynamic.py)
+  * [AOT llama2](https://github.com/nod-ai/SHARK-Turbine/blob/main/core/examples/llama2_inference/llama2.ipynb):
     Dynamic sequence length custom compiled module with state management internal to the model.
-  * [Eager MNIST with `torch.compile`](https://github.com/nod-ai/SHARK-Turbine/blob/main/examples/eager_mlp/mlp_eager_simple.py)
+  * [Eager MNIST with `torch.compile`](https://github.com/nod-ai/SHARK-Turbine/blob/main/core/examples/eager_mlp/mlp_eager_simple.py)
 
 ## Developers
 
 ### Getting Up and Running
 
 If only looking to develop against this project, then you need to install Python
 deps for the following:
@@ -108,14 +106,15 @@
 therefore require additional pip flags to install. Therefore, to satisfy
 development, we provide a `requirements.txt` file which installs precise
 versions and has all flags. This can be installed prior to the package:
 
 Installing into a venv is highly recommended.
 
 ```
+pip install -r core/pytorch-cpu-requirements.txt
 pip install --upgrade -r core/requirements.txt
 pip install --upgrade -e "core[torch-cpu-nightly,testing]"
 ```
 
 Run tests:
 
 ```
```

## Comparing `shark_turbine-0.9.6.dist-info/RECORD` & `shark_turbine-2.3.0rc20240410.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-shark_turbine/aot/__init__.py,sha256=L4uAWAtcWhqwjiaxD0KLuYns2QY7X-T1HG1SFLfImpY,313
-shark_turbine/aot/compiled_module.py,sha256=y-RPNO04nYUp4id3JLr3KA39VBJxiW-InNdwq3ny4W8,20685
-shark_turbine/aot/exporter.py,sha256=C4OVozd28EJoAVQ3mEUmLepLT70pwW3M2y46WATAytg,6938
+iree/turbine/__init__.py,sha256=aO-CTTyuCpkbBU7TwbF7t2hngKgFaLrFJYXOcZYjMCA,700
+shark_turbine/aot/__init__.py,sha256=adA_ZT60MsEFm9sCAMQHzpSZX6viiNODOS5HTzDGWkg,430
+shark_turbine/aot/compiled_module.py,sha256=uYIrK3lb-Jr4aiOrd5ljnMfkLc-qcFAgfXFrHoPwK4Y,23347
+shark_turbine/aot/decompositions.py,sha256=ouYk2ccigcWNtxo-oy3jSgJNBK1wG42fMJSQxZrqVo8,2815
+shark_turbine/aot/exporter.py,sha256=BueVZvHkAGcyrJiC6IgIaCo5WiwazaGhOFVwOD-4of4,9666
+shark_turbine/aot/fx_programs.py,sha256=jrRZqZDbCot8bu3L5JDn21bo8kf2ZGOWLr9RyjNp3AI,12219
+shark_turbine/aot/params.py,sha256=afhJLynl0QFn5PzF7XfIGhUiu2oytnoHhlfubx_MHSU,4751
+shark_turbine/aot/tensor_traits.py,sha256=u_IuLi_SAJsh7BxCwiWueYbA0gxNIbdRRZCIFASnfP0,1023
 shark_turbine/aot/builtins/__init__.py,sha256=vx1VcMmc-yQidXaf1PPufmkrWX8RastJM1HYc_L_IlE,884
-shark_turbine/aot/builtins/globals.py,sha256=ePsmk987F7SxpwjH0S8F1QDWAiDazCJc2cHZGiXe0-I,5409
-shark_turbine/aot/builtins/jittable.py,sha256=YB9z6gcKDrwkjTuTxz9rTDICeGorMLsdfWVgGx_LeEA,17841
+shark_turbine/aot/builtins/globals.py,sha256=HxQcY2724-0bcuwvLObp-Xf2TCdCVG9s0OAzkPu5_Q4,5431
+shark_turbine/aot/builtins/jittable.py,sha256=w3XEtd_XcdqFrRr0Duwi5XfwS4hjga4Sxsemw00JxB0,18037
 shark_turbine/aot/passes/__init__.py,sha256=mkiANoenJUYzb2NsRgQV4sDfVPi-0b9VWotNDJ6ayHI,262
-shark_turbine/aot/passes/functorch.py,sha256=72jOBylMa8QQgJu3Y2YlVt2HAx5TJmbXlueqhwwFf6Y,3522
-shark_turbine/aot/support/ir_utils.py,sha256=7bBWeH8KVI7-aGoBR86jZs9P0mdBjIRAHX660j8krPw,14145
-shark_turbine/aot/support/utils.py,sha256=sG_OQJRw45Y_T-61Pw1yr2LggQ_4tO7VlZQP97beudo,2158
+shark_turbine/aot/passes/functorch.py,sha256=SwzWVkWLDq7ud_y-kODNEB1wPk_EaGsaHCdCqYQyr1w,3537
+shark_turbine/aot/support/ir_utils.py,sha256=LMAsXEzNZpyHA5BvRJyyHTuNsibGSaWFIy9-AzWlpwQ,15795
 shark_turbine/aot/support/procedural/__init__.py,sha256=AAKJuYXBVmBbq-cClOOlzh3kbRiGW-Bkbwj982n8BiA,646
-shark_turbine/aot/support/procedural/base.py,sha256=Y6Fx65xF71-p8SYx9fgSuwLOlS_Nf_kmqlQ4Ii242yk,7470
-shark_turbine/aot/support/procedural/globals.py,sha256=NO7Oc8Rtetfk0-t2ZRTA9LmcboFrZkr-rXJrUixwpEw,9202
-shark_turbine/aot/support/procedural/iree_emitter.py,sha256=hpziNRaDdIXWyg_LhJniMYM9QbNW5vPwuF1bJeunTPE,12361
-shark_turbine/aot/support/procedural/primitives.py,sha256=bgljTlMiMvvt07SUzPwmC84e0sGsCJB4BkMBjAevoOE,11588
-shark_turbine/aot/support/procedural/tracer.py,sha256=K_ElqrNcq5d9t00gae72xwaZ8jPisa0JRCP17PIOiWA,7157
+shark_turbine/aot/support/procedural/base.py,sha256=2F5wdROfa75OQ96Y8by86FzoY5trK3C-fgrplWhC_ZQ,7507
+shark_turbine/aot/support/procedural/exported_program.py,sha256=sKjq22F4Yd1dR2qREZHTUgoeVagYyD1RaEiS7IhxDSY,11775
+shark_turbine/aot/support/procedural/globals.py,sha256=-clKFI0hGU6qfPfh0FjsXHYIWkW8cPllsuAkghpuBdw,9338
+shark_turbine/aot/support/procedural/iree_emitter.py,sha256=A0AU6KuE8r1A9HTfq6KHZkluO-ZAY3Dr8rwfB7GCGV4,12373
+shark_turbine/aot/support/procedural/primitives.py,sha256=O2xh2FdDg23cAbzUXMuH8uG1CzESwhH7sG85CXtsHNo,11744
+shark_turbine/aot/support/procedural/tracer.py,sha256=Eq6RVrl0wUVu1qUXxO5Aal6F-BUUuwspVWDRV3HeKcI,7211
 shark_turbine/dynamo/__init__.py,sha256=fsprbtYTtyX2jxbs8O8VZqutbrDJG87T1YkAGhwXisk,287
-shark_turbine/dynamo/executor.py,sha256=BF5sR5OILGJXeXSA5C9yJUYM33p-qLcsEeVmspJbiog,8147
-shark_turbine/dynamo/passes.py,sha256=n0xy8frl46hwTb0a2__IDgA6smVqCBsCCVrGrFeCY8A,2646
-shark_turbine/dynamo/tensor.py,sha256=3_DipoKwdY3c19jk0vLKQ563XfWldnZHEZ2ye_sZT2s,21923
-shark_turbine/dynamo/type_conversion.py,sha256=LZsEKZpFxUTLiCohSTmrqS2OPBKQe-bBBJesxYMouq0,6986
-shark_turbine/dynamo/utils.py,sha256=-26Cmoi-m-gqFZ4cYvDbAO15UGfYPrhYUOQ40XNFkxQ,3272
-shark_turbine/dynamo/backends/cpu.py,sha256=SmHqtF4ZNUguF6eB_Y7ACnjfHX9774iw2defIfojOKI,2808
-shark_turbine/importers/fx_importer.py,sha256=NWeMxn7WhWguMYWgszLCmjyVwVrYmafZkTw_YCAuwS0,67460
+shark_turbine/dynamo/decompositions.py,sha256=Omyu5TesiPAjYBqoZK9UG3Sv_rV_NrQnZx0US47VXu4,4096
+shark_turbine/dynamo/executor.py,sha256=vUTWn1czmZkrvoroXuYTtsWKyzCWeKtUx4FJW98A2Ss,8179
+shark_turbine/dynamo/passes.py,sha256=jFZdcVBL-fOaIJfjp2J66_iD1Hz2j5HRaM9JEo09WgE,814
+shark_turbine/dynamo/tensor.py,sha256=8DHnzqBoWCqCh7cxEaT1t3bNme6JpFR9deb9oB4YIF4,21970
+shark_turbine/dynamo/type_conversion.py,sha256=LMctGCReXwZuXXjEBr6L21gRvq-co09nQPpf2MEbgTo,7017
+shark_turbine/dynamo/backends/cpu.py,sha256=i_1bYvn8tEisN32s9vJ2lDClK8h1bgtPEc59nNu5la8,2816
 shark_turbine/importers/ir.py,sha256=ufPQWLqroZ6Ul05k1RXLQHvstzAUD46IxABrIKtHaJM,857
-shark_turbine/importers/utils.py,sha256=cT9lw1bKqoCsHHEMEdcYzHQKzr2L90fL-_q8CSj34eI,2675
+shark_turbine/importers/utils.py,sha256=9K8S7Wu7R3kqgiU8r_2hBET1VKGgQgTyv_0svK7Z_bw,1192
 shark_turbine/kernel/__init__.py,sha256=IontD5viYSNeQbAhKYpTDYyZVDIYV6zn98yXaL6GxWE,518
 shark_turbine/kernel/_support/context.py,sha256=7lr1iRE1YEJyYP8bBTHh5dyN_itoOpKUd7C0VK0LaBo,1484
 shark_turbine/kernel/_support/dtype.py,sha256=87HosOz7HNZovMptbpEPm_B3FkywlUaZPONMc4HQc8w,1157
 shark_turbine/kernel/_support/indexing.py,sha256=gss4gd2fsGcw8JCJBUBFOv5AZJcObI1Fpg0Jd152o08,12390
 shark_turbine/kernel/_support/regions.py,sha256=TvQk6v2KFPsxcVrXZz-Z-bDr2tYAsktSmaAJVpLgLHc,5147
 shark_turbine/kernel/_support/shaped_type.py,sha256=crompGTpkHrjn_7uZwfEMiOwghKR_XxaPl0Dmxb5LOk,3549
 shark_turbine/kernel/_support/tracing.py,sha256=hZi-HwfZbAFnG36BEhzQUQiCOh8ATT9LTF7H6_CwK18,15676
@@ -52,30 +56,30 @@
 shark_turbine/kernel/ops/control_flow.py,sha256=fHcTKIWB_0j75XM1Y_sFnB2RcmQ5pM8Zbrx2ovMZxDE,638
 shark_turbine/kernel/ops/core.py,sha256=N-gClns5wt9SKoYI_OAYVV9eH7sVa8vfrtBBHs3tgmU,581
 shark_turbine/kernel/ops/math.py,sha256=O7n8wXQHYvU9x00WN0J1xJeSdKd481JBhsBxkppwxQc,330
 shark_turbine/kernel/ops/memory.py,sha256=ZtyNLdWsDC_xkYyxqzs5bGp1wnQjCOGT0J7QfFRh4VI,577
 shark_turbine/kernel/ops/reduction.py,sha256=AfJHtJM6Iwy3dO6chdi4J1A04PZ6VkEwuSof8sgXY0s,487
 shark_turbine/kernel/ops/shape_manipulation.py,sha256=IswoyHQ1Zt6LHZrg4i0yI9CfW4v_0jxj2yrS4xmP5g0,555
 shark_turbine/ops/__init__.py,sha256=3ryhltgCM5UEUUBmn10xIn6RV0whheutIAgfK_QA_yg,248
-shark_turbine/ops/iree.py,sha256=pNfHDaKY9qDkr_noWIHJaC1v0VsR-LpqFf1lJZ33vBQ,2169
+shark_turbine/ops/iree.py,sha256=J3q-B_Mag_ArGhMqkdfe_mnZVQBC0yZvx1Do9smcUrM,1832
 shark_turbine/runtime/__init__.py,sha256=d5d9eGH_T80qOMPBSWC6vRw8EOKjBXx5gYYnGOAg65Y,272
-shark_turbine/runtime/device.py,sha256=bGB8A-l5iwpjVwPuSoVPPbOCw25joVSWZ_mubJGI5cs,12431
+shark_turbine/runtime/device.py,sha256=58EAES0r517Q9u5NGfvjCT8z-o9GUNG41iNcEj0FDLI,12469
 shark_turbine/runtime/op_reg/__init__.py,sha256=Rg00q1Po-JFpWoHYcvqTqvNkVmwL7blhkKyxeIDZirU,249
-shark_turbine/runtime/op_reg/base.py,sha256=P4ZA_wPa268cnY2uNbh7nnMa04Pzt0cdb5tkt_WNZQw,27042
+shark_turbine/runtime/op_reg/base.py,sha256=nlRUci6NPHFhaATGY0aB6QxgWFicLNBfEF4WaAw-Adk,28076
 shark_turbine/runtime/op_reg/compiler.py,sha256=Rv2Fn8R_Sl0q3j_P8KW9ifDR86Ny4ECFxlOwOfJ-p7Y,4442
-shark_turbine/runtime/op_reg/eager.py,sha256=My_ndsfvBa5EYrVQzBmBl6iKI_dfavzZxgSnaKuXfN8,5673
+shark_turbine/runtime/op_reg/eager.py,sha256=2BLuLG5biL8fqryqEos-OE46zzXCe97xV0netnHgjzc,6341
 shark_turbine/support/__init__.py,sha256=k_LVx8MyNLqne6v1i9ZryQgw_z5gOYiQXfhZ8cSC8cg,241
-shark_turbine/support/conversions.py,sha256=opfZK5Qp_FqizshtYvSGtM7FVeNQcGIXhJfU0IgcZ9c,4109
+shark_turbine/support/conversions.py,sha256=UngumsU4nDkJ1NgBOL8hWWHDRgJXNIGmoyZaPlawdJU,4118
 shark_turbine/support/exceptions.py,sha256=EhMtpUEWT4wXo1ANF688oQP5H4ry2it9fjnEhJ9Nd24,1341
 shark_turbine/support/ir_imports.py,sha256=rx7gwuMqvzxGCOCTXNj-4wypeJauOsq_lZ3N6pAajZU,1128
-shark_turbine/support/logging.py,sha256=M4imcanOg3GBK_xuipXf3ERdXa4ihz2Ej07MAHUIOKY,305
+shark_turbine/support/logging.py,sha256=Zk1eX0FE9ZO6MARJTLslUdYZUgPoszK251Z6bFncuAQ,357
 shark_turbine/transforms/builder.py,sha256=YDDfIZF28REmEUEyLRBRF5Y1oNyu9QKM59_snzgVI8w,2365
-shark_turbine/transforms/merger.py,sha256=mDet4JpE9xpYQVTLQjFkKHCfuUPnvm78klemCZ7TR1E,7910
-shark_turbine/transforms/rewriter.py,sha256=NVkW1lHaYijIP3D8OQh3EYgLgf2uBC7OQwEq-T4S-G4,10697
-shark_turbine/transforms/general/custom_op_expansion.py,sha256=S60IQRejWWwcpLjWwUVn03anjW2CzXsDowwgCM_5ZZk,8563
-shark_turbine/transforms/general/rename_parameters.py,sha256=tlEsinB63F-194FaEBykrAWqYxeN2CCtnV-wh3lb-Q0,4989
-shark_turbine/transforms/quantization/mm_group_quant.py,sha256=bPubW11VVHOnxrCok5NbnzhOn15Jb5RB3WF9k2OgjbY,7693
-shark_turbine-0.9.6.dist-info/METADATA,sha256=a0yHwWOEfeZYqV9ybwDLaVSvL-Gm7eQM8Wt6Bt0ccjc,6229
-shark_turbine-0.9.6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-shark_turbine-0.9.6.dist-info/entry_points.txt,sha256=-bxFqt7ywvSixYOWlz1sZ8MXChj-5joPPR_gZfT3Kn4,80
-shark_turbine-0.9.6.dist-info/top_level.txt,sha256=_Z7VXPJRosdcUR5nr-0U098w2vwfVLr6CepyIV7tLCQ,14
-shark_turbine-0.9.6.dist-info/RECORD,,
+shark_turbine/transforms/merger.py,sha256=trtv4JT9cIdRtw95lbqaBx5LvOvEaz28Kice6yTLp9g,8202
+shark_turbine/transforms/rewriter.py,sha256=UfTg26XJONA7dIipzyV6TMxq4Wgr2I7TxhqrWMwyktY,10997
+shark_turbine/transforms/general/custom_op_expansion.py,sha256=rlStftau1NF9upIcUh3FUalGJM-OIHhg-AqCIQry9Sk,9012
+shark_turbine/transforms/general/rename_parameters.py,sha256=bPmDqRuCMJJFN5SjP8-b0ajcfDpIx5zpSKQZ_nB-jbg,4995
+shark_turbine/transforms/quantization/mm_group_quant.py,sha256=DyqTvSJExiS2YlOajOO1Y8if7LBR_kslCc00BjJytTE,7793
+shark_turbine-2.3.0rc20240410.dist-info/METADATA,sha256=EdnNXZ9_cECGezkLs6tHy4FS8CysK7E8jfqa1LnGYkE,6263
+shark_turbine-2.3.0rc20240410.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+shark_turbine-2.3.0rc20240410.dist-info/entry_points.txt,sha256=-bxFqt7ywvSixYOWlz1sZ8MXChj-5joPPR_gZfT3Kn4,80
+shark_turbine-2.3.0rc20240410.dist-info/top_level.txt,sha256=HC8-angiduPf60mk4TnoHh0l6DedI5geRT925eyi6mc,19
+shark_turbine-2.3.0rc20240410.dist-info/RECORD,,
```

